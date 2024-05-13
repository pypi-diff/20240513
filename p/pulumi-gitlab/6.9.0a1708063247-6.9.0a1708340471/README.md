# Comparing `tmp/pulumi_gitlab-6.9.0a1708063247.tar.gz` & `tmp/pulumi_gitlab-6.9.0a1708340471.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_gitlab-6.9.0a1708063247.tar", last modified: Fri Feb 16 06:03:56 2024, max compression
+gzip compressed data, was "pulumi_gitlab-6.9.0a1708340471.tar", last modified: Mon Feb 19 11:04:52 2024, max compression
```

## Comparing `pulumi_gitlab-6.9.0a1708063247.tar` & `pulumi_gitlab-6.9.0a1708340471.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:03:56.503902 pulumi_gitlab-6.9.0a1708063247/
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-02-16 06:03:56.503902 pulumi_gitlab-6.9.0a1708063247/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:03:56.499902 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    90977 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    19366 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/application.py
--rw-r--r--   0 runner    (1001) docker     (127)   693424 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/application_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    19638 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    31974 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/branch_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/cluster_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    21353 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/cluster_agent_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    21839 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/compliance_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:03:56.503902 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    14138 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/deploy_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/deploy_key_enable.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/deploy_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     7993 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_cluster_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_cluster_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_current_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_group_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_group_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_group_membership.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_group_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8146 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_group_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_group_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_instance_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_instance_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_instance_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    45634 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_branches.py
--rw-r--r--   0 runner    (1001) docker     (127)    13966 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    24930 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_issue.py
--rw-r--r--   0 runner    (1001) docker     (127)    28861 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_membership.py
--rw-r--r--   0 runner    (1001) docker     (127)     9756 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_milestone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_milestones.py
--rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_protected_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_protected_branches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    24982 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_release_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_release_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_repository_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    18316 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_user_sshkeys.py
--rw-r--r--   0 runner    (1001) docker     (127)    11103 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    49573 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/global_level_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)    77301 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_badge.py
--rw-r--r--   0 runner    (1001) docker     (127)    33677 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    10030 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_epic_board.py
--rw-r--r--   0 runner    (1001) docker     (127)    46607 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_issue_board.py
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_label.py
--rw-r--r--   0 runner    (1001) docker     (127)    24122 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_ldap_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    20006 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_membership.py
--rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_project_file_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    19376 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_protected_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_saml_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_share_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    23000 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    34417 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/instance_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    18251 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/instance_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    17058 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_custom_issue_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_emails_on_push.py
--rw-r--r--   0 runner    (1001) docker     (127)    15424 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_external_wiki.py
--rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    45239 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_jira.py
--rw-r--r--   0 runner    (1001) docker     (127)    57608 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_mattermost.py
--rw-r--r--   0 runner    (1001) docker     (127)    38074 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_microsoft_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)    15602 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_pipelines_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    60130 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_slack.py
--rw-r--r--   0 runner    (1001) docker     (127)    13052 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/label.py
--rw-r--r--   0 runner    (1001) docker     (127)   273416 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22868 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/pages_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    20181 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/personal_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    22167 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/pipeline_schedule_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    11098 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/pipeline_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)   269138 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    23818 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    27480 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_approval_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    17057 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_badge.py
--rw-r--r--   0 runner    (1001) docker     (127)    36174 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_compliance_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    18416 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13421 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_freeze_period.py
--rw-r--r--   0 runner    (1001) docker     (127)    43656 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    73617 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_issue.py
--rw-r--r--   0 runner    (1001) docker     (127)    19785 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_issue_board.py
--rw-r--r--   0 runner    (1001) docker     (127)     8875 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_job_token_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_label.py
--rw-r--r--   0 runner    (1001) docker     (127)    26629 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_level_mr_approvals.py
--rw-r--r--   0 runner    (1001) docker     (127)    50634 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_level_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)    13986 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_membership.py
--rw-r--r--   0 runner    (1001) docker     (127)    25236 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_milestone.py
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_mirror.py
--rw-r--r--   0 runner    (1001) docker     (127)    19233 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_protected_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_runner_enablement.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_share_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    23750 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21521 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/release_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    41365 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/repository_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    29221 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_custom_issue_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    26696 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_emails_on_push.py
--rw-r--r--   0 runner    (1001) docker     (127)    15460 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_external_wiki.py
--rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    45259 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_jira.py
--rw-r--r--   0 runner    (1001) docker     (127)    38114 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_microsoft_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)    15642 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_pipelines_email.py
--rw-r--r--   0 runner    (1001) docker     (127)    60152 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_slack.py
--rw-r--r--   0 runner    (1001) docker     (127)    21892 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/system_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    14206 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/tag_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20565 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    32464 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/user_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/user_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    26708 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/user_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    16500 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/user_ssh_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 06:03:56.503902 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-02-16 06:03:56.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-02-16 06:03:56.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 06:03:56.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-16 06:03:56.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-16 06:03:56.000000 pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-16 06:03:45.000000 pulumi_gitlab-6.9.0a1708063247/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 06:03:56.503902 pulumi_gitlab-6.9.0a1708063247/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:04:52.696489 pulumi_gitlab-6.9.0a1708340471/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-02-19 11:04:52.696489 pulumi_gitlab-6.9.0a1708340471/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:04:52.696489 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90977 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19366 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)   693424 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19638 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31974 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/branch_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/cluster_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21353 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/cluster_agent_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21839 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/compliance_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:04:52.696489 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14138 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/deploy_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/deploy_key_enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/deploy_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7993 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_cluster_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_cluster_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_current_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_group_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_group_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_group_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_group_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_instance_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_instance_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_instance_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46611 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13966 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24930 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28861 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9756 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_milestones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_protected_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_protected_branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24982 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_release_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_release_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_repository_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18316 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_user_sshkeys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11103 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49573 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/global_level_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77301 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33677 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10030 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_epic_board.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46607 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_issue_board.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24122 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_ldap_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20006 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_project_file_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19376 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_protected_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_saml_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_share_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24834 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34417 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/instance_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18251 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/instance_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17058 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_custom_issue_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_emails_on_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15424 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_external_wiki.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45239 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57608 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_mattermost.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38074 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_microsoft_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15602 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_pipelines_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60130 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13052 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)   274874 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22868 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/pages_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20181 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/personal_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22167 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/pipeline_schedule_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11098 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/pipeline_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)   272775 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23818 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27480 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_approval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17057 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36174 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_compliance_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18416 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13421 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_freeze_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43656 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73617 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19785 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_issue_board.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8875 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_job_token_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26629 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_level_mr_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50634 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_level_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13986 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25236 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19233 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_protected_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_runner_enablement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_share_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25584 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21521 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/release_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41365 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29221 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_custom_issue_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26696 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_emails_on_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15460 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_external_wiki.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45259 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38114 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_microsoft_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15642 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_pipelines_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60152 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21892 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/system_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14206 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/tag_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20565 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32464 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/user_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/user_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26708 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/user_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16500 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/user_ssh_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 11:04:52.696489 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-02-19 11:04:52.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-02-19 11:04:52.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 11:04:52.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-19 11:04:52.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-19 11:04:52.000000 pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-19 11:04:42.000000 pulumi_gitlab-6.9.0a1708340471/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 11:04:52.696489 pulumi_gitlab-6.9.0a1708340471/setup.cfg
```

### Comparing `pulumi_gitlab-6.9.0a1708063247/PKG-INFO` & `pulumi_gitlab-6.9.0a1708340471/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_gitlab
-Version: 6.9.0a1708063247
+Version: 6.9.0a1708340471
 Summary: A Pulumi package for creating and managing GitLab resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-gitlab
 Keywords: pulumi,gitlab
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_gitlab-6.9.0a1708063247/README.md` & `pulumi_gitlab-6.9.0a1708340471/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/__init__.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/_inputs.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/_utilities.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/application.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/application.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/application_settings.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/application_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,17 +77,17 @@
                  elasticsearch_aws_secret_access_key: Optional[pulumi.Input[str]] = None,
                  elasticsearch_indexed_field_length_limit: Optional[pulumi.Input[int]] = None,
                  elasticsearch_indexed_file_size_limit_kb: Optional[pulumi.Input[int]] = None,
                  elasticsearch_indexing: Optional[pulumi.Input[bool]] = None,
                  elasticsearch_limit_indexing: Optional[pulumi.Input[bool]] = None,
                  elasticsearch_max_bulk_concurrency: Optional[pulumi.Input[int]] = None,
                  elasticsearch_max_bulk_size_mb: Optional[pulumi.Input[int]] = None,
-                 elasticsearch_namespace_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 elasticsearch_namespace_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  elasticsearch_password: Optional[pulumi.Input[str]] = None,
-                 elasticsearch_project_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 elasticsearch_project_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  elasticsearch_search: Optional[pulumi.Input[bool]] = None,
                  elasticsearch_urls: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  elasticsearch_username: Optional[pulumi.Input[str]] = None,
                  email_additional_text: Optional[pulumi.Input[str]] = None,
                  email_author_in_body: Optional[pulumi.Input[bool]] = None,
                  enabled_git_access_protocol: Optional[pulumi.Input[str]] = None,
                  enforce_namespace_storage_limit: Optional[pulumi.Input[bool]] = None,
@@ -320,17 +320,17 @@
         :param pulumi.Input[str] elasticsearch_aws_secret_access_key: AWS IAM secret access key.
         :param pulumi.Input[int] elasticsearch_indexed_field_length_limit: Maximum size of text fields to index by Elasticsearch. 0 value means no limit. This does not apply to repository and wiki indexing.
         :param pulumi.Input[int] elasticsearch_indexed_file_size_limit_kb: Maximum size of repository and wiki files that are indexed by Elasticsearch.
         :param pulumi.Input[bool] elasticsearch_indexing: Enable Elasticsearch indexing.
         :param pulumi.Input[bool] elasticsearch_limit_indexing: Limit Elasticsearch to index certain namespaces and projects.
         :param pulumi.Input[int] elasticsearch_max_bulk_concurrency: Maximum concurrency of Elasticsearch bulk requests per indexing operation. This only applies to repository indexing operations.
         :param pulumi.Input[int] elasticsearch_max_bulk_size_mb: Maximum size of Elasticsearch bulk indexing requests in MB. This only applies to repository indexing operations.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elasticsearch_namespace_ids: The namespaces to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
+        :param pulumi.Input[Sequence[pulumi.Input[int]]] elasticsearch_namespace_ids: The namespaces to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
         :param pulumi.Input[str] elasticsearch_password: The password of your Elasticsearch instance.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elasticsearch_project_ids: The projects to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
