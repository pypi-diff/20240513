# Comparing `tmp/sc_diff_analysis-0.0.29-py3-none-any.whl.zip` & `tmp/sc_diff_analysis-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,19 @@
-Zip file size: 34471 bytes, number of entries: 23
--rw-r--r--  2.0 unx     1173 b- defN 24-May-13 02:45 sc_diff_analysis/__init__.py
--rw-r--r--  2.0 unx     1960 b- defN 24-May-13 02:44 sc_diff_analysis/main.py
--rw-r--r--  2.0 unx     1852 b- defN 24-May-13 02:44 sc_diff_analysis/utils.py
--rw-r--r--  2.0 unx     1725 b- defN 24-May-13 02:44 sc_diff_analysis/analyzer/__init__.py
--rw-r--r--  2.0 unx     3880 b- defN 24-May-13 02:44 sc_diff_analysis/analyzer/branch_summary_group_by_branch_diff_analyzer.py
--rw-r--r--  2.0 unx     9875 b- defN 24-May-13 02:44 sc_diff_analysis/analyzer/branch_summary_group_by_item_type_diff_analyzer.py
--rw-r--r--  2.0 unx     3083 b- defN 24-May-13 02:44 sc_diff_analysis/analyzer/common_summary_diff_analyzer.py
--rw-r--r--  2.0 unx     5587 b- defN 24-May-13 02:44 sc_diff_analysis/analyzer/customer_summary_diff_analyzer.py
--rw-r--r--  2.0 unx     4052 b- defN 24-May-13 02:44 sc_diff_analysis/analyzer/diff_analyzer.py
--rw-r--r--  2.0 unx     1562 b- defN 24-May-13 02:44 sc_diff_analysis/analyzer/loan_detail_summary_diff_analyzer.py
--rw-r--r--  2.0 unx     5586 b- defN 24-May-13 02:44 sc_diff_analysis/analyzer/manager_summary_diff_analyzer.py
--rw-r--r--  2.0 unx    21586 b- defN 24-May-13 02:44 sc_diff_analysis/analyzer/xinka_summary_diff_analyzer.py
--rw-r--r--  2.0 unx     1114 b- defN 24-May-13 02:44 sc_diff_analysis/tests/__init__.py
--rw-r--r--  2.0 unx     4901 b- defN 24-May-13 02:44 sc_diff_analysis/tests/merge_tests.py
--rw-r--r--  2.0 unx     5063 b- defN 24-May-11 08:31 sc_diff_analysis/tests/sample_config/production-inclusive-balance-detail.yml
--rw-r--r--  2.0 unx     7102 b- defN 23-Nov-30 00:59 sc_diff_analysis/tests/sample_config/production-peak-season.yml
--rw-r--r--  2.0 unx     8697 b- defN 23-Nov-30 00:58 sc_diff_analysis/tests/sample_config/production.yml
--rw-r--r--  2.0 unx     1076 b- defN 24-May-13 02:47 sc_diff_analysis-0.0.29.dist-info/LICENSE
--rw-r--r--  2.0 unx     2124 b- defN 24-May-13 02:47 sc_diff_analysis-0.0.29.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-13 02:47 sc_diff_analysis-0.0.29.dist-info/WHEEL
--rw-r--r--  2.0 unx       64 b- defN 24-May-13 02:47 sc_diff_analysis-0.0.29.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 24-May-13 02:47 sc_diff_analysis-0.0.29.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2369 b- defN 24-May-13 02:47 sc_diff_analysis-0.0.29.dist-info/RECORD
-23 files, 94540 bytes uncompressed, 30467 bytes compressed:  67.8%
+Zip file size: 21908 bytes, number of entries: 17
+-rw-r--r--  2.0 unx     1137 b- defN 21-Jul-29 08:42 sc_diff_analysis/__init__.py
+-rw-r--r--  2.0 unx    20264 b- defN 21-Jul-30 01:39 sc_diff_analysis/diff_analyzer.py
+-rw-r--r--  2.0 unx    20864 b- defN 21-Jul-30 08:31 sc_diff_analysis/diff_analyzer_group_by_item_type.py
+-rw-r--r--  2.0 unx     1651 b- defN 21-Jul-30 01:51 sc_diff_analysis/main.py
+-rw-r--r--  2.0 unx     2724 b- defN 21-Jul-30 07:58 sc_diff_analysis/utils.py
+-rw-r--r--  2.0 unx     1114 b- defN 21-Jun-02 08:33 sc_diff_analysis/configs/__init__.py
+-rw-r--r--  2.0 unx     1241 b- defN 21-Jun-02 08:33 sc_diff_analysis/configs/default.py
+-rw-r--r--  2.0 unx     1114 b- defN 21-Jun-02 08:33 sc_diff_analysis/tests/__init__.py
+-rw-r--r--  2.0 unx     1133 b- defN 21-Jun-11 03:14 sc_diff_analysis/tests/pandas_test/__init__.py
+-rw-r--r--  2.0 unx     2542 b- defN 21-Jun-11 07:29 sc_diff_analysis/tests/pandas_test/pandas_test.py
+-rw-r--r--  2.0 unx     3014 b- defN 21-Jul-30 07:50 sc_diff_analysis/tests/sample_config/production.yml
+-rw-r--r--  2.0 unx     1076 b- defN 21-Jul-30 08:44 sc_diff_analysis-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2095 b- defN 21-Jul-30 08:44 sc_diff_analysis-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Jul-30 08:44 sc_diff_analysis-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       65 b- defN 21-Jul-30 08:44 sc_diff_analysis-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 21-Jul-30 08:44 sc_diff_analysis-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1577 b- defN 21-Jul-30 08:44 sc_diff_analysis-0.0.9.dist-info/RECORD
+17 files, 61720 bytes uncompressed, 19262 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -1,70 +1,52 @@
 Filename: sc_diff_analysis/__init__.py
 Comment: 
 
