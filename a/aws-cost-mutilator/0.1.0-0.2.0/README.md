# Comparing `tmp/aws_cost_mutilator-0.1.0.tar.gz` & `tmp/aws_cost_mutilator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_cost_mutilator-0.1.0.tar", max compression
+gzip compressed data, was "aws_cost_mutilator-0.2.0.tar", max compression
```

## Comparing `aws_cost_mutilator-0.1.0.tar` & `aws_cost_mutilator-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1048 2024-05-08 17:12:15.378273 aws_cost_mutilator-0.1.0/LICENSE
--rw-r--r--   0        0        0      179 2024-05-08 17:12:15.378273 aws_cost_mutilator-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-08 17:12:15.378273 aws_cost_mutilator-0.1.0/aws_cost_mutilator/__init__.py
--rw-r--r--   0        0        0     5224 2024-05-08 17:12:15.378273 aws_cost_mutilator-0.1.0/aws_cost_mutilator/__main__.py
--rw-r--r--   0        0        0     9274 2024-05-08 17:12:15.378273 aws_cost_mutilator-0.1.0/aws_cost_mutilator/lib.py
--rw-r--r--   0        0        0    10398 2024-05-08 17:12:15.378273 aws_cost_mutilator-0.1.0/aws_cost_mutilator/tests.py
--rw-r--r--   0        0        0      812 2024-05-08 17:12:15.378273 aws_cost_mutilator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 aws_cost_mutilator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1048 2024-05-13 16:10:40.035313 aws_cost_mutilator-0.2.0/LICENSE
+-rw-r--r--   0        0        0      330 2024-05-13 16:10:40.035313 aws_cost_mutilator-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 16:10:40.035313 aws_cost_mutilator-0.2.0/aws_cost_mutilator/__init__.py
+-rw-r--r--   0        0        0     9994 2024-05-13 16:10:40.035313 aws_cost_mutilator-0.2.0/aws_cost_mutilator/__main__.py
+-rw-r--r--   0        0        0    10171 2024-05-13 16:10:40.035313 aws_cost_mutilator-0.2.0/aws_cost_mutilator/ec2.py
+-rw-r--r--   0        0        0     1311 2024-05-13 16:10:40.035313 aws_cost_mutilator-0.2.0/aws_cost_mutilator/iam.py
+-rw-r--r--   0        0        0     1335 2024-05-13 16:10:40.035313 aws_cost_mutilator-0.2.0/aws_cost_mutilator/s3.py
+-rw-r--r--   0        0        0    12552 2024-05-13 16:10:40.035313 aws_cost_mutilator-0.2.0/aws_cost_mutilator/tests.py
+-rw-r--r--   0        0        0      812 2024-05-13 16:10:40.035313 aws_cost_mutilator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 aws_cost_mutilator-0.2.0/PKG-INFO
```

### Comparing `aws_cost_mutilator-0.1.0/LICENSE` & `aws_cost_mutilator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_cost_mutilator-0.1.0/aws_cost_mutilator/lib.py` & `aws_cost_mutilator-0.2.0/aws_cost_mutilator/ec2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-import boto3
 import json
 from tqdm import tqdm
 from time import sleep
-
-
-def boto_session(region, profile):
-    try:
-        session = boto3.Session(region_name=region, profile_name=profile)
-        session.client("sts").get_caller_identity()
-        return session
-
-    except Exception as e:
-        print(f"Error: {e}")
-        return None
+from datetime import datetime, timedelta
 
 
 def get_lb_hourly_costs(session):
-    # Set up AWS client
     client = session.client("pricing", region_name="us-east-1")
 