+        :param pulumi.Input[Sequence[pulumi.Input[int]]] elasticsearch_project_ids: The projects to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
         :param pulumi.Input[bool] elasticsearch_search: Enable Elasticsearch search.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elasticsearch_urls: The URL to use for connecting to Elasticsearch. Use a comma-separated list to support cluster (for example, http://localhost:9200, http://localhost:9201).
         :param pulumi.Input[str] elasticsearch_username: The username of your Elasticsearch instance.
         :param pulumi.Input[str] email_additional_text: Additional text added to the bottom of every email for legal/auditing/compliance reasons.
         :param pulumi.Input[bool] email_author_in_body: Some email servers do not support overriding the email sender name. Enable this option to include the name of the author of the issue, merge request or comment in the email body instead.
         :param pulumi.Input[str] enabled_git_access_protocol: Enabled protocols for Git access. Allowed values are: ssh, http, and nil to allow both protocols.
         :param pulumi.Input[bool] enforce_namespace_storage_limit: Enabling this permits enforcement of namespace storage limits.
@@ -1795,22 +1795,22 @@
 
     @elasticsearch_max_bulk_size_mb.setter
     def elasticsearch_max_bulk_size_mb(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "elasticsearch_max_bulk_size_mb", value)
 
     @property
     @pulumi.getter(name="elasticsearchNamespaceIds")
-    def elasticsearch_namespace_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def elasticsearch_namespace_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]:
         """
         The namespaces to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
         """
         return pulumi.get(self, "elasticsearch_namespace_ids")
 
     @elasticsearch_namespace_ids.setter
-    def elasticsearch_namespace_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+    def elasticsearch_namespace_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]):
         pulumi.set(self, "elasticsearch_namespace_ids", value)
 
     @property
     @pulumi.getter(name="elasticsearchPassword")
     def elasticsearch_password(self) -> Optional[pulumi.Input[str]]:
         """
         The password of your Elasticsearch instance.
@@ -1819,22 +1819,22 @@
 
     @elasticsearch_password.setter
     def elasticsearch_password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "elasticsearch_password", value)
 
     @property
     @pulumi.getter(name="elasticsearchProjectIds")
-    def elasticsearch_project_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def elasticsearch_project_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]:
         """
         The projects to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
         """
         return pulumi.get(self, "elasticsearch_project_ids")
 
     @elasticsearch_project_ids.setter
-    def elasticsearch_project_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+    def elasticsearch_project_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]):
         pulumi.set(self, "elasticsearch_project_ids", value)
 
     @property
     @pulumi.getter(name="elasticsearchSearch")
     def elasticsearch_search(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable Elasticsearch search.
@@ -3963,17 +3963,17 @@
                  elasticsearch_aws_secret_access_key: Optional[pulumi.Input[str]] = None,
                  elasticsearch_indexed_field_length_limit: Optional[pulumi.Input[int]] = None,
                  elasticsearch_indexed_file_size_limit_kb: Optional[pulumi.Input[int]] = None,
                  elasticsearch_indexing: Optional[pulumi.Input[bool]] = None,
                  elasticsearch_limit_indexing: Optional[pulumi.Input[bool]] = None,
                  elasticsearch_max_bulk_concurrency: Optional[pulumi.Input[int]] = None,
                  elasticsearch_max_bulk_size_mb: Optional[pulumi.Input[int]] = None,
-                 elasticsearch_namespace_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 elasticsearch_namespace_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  elasticsearch_password: Optional[pulumi.Input[str]] = None,
-                 elasticsearch_project_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 elasticsearch_project_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  elasticsearch_search: Optional[pulumi.Input[bool]] = None,
                  elasticsearch_urls: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  elasticsearch_username: Optional[pulumi.Input[str]] = None,
                  email_additional_text: Optional[pulumi.Input[str]] = None,
                  email_author_in_body: Optional[pulumi.Input[bool]] = None,
                  enabled_git_access_protocol: Optional[pulumi.Input[str]] = None,
                  enforce_namespace_storage_limit: Optional[pulumi.Input[bool]] = None,
@@ -4206,17 +4206,17 @@
         :param pulumi.Input[str] elasticsearch_aws_secret_access_key: AWS IAM secret access key.
         :param pulumi.Input[int] elasticsearch_indexed_field_length_limit: Maximum size of text fields to index by Elasticsearch. 0 value means no limit. This does not apply to repository and wiki indexing.
         :param pulumi.Input[int] elasticsearch_indexed_file_size_limit_kb: Maximum size of repository and wiki files that are indexed by Elasticsearch.
         :param pulumi.Input[bool] elasticsearch_indexing: Enable Elasticsearch indexing.
         :param pulumi.Input[bool] elasticsearch_limit_indexing: Limit Elasticsearch to index certain namespaces and projects.
         :param pulumi.Input[int] elasticsearch_max_bulk_concurrency: Maximum concurrency of Elasticsearch bulk requests per indexing operation. This only applies to repository indexing operations.
         :param pulumi.Input[int] elasticsearch_max_bulk_size_mb: Maximum size of Elasticsearch bulk indexing requests in MB. This only applies to repository indexing operations.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elasticsearch_namespace_ids: The namespaces to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
+        :param pulumi.Input[Sequence[pulumi.Input[int]]] elasticsearch_namespace_ids: The namespaces to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
         :param pulumi.Input[str] elasticsearch_password: The password of your Elasticsearch instance.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elasticsearch_project_ids: The projects to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
+        :param pulumi.Input[Sequence[pulumi.Input[int]]] elasticsearch_project_ids: The projects to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
         :param pulumi.Input[bool] elasticsearch_search: Enable Elasticsearch search.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elasticsearch_urls: The URL to use for connecting to Elasticsearch. Use a comma-separated list to support cluster (for example, http://localhost:9200, http://localhost:9201).
         :param pulumi.Input[str] elasticsearch_username: The username of your Elasticsearch instance.
         :param pulumi.Input[str] email_additional_text: Additional text added to the bottom of every email for legal/auditing/compliance reasons.
         :param pulumi.Input[bool] email_author_in_body: Some email servers do not support overriding the email sender name. Enable this option to include the name of the author of the issue, merge request or comment in the email body instead.
         :param pulumi.Input[str] enabled_git_access_protocol: Enabled protocols for Git access. Allowed values are: ssh, http, and nil to allow both protocols.
         :param pulumi.Input[bool] enforce_namespace_storage_limit: Enabling this permits enforcement of namespace storage limits.
@@ -5681,22 +5681,22 @@
 
     @elasticsearch_max_bulk_size_mb.setter
     def elasticsearch_max_bulk_size_mb(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "elasticsearch_max_bulk_size_mb", value)
 
     @property
     @pulumi.getter(name="elasticsearchNamespaceIds")
-    def elasticsearch_namespace_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def elasticsearch_namespace_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]:
         """
         The namespaces to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
         """
         return pulumi.get(self, "elasticsearch_namespace_ids")
 
     @elasticsearch_namespace_ids.setter
-    def elasticsearch_namespace_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+    def elasticsearch_namespace_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]):
         pulumi.set(self, "elasticsearch_namespace_ids", value)
 
     @property
     @pulumi.getter(name="elasticsearchPassword")
     def elasticsearch_password(self) -> Optional[pulumi.Input[str]]:
         """
         The password of your Elasticsearch instance.
@@ -5705,22 +5705,22 @@
 
     @elasticsearch_password.setter
     def elasticsearch_password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "elasticsearch_password", value)
 
     @property
     @pulumi.getter(name="elasticsearchProjectIds")
-    def elasticsearch_project_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def elasticsearch_project_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]:
         """
         The projects to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
         """
         return pulumi.get(self, "elasticsearch_project_ids")
 
     @elasticsearch_project_ids.setter