-Filename: sc_diff_analysis/main.py
-Comment: 
-
-Filename: sc_diff_analysis/utils.py
-Comment: 
-
-Filename: sc_diff_analysis/analyzer/__init__.py
-Comment: 
-
-Filename: sc_diff_analysis/analyzer/branch_summary_group_by_branch_diff_analyzer.py
+Filename: sc_diff_analysis/diff_analyzer.py
 Comment: 
 
-Filename: sc_diff_analysis/analyzer/branch_summary_group_by_item_type_diff_analyzer.py
+Filename: sc_diff_analysis/diff_analyzer_group_by_item_type.py
 Comment: 
 
-Filename: sc_diff_analysis/analyzer/common_summary_diff_analyzer.py
-Comment: 
-
-Filename: sc_diff_analysis/analyzer/customer_summary_diff_analyzer.py
-Comment: 
-
-Filename: sc_diff_analysis/analyzer/diff_analyzer.py
+Filename: sc_diff_analysis/main.py
 Comment: 
 
-Filename: sc_diff_analysis/analyzer/loan_detail_summary_diff_analyzer.py
+Filename: sc_diff_analysis/utils.py
 Comment: 
 
-Filename: sc_diff_analysis/analyzer/manager_summary_diff_analyzer.py
+Filename: sc_diff_analysis/configs/__init__.py
 Comment: 
 
-Filename: sc_diff_analysis/analyzer/xinka_summary_diff_analyzer.py
+Filename: sc_diff_analysis/configs/default.py
 Comment: 
 
 Filename: sc_diff_analysis/tests/__init__.py
 Comment: 
 
-Filename: sc_diff_analysis/tests/merge_tests.py
-Comment: 
-
-Filename: sc_diff_analysis/tests/sample_config/production-inclusive-balance-detail.yml
+Filename: sc_diff_analysis/tests/pandas_test/__init__.py
 Comment: 
 
-Filename: sc_diff_analysis/tests/sample_config/production-peak-season.yml
+Filename: sc_diff_analysis/tests/pandas_test/pandas_test.py
 Comment: 
 
 Filename: sc_diff_analysis/tests/sample_config/production.yml
 Comment: 
 
-Filename: sc_diff_analysis-0.0.29.dist-info/LICENSE
+Filename: sc_diff_analysis-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: sc_diff_analysis-0.0.29.dist-info/METADATA
+Filename: sc_diff_analysis-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: sc_diff_analysis-0.0.29.dist-info/WHEEL
+Filename: sc_diff_analysis-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: sc_diff_analysis-0.0.29.dist-info/entry_points.txt
+Filename: sc_diff_analysis-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: sc_diff_analysis-0.0.29.dist-info/top_level.txt
+Filename: sc_diff_analysis-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: sc_diff_analysis-0.0.29.dist-info/RECORD
+Filename: sc_diff_analysis-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sc_diff_analysis/__init__.py

```diff
@@ -1,10 +1,10 @@
 # The MIT License (MIT)
 #
-# Copyright (c) 2024 Scott Lau
+# Copyright (c) 2021 Scott Lau
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,10 +16,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = "0.0.29"
-
-PROJECT_NAME = 'sc-diff-analysis'
+__version__ = "0.0.9"
```