-    # Set up the parameters for the API call
     net_params = {
         "ServiceCode": "AmazonEC2",
         "Filters": [
             {
                 "Type": "TERM_MATCH",
                 "Field": "productFamily",
                 "Value": "Load Balancer-Network",
@@ -43,60 +30,53 @@
     }
 
     # classic_params = {
     #     "ServiceCode": "AmazonEC2",
     #     "Filters": [{"Type": "TERM_MATCH", "Field": "productFamily", "Value": "Load Balancer"}],
     # }
 
-    # Make the API call to get the pricing information
     net_response = client.get_products(**net_params)
     app_response = client.get_products(**app_params)
     # classic_response = client.get_products(**classic_params)
 
-    # Create a dictionary to store the hourly costs
     hourly_costs = {"network": {}, "application": {}}  # , "classic": {}}
     responses = {
         "network": net_response,
         "application": app_response,
     }  # , "classic": classic_response}
 
     for response in responses:
         for product in responses[response]["PriceList"]:
-            # Parse the JSON data
             data = json.loads(product)
 
             product_key = list(data["terms"]["OnDemand"].keys())[0]
             price_dimensions_key = list(
                 data["terms"]["OnDemand"][product_key]["priceDimensions"].keys()
             )[0]
 
             if (
                 data["terms"]["OnDemand"][product_key]["priceDimensions"][
                     price_dimensions_key
                 ]["unit"]
                 != "Hrs"
             ):
-                # not worried about data costs because these are not in active use
                 continue
 
-            # Get the region and hourly cost
             region = data["product"]["attributes"]["regionCode"]
             ppu = data["terms"]["OnDemand"][product_key]["priceDimensions"][
                 price_dimensions_key
             ]["pricePerUnit"]
 
             if region not in hourly_costs[response]:
-                # Add the cost to the dictionary
                 hourly_costs[response][region] = ppu
 
     return hourly_costs
 
 
 def delete_tgs(session, tgs, dry_run=False):
-    # Create an AWS client for the Elastic Load Balancing service
     elb_client = session.client("elbv2")
 
     pbar = tqdm(tgs)
     for tg_arn in pbar:
         if not dry_run:
             try:
                 elb_client.delete_target_group(TargetGroupArn=tg_arn)
@@ -111,23 +91,20 @@
     client.modify_load_balancer_attributes(
         LoadBalancerArn=lb_arn,
         Attributes=[{"Key": "deletion_protection.enabled", "Value": "false"}],
     )
 
 
 def delete_lbs(session, lbs, dry_run=False):
-    # Create an AWS client for the Elastic Load Balancing service
     elb_client = session.client("elbv2")
     waiter = elb_client.get_waiter("load_balancers_deleted")
 
     pbar = tqdm(lbs)
     for lb_arn in pbar:
-
         if not dry_run and "populated_target_groups" not in lbs[lb_arn]:
-            # Delete the load balancer
             try:
                 lb_attributes = elb_client.describe_load_balancer_attributes(
                     LoadBalancerArn=lb_arn
                 )["Attributes"]
 
                 if any(
                     attr["Key"] == "deletion_protection.enabled"
@@ -151,22 +128,68 @@
             waiter.wait(
                 LoadBalancerArns=[lb_arn],
                 WaiterConfig={"Delay": 15, "MaxAttempts": 100},
             )
             sleep(5)
         pbar.write(f"deleted load balancer {lb_arn} (dry run: {dry_run})")
 
-        # Delete the target groups
         delete_tgs(session, lbs[lb_arn]["empty_target_groups"])
 
     return None
 
 
-def get_tgs_no_targets_or_lb(session):
-    # Create an elbv2 client
+def delete_ebs_volumes(volume_ids, session, dry_run=False):
+    ec2 = session.resource("ec2")
+    for volume_id in volume_ids:
+        volume = ec2.Volume(volume_id)
+        print("Deleting volume {}".format(volume_id))
+        if not dry_run:
+            volume.delete()
+
+
+def estimate_snapshots_cost(session, snapshot_ids):
+    ec2 = session.client("ec2")
+
+    # Pricing details (as of September 2021)
+    # This value might change, so you should update it based on the current pricing details
+    price_per_gb_month = 0.05
+
+    total_size_gb = 0
+    for snapshot_id in snapshot_ids:
+        snapshot = ec2.describe_snapshots(SnapshotIds=[snapshot_id])["Snapshots"][0]
+        total_size_gb += snapshot["VolumeSize"]
+
+    cost = total_size_gb * price_per_gb_month
+
+    return cost
+
+
+def delete_ebs_snapshots(snapshot_ids, session, dry_run=False):
+    ec2 = session.client("ec2")
+    for snapshot_id in snapshot_ids:
+        print("Deleting snapshot {}".format(snapshot_id))
+        if not dry_run:
+            ec2.delete_snapshot(SnapshotId=snapshot_id)
+
+
+def get_old_snapshots(session, days):
+    ec2 = session.client("ec2")
+
+    now = datetime.now()
+    snapshots = ec2.describe_snapshots(OwnerIds=["self"])["Snapshots"]
+    old_snapshots = [
+        snapshot["SnapshotId"]
+        for snapshot in snapshots
+        if (now - snapshot["StartTime"].replace(tzinfo=None)) > timedelta(days=days)
+    ]
+
+    return old_snapshots
+
+
+def scan_for_tgs_no_targets_or_lb(session):
     elb_client = session.client("elbv2")
 
     unused_target_groups = {
         tg["TargetGroupArn"]: {
             "TargetHealthDescriptions": elb_client.describe_target_health(
                 TargetGroupArn=tg["TargetGroupArn"]
             )["TargetHealthDescriptions"],
@@ -174,55 +197,46 @@
         }
         for tg in elb_client.describe_target_groups()["TargetGroups"]
     }
 
     tgs = []
 
     print("getting target groups with zero targets or no configured load balancer...")
-    # Print the ARN of each target group that has 0 targets or no load balancers
     for target_group_arn in tqdm(unused_target_groups):
-        # sleep so progress par displays correctly
         sleep(0.05)
 
         if len(unused_target_groups[target_group_arn]["TargetHealthDescriptions"]) == 0:
             tgs.append(target_group_arn)
 
         if len(unused_target_groups[target_group_arn]["LoadBalancerArns"]) == 0:
             tgs.append(target_group_arn)
 
     return tgs
 
 
-def get_lbs_no_targets(session, region, omit_pricing=False):
-    # Create an AWS client for the Elastic Load Balancing service
+def scan_for_lbs_no_targets(session, region, omit_pricing=False):
     elb_client = session.client("elbv2")
 
-    # Get the hourly costs of the load balancers
     print("getting hourly costs of load balancers...")
 
     if not omit_pricing:
         hourly_costs = get_lb_hourly_costs(session)
 
-    # Get the list of load balancers in the specified region
     response = elb_client.describe_load_balancers()
 
     if len(response["LoadBalancers"]) == 0:
         print(f"No load balancers found in region {region}")
         return {"total_monthly_cost": 0}
 
-    # List to store the ARNs of load balancers with no targets
     lbs = {}
 
-    # Iterate over the load balancers
     for lb in tqdm(response["LoadBalancers"]):
-        # Get the ARN of the load balancer
         lb_arn = lb["LoadBalancerArn"]
 
         if not omit_pricing:
-            # Get the monthly cost of the load balancer
             lb_cost_value = (
                 float(list(hourly_costs[lb["Type"]][region].values())[0]) * 730
             )
         else:
             lb_cost_value = 0
 
         lb_target_groups = {
@@ -231,32 +245,28 @@
             )
             for tg in elb_client.describe_target_groups(LoadBalancerArn=lb_arn)[
                 "TargetGroups"
             ]
         }
 
         for lb_target_group_arn in lb_target_groups:
-            # If the target group has no targets
             if (
                 len(lb_target_groups[lb_target_group_arn]["TargetHealthDescriptions"])
                 == 0
             ):
                 if lb_arn not in lbs:
                     lbs[lb_arn] = {
                         "monthly_cost": lb_cost_value,
                         "empty_target_groups": [lb_target_group_arn],
                     }
                 else:
                     lbs[lb_arn]["empty_target_groups"].append(lb_target_group_arn)
 
-        # if the lb has a target group with no targets
         if lb_arn in lbs:
-            # cross reference for populated target groups
             for lb_target_group_arn in lb_target_groups:
-                # If the target group has targets
                 if (
                     len(
                         lb_target_groups[lb_target_group_arn][
                             "TargetHealthDescriptions"
                         ]
                     )
                     != 0
@@ -267,7 +277,45 @@
                         lbs[lb_arn]["populated_target_groups"].append(
                             lb_target_group_arn
                         )
 
     lbs["total_monthly_cost"] = sum([lbs[lb]["monthly_cost"] for lb in lbs])
 
     return lbs
+
+
+def scan_for_unused_ebs_volumes(session):
+    client = session.client("ec2")
+
+    cost_per_gb_map = {
+        "gp3": 0.08,
+        "gp2": 0.1,
+        "io1": 0.125,
+        "io2": 0.125,
+        "st1": 0.045,
+        "sc1": 0.025,
+        "standard": 0.05,
+    }
+
+    volumes = client.describe_volumes()["Volumes"]
+
+    print("getting unused ebs volumes...")
+    unused_volumes = {
+        "volumes": [
+            {
+                "VolumeId": volume["VolumeId"],
+                "Size": volume["Size"],
+                "CreateTime": str(volume["CreateTime"]),
+                "MultiAttachEnabled": volume["MultiAttachEnabled"],
+                "Attachments": volume["Attachments"],
+                "MonthlyCost": volume["Size"] * cost_per_gb_map[volume["VolumeType"]],
+            }
+            for volume in tqdm(volumes)
+            if volume["State"] == "available"
+        ]
+    }
+
+    unused_volumes["total_monthly_cost"] = sum(
+        [volume["MonthlyCost"] for volume in unused_volumes["volumes"]]
+    )
+
+    return unused_volumes
```

### Comparing `aws_cost_mutilator-0.1.0/aws_cost_mutilator/tests.py` & `aws_cost_mutilator-0.2.0/aws_cost_mutilator/tests.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,16 @@
-from .lib import boto_session, delete_tgs, delete_lbs, disable_lb_deletion_protection
-from .lib import get_tgs_no_targets_or_lb, get_lbs_no_targets
+from .ec2 import delete_tgs, delete_lbs, disable_lb_deletion_protection
+from .ec2 import (
+    scan_for_tgs_no_targets_or_lb,
+    scan_for_lbs_no_targets,
+    delete_ebs_volumes,
+)
+from .s3 import get_buckets, get_bucket_cost
 import boto3
-from moto import mock_elbv2, mock_sts, mock_ec2
-
-
-@mock_sts
-def test_boto_session():
-    # Test successful boto session creation
-    region = "us-west-2"
-    profile = "default"
-    session = boto_session(region, profile)
-    assert session is not None
-    assert session.region_name == region
-    assert session.profile_name == profile
-
-    # Test error when creating boto session
-    region = "invalid"
-    profile = "invalid"
-    session = boto_session(region, profile)
-    assert session is None
+from moto import mock_elbv2, mock_ec2, mock_s3
 
 
 # Create a mock Elastic Load Balancing client
 @mock_elbv2
 def test_delete_tgs():
     # Create a mock Elastic Load Balancing client
     elb_client = boto3.client("elbv2")
@@ -178,15 +166,15 @@
         attr["Key"] == "deletion_protection.enabled" and attr["Value"] == "false"
         for attr in attributes
     )
 
 
 @mock_ec2
 @mock_elbv2
-def test_get_tgs_no_targets_or_lb():
+def test_scan_for_tgs_no_targets_or_lb():
     # Create a mock AWS session
     session = boto3.Session(
         region_name="us-east-1",
         aws_access_key_id="mock_access_key",
         aws_secret_access_key="mock_secret_key",
     )
 
@@ -228,15 +216,15 @@
                 "Type": "forward",
                 "TargetGroupArn": tg_arn,
             },
         ],
     )["Listeners"][0]["ListenerArn"]
 
     # Call the get_tgs_no_targets_or_lb function