-    def elasticsearch_project_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+    def elasticsearch_project_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]):
         pulumi.set(self, "elasticsearch_project_ids", value)
 
     @property
     @pulumi.getter(name="elasticsearchSearch")
     def elasticsearch_search(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable Elasticsearch search.
@@ -7851,17 +7851,17 @@
                  elasticsearch_aws_secret_access_key: Optional[pulumi.Input[str]] = None,
                  elasticsearch_indexed_field_length_limit: Optional[pulumi.Input[int]] = None,
                  elasticsearch_indexed_file_size_limit_kb: Optional[pulumi.Input[int]] = None,
                  elasticsearch_indexing: Optional[pulumi.Input[bool]] = None,
                  elasticsearch_limit_indexing: Optional[pulumi.Input[bool]] = None,
                  elasticsearch_max_bulk_concurrency: Optional[pulumi.Input[int]] = None,
                  elasticsearch_max_bulk_size_mb: Optional[pulumi.Input[int]] = None,
-                 elasticsearch_namespace_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 elasticsearch_namespace_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  elasticsearch_password: Optional[pulumi.Input[str]] = None,
-                 elasticsearch_project_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 elasticsearch_project_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  elasticsearch_search: Optional[pulumi.Input[bool]] = None,
                  elasticsearch_urls: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  elasticsearch_username: Optional[pulumi.Input[str]] = None,
                  email_additional_text: Optional[pulumi.Input[str]] = None,
                  email_author_in_body: Optional[pulumi.Input[bool]] = None,
                  enabled_git_access_protocol: Optional[pulumi.Input[str]] = None,
                  enforce_namespace_storage_limit: Optional[pulumi.Input[bool]] = None,
@@ -8108,17 +8108,17 @@
         :param pulumi.Input[str] elasticsearch_aws_secret_access_key: AWS IAM secret access key.
         :param pulumi.Input[int] elasticsearch_indexed_field_length_limit: Maximum size of text fields to index by Elasticsearch. 0 value means no limit. This does not apply to repository and wiki indexing.
         :param pulumi.Input[int] elasticsearch_indexed_file_size_limit_kb: Maximum size of repository and wiki files that are indexed by Elasticsearch.
         :param pulumi.Input[bool] elasticsearch_indexing: Enable Elasticsearch indexing.
         :param pulumi.Input[bool] elasticsearch_limit_indexing: Limit Elasticsearch to index certain namespaces and projects.
         :param pulumi.Input[int] elasticsearch_max_bulk_concurrency: Maximum concurrency of Elasticsearch bulk requests per indexing operation. This only applies to repository indexing operations.
         :param pulumi.Input[int] elasticsearch_max_bulk_size_mb: Maximum size of Elasticsearch bulk indexing requests in MB. This only applies to repository indexing operations.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elasticsearch_namespace_ids: The namespaces to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
+        :param pulumi.Input[Sequence[pulumi.Input[int]]] elasticsearch_namespace_ids: The namespaces to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
         :param pulumi.Input[str] elasticsearch_password: The password of your Elasticsearch instance.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elasticsearch_project_ids: The projects to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
+        :param pulumi.Input[Sequence[pulumi.Input[int]]] elasticsearch_project_ids: The projects to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
         :param pulumi.Input[bool] elasticsearch_search: Enable Elasticsearch search.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elasticsearch_urls: The URL to use for connecting to Elasticsearch. Use a comma-separated list to support cluster (for example, http://localhost:9200, http://localhost:9201).
         :param pulumi.Input[str] elasticsearch_username: The username of your Elasticsearch instance.
         :param pulumi.Input[str] email_additional_text: Additional text added to the bottom of every email for legal/auditing/compliance reasons.
         :param pulumi.Input[bool] email_author_in_body: Some email servers do not support overriding the email sender name. Enable this option to include the name of the author of the issue, merge request or comment in the email body instead.
         :param pulumi.Input[str] enabled_git_access_protocol: Enabled protocols for Git access. Allowed values are: ssh, http, and nil to allow both protocols.
         :param pulumi.Input[bool] enforce_namespace_storage_limit: Enabling this permits enforcement of namespace storage limits.
@@ -8386,17 +8386,17 @@
                  elasticsearch_aws_secret_access_key: Optional[pulumi.Input[str]] = None,
                  elasticsearch_indexed_field_length_limit: Optional[pulumi.Input[int]] = None,
                  elasticsearch_indexed_file_size_limit_kb: Optional[pulumi.Input[int]] = None,
                  elasticsearch_indexing: Optional[pulumi.Input[bool]] = None,
                  elasticsearch_limit_indexing: Optional[pulumi.Input[bool]] = None,
                  elasticsearch_max_bulk_concurrency: Optional[pulumi.Input[int]] = None,
                  elasticsearch_max_bulk_size_mb: Optional[pulumi.Input[int]] = None,
-                 elasticsearch_namespace_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 elasticsearch_namespace_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  elasticsearch_password: Optional[pulumi.Input[str]] = None,
-                 elasticsearch_project_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 elasticsearch_project_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  elasticsearch_search: Optional[pulumi.Input[bool]] = None,
                  elasticsearch_urls: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  elasticsearch_username: Optional[pulumi.Input[str]] = None,
                  email_additional_text: Optional[pulumi.Input[str]] = None,
                  email_author_in_body: Optional[pulumi.Input[bool]] = None,
                  enabled_git_access_protocol: Optional[pulumi.Input[str]] = None,
                  enforce_namespace_storage_limit: Optional[pulumi.Input[bool]] = None,
@@ -8889,17 +8889,17 @@
             elasticsearch_aws_secret_access_key: Optional[pulumi.Input[str]] = None,
             elasticsearch_indexed_field_length_limit: Optional[pulumi.Input[int]] = None,
             elasticsearch_indexed_file_size_limit_kb: Optional[pulumi.Input[int]] = None,
             elasticsearch_indexing: Optional[pulumi.Input[bool]] = None,
             elasticsearch_limit_indexing: Optional[pulumi.Input[bool]] = None,
             elasticsearch_max_bulk_concurrency: Optional[pulumi.Input[int]] = None,
             elasticsearch_max_bulk_size_mb: Optional[pulumi.Input[int]] = None,
-            elasticsearch_namespace_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            elasticsearch_namespace_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
             elasticsearch_password: Optional[pulumi.Input[str]] = None,
-            elasticsearch_project_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            elasticsearch_project_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
             elasticsearch_search: Optional[pulumi.Input[bool]] = None,
             elasticsearch_urls: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             elasticsearch_username: Optional[pulumi.Input[str]] = None,
             email_additional_text: Optional[pulumi.Input[str]] = None,
             email_author_in_body: Optional[pulumi.Input[bool]] = None,
             enabled_git_access_protocol: Optional[pulumi.Input[str]] = None,
             enforce_namespace_storage_limit: Optional[pulumi.Input[bool]] = None,
@@ -9137,17 +9137,17 @@
         :param pulumi.Input[str] elasticsearch_aws_secret_access_key: AWS IAM secret access key.
         :param pulumi.Input[int] elasticsearch_indexed_field_length_limit: Maximum size of text fields to index by Elasticsearch. 0 value means no limit. This does not apply to repository and wiki indexing.
         :param pulumi.Input[int] elasticsearch_indexed_file_size_limit_kb: Maximum size of repository and wiki files that are indexed by Elasticsearch.
         :param pulumi.Input[bool] elasticsearch_indexing: Enable Elasticsearch indexing.
         :param pulumi.Input[bool] elasticsearch_limit_indexing: Limit Elasticsearch to index certain namespaces and projects.
         :param pulumi.Input[int] elasticsearch_max_bulk_concurrency: Maximum concurrency of Elasticsearch bulk requests per indexing operation. This only applies to repository indexing operations.
         :param pulumi.Input[int] elasticsearch_max_bulk_size_mb: Maximum size of Elasticsearch bulk indexing requests in MB. This only applies to repository indexing operations.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elasticsearch_namespace_ids: The namespaces to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
+        :param pulumi.Input[Sequence[pulumi.Input[int]]] elasticsearch_namespace_ids: The namespaces to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
         :param pulumi.Input[str] elasticsearch_password: The password of your Elasticsearch instance.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] elasticsearch_project_ids: The projects to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
+        :param pulumi.Input[Sequence[pulumi.Input[int]]] elasticsearch_project_ids: The projects to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
         :param pulumi.Input[bool] elasticsearch_search: Enable Elasticsearch search.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] elasticsearch_urls: The URL to use for connecting to Elasticsearch. Use a comma-separated list to support cluster (for example, http://localhost:9200, http://localhost:9201).
         :param pulumi.Input[str] elasticsearch_username: The username of your Elasticsearch instance.
         :param pulumi.Input[str] email_additional_text: Additional text added to the bottom of every email for legal/auditing/compliance reasons.
         :param pulumi.Input[bool] email_author_in_body: Some email servers do not support overriding the email sender name. Enable this option to include the name of the author of the issue, merge request or comment in the email body instead.
         :param pulumi.Input[str] enabled_git_access_protocol: Enabled protocols for Git access. Allowed values are: ssh, http, and nil to allow both protocols.
         :param pulumi.Input[bool] enforce_namespace_storage_limit: Enabling this permits enforcement of namespace storage limits.
@@ -10099,15 +10099,15 @@
         """
         Maximum size of Elasticsearch bulk indexing requests in MB. This only applies to repository indexing operations.
         """
         return pulumi.get(self, "elasticsearch_max_bulk_size_mb")
 
     @property
     @pulumi.getter(name="elasticsearchNamespaceIds")
-    def elasticsearch_namespace_ids(self) -> pulumi.Output[Sequence[str]]:
+    def elasticsearch_namespace_ids(self) -> pulumi.Output[Sequence[int]]:
         """
         The namespaces to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
         """
         return pulumi.get(self, "elasticsearch_namespace_ids")
 
     @property
     @pulumi.getter(name="elasticsearchPassword")
@@ -10115,15 +10115,15 @@
         """
         The password of your Elasticsearch instance.
         """
         return pulumi.get(self, "elasticsearch_password")
 
     @property
     @pulumi.getter(name="elasticsearchProjectIds")
-    def elasticsearch_project_ids(self) -> pulumi.Output[Sequence[str]]:
+    def elasticsearch_project_ids(self) -> pulumi.Output[Sequence[int]]:
         """
         The projects to index via Elasticsearch if elasticsearch*limit*indexing is enabled.
         """
         return pulumi.get(self, "elasticsearch_project_ids")
 
     @property
     @pulumi.getter(name="elasticsearchSearch")
```

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/branch.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/branch_protection.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/branch_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/cluster_agent.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/cluster_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/cluster_agent_token.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/cluster_agent_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/compliance_framework.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/compliance_framework.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/config/__init__.pyi` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/config/vars.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/deploy_key.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/deploy_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/deploy_key_enable.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/deploy_key_enable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/deploy_token.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/deploy_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_application.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_branch.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_cluster_agent.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_cluster_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_cluster_agents.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_cluster_agents.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_current_user.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_current_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_group.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_group_hook.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_group_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_group_hooks.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_group_hooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_group_membership.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_group_subgroups.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_group_subgroups.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_group_variable.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_group_variable.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 ]
 
 @pulumi.output_type
 class GetGroupVariableResult:
     """
     A collection of values returned by getGroupVariable.
     """
-    def __init__(__self__, environment_scope=None, group=None, id=None, key=None, masked=None, protected=None, raw=None, value=None, variable_type=None):
+    def __init__(__self__, description=None, environment_scope=None, group=None, id=None, key=None, masked=None, protected=None, raw=None, value=None, variable_type=None):
+        if description and not isinstance(description, str):
+            raise TypeError("Expected argument 'description' to be a str")
+        pulumi.set(__self__, "description", description)
         if environment_scope and not isinstance(environment_scope, str):
             raise TypeError("Expected argument 'environment_scope' to be a str")
         pulumi.set(__self__, "environment_scope", environment_scope)
         if group and not isinstance(group, str):
             raise TypeError("Expected argument 'group' to be a str")
         pulumi.set(__self__, "group", group)
         if id and not isinstance(id, str):
@@ -47,14 +50,22 @@
             raise TypeError("Expected argument 'value' to be a str")
         pulumi.set(__self__, "value", value)
         if variable_type and not isinstance(variable_type, str):
             raise TypeError("Expected argument 'variable_type' to be a str")
         pulumi.set(__self__, "variable_type", variable_type)
 
     @property
+    @pulumi.getter
+    def description(self) -> str:
+        """
+        The description of the variable.
+        """
+        return pulumi.get(self, "description")
+
+    @property
     @pulumi.getter(name="environmentScope")
     def environment_scope(self) -> str:
         """
         The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         """
         return pulumi.get(self, "environment_scope")
 