## sc_diff_analysis/main.py

```diff
@@ -1,10 +1,10 @@
 # The MIT License (MIT)
 #
-# Copyright (c) 2024 Scott Lau
+# Copyright (c) 2021 Scott Lau
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,36 +18,29 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import logging
 
-from sc_utilities import Singleton
-from sc_utilities import log_init
+from scutils import Singleton
+from scutils import log_init
 
 log_init()
 
-from .analyzer import DiffAnalyzer
-from sc_config import ConfigUtils
-
-from sc_diff_analysis import PROJECT_NAME, __version__
+from .diff_analyzer_group_by_item_type import DiffAnalyzerGroupByItemType
 
 
 class Runner(metaclass=Singleton):
 
     def __init__(self):
-        project_name = PROJECT_NAME
-        ConfigUtils.clear(project_name)
-        self._config = ConfigUtils.get_config(project_name)
+        pass
 
     def run(self) -> int:
-        logging.getLogger(__name__).info("program {} version {}".format(PROJECT_NAME, __version__))
-        analyzer = DiffAnalyzer(self._config)
-        return analyzer.analysis()
+        return DiffAnalyzerGroupByItemType().analysis()
 
 
 def main() -> int:
     try:
         state = Runner().run()
     except Exception as e:
         logging.getLogger(__name__).exception('An error occurred.', exc_info=e)
```

## sc_diff_analysis/utils.py

```diff
@@ -1,10 +1,10 @@
 #  The MIT License (MIT)
 #
-#  Copyright (c) 2024. Scott Lau
+#  Copyright (c) 2021. Scott Lau
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
 #  furnished to do so, subject to the following conditions:
@@ -15,22 +15,51 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
+import logging
 
+from scconfig.config import Config
+from scutils import Singleton
+
+from .configs.default import DEFAULT_CONFIG
 
-__all__ = {
-    "MoneyUtils",
-}
 
+class ConfigUtils(metaclass=Singleton):
+    """
+    配置文件相关工具类
+    """
 
-from sc_utilities import Singleton
+    _config = None
+
+    @classmethod
+    def load_configurations(cls):
+        """
+        加载配置文件
+        :return:
+        """
+        try:
+            # load configurations
+            cls._config = Config.create(project_name="sc-diff-analysis", defaults=DEFAULT_CONFIG)
+        except Exception as error:
+            cls._config = {}
+            logging.getLogger(__name__).exception("failed to read configuration", exc_info=error)
+
+    @classmethod
+    def get_config(cls):
+        """
+        获取配置信息
+        :return: 配置信息字典
+        """
+        if cls._config is None:
+            cls.load_configurations()
+        return cls._config
 
 
 class MoneyUtils(metaclass=Singleton):
     """
     金额相关工具类
     """
 
@@ -49,7 +78,13 @@
         if amount_unit == "元":
             divider = 1
         elif amount_unit == "万元":
             divider = 10000
         elif amount_unit == "亿元":
             divider = 100000000
         return divider
+
+
+__all__ = {
+    "ConfigUtils",
+    "MoneyUtils",
+}
```

## sc_diff_analysis/tests/__init__.py

```diff
@@ -1,10 +1,10 @@
 # The MIT License (MIT)
 #
-# Copyright (c) 2024 Scott Lau
+# Copyright (c) 2021 Scott Lau
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

## sc_diff_analysis/tests/sample_config/production.yml

```diff
@@ -1,264 +1,84 @@
 # 说明：
 # 1. 如下配置的索引均从0开始计数，第1列为0、第2列为1，依此类推
 # 2. 如果需要配置的是列名，则此列名在Excel中必须唯一
 
-environment: production
-
-# 批量
-batch:
-  # 零售批量重跑日期列表
-  retail_rerun_dates:
-    - 20211231
-    - 20220213
-    - 20220216
-
-
 # 机构配置
 branch:
   # 选中需要处理的机构清单
   selected_list:
-    - 公司业务三部
-    - 公司业务二部
-    - 分行营业部
-    - 南沙支行
-    - 江湾支行
-    - 粤能支行
-    - 财智支行
-    - 黄埔支行
-    - 东风支行
+    - "东风支行"
+    - "中小企业管理部"
+    - "人力财务部"
+    - "公司业务一部"
+    - "公司业务三部"
+    - "公司业务二部"
+    - "公司业务管理部"
+    - "分行营业部"
+    - "南沙支行"
+    - "广州分行公共"
+    - "广州分行行领导"
+    - "授信审批部"
+    - "江湾支行"
+    - "法律合规部"
+    - "粤能支行"
+    - "综合保卫部"
+    - "计划财务部"
+    - "财智支行"
+    - "运营管理部"
+    - "零售业务管理部"
+    - "风险管理部"
+    - "黄埔支行"
 
 # 差异分析（比较结果为第二个文件的数据减去第一个文件的数据）
 diff:
   # 年初分析结果文件路径