-    target_groups = get_tgs_no_targets_or_lb(session)
+    target_groups = scan_for_tgs_no_targets_or_lb(session)
 
     # Verify that the target group is returned by the function
     assert tg_arn in target_groups
 
     ami_id = ec2_client.describe_images()["Images"][0]["ImageId"]
 
     # Create a mock EC2 instance
@@ -265,15 +253,15 @@
                 "Id": instance_id,
                 "Port": 80,
             },
         ],
     )
 
     # Call the get_tgs_no_targets_or_lb function
-    target_groups = get_tgs_no_targets_or_lb(session)
+    target_groups = scan_for_tgs_no_targets_or_lb(session)
 
     # Verify that the target group is not returned by the function
     assert tg_arn not in target_groups
 
     # Remove the load balancer from the target group
     elb_client.delete_listener(
         ListenerArn=listener_arn,
@@ -285,23 +273,23 @@
                 "Id": instance_id,
                 "Port": 80,
             },
         ],
     )
 
     # Call the get_tgs_no_targets_or_lb function
-    target_groups = get_tgs_no_targets_or_lb(session)
+    target_groups = scan_for_tgs_no_targets_or_lb(session)
 
     # Verify that the target group is returned by the function
     assert tg_arn in target_groups
 
 
 @mock_ec2
 @mock_elbv2