@@ -125,14 +136,15 @@
 
 class AwaitableGetGroupVariableResult(GetGroupVariableResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetGroupVariableResult(
+            description=self.description,
             environment_scope=self.environment_scope,
             group=self.group,
             id=self.id,
             key=self.key,
             masked=self.masked,
             protected=self.protected,
             raw=self.raw,
@@ -171,14 +183,15 @@
     __args__['environmentScope'] = environment_scope
     __args__['group'] = group
     __args__['key'] = key
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getGroupVariable:getGroupVariable', __args__, opts=opts, typ=GetGroupVariableResult).value
 
     return AwaitableGetGroupVariableResult(
+        description=pulumi.get(__ret__, 'description'),
         environment_scope=pulumi.get(__ret__, 'environment_scope'),
         group=pulumi.get(__ret__, 'group'),
         id=pulumi.get(__ret__, 'id'),
         key=pulumi.get(__ret__, 'key'),
         masked=pulumi.get(__ret__, 'masked'),
         protected=pulumi.get(__ret__, 'protected'),
         raw=pulumi.get(__ret__, 'raw'),
```

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_group_variables.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_group_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_groups.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_instance_deploy_keys.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_instance_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_instance_variable.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_instance_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_instance_variables.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_instance_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_metadata.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_metadata.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetProjectResult:
     """
     A collection of values returned by getProject.
     """
-    def __init__(__self__, analytics_access_level=None, archived=None, auto_cancel_pending_pipelines=None, auto_devops_deploy_strategy=None, auto_devops_enabled=None, autoclose_referenced_issues=None, build_git_strategy=None, build_timeout=None, builds_access_level=None, ci_config_path=None, ci_default_git_depth=None, ci_separated_caches=None, container_expiration_policies=None, container_registry_access_level=None, default_branch=None, description=None, emails_disabled=None, empty_repo=None, environments_access_level=None, external_authorization_classification_label=None, feature_flags_access_level=None, forking_access_level=None, http_url_to_repo=None, id=None, import_url=None, infrastructure_access_level=None, issues_access_level=None, issues_enabled=None, keep_latest_artifact=None, lfs_enabled=None, merge_commit_template=None, merge_pipelines_enabled=None, merge_requests_access_level=None, merge_requests_enabled=None, merge_trains_enabled=None, monitor_access_level=None, name=None, namespace_id=None, path=None, path_with_namespace=None, pipelines_enabled=None, printing_merge_request_link_enabled=None, public_builds=None, push_rules=None, releases_access_level=None, remove_source_branch_after_merge=None, repository_access_level=None, repository_storage=None, request_access_enabled=None, requirements_access_level=None, resolve_outdated_diff_discussions=None, restrict_user_defined_variables=None, runners_token=None, security_and_compliance_access_level=None, shared_with_groups=None, snippets_access_level=None, snippets_enabled=None, squash_commit_template=None, ssh_url_to_repo=None, suggestion_commit_message=None, topics=None, visibility_level=None, web_url=None, wiki_access_level=None, wiki_enabled=None):
+    def __init__(__self__, analytics_access_level=None, archived=None, auto_cancel_pending_pipelines=None, auto_devops_deploy_strategy=None, auto_devops_enabled=None, autoclose_referenced_issues=None, build_git_strategy=None, build_timeout=None, builds_access_level=None, ci_config_path=None, ci_default_git_depth=None, ci_restrict_pipeline_cancellation_role=None, ci_separated_caches=None, container_expiration_policies=None, container_registry_access_level=None, default_branch=None, description=None, emails_disabled=None, empty_repo=None, environments_access_level=None, external_authorization_classification_label=None, feature_flags_access_level=None, forking_access_level=None, http_url_to_repo=None, id=None, import_url=None, infrastructure_access_level=None, issues_access_level=None, issues_enabled=None, keep_latest_artifact=None, lfs_enabled=None, merge_commit_template=None, merge_pipelines_enabled=None, merge_requests_access_level=None, merge_requests_enabled=None, merge_trains_enabled=None, monitor_access_level=None, name=None, namespace_id=None, path=None, path_with_namespace=None, pipelines_enabled=None, printing_merge_request_link_enabled=None, public_builds=None, push_rules=None, releases_access_level=None, remove_source_branch_after_merge=None, repository_access_level=None, repository_storage=None, request_access_enabled=None, requirements_access_level=None, resolve_outdated_diff_discussions=None, restrict_user_defined_variables=None, runners_token=None, security_and_compliance_access_level=None, shared_with_groups=None, snippets_access_level=None, snippets_enabled=None, squash_commit_template=None, ssh_url_to_repo=None, suggestion_commit_message=None, topics=None, visibility_level=None, web_url=None, wiki_access_level=None, wiki_enabled=None):
         if analytics_access_level and not isinstance(analytics_access_level, str):
             raise TypeError("Expected argument 'analytics_access_level' to be a str")
         pulumi.set(__self__, "analytics_access_level", analytics_access_level)
         if archived and not isinstance(archived, bool):
             raise TypeError("Expected argument 'archived' to be a bool")
         pulumi.set(__self__, "archived", archived)
         if auto_cancel_pending_pipelines and not isinstance(auto_cancel_pending_pipelines, str):
@@ -52,14 +52,17 @@
         pulumi.set(__self__, "builds_access_level", builds_access_level)
         if ci_config_path and not isinstance(ci_config_path, str):
             raise TypeError("Expected argument 'ci_config_path' to be a str")
         pulumi.set(__self__, "ci_config_path", ci_config_path)
         if ci_default_git_depth and not isinstance(ci_default_git_depth, int):
             raise TypeError("Expected argument 'ci_default_git_depth' to be a int")
         pulumi.set(__self__, "ci_default_git_depth", ci_default_git_depth)
+        if ci_restrict_pipeline_cancellation_role and not isinstance(ci_restrict_pipeline_cancellation_role, str):
+            raise TypeError("Expected argument 'ci_restrict_pipeline_cancellation_role' to be a str")
+        pulumi.set(__self__, "ci_restrict_pipeline_cancellation_role", ci_restrict_pipeline_cancellation_role)
         if ci_separated_caches and not isinstance(ci_separated_caches, bool):
             raise TypeError("Expected argument 'ci_separated_caches' to be a bool")
         pulumi.set(__self__, "ci_separated_caches", ci_separated_caches)
         if container_expiration_policies and not isinstance(container_expiration_policies, list):
             raise TypeError("Expected argument 'container_expiration_policies' to be a list")
         pulumi.set(__self__, "container_expiration_policies", container_expiration_policies)
         if container_registry_access_level and not isinstance(container_registry_access_level, str):
@@ -304,14 +307,22 @@
     def ci_default_git_depth(self) -> int:
         """
         Default number of revisions for shallow cloning.
         """
         return pulumi.get(self, "ci_default_git_depth")
 
     @property
+    @pulumi.getter(name="ciRestrictPipelineCancellationRole")
+    def ci_restrict_pipeline_cancellation_role(self) -> str:
+        """
+        The role required to cancel a pipeline or job. Introduced in GitLab 16.8. Premium and Ultimate only. Valid values are `developer`, `maintainer`, `no one`
+        """
+        return pulumi.get(self, "ci_restrict_pipeline_cancellation_role")
+
+    @property
     @pulumi.getter(name="ciSeparatedCaches")
     def ci_separated_caches(self) -> bool:
         """
         Use separate caches for protected branches.
         """
         return pulumi.get(self, "ci_separated_caches")
 
@@ -753,14 +764,15 @@
             auto_devops_enabled=self.auto_devops_enabled,
             autoclose_referenced_issues=self.autoclose_referenced_issues,
             build_git_strategy=self.build_git_strategy,
             build_timeout=self.build_timeout,
             builds_access_level=self.builds_access_level,
             ci_config_path=self.ci_config_path,
             ci_default_git_depth=self.ci_default_git_depth,
+            ci_restrict_pipeline_cancellation_role=self.ci_restrict_pipeline_cancellation_role,
             ci_separated_caches=self.ci_separated_caches,
             container_expiration_policies=self.container_expiration_policies,
             container_registry_access_level=self.container_registry_access_level,
             default_branch=self.default_branch,
             description=self.description,
             emails_disabled=self.emails_disabled,
             empty_repo=self.empty_repo,
@@ -854,14 +866,15 @@
         auto_devops_enabled=pulumi.get(__ret__, 'auto_devops_enabled'),
         autoclose_referenced_issues=pulumi.get(__ret__, 'autoclose_referenced_issues'),
         build_git_strategy=pulumi.get(__ret__, 'build_git_strategy'),
         build_timeout=pulumi.get(__ret__, 'build_timeout'),
         builds_access_level=pulumi.get(__ret__, 'builds_access_level'),
         ci_config_path=pulumi.get(__ret__, 'ci_config_path'),
         ci_default_git_depth=pulumi.get(__ret__, 'ci_default_git_depth'),
+        ci_restrict_pipeline_cancellation_role=pulumi.get(__ret__, 'ci_restrict_pipeline_cancellation_role'),
         ci_separated_caches=pulumi.get(__ret__, 'ci_separated_caches'),
         container_expiration_policies=pulumi.get(__ret__, 'container_expiration_policies'),
         container_registry_access_level=pulumi.get(__ret__, 'container_registry_access_level'),
         default_branch=pulumi.get(__ret__, 'default_branch'),
         description=pulumi.get(__ret__, 'description'),
         emails_disabled=pulumi.get(__ret__, 'emails_disabled'),
         empty_repo=pulumi.get(__ret__, 'empty_repo'),
```

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_branches.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_branches.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_hook.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_hooks.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_hooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_issue.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_issue.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_issues.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_issues.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_membership.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_milestone.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_milestones.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_milestones.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_protected_branch.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_protected_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_protected_branches.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_protected_branches.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_tag.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_tags.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_tags.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_variable.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_variable.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 ]
 
 @pulumi.output_type
 class GetProjectVariableResult:
     """
     A collection of values returned by getProjectVariable.
     """
-    def __init__(__self__, environment_scope=None, id=None, key=None, masked=None, project=None, protected=None, raw=None, value=None, variable_type=None):
+    def __init__(__self__, description=None, environment_scope=None, id=None, key=None, masked=None, project=None, protected=None, raw=None, value=None, variable_type=None):
+        if description and not isinstance(description, str):
+            raise TypeError("Expected argument 'description' to be a str")
+        pulumi.set(__self__, "description", description)
         if environment_scope and not isinstance(environment_scope, str):
             raise TypeError("Expected argument 'environment_scope' to be a str")
         pulumi.set(__self__, "environment_scope", environment_scope)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if key and not isinstance(key, str):
@@ -47,14 +50,22 @@
             raise TypeError("Expected argument 'value' to be a str")
         pulumi.set(__self__, "value", value)
         if variable_type and not isinstance(variable_type, str):
             raise TypeError("Expected argument 'variable_type' to be a str")
         pulumi.set(__self__, "variable_type", variable_type)
 
     @property
+    @pulumi.getter
+    def description(self) -> str:
+        """
+        The description of the variable.
+        """
+        return pulumi.get(self, "description")
+
+    @property
     @pulumi.getter(name="environmentScope")
     def environment_scope(self) -> str:
         """
         The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         """
         return pulumi.get(self, "environment_scope")
 
@@ -125,14 +136,15 @@
 
 class AwaitableGetProjectVariableResult(GetProjectVariableResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetProjectVariableResult(
+            description=self.description,
             environment_scope=self.environment_scope,
             id=self.id,
             key=self.key,
             masked=self.masked,
             project=self.project,
             protected=self.protected,
             raw=self.raw,
@@ -171,14 +183,15 @@
     __args__['environmentScope'] = environment_scope
     __args__['key'] = key
     __args__['project'] = project
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectVariable:getProjectVariable', __args__, opts=opts, typ=GetProjectVariableResult).value
 
     return AwaitableGetProjectVariableResult(
+        description=pulumi.get(__ret__, 'description'),
         environment_scope=pulumi.get(__ret__, 'environment_scope'),
         id=pulumi.get(__ret__, 'id'),
         key=pulumi.get(__ret__, 'key'),
         masked=pulumi.get(__ret__, 'masked'),
         project=pulumi.get(__ret__, 'project'),
         protected=pulumi.get(__ret__, 'protected'),
         raw=pulumi.get(__ret__, 'raw'),
```

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_project_variables.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_project_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_projects.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_projects.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_release_link.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_release_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_release_links.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_release_links.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_repository_file.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_repository_tree.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_repository_tree.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_user.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_user_sshkeys.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_user_sshkeys.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/get_users.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/global_level_notifications.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/global_level_notifications.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_access_token.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_badge.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_badge.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_cluster.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_custom_attribute.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_epic_board.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_epic_board.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_hook.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_issue_board.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_issue_board.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_label.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_label.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_ldap_link.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_ldap_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_membership.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_project_file_template.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_project_file_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_protected_environment.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_protected_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_saml_link.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_saml_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_share_group.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_share_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/group_variable.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/group_variable.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,33 +13,37 @@
 
 @pulumi.input_type
 class GroupVariableArgs:
     def __init__(__self__, *,
                  group: pulumi.Input[str],
                  key: pulumi.Input[str],
                  value: pulumi.Input[str],
+                 description: Optional[pulumi.Input[str]] = None,
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
                  raw: Optional[pulumi.Input[bool]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a GroupVariable resource.
         :param pulumi.Input[str] group: The name or id of the group.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[str] value: The value of the variable.
+        :param pulumi.Input[str] description: The description of the variable.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         pulumi.set(__self__, "group", group)
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "value", value)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
         if environment_scope is not None:
             pulumi.set(__self__, "environment_scope", environment_scope)
         if masked is not None:
             pulumi.set(__self__, "masked", masked)
         if protected is not None:
             pulumi.set(__self__, "protected", protected)
         if raw is not None:
@@ -80,14 +84,26 @@
         return pulumi.get(self, "value")
 
     @value.setter
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
 
     @property
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
+        """
+        The description of the variable.
+        """
+        return pulumi.get(self, "description")
+
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
+
+    @property
     @pulumi.getter(name="environmentScope")
     def environment_scope(self) -> Optional[pulumi.Input[str]]:
         """
         The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         """
         return pulumi.get(self, "environment_scope")
 
@@ -143,33 +159,37 @@
     def variable_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "variable_type", value)
 
 
 @pulumi.input_type
 class _GroupVariableState:
     def __init__(__self__, *,
+                 description: Optional[pulumi.Input[str]] = None,
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  group: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
                  raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering GroupVariable resources.
+        :param pulumi.Input[str] description: The description of the variable.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[str] group: The name or id of the group.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
+        if description is not None:
+            pulumi.set(__self__, "description", description)
         if environment_scope is not None:
             pulumi.set(__self__, "environment_scope", environment_scope)
         if group is not None:
             pulumi.set(__self__, "group", group)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if masked is not None:
@@ -180,14 +200,26 @@
             pulumi.set(__self__, "raw", raw)
         if value is not None:
             pulumi.set(__self__, "value", value)
         if variable_type is not None:
             pulumi.set(__self__, "variable_type", variable_type)
 
     @property
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
+        """
+        The description of the variable.
+        """
+        return pulumi.get(self, "description")
+
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
+
+    @property
     @pulumi.getter(name="environmentScope")
     def environment_scope(self) -> Optional[pulumi.Input[str]]:
         """
         The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         """
         return pulumi.get(self, "environment_scope")
 
@@ -281,14 +313,15 @@
 
 
 class GroupVariable(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 description: Optional[pulumi.Input[str]] = None,
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  group: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
                  raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
@@ -320,14 +353,15 @@
 
         ```sh
         $ pulumi import gitlab:index/groupVariable:GroupVariable example 12345:group_variable_key:*
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] description: The description of the variable.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[str] group: The name or id of the group.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
@@ -378,14 +412,15 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 description: Optional[pulumi.Input[str]] = None,
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  group: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
                  raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
@@ -395,14 +430,15 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GroupVariableArgs.__new__(GroupVariableArgs)
 
+            __props__.__dict__["description"] = description
             __props__.__dict__["environment_scope"] = environment_scope
             if group is None and not opts.urn:
                 raise TypeError("Missing required property 'group'")
             __props__.__dict__["group"] = group
             if key is None and not opts.urn:
                 raise TypeError("Missing required property 'key'")
             __props__.__dict__["key"] = key
@@ -419,14 +455,15 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            description: Optional[pulumi.Input[str]] = None,
             environment_scope: Optional[pulumi.Input[str]] = None,
             group: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             masked: Optional[pulumi.Input[bool]] = None,
             protected: Optional[pulumi.Input[bool]] = None,
             raw: Optional[pulumi.Input[bool]] = None,
             value: Optional[pulumi.Input[str]] = None,
@@ -434,38 +471,48 @@
         """
         Get an existing GroupVariable resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] description: The description of the variable.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[str] group: The name or id of the group.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _GroupVariableState.__new__(_GroupVariableState)
 
+        __props__.__dict__["description"] = description
         __props__.__dict__["environment_scope"] = environment_scope
         __props__.__dict__["group"] = group
         __props__.__dict__["key"] = key
         __props__.__dict__["masked"] = masked
         __props__.__dict__["protected"] = protected
         __props__.__dict__["raw"] = raw
         __props__.__dict__["value"] = value
         __props__.__dict__["variable_type"] = variable_type
         return GroupVariable(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter
+    def description(self) -> pulumi.Output[Optional[str]]:
+        """
+        The description of the variable.
+        """
+        return pulumi.get(self, "description")
+
+    @property
     @pulumi.getter(name="environmentScope")
     def environment_scope(self) -> pulumi.Output[Optional[str]]:
         """
         The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         """
         return pulumi.get(self, "environment_scope")
```

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/instance_cluster.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/instance_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/instance_variable.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/instance_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_custom_issue_tracker.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_custom_issue_tracker.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_emails_on_push.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_emails_on_push.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_external_wiki.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_external_wiki.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_github.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_jira.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_jira.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_mattermost.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_mattermost.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_microsoft_teams.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_microsoft_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_pipelines_email.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_pipelines_email.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/integration_slack.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/integration_slack.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/label.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/label.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/outputs.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2686,42 +2686,53 @@
     def wiki_access_level(self) -> str:
         return pulumi.get(self, "wiki_access_level")
 
 
 @pulumi.output_type
 class GetGroupVariablesVariableResult(dict):
     def __init__(__self__, *,
+                 description: str,
                  environment_scope: str,
                  group: str,
                  key: str,
                  masked: bool,
                  protected: bool,
                  raw: bool,
                  value: str,
                  variable_type: str):
         """
+        :param str description: The description of the variable.
         :param str environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param str group: The name or id of the group.
         :param str key: The name of the variable.
         :param bool masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param bool protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         :param bool raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param str value: The value of the variable.
         :param str variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
+        pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "environment_scope", environment_scope)
         pulumi.set(__self__, "group", group)
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "masked", masked)
         pulumi.set(__self__, "protected", protected)
         pulumi.set(__self__, "raw", raw)
         pulumi.set(__self__, "value", value)
         pulumi.set(__self__, "variable_type", variable_type)
 
     @property
+    @pulumi.getter
+    def description(self) -> str:
+        """
+        The description of the variable.
+        """
+        return pulumi.get(self, "description")
+
+    @property
     @pulumi.getter(name="environmentScope")
     def environment_scope(self) -> str:
         """
         The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         """
         return pulumi.get(self, "environment_scope")
 
@@ -5374,42 +5385,53 @@
         """
         return pulumi.get(self, "tag_name")
 
 
 @pulumi.output_type
 class GetProjectVariablesVariableResult(dict):
     def __init__(__self__, *,
+                 description: str,
                  environment_scope: str,
                  key: str,
                  masked: bool,
                  project: str,
                  protected: bool,
                  raw: bool,
                  value: str,
                  variable_type: str):
         """
+        :param str description: The description of the variable.
         :param str environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param str key: The name of the variable.
         :param bool masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param str project: The name or id of the project.
         :param bool protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         :param bool raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param str value: The value of the variable.
         :param str variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
+        pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "environment_scope", environment_scope)
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "masked", masked)
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "protected", protected)
         pulumi.set(__self__, "raw", raw)
         pulumi.set(__self__, "value", value)
         pulumi.set(__self__, "variable_type", variable_type)
 
     @property