-  yearly_base_file_path: ./20211231/广州分行考核指标统计.xlsx
+  yearly_base_file_path: "./20201231/广州分行考核指标统计.xlsx"
   # 季度初分析结果文件路径
-  seasonal_base_file_path: ./2022/广州分行考核指标统计.xlsx
+  seasonal_base_file_path: "./20210331/广州分行考核指标统计.xlsx"
   # 月初分析结果文件路径
-  monthly_base_file_path: ./20220331/广州分行考核指标统计.xlsx
+  monthly_base_file_path: "./20210430/广州分行考核指标统计.xlsx"
   # 上周分析结果文件路径
-  last_week_file_path: ./20220401/广州分行考核指标统计.xlsx
+  last_week_file_path: "./20210531/广州分行考核指标统计.xlsx"
   # 昨日分析结果文件路径
-  yesterday_file_path: ./20220406/广州分行考核指标统计.xlsx
+  yesterday_file_path: "./20210628/广州分行考核指标统计.xlsx"
   # 当日分析结果文件路径
-  current_day_file_path: ./20220407/广州分行考核指标统计.xlsx
-  # # 基数数据文件路径
-  # base_file_path: ./base/广州分行考核指标统计.xlsx
-  # # 目标数据文件路径
-  # target_file_path: ./target/广州分行考核指标统计.xlsx
+  current_day_file_path: "./20210629/广州分行考核指标统计.xlsx"
   # 生成的目标Excel文件存放路径
-  target_directory: ./
+  target_directory: "./"
   # 目标文件名称
-  target_filename: 广州分行考核指标差异分析.xlsx
+  target_filename: "广州分行考核指标差异分析.xlsx"
+  # 生成的Excel中Sheet的名称
+  target_sheet_name: "机构汇总-差异分析"
+  # 指标名称列名称
+  target_compare_item_column_name: "指标名称"
   # 比较类型列名称
-  target_compare_type_column_name: 比较类型
+  target_compare_type_column_name: "比较类型"
   # 较年初分析结果列名称
-  target_yearly_base_compare_column_name: 较年初
+  target_yearly_base_compare_column_name: "较年初"
   # 较季初分析结果列名称
-  target_seasonal_base_compare_column_name: 较季初
+  target_seasonal_base_compare_column_name: "较季初"
   # 较月初分析结果列名称
-  target_monthly_base_compare_column_name: 较月初
+  target_monthly_base_compare_column_name: "较月初"
   # 较上周分析结果列名称
-  target_last_week_compare_column_name: 较上周
+  target_last_week_compare_column_name: "较上周"
   # 较昨日分析结果列名称
-  target_yesterday_compare_column_name: 较昨日
+  target_yesterday_compare_column_name: "较昨日"
   # 当前日期分析结果列名称