-def test_get_lbs_no_targets():
+def test_scan_for_lbs_no_targets():
     region = "us-east-1"
     # Create a mock AWS session
     session = boto3.Session(
         region_name="us-east-1",
         aws_access_key_id="mock_access_key",
         aws_secret_access_key="mock_secret_key",
     )
@@ -344,10 +332,90 @@
                 "Type": "forward",
                 "TargetGroupArn": tg_arn,
             },
         ],
     )["Listeners"][0]["ListenerArn"]
 
     # Call the get_lbs_no_targets function
-    load_balancers = get_lbs_no_targets(session, region, omit_pricing=True)
+    load_balancers = scan_for_lbs_no_targets(session, region, omit_pricing=True)
 
     assert elb_arn in load_balancers
+
+
+@mock_ec2
+def test_scan_for_unused_ebs_volumes():
+    session = boto3.Session(region_name="us-east-1")
+    client = session.client("ec2")
+
+    # Create an EBS volume
+    client.create_volume(AvailabilityZone="us-east-1a", Size=1, VolumeType="gp2")
+
+    # Get the list of all EBS volumes in the region
+    volumes = client.describe_volumes()["Volumes"]
+
+    # Filter the list to include only volumes that are not attached to any EC2 instances
+    unused_volumes = [volume for volume in volumes if volume["State"] == "available"]
+
+    # Assert that the list is not empty
+    assert len(unused_volumes) > 0
+
+    # Assert that the list contains the EBS volume that we created
+    assert len([volume for volume in unused_volumes if volume["Size"] == 1]) == 1
+
+
+@mock_ec2
+def test_delete_ebs_volumes():
+    session = boto3.Session(region_name="us-east-1")
+    ec2 = session.resource("ec2")
+
+    # create a volume to delete
+    volume = ec2.create_volume(AvailabilityZone="us-east-1a", Size=10)
+
+    # delete the volume and confirm it is deleted
+    assert delete_ebs_volumes([volume.id], session) is None
+    assert list(ec2.volumes.all()) == []
+
+
+@mock_s3
+def test_get_old_buckets():
+    # Create a boto3 session for testing
+    session = boto3.Session(region_name="us-east-1")
+
+    # Create a client for the S3 service
+    s3 = session.client("s3")
+
+    # Create a test bucket
+    s3.create_bucket(Bucket="test-bucket")
+
+    # Check that the function correctly identifies an empty bucket as old
+    buckets = get_buckets(session, 365)
+    assert "test-bucket" in buckets["empty"]
+
+    # Add a new object to the test bucket
+    s3.put_object(Bucket="test-bucket", Key="test.txt", Body=b"test")
+
+    # Check that the function does not consider the bucket to be old
+    buckets = get_buckets(session, 365)
+    assert "test-bucket" not in buckets["old"]
+
+
+@mock_s3
+def test_get_bucket_cost():
+    # Create a boto3 session for testing
+    session = boto3.Session(region_name="us-east-1")
+
+    # Create a client for the S3 service
+    s3 = session.client("s3")
+
+    # Create a test bucket
+    s3.create_bucket(Bucket="test-bucket")
+
+    # Check that the cost of an empty bucket is 0
+    cost = get_bucket_cost(session, "test-bucket")
+    assert cost == 0
+
+    # Add an object to the test bucket
+    s3.put_object(Bucket="test-bucket", Key="test.txt", Body=b"0123456789")
+
+    # Check that the cost of the bucket is calculated correctly
+    cost = get_bucket_cost(session, "test-bucket")
+    assert cost > 0
```

### Comparing `aws_cost_mutilator-0.1.0/pyproject.toml` & `aws_cost_mutilator-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "aws-cost-mutilator"
-version = "0.1.0"
+version = "0.2.0"
 description = "A cli to mutilate aws costs, it's what accounting craves."
 authors = ["Sky Moore <i@msky.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/skymoore/aws-cost-mutilator"
 keywords = ["aws", "cloud"]
-classifiers = ["Intended Audience :: Developers", "Natural Language :: English", "Programming Language :: Python :: 3.10",]
+classifiers = ["Intended Audience :: Developers", "Natural Language :: English", "Programming Language :: Python :: 3.11",]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 boto3 = "^1.34.99"
 click = "^8.1.7"
 tqdm = "^4.64.1"
 
 [tool.poetry.dev-dependencies]
 moto = "^4.0.11"
 pytest = "^7.2.0"
```