+    @pulumi.getter
+    def description(self) -> str:
+        """
+        The description of the variable.
+        """
+        return pulumi.get(self, "description")
+
+    @property
     @pulumi.getter(name="environmentScope")
     def environment_scope(self) -> str:
         """
         The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         """
         return pulumi.get(self, "environment_scope")
 
@@ -5486,14 +5508,15 @@
                  build_coverage_regex: str,
                  build_git_strategy: str,
                  build_timeout: int,
                  builds_access_level: str,
                  ci_config_path: str,
                  ci_default_git_depth: int,
                  ci_forward_deployment_enabled: bool,
+                 ci_restrict_pipeline_cancellation_role: str,
                  container_expiration_policies: Sequence['outputs.GetProjectsProjectContainerExpirationPolicyResult'],
                  container_registry_access_level: str,
                  container_registry_enabled: bool,
                  created_at: str,
                  creator_id: int,
                  custom_attributes: Sequence[Mapping[str, str]],
                  default_branch: str,
@@ -5583,14 +5606,15 @@
         :param str build_coverage_regex: Build coverage regex for the project.
         :param str build_git_strategy: The Git strategy. Defaults to fetch.
         :param int build_timeout: The maximum amount of time, in seconds, that a job can run.
         :param str builds_access_level: Set the builds access level. Valid values are `disabled`, `private`, `enabled`.
         :param str ci_config_path: CI config file path for the project.
         :param int ci_default_git_depth: Default number of revisions for shallow cloning.
         :param bool ci_forward_deployment_enabled: When a new deployment job starts, skip older deployment jobs that are still pending.