-  target_current_day_column_name: 时点数
-  # 较基数分析结果列名称
-  target_base_compare_column_name: 较基数
-  # 较目标差距分析结果列名称
-  target_target_compare_column_name: 较目标
-  # 比较类型排序规则
-  compare_type_orders:
-    - 时点数
-    - 较年初
-    - 较季初
-    - 较月初
-    - 较上周
-    - 较昨日
-    - 较基数
-    - 较目标
-  # 机构汇总
-  branch_summary_group_by_branch:
-    enabled: True
-    # 生成的Excel中Sheet的名称
-    target_sheet_name: 机构汇总(按机构分组)-差异分析
-    # Sheet名称
-    sheet_name: 机构汇总
-    # 表头行索引
-    header_row: 0
-    # 索引列名称（可以是多个，Excel中列名必须唯一）
-    index_column_names:
-      - 所在部门
-    # 待分析差异列名称列表（Excel中列名必须唯一）
-    diff_column_list:
-      湘籍客户数: 户
-      财富客户数: 户
-      储蓄存款(时期): 元
-      储蓄存款(时点): 元
-      理财年化日均: 元
-      理财中收（CIF）: 元
-      基金确认金额: 元
-      基金确认金额中收: 元
-      贵金属交易金额: 元
-      贵金属交易手续费: 元
-      保费金额: 元
-      代理保险中收: 元
-      分期投放: 万元
-      信用卡有效发卡（2022考核口径）: 张
-      信用卡发卡量: 张
-      贷款合计: 万元
-      个经小计: 万元
-      个消小计: 万元
-      个人业务非息收入小计: 元
-      信用卡非息收入合计: 元
-      分期余额: 万元
-      大额分期余额: 元
-      消贷小计: 万元
-      易得贷: 万元
-      心卡: 万元
-      按揭: 万元
-      秒贷: 万元
-      消费: 万元
-
-  # 机构汇总（按指标类型分组）
-  branch_summary_group_by_item_type:
-    enabled: True
-    # 生成的Excel中Sheet的名称
-    target_sheet_name: 机构汇总(按指标类型分组)-差异分析
-    # 指标名称列名称
-    target_compare_item_column_name: 指标名称
-    # Sheet名称
-    sheet_name: 机构汇总
-    # 表头行索引
-    header_row: 0
-    # 索引列名称（可以是多个，Excel中列名必须唯一）
-    index_column_names:
-      - 所在部门
-    # 待分析差异列名称列表（Excel中列名必须唯一）
-    diff_column_list:
-      湘籍客户数: 户
-      财富客户数: 户
-      储蓄存款(时期): 元
-      储蓄存款(时点): 元
-      理财年化日均: 元
-      理财中收（CIF）: 元
-      基金确认金额: 元
-      基金确认金额中收: 元
-      贵金属交易金额: 元
-      贵金属交易手续费: 元
-      保费金额: 元
-      代理保险中收: 元
-      分期投放: 万元
-      信用卡有效发卡（2022考核口径）: 张
-      信用卡发卡量: 张
-      贷款合计: 万元
-      个经小计: 万元
-      个消小计: 万元
-      个人业务非息收入小计: 元
-      信用卡非息收入合计: 元
-      分期余额: 万元
-      大额分期余额: 元
-      消贷小计: 万元
-      易得贷: 万元
-      心卡: 万元
-      按揭: 万元
-      秒贷: 万元
-      消费: 万元
-
-  # 其他自定义Sheet的汇总
-  customized_summary:
-    "心卡-按客户统计":
-      enabled: True
-      module_name: sc_diff_analysis.analyzer.xinka_summary_diff_analyzer
-      class_name: XinkaSummaryDiffAnalyzer
-      positive_column_name: 投放
-      negative_column_name: 还款
-      branch_column_name: 所在部门
-      # 生成的Excel中Sheet的名称
-      target_sheet_name: 心卡-按客户统计-差异分析
-      # Sheet名称
-      sheet_name: 心卡-按客户统计
-      # 表头行索引
-      header_row: 0
-      # 索引列名称（可以是多个，Excel中列名必须唯一）
-      index_column_names:
-        - 客户姓名
-        - 联系方式
-        - 客户经理
-        - 所在部门
-      # 待分析差异列名称列表（Excel中列名必须唯一）
-      diff_column_list:
-        心卡: 万元
-    "线下+房抵贷+秒贷-按客户统计":
-      enabled: True
-      module_name: sc_diff_analysis.analyzer.loan_detail_summary_diff_analyzer
-      class_name: LoanDetailSummaryDiffAnalyzer
-      positive_column_name: 投放
-      negative_column_name: 还款
-      branch_column_name: 所在部门
-      # 生成的Excel中Sheet的名称
-      target_sheet_name: 线下+房抵贷+秒贷-按客户统计-差异分析
-      # Sheet名称
-      sheet_name: 线下+房抵贷+秒贷-按客户统计
-      # 表头行索引
-      header_row: 0
-      # 索引列名称（可以是多个，Excel中列名必须唯一）
-      index_column_names:
-        - 客户名称
-        - 证件号码
-        - 客户经理
-        - 所在部门
-      # 待分析差异列名称列表（Excel中列名必须唯一）
-      diff_column_list:
-        按揭: 万元
-        消费: 万元
-        秒贷: 万元
-        经营: 万元
-    # 客户经理汇总
-    "客户经理汇总":
-      enabled: True
-      module_name: sc_diff_analysis.analyzer.customer_summary_diff_analyzer
-      class_name: CustomerSummaryDiffAnalyzer
-      # 生成的Excel中Sheet的名称
-      target_sheet_name: 客户经理汇总-差异分析
-      # Sheet名称
-      sheet_name: 客户经理汇总
-      # 表头行索引
-      header_row: 0
-      # 索引列名称（可以是多个，Excel中列名必须唯一）
-      index_column_names:
-        - 姓名
-      split_branches:
-        enabled: True
-        column_name: 所在部门
-      # 待分析差异列名称列表（Excel中列名必须唯一）
-      diff_column_list:
-        湘籍客户数: 户
-        财富客户数: 户
-        储蓄存款(时期): 元
-        储蓄存款(时点): 元
-        贷款合计: 万元
-        个经小计: 万元
-        个消小计: 万元
-        信用卡有效发卡（2022考核口径）: 张
-        信用卡发卡量: 张
-        分期投放: 万元
-        理财年化日均: 元
-        理财中收（CIF）: 元
-        基金确认金额: 元
-        基金确认金额中收: 元
-        贵金属交易金额: 元
-        贵金属交易手续费: 元
-        保费金额: 元
-        代理保险中收: 元
-        信用卡进件: 张
-        个人业务非息收入小计: 元
-        信用卡非息收入合计: 元
-        分期余额: 万元
-        大额分期余额: 元
-        消贷小计: 万元
-        易得贷: 万元
-        心卡: 万元
-        按揭: 万元
-        秒贷: 万元
-        消费: 万元
+  target_current_day_column_name: "时点数"
+  # Sheet名称
+  sheet_name: "机构汇总"
+  # 表头行索引
+  header_row: 0
+  # 所属机构列名称（Excel中列名必须唯一）
+  branch_column_name: "所在部门"
+  # 待分析差异列名称列表（Excel中列名必须唯一）
+  diff_column_list:
+    "贷款合计": "万元"
+    "个经小计": "万元"
+    "个消小计": "万元"
+    "分期投放": "万元"
+    "信用卡发卡量": "张"
+    "信用卡收入": "元"
+    "个人业务非息收入小计": "元"
+    "财富客户数": "户"
+    "湘籍客户数": "户"
```

## Comparing `sc_diff_analysis/analyzer/__init__.py` & `sc_diff_analysis/configs/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,21 @@
-#  The MIT License (MIT)
+# The MIT License (MIT)
 #