+        :param str ci_restrict_pipeline_cancellation_role: The role required to cancel a pipeline or job. Introduced in GitLab 16.8. Premium and Ultimate only. Valid values are `developer`, `maintainer`, `no one`
         :param Sequence['GetProjectsProjectContainerExpirationPolicyArgs'] container_expiration_policies: Set the image cleanup policy for this project. **Note**: this field is sometimes named `container_expiration_policy_attributes` in the GitLab Upstream API.
         :param str container_registry_access_level: Set visibility of container registry, for this project. Valid values are `disabled`, `private`, `enabled`.
         :param bool container_registry_enabled: Whether the container registry is enabled for the project.
         :param str created_at: Creation time for the project.
         :param int creator_id: Creator ID for the project.
         :param Sequence[Mapping[str, str]] custom_attributes: Custom attributes for the project.
         :param str default_branch: The default branch name of the project.
@@ -5679,14 +5703,15 @@
         pulumi.set(__self__, "build_coverage_regex", build_coverage_regex)
         pulumi.set(__self__, "build_git_strategy", build_git_strategy)
         pulumi.set(__self__, "build_timeout", build_timeout)
         pulumi.set(__self__, "builds_access_level", builds_access_level)
         pulumi.set(__self__, "ci_config_path", ci_config_path)
         pulumi.set(__self__, "ci_default_git_depth", ci_default_git_depth)
         pulumi.set(__self__, "ci_forward_deployment_enabled", ci_forward_deployment_enabled)
+        pulumi.set(__self__, "ci_restrict_pipeline_cancellation_role", ci_restrict_pipeline_cancellation_role)
         pulumi.set(__self__, "container_expiration_policies", container_expiration_policies)
         pulumi.set(__self__, "container_registry_access_level", container_registry_access_level)
         pulumi.set(__self__, "container_registry_enabled", container_registry_enabled)
         pulumi.set(__self__, "created_at", created_at)
         pulumi.set(__self__, "creator_id", creator_id)
         pulumi.set(__self__, "custom_attributes", custom_attributes)
         pulumi.set(__self__, "default_branch", default_branch)
@@ -5896,14 +5921,22 @@
     def ci_forward_deployment_enabled(self) -> bool:
         """
         When a new deployment job starts, skip older deployment jobs that are still pending.
         """
         return pulumi.get(self, "ci_forward_deployment_enabled")
 
     @property
+    @pulumi.getter(name="ciRestrictPipelineCancellationRole")
+    def ci_restrict_pipeline_cancellation_role(self) -> str:
+        """
+        The role required to cancel a pipeline or job. Introduced in GitLab 16.8. Premium and Ultimate only. Valid values are `developer`, `maintainer`, `no one`
+        """
+        return pulumi.get(self, "ci_restrict_pipeline_cancellation_role")
+
+    @property
     @pulumi.getter(name="containerExpirationPolicies")
     def container_expiration_policies(self) -> Sequence['outputs.GetProjectsProjectContainerExpirationPolicyResult']:
         """
         Set the image cleanup policy for this project. **Note**: this field is sometimes named `container_expiration_policy_attributes` in the GitLab Upstream API.
         """
         return pulumi.get(self, "container_expiration_policies")
```

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/pages_domain.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/pages_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/personal_access_token.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/personal_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/pipeline_schedule.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/pipeline_schedule_variable.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/pipeline_schedule_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/pipeline_trigger.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/pipeline_trigger.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
                  build_coverage_regex: Optional[pulumi.Input[str]] = None,
                  build_git_strategy: Optional[pulumi.Input[str]] = None,
                  build_timeout: Optional[pulumi.Input[int]] = None,
                  builds_access_level: Optional[pulumi.Input[str]] = None,
                  ci_config_path: Optional[pulumi.Input[str]] = None,
                  ci_default_git_depth: Optional[pulumi.Input[int]] = None,
                  ci_forward_deployment_enabled: Optional[pulumi.Input[bool]] = None,
+                 ci_restrict_pipeline_cancellation_role: Optional[pulumi.Input[str]] = None,
                  ci_separated_caches: Optional[pulumi.Input[bool]] = None,
                  container_expiration_policy: Optional[pulumi.Input['ProjectContainerExpirationPolicyArgs']] = None,
                  container_registry_access_level: Optional[pulumi.Input[str]] = None,
                  container_registry_enabled: Optional[pulumi.Input[bool]] = None,
                  default_branch: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  emails_disabled: Optional[pulumi.Input[bool]] = None,
@@ -126,14 +127,15 @@
         :param pulumi.Input[str] build_coverage_regex: Test coverage parsing for the project. This is deprecated feature in GitLab 15.0.
         :param pulumi.Input[str] build_git_strategy: The Git strategy. Defaults to fetch. Valid values are `clone`, `fetch`.
         :param pulumi.Input[int] build_timeout: The maximum amount of time, in seconds, that a job can run.
         :param pulumi.Input[str] builds_access_level: Set the builds access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] ci_config_path: Custom Path to CI config file.
         :param pulumi.Input[int] ci_default_git_depth: Default number of revisions for shallow cloning.
         :param pulumi.Input[bool] ci_forward_deployment_enabled: When a new deployment job starts, skip older deployment jobs that are still pending.
+        :param pulumi.Input[str] ci_restrict_pipeline_cancellation_role: The role required to cancel a pipeline or job. Introduced in GitLab 16.8. Premium and Ultimate only. Valid values are `developer`, `maintainer`, `no one`
         :param pulumi.Input[bool] ci_separated_caches: Use separate caches for protected branches.
         :param pulumi.Input['ProjectContainerExpirationPolicyArgs'] container_expiration_policy: Set the image cleanup policy for this project. **Note**: this field is sometimes named `container_expiration_policy_attributes` in the GitLab Upstream API.
         :param pulumi.Input[str] container_registry_access_level: Set visibility of container registry, for this project. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] container_registry_enabled: Enable container registry for the project.
         :param pulumi.Input[str] default_branch: The default branch for the project.
         :param pulumi.Input[str] description: A description of the project.
         :param pulumi.Input[bool] emails_disabled: Disable email notifications.
@@ -243,14 +245,16 @@
             pulumi.set(__self__, "builds_access_level", builds_access_level)
         if ci_config_path is not None:
             pulumi.set(__self__, "ci_config_path", ci_config_path)
         if ci_default_git_depth is not None:
             pulumi.set(__self__, "ci_default_git_depth", ci_default_git_depth)
         if ci_forward_deployment_enabled is not None:
             pulumi.set(__self__, "ci_forward_deployment_enabled", ci_forward_deployment_enabled)
+        if ci_restrict_pipeline_cancellation_role is not None:
+            pulumi.set(__self__, "ci_restrict_pipeline_cancellation_role", ci_restrict_pipeline_cancellation_role)
         if ci_separated_caches is not None:
             pulumi.set(__self__, "ci_separated_caches", ci_separated_caches)
         if container_expiration_policy is not None:
             pulumi.set(__self__, "container_expiration_policy", container_expiration_policy)
         if container_registry_access_level is not None:
             pulumi.set(__self__, "container_registry_access_level", container_registry_access_level)
         if container_registry_enabled is not None:
@@ -622,14 +626,26 @@
         return pulumi.get(self, "ci_forward_deployment_enabled")
 
     @ci_forward_deployment_enabled.setter
     def ci_forward_deployment_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ci_forward_deployment_enabled", value)
 
     @property
+    @pulumi.getter(name="ciRestrictPipelineCancellationRole")
+    def ci_restrict_pipeline_cancellation_role(self) -> Optional[pulumi.Input[str]]:
+        """
+        The role required to cancel a pipeline or job. Introduced in GitLab 16.8. Premium and Ultimate only. Valid values are `developer`, `maintainer`, `no one`
+        """
+        return pulumi.get(self, "ci_restrict_pipeline_cancellation_role")
+
+    @ci_restrict_pipeline_cancellation_role.setter
+    def ci_restrict_pipeline_cancellation_role(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ci_restrict_pipeline_cancellation_role", value)
+
+    @property
     @pulumi.getter(name="ciSeparatedCaches")
     def ci_separated_caches(self) -> Optional[pulumi.Input[bool]]:
         """
         Use separate caches for protected branches.
         """
         return pulumi.get(self, "ci_separated_caches")
 
@@ -1533,14 +1549,15 @@
                  build_coverage_regex: Optional[pulumi.Input[str]] = None,
                  build_git_strategy: Optional[pulumi.Input[str]] = None,
                  build_timeout: Optional[pulumi.Input[int]] = None,
                  builds_access_level: Optional[pulumi.Input[str]] = None,
                  ci_config_path: Optional[pulumi.Input[str]] = None,
                  ci_default_git_depth: Optional[pulumi.Input[int]] = None,
                  ci_forward_deployment_enabled: Optional[pulumi.Input[bool]] = None,
+                 ci_restrict_pipeline_cancellation_role: Optional[pulumi.Input[str]] = None,
                  ci_separated_caches: Optional[pulumi.Input[bool]] = None,
                  container_expiration_policy: Optional[pulumi.Input['ProjectContainerExpirationPolicyArgs']] = None,
                  container_registry_access_level: Optional[pulumi.Input[str]] = None,
                  container_registry_enabled: Optional[pulumi.Input[bool]] = None,
                  default_branch: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  emails_disabled: Optional[pulumi.Input[bool]] = None,
@@ -1636,14 +1653,15 @@
         :param pulumi.Input[str] build_coverage_regex: Test coverage parsing for the project. This is deprecated feature in GitLab 15.0.
         :param pulumi.Input[str] build_git_strategy: The Git strategy. Defaults to fetch. Valid values are `clone`, `fetch`.
         :param pulumi.Input[int] build_timeout: The maximum amount of time, in seconds, that a job can run.
         :param pulumi.Input[str] builds_access_level: Set the builds access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] ci_config_path: Custom Path to CI config file.
         :param pulumi.Input[int] ci_default_git_depth: Default number of revisions for shallow cloning.
         :param pulumi.Input[bool] ci_forward_deployment_enabled: When a new deployment job starts, skip older deployment jobs that are still pending.
+        :param pulumi.Input[str] ci_restrict_pipeline_cancellation_role: The role required to cancel a pipeline or job. Introduced in GitLab 16.8. Premium and Ultimate only. Valid values are `developer`, `maintainer`, `no one`
         :param pulumi.Input[bool] ci_separated_caches: Use separate caches for protected branches.
         :param pulumi.Input['ProjectContainerExpirationPolicyArgs'] container_expiration_policy: Set the image cleanup policy for this project. **Note**: this field is sometimes named `container_expiration_policy_attributes` in the GitLab Upstream API.
         :param pulumi.Input[str] container_registry_access_level: Set visibility of container registry, for this project. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] container_registry_enabled: Enable container registry for the project.
         :param pulumi.Input[str] default_branch: The default branch for the project.
         :param pulumi.Input[str] description: A description of the project.
         :param pulumi.Input[bool] emails_disabled: Disable email notifications.
@@ -1761,14 +1779,16 @@
             pulumi.set(__self__, "builds_access_level", builds_access_level)
         if ci_config_path is not None:
             pulumi.set(__self__, "ci_config_path", ci_config_path)
         if ci_default_git_depth is not None:
             pulumi.set(__self__, "ci_default_git_depth", ci_default_git_depth)
         if ci_forward_deployment_enabled is not None:
             pulumi.set(__self__, "ci_forward_deployment_enabled", ci_forward_deployment_enabled)
+        if ci_restrict_pipeline_cancellation_role is not None:
+            pulumi.set(__self__, "ci_restrict_pipeline_cancellation_role", ci_restrict_pipeline_cancellation_role)
         if ci_separated_caches is not None:
             pulumi.set(__self__, "ci_separated_caches", ci_separated_caches)
         if container_expiration_policy is not None:
             pulumi.set(__self__, "container_expiration_policy", container_expiration_policy)
         if container_registry_access_level is not None:
             pulumi.set(__self__, "container_registry_access_level", container_registry_access_level)
         if container_registry_enabled is not None:
@@ -2164,14 +2184,26 @@
         return pulumi.get(self, "ci_forward_deployment_enabled")
 
     @ci_forward_deployment_enabled.setter
     def ci_forward_deployment_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ci_forward_deployment_enabled", value)
 
     @property
+    @pulumi.getter(name="ciRestrictPipelineCancellationRole")
+    def ci_restrict_pipeline_cancellation_role(self) -> Optional[pulumi.Input[str]]:
+        """
+        The role required to cancel a pipeline or job. Introduced in GitLab 16.8. Premium and Ultimate only. Valid values are `developer`, `maintainer`, `no one`
+        """
+        return pulumi.get(self, "ci_restrict_pipeline_cancellation_role")
+
+    @ci_restrict_pipeline_cancellation_role.setter
+    def ci_restrict_pipeline_cancellation_role(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ci_restrict_pipeline_cancellation_role", value)
+
+    @property
     @pulumi.getter(name="ciSeparatedCaches")
     def ci_separated_caches(self) -> Optional[pulumi.Input[bool]]:
         """
         Use separate caches for protected branches.
         """
         return pulumi.get(self, "ci_separated_caches")
 
@@ -3148,14 +3180,15 @@
                  build_coverage_regex: Optional[pulumi.Input[str]] = None,
                  build_git_strategy: Optional[pulumi.Input[str]] = None,
                  build_timeout: Optional[pulumi.Input[int]] = None,
                  builds_access_level: Optional[pulumi.Input[str]] = None,
                  ci_config_path: Optional[pulumi.Input[str]] = None,
                  ci_default_git_depth: Optional[pulumi.Input[int]] = None,
                  ci_forward_deployment_enabled: Optional[pulumi.Input[bool]] = None,
+                 ci_restrict_pipeline_cancellation_role: Optional[pulumi.Input[str]] = None,
                  ci_separated_caches: Optional[pulumi.Input[bool]] = None,
                  container_expiration_policy: Optional[pulumi.Input[pulumi.InputType['ProjectContainerExpirationPolicyArgs']]] = None,
                  container_registry_access_level: Optional[pulumi.Input[str]] = None,
                  container_registry_enabled: Optional[pulumi.Input[bool]] = None,
                  default_branch: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  emails_disabled: Optional[pulumi.Input[bool]] = None,
@@ -3315,14 +3348,15 @@
         :param pulumi.Input[str] build_coverage_regex: Test coverage parsing for the project. This is deprecated feature in GitLab 15.0.
         :param pulumi.Input[str] build_git_strategy: The Git strategy. Defaults to fetch. Valid values are `clone`, `fetch`.
         :param pulumi.Input[int] build_timeout: The maximum amount of time, in seconds, that a job can run.
         :param pulumi.Input[str] builds_access_level: Set the builds access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] ci_config_path: Custom Path to CI config file.
         :param pulumi.Input[int] ci_default_git_depth: Default number of revisions for shallow cloning.
         :param pulumi.Input[bool] ci_forward_deployment_enabled: When a new deployment job starts, skip older deployment jobs that are still pending.
+        :param pulumi.Input[str] ci_restrict_pipeline_cancellation_role: The role required to cancel a pipeline or job. Introduced in GitLab 16.8. Premium and Ultimate only. Valid values are `developer`, `maintainer`, `no one`
         :param pulumi.Input[bool] ci_separated_caches: Use separate caches for protected branches.
         :param pulumi.Input[pulumi.InputType['ProjectContainerExpirationPolicyArgs']] container_expiration_policy: Set the image cleanup policy for this project. **Note**: this field is sometimes named `container_expiration_policy_attributes` in the GitLab Upstream API.
         :param pulumi.Input[str] container_registry_access_level: Set visibility of container registry, for this project. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] container_registry_enabled: Enable container registry for the project.
         :param pulumi.Input[str] default_branch: The default branch for the project.
         :param pulumi.Input[str] description: A description of the project.
         :param pulumi.Input[bool] emails_disabled: Disable email notifications.
@@ -3502,14 +3536,15 @@
                  build_coverage_regex: Optional[pulumi.Input[str]] = None,
                  build_git_strategy: Optional[pulumi.Input[str]] = None,
                  build_timeout: Optional[pulumi.Input[int]] = None,
                  builds_access_level: Optional[pulumi.Input[str]] = None,
                  ci_config_path: Optional[pulumi.Input[str]] = None,
                  ci_default_git_depth: Optional[pulumi.Input[int]] = None,
                  ci_forward_deployment_enabled: Optional[pulumi.Input[bool]] = None,
+                 ci_restrict_pipeline_cancellation_role: Optional[pulumi.Input[str]] = None,
                  ci_separated_caches: Optional[pulumi.Input[bool]] = None,
                  container_expiration_policy: Optional[pulumi.Input[pulumi.InputType['ProjectContainerExpirationPolicyArgs']]] = None,
                  container_registry_access_level: Optional[pulumi.Input[str]] = None,
                  container_registry_enabled: Optional[pulumi.Input[bool]] = None,
                  default_branch: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  emails_disabled: Optional[pulumi.Input[bool]] = None,
@@ -3602,14 +3637,15 @@
             __props__.__dict__["build_coverage_regex"] = build_coverage_regex
             __props__.__dict__["build_git_strategy"] = build_git_strategy
             __props__.__dict__["build_timeout"] = build_timeout
             __props__.__dict__["builds_access_level"] = builds_access_level
             __props__.__dict__["ci_config_path"] = ci_config_path
             __props__.__dict__["ci_default_git_depth"] = ci_default_git_depth
             __props__.__dict__["ci_forward_deployment_enabled"] = ci_forward_deployment_enabled
+            __props__.__dict__["ci_restrict_pipeline_cancellation_role"] = ci_restrict_pipeline_cancellation_role
             __props__.__dict__["ci_separated_caches"] = ci_separated_caches
             __props__.__dict__["container_expiration_policy"] = container_expiration_policy
             __props__.__dict__["container_registry_access_level"] = container_registry_access_level
             __props__.__dict__["container_registry_enabled"] = container_registry_enabled
             __props__.__dict__["default_branch"] = default_branch
             __props__.__dict__["description"] = description
             __props__.__dict__["emails_disabled"] = emails_disabled
@@ -3713,14 +3749,15 @@
             build_coverage_regex: Optional[pulumi.Input[str]] = None,
             build_git_strategy: Optional[pulumi.Input[str]] = None,
             build_timeout: Optional[pulumi.Input[int]] = None,
             builds_access_level: Optional[pulumi.Input[str]] = None,
             ci_config_path: Optional[pulumi.Input[str]] = None,
             ci_default_git_depth: Optional[pulumi.Input[int]] = None,
             ci_forward_deployment_enabled: Optional[pulumi.Input[bool]] = None,
+            ci_restrict_pipeline_cancellation_role: Optional[pulumi.Input[str]] = None,
             ci_separated_caches: Optional[pulumi.Input[bool]] = None,
             container_expiration_policy: Optional[pulumi.Input[pulumi.InputType['ProjectContainerExpirationPolicyArgs']]] = None,
             container_registry_access_level: Optional[pulumi.Input[str]] = None,
             container_registry_enabled: Optional[pulumi.Input[bool]] = None,
             default_branch: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             emails_disabled: Optional[pulumi.Input[bool]] = None,
@@ -3821,14 +3858,15 @@
         :param pulumi.Input[str] build_coverage_regex: Test coverage parsing for the project. This is deprecated feature in GitLab 15.0.
         :param pulumi.Input[str] build_git_strategy: The Git strategy. Defaults to fetch. Valid values are `clone`, `fetch`.
         :param pulumi.Input[int] build_timeout: The maximum amount of time, in seconds, that a job can run.
         :param pulumi.Input[str] builds_access_level: Set the builds access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] ci_config_path: Custom Path to CI config file.
         :param pulumi.Input[int] ci_default_git_depth: Default number of revisions for shallow cloning.
         :param pulumi.Input[bool] ci_forward_deployment_enabled: When a new deployment job starts, skip older deployment jobs that are still pending.
+        :param pulumi.Input[str] ci_restrict_pipeline_cancellation_role: The role required to cancel a pipeline or job. Introduced in GitLab 16.8. Premium and Ultimate only. Valid values are `developer`, `maintainer`, `no one`
         :param pulumi.Input[bool] ci_separated_caches: Use separate caches for protected branches.
         :param pulumi.Input[pulumi.InputType['ProjectContainerExpirationPolicyArgs']] container_expiration_policy: Set the image cleanup policy for this project. **Note**: this field is sometimes named `container_expiration_policy_attributes` in the GitLab Upstream API.
         :param pulumi.Input[str] container_registry_access_level: Set visibility of container registry, for this project. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] container_registry_enabled: Enable container registry for the project.
         :param pulumi.Input[str] default_branch: The default branch for the project.
         :param pulumi.Input[str] description: A description of the project.
         :param pulumi.Input[bool] emails_disabled: Disable email notifications.
@@ -3928,14 +3966,15 @@
         __props__.__dict__["build_coverage_regex"] = build_coverage_regex
         __props__.__dict__["build_git_strategy"] = build_git_strategy
         __props__.__dict__["build_timeout"] = build_timeout
         __props__.__dict__["builds_access_level"] = builds_access_level
         __props__.__dict__["ci_config_path"] = ci_config_path
         __props__.__dict__["ci_default_git_depth"] = ci_default_git_depth
         __props__.__dict__["ci_forward_deployment_enabled"] = ci_forward_deployment_enabled
+        __props__.__dict__["ci_restrict_pipeline_cancellation_role"] = ci_restrict_pipeline_cancellation_role
         __props__.__dict__["ci_separated_caches"] = ci_separated_caches
         __props__.__dict__["container_expiration_policy"] = container_expiration_policy
         __props__.__dict__["container_registry_access_level"] = container_registry_access_level
         __props__.__dict__["container_registry_enabled"] = container_registry_enabled
         __props__.__dict__["default_branch"] = default_branch
         __props__.__dict__["description"] = description
         __props__.__dict__["emails_disabled"] = emails_disabled
@@ -4168,14 +4207,22 @@
     def ci_forward_deployment_enabled(self) -> pulumi.Output[bool]:
         """
         When a new deployment job starts, skip older deployment jobs that are still pending.
         """
         return pulumi.get(self, "ci_forward_deployment_enabled")
 
     @property
+    @pulumi.getter(name="ciRestrictPipelineCancellationRole")
+    def ci_restrict_pipeline_cancellation_role(self) -> pulumi.Output[str]:
+        """
+        The role required to cancel a pipeline or job. Introduced in GitLab 16.8. Premium and Ultimate only. Valid values are `developer`, `maintainer`, `no one`
+        """
+        return pulumi.get(self, "ci_restrict_pipeline_cancellation_role")
+
+    @property
     @pulumi.getter(name="ciSeparatedCaches")
     def ci_separated_caches(self) -> pulumi.Output[bool]:
         """
         Use separate caches for protected branches.
         """
         return pulumi.get(self, "ci_separated_caches")
```

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_access_token.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_approval_rule.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_approval_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_badge.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_badge.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_cluster.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_compliance_framework.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_compliance_framework.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_custom_attribute.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_environment.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_freeze_period.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_freeze_period.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_hook.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_issue.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_issue.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_issue_board.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_issue_board.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_job_token_scope.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_job_token_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_label.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_label.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_level_mr_approvals.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_level_mr_approvals.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_level_notifications.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_level_notifications.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_membership.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_milestone.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_mirror.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_mirror.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_protected_environment.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_protected_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_runner_enablement.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_runner_enablement.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_share_group.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_share_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_tag.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/project_variable.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/project_variable.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,33 +13,37 @@
 
 @pulumi.input_type
 class ProjectVariableArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  project: pulumi.Input[str],
                  value: pulumi.Input[str],