-#  Copyright (c) 2024. Scott Lau
+# Copyright (c) 2021 Scott Lau
 #
-#  Permission is hereby granted, free of charge, to any person obtaining a copy
-#  of this software and associated documentation files (the "Software"), to deal
-#  in the Software without restriction, including without limitation the rights
-#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-#  copies of the Software, and to permit persons to whom the Software is
-#  furnished to do so, subject to the following conditions:
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-#  The above copyright notice and this permission notice shall be included in all
-#  copies or substantial portions of the Software.
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 #
-#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-#  SOFTWARE.
-
-__all__ = [
-    "BranchSummaryGroupByBranchDiffAnalyzer",
-    "BranchSummaryGroupByItemTypeDiffAnalyzer",
-    "CommonSummaryDiffAnalyzer",
-    "DiffAnalyzer",
-]
-
-from .branch_summary_group_by_branch_diff_analyzer import BranchSummaryGroupByBranchDiffAnalyzer
-from .branch_summary_group_by_item_type_diff_analyzer import BranchSummaryGroupByItemTypeDiffAnalyzer
-from .common_summary_diff_analyzer import CommonSummaryDiffAnalyzer
-# DiffAnalyzer的引用必须放到最后，因为它引用上面两个，如果调整顺序会引起循环引入的问题
-from .diff_analyzer import DiffAnalyzer
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `sc_diff_analysis/analyzer/loan_detail_summary_diff_analyzer.py` & `sc_diff_analysis/tests/pandas_test/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  The MIT License (MIT)
 #
-#  Copyright (c) 2024. Scott Lau
+#  Copyright (c) 2021. Scott Lau
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
 #  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 #  copies of the Software, and to permit persons to whom the Software is
 #  furnished to do so, subject to the following conditions:
@@ -16,19 +16,7 @@
 #  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
-from config42 import ConfigManager
-
-from .xinka_summary_diff_analyzer import XinkaSummaryDiffAnalyzer
-
-
-class LoanDetailSummaryDiffAnalyzer(XinkaSummaryDiffAnalyzer):
-    """
-    贷款明细汇总差异分析类
-    """
-
-    def __init__(self, *, config: ConfigManager, diff_sheet_name: str, is_first_analyzer=False):
-        super().__init__(config=config, diff_sheet_name=diff_sheet_name, is_first_analyzer=is_first_analyzer)
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `sc_diff_analysis-0.0.29.dist-info/LICENSE` & `sc_diff_analysis-0.0.9.dist-info/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2024 Scott Lau
+Copyright (c) 2021 Scott Lau
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `sc_diff_analysis-0.0.29.dist-info/METADATA` & `sc_diff_analysis-0.0.9.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-diff-analysis
-Version: 0.0.29
+Version: 0.0.9
 Summary: A python project to analysis the difference between two excel reports
 Home-page: https://github.com/Scott-Lau/sc-diff-analysis
 Author: Scott Lau
 Author-email: exceedego@126.com
 License: MIT
 Keywords: python difference reports
 Platform: POSIX
@@ -15,29 +15,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 License-File: LICENSE
-Requires-Dist: sc-utilities >=0.0.7
-Requires-Dist: sc-config >=0.0.11
-Requires-Dist: sc-analyzer-base >=0.0.18
-Requires-Dist: pandas >=1.3.2
-Requires-Dist: openpyxl >=3.0.7
+Requires-Dist: sc-utilities (>=0.0.5)
+Requires-Dist: sc-config (>=0.0.7)
+Requires-Dist: pandas (>=1.2.5)
+Requires-Dist: openpyxl (>=3.0.7)
 
 .. image:: https://badge.fury.io/py/sc-diff-analysis.svg
     :target: https://badge.fury.io/py/sc-diff-analysis
 .. image:: https://img.shields.io/pypi/pyversions/sc-diff-analysis
     :alt: PyPI - Python Version
 
-A simple Python project
+A simple Python project sample structure
 ========================================
 
-This project provides a simple utility for analyzing difference of retail reports.
+This project provides a sample structure for creating python project.
 
 
 Installation
 ------------
 
 It is possible to install the tool with `pip`::
 
@@ -62,7 +61,9 @@
 License
 -------
 
 The script is released under the MIT License.  The MIT License is registered
 with and approved by the Open Source Initiative [1]_.
 
 .. [1] https://opensource.org/licenses/MIT
+
+
```