+                 description: Optional[pulumi.Input[str]] = None,
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
                  raw: Optional[pulumi.Input[bool]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ProjectVariable resource.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[str] project: The name or id of the project.
         :param pulumi.Input[str] value: The value of the variable.
+        :param pulumi.Input[str] description: The description of the variable.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "value", value)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
         if environment_scope is not None:
             pulumi.set(__self__, "environment_scope", environment_scope)
         if masked is not None:
             pulumi.set(__self__, "masked", masked)
         if protected is not None:
             pulumi.set(__self__, "protected", protected)
         if raw is not None:
@@ -80,14 +84,26 @@
         return pulumi.get(self, "value")
 
     @value.setter
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
 
     @property
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
+        """
+        The description of the variable.
+        """
+        return pulumi.get(self, "description")
+
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
+
+    @property
     @pulumi.getter(name="environmentScope")
     def environment_scope(self) -> Optional[pulumi.Input[str]]:
         """
         The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         """
         return pulumi.get(self, "environment_scope")
 
@@ -143,33 +159,37 @@
     def variable_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "variable_type", value)
 
 
 @pulumi.input_type
 class _ProjectVariableState:
     def __init__(__self__, *,
+                 description: Optional[pulumi.Input[str]] = None,
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
                  raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  variable_type: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ProjectVariable resources.
+        :param pulumi.Input[str] description: The description of the variable.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[str] project: The name or id of the project.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
+        if description is not None:
+            pulumi.set(__self__, "description", description)
         if environment_scope is not None:
             pulumi.set(__self__, "environment_scope", environment_scope)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if masked is not None:
             pulumi.set(__self__, "masked", masked)
         if project is not None:
@@ -180,14 +200,26 @@
             pulumi.set(__self__, "raw", raw)
         if value is not None:
             pulumi.set(__self__, "value", value)
         if variable_type is not None:
             pulumi.set(__self__, "variable_type", variable_type)
 
     @property
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
+        """
+        The description of the variable.
+        """
+        return pulumi.get(self, "description")
+
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
+
+    @property
     @pulumi.getter(name="environmentScope")
     def environment_scope(self) -> Optional[pulumi.Input[str]]:
         """
         The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         """
         return pulumi.get(self, "environment_scope")
 
@@ -281,14 +313,15 @@
 
 
 class ProjectVariable(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 description: Optional[pulumi.Input[str]] = None,
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
                  raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
@@ -320,14 +353,15 @@
 
         ```sh
         $ pulumi import gitlab:index/projectVariable:ProjectVariable example '12345:project_variable_key:*'
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] description: The description of the variable.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[str] project: The name or id of the project.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
@@ -378,14 +412,15 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 description: Optional[pulumi.Input[str]] = None,
                  environment_scope: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  masked: Optional[pulumi.Input[bool]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  protected: Optional[pulumi.Input[bool]] = None,
                  raw: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
@@ -395,14 +430,15 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProjectVariableArgs.__new__(ProjectVariableArgs)
 
+            __props__.__dict__["description"] = description
             __props__.__dict__["environment_scope"] = environment_scope
             if key is None and not opts.urn:
                 raise TypeError("Missing required property 'key'")
             __props__.__dict__["key"] = key
             __props__.__dict__["masked"] = masked
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
@@ -419,14 +455,15 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            description: Optional[pulumi.Input[str]] = None,
             environment_scope: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             masked: Optional[pulumi.Input[bool]] = None,
             project: Optional[pulumi.Input[str]] = None,
             protected: Optional[pulumi.Input[bool]] = None,
             raw: Optional[pulumi.Input[bool]] = None,
             value: Optional[pulumi.Input[str]] = None,
@@ -434,38 +471,48 @@
         """
         Get an existing ProjectVariable resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] description: The description of the variable.
         :param pulumi.Input[str] environment_scope: The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         :param pulumi.Input[str] key: The name of the variable.
         :param pulumi.Input[bool] masked: If set to `true`, the value of the variable will be hidden in job logs. The value must meet the [masking requirements](https://docs.gitlab.com/ee/ci/variables/#masked-variables). Defaults to `false`.
         :param pulumi.Input[str] project: The name or id of the project.
         :param pulumi.Input[bool] protected: If set to `true`, the variable will be passed only to pipelines running on protected branches and tags. Defaults to `false`.
         :param pulumi.Input[bool] raw: Whether the variable is treated as a raw string. Default: false. When true, variables in the value are not expanded.
         :param pulumi.Input[str] value: The value of the variable.
         :param pulumi.Input[str] variable_type: The type of a variable. Valid values are: `env_var`, `file`. Default is `env_var`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ProjectVariableState.__new__(_ProjectVariableState)
 
+        __props__.__dict__["description"] = description
         __props__.__dict__["environment_scope"] = environment_scope
         __props__.__dict__["key"] = key
         __props__.__dict__["masked"] = masked
         __props__.__dict__["project"] = project
         __props__.__dict__["protected"] = protected
         __props__.__dict__["raw"] = raw
         __props__.__dict__["value"] = value
         __props__.__dict__["variable_type"] = variable_type
         return ProjectVariable(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter
+    def description(self) -> pulumi.Output[Optional[str]]:
+        """
+        The description of the variable.
+        """
+        return pulumi.get(self, "description")
+
+    @property
     @pulumi.getter(name="environmentScope")
     def environment_scope(self) -> pulumi.Output[Optional[str]]:
         """
         The environment scope of the variable. Defaults to all environment (`*`). Note that in Community Editions of Gitlab, values other than `*` will cause inconsistent plans.
         """
         return pulumi.get(self, "environment_scope")
```

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/provider.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/release_link.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/release_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/repository_file.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/runner.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/runner.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_custom_issue_tracker.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_custom_issue_tracker.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_emails_on_push.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_emails_on_push.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_external_wiki.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_external_wiki.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_github.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_jira.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_jira.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_microsoft_teams.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_microsoft_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_pipelines_email.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_pipelines_email.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/service_slack.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/service_slack.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/system_hook.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/system_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/tag_protection.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/tag_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/topic.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/user.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/user_custom_attribute.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/user_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/user_gpg_key.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/user_gpg_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/user_runner.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/user_runner.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab/user_ssh_key.py` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab/user_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab.egg-info/PKG-INFO` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_gitlab
-Version: 6.9.0a1708063247
+Version: 6.9.0a1708340471
 Summary: A Pulumi package for creating and managing GitLab resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-gitlab
 Keywords: pulumi,gitlab
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_gitlab-6.9.0a1708063247/pulumi_gitlab.egg-info/SOURCES.txt` & `pulumi_gitlab-6.9.0a1708340471/pulumi_gitlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.9.0a1708063247/pyproject.toml` & `pulumi_gitlab-6.9.0a1708340471/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_gitlab"
   description = "A Pulumi package for creating and managing GitLab resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "gitlab"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "6.9.0a1708063247"
+  version = "6.9.0a1708340471"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-gitlab"
 
 [build-system]
```