## Comparing `sc_diff_analysis-0.0.29.dist-info/RECORD` & `sc_diff_analysis-0.0.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,17 @@
-sc_diff_analysis/__init__.py,sha256=1Nic2Qu5cu7RdiK_4LRxIZ_CafNa3qfEsNhfToM9JsY,1173
-sc_diff_analysis/main.py,sha256=rSq6vWCiz32NX7XL2qLld67UwSRIenFnSwp5fV_3Ci4,1960
-sc_diff_analysis/utils.py,sha256=7k_Cc1D8q17Q47PWSOc2QARy4ey1f1RHcgYNGbueqKA,1852
-sc_diff_analysis/analyzer/__init__.py,sha256=A5JPfOo1g1en9gyJRrWxRaqgmf137-xDMN-NrdjISz4,1725
-sc_diff_analysis/analyzer/branch_summary_group_by_branch_diff_analyzer.py,sha256=uYlJfRlBnXLVw7dO22ez7gd7fbsX4gjhi9Fr9IreI3c,3880
-sc_diff_analysis/analyzer/branch_summary_group_by_item_type_diff_analyzer.py,sha256=V196YhOIxFCYB6ejmlIFVwe27ZEFe4smHa16AvXX_b0,9875
-sc_diff_analysis/analyzer/common_summary_diff_analyzer.py,sha256=QHSf7Ei8lQuV_dDWMCIeFuaplvUWsS1ioquoK1CYGM4,3083
-sc_diff_analysis/analyzer/customer_summary_diff_analyzer.py,sha256=BcSOtT_s5iOJ1xCDvbElARd6NuKEnXJ-Osvce96KvOY,5587
-sc_diff_analysis/analyzer/diff_analyzer.py,sha256=lIlYWKZ9EqAgJrbeM7LfXeepbiAXts6WgZ5LFrkvl40,4052
-sc_diff_analysis/analyzer/loan_detail_summary_diff_analyzer.py,sha256=UU_8_zEZ2pCMkhjYrmjZp5Y4XkEXPAMGl-n9DppPFto,1562
-sc_diff_analysis/analyzer/manager_summary_diff_analyzer.py,sha256=Wnfizux_VgJshuEbwktIpFyDWlOUQv9WySYXc2-8l5g,5586
-sc_diff_analysis/analyzer/xinka_summary_diff_analyzer.py,sha256=hCbCItUF6-uJq65-7PeUowGZVYsAvETcOcIwH62hIqk,21586
-sc_diff_analysis/tests/__init__.py,sha256=Fgsv7kmTdE6VUCY09rmQiM4eHHaziC60aOF0kA6Y8Pw,1114
-sc_diff_analysis/tests/merge_tests.py,sha256=Rh25YAZmoW8hn31cQM3Lgn5EOSu1-VhOVFnv3y02IG8,4901
-sc_diff_analysis/tests/sample_config/production-inclusive-balance-detail.yml,sha256=rLsPnp1zum_PCHrK9_w7eVPtYUFdPAVcNbZO3DoJPww,5063
-sc_diff_analysis/tests/sample_config/production-peak-season.yml,sha256=hApzeGD7SYSx_VcJIbsPQdhnnB2l6eP7i06QK6BBLBE,7102
-sc_diff_analysis/tests/sample_config/production.yml,sha256=3bTg9bYJhAXJl4G9WGkMQ5R--dzdYnD3uEp8F0k4Da0,8697
-sc_diff_analysis-0.0.29.dist-info/LICENSE,sha256=gAuQR9WCISwCCgA3rUNidk-y12Z6fGCGvDp8zPNEidw,1076
-sc_diff_analysis-0.0.29.dist-info/METADATA,sha256=jK2snMrgu90FYhtHHU8nccsRKIyiheZzGzaysI2Mbjw,2124
-sc_diff_analysis-0.0.29.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-sc_diff_analysis-0.0.29.dist-info/entry_points.txt,sha256=CInhv-gfYbRh985B78jS12Ur7IIT0AE50JvLtv4wooo,64
-sc_diff_analysis-0.0.29.dist-info/top_level.txt,sha256=gLhJrGt8uDTBy0VsAA4uI3zXp4FFrLqh1ntY8DfTA5k,17
-sc_diff_analysis-0.0.29.dist-info/RECORD,,
+sc_diff_analysis/__init__.py,sha256=8CLWHYRcnWdTW0au14M2iy1Ta6sqqcusn6cltgl-kqc,1137
+sc_diff_analysis/diff_analyzer.py,sha256=qy2-rEHLtoUoQZyXUD_KLgo-hJv34QDbRXCYqck7CCU,20264
+sc_diff_analysis/diff_analyzer_group_by_item_type.py,sha256=6yUR7lKcKAq338wl_Fj6Uh_hE5LKQD79D9Eqr7mZM9Y,20864
+sc_diff_analysis/main.py,sha256=YbH0KfnsU92ND7v2eY8qI-aRgWU68TYRa45aulx3n_s,1651
+sc_diff_analysis/utils.py,sha256=k-W6AXMn9QAgF8qfzQOAsBU7IAC3Wk2dahmk-4fsfYA,2724
+sc_diff_analysis/configs/__init__.py,sha256=rg-0D5uJamNQhAE7bZod5fptToqSlX-d16SAwuiBhKA,1114
+sc_diff_analysis/configs/default.py,sha256=ULDcYcxLj90ZinHIgSmIEtzrTHX6aD-mlV5EbReW918,1241
+sc_diff_analysis/tests/__init__.py,sha256=rg-0D5uJamNQhAE7bZod5fptToqSlX-d16SAwuiBhKA,1114
+sc_diff_analysis/tests/pandas_test/__init__.py,sha256=geiVmsc9iPhOzHUHdCPrdVcoT42GBjMoafy2eT_JloI,1133
+sc_diff_analysis/tests/pandas_test/pandas_test.py,sha256=blLpJ6oAlcYRm43XwtBh3W7e6OmSxfsdsswEvh_TPpU,2542
+sc_diff_analysis/tests/sample_config/production.yml,sha256=Yun8UVuagHDnx6zgU2PSXIfZmqunz-5ZurNMnPYcKKw,3014
+sc_diff_analysis-0.0.9.dist-info/LICENSE,sha256=qE1ONTqO-JURigwx0cciswGHX9-E7RkwoDtJCqnqBT4,1076
+sc_diff_analysis-0.0.9.dist-info/METADATA,sha256=4MQaON-aa5pyc2q-YWhJg1xNOhdyFL6aYqCFxDlYtJQ,2095
+sc_diff_analysis-0.0.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sc_diff_analysis-0.0.9.dist-info/entry_points.txt,sha256=Qq9oxWvTUKWbfyLzZ5qD9jPEGvqjV8GWxDBZWH7O2pw,65
+sc_diff_analysis-0.0.9.dist-info/top_level.txt,sha256=gLhJrGt8uDTBy0VsAA4uI3zXp4FFrLqh1ntY8DfTA5k,17
+sc_diff_analysis-0.0.9.dist-info/RECORD,,
```

