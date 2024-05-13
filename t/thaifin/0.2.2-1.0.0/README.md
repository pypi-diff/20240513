# Comparing `tmp/thaifin-0.2.2.tar.gz` & `tmp/thaifin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thaifin-0.2.2.tar", last modified: Sat Jan 30 18:56:42 2021, max compression
+gzip compressed data, was "thaifin-1.0.0.tar", max compression
```

## Comparing `thaifin-0.2.2.tar` & `thaifin-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0      757 2021-01-30 18:56:34.648995 thaifin-0.2.2/LICENSE.md
--rw-r--r--   0        0        0     7577 2021-01-30 18:56:34.648995 thaifin-0.2.2/README.md
--rw-r--r--   0        0        0      859 2021-01-30 18:56:34.652996 thaifin-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       53 2021-01-30 18:56:34.652996 thaifin-0.2.2/thaifin/__init__.py
--rw-r--r--   0        0        0        0 2021-01-30 18:56:34.652996 thaifin-0.2.2/thaifin/models/__init__.py
--rw-r--r--   0        0        0        0 2021-01-30 18:56:34.652996 thaifin-0.2.2/thaifin/sources/__init__.py
--rw-r--r--   0        0        0     4299 2021-01-30 18:56:34.652996 thaifin-0.2.2/thaifin/sources/finnomena.py
--rw-r--r--   0        0        0     1379 2021-01-30 18:56:34.652996 thaifin-0.2.2/thaifin/sources/set.py
--rw-r--r--   0        0        0      340 2021-01-30 18:56:34.652996 thaifin-0.2.2/thaifin/sources/settrade.py
--rw-r--r--   0        0        0     2166 2021-01-30 18:56:34.652996 thaifin-0.2.2/thaifin/stock.py
--rw-r--r--   0        0        0     8815 2021-01-30 18:56:43.015348 thaifin-0.2.2/setup.py
--rw-r--r--   0        0        0     8577 2021-01-30 18:56:43.016058 thaifin-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      757 2024-05-13 15:42:01.894346 thaifin-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0     7566 2024-05-13 18:14:34.054670 thaifin-1.0.0/README.md
+-rw-r--r--   0        0        0      847 2024-05-13 18:07:20.904583 thaifin-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       53 2024-05-13 15:42:01.894346 thaifin-1.0.0/thaifin/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 15:42:01.894346 thaifin-1.0.0/thaifin/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:46:02.003588 thaifin-1.0.0/thaifin/py.typed
+-rw-r--r--   0        0        0        0 2024-05-13 15:42:01.894346 thaifin-1.0.0/thaifin/sources/__init__.py
+-rw-r--r--   0        0        0       54 2024-05-13 17:08:17.936671 thaifin-1.0.0/thaifin/sources/finnomena/__init__.py
+-rw-r--r--   0        0        0     1125 2024-05-13 17:17:14.214269 thaifin-1.0.0/thaifin/sources/finnomena/api.py
+-rw-r--r--   0        0        0     1745 2024-05-13 17:38:25.962648 thaifin-1.0.0/thaifin/sources/finnomena/model.py
+-rw-r--r--   0        0        0     1379 2024-05-13 15:42:01.894346 thaifin-1.0.0/thaifin/sources/set.py
+-rw-r--r--   0        0        0      340 2024-05-13 15:42:01.894346 thaifin-1.0.0/thaifin/sources/settrade.py
+-rw-r--r--   0        0        0     4086 2024-05-13 18:27:27.416893 thaifin-1.0.0/thaifin/stock.py
+-rw-r--r--   0        0        0     8610 1970-01-01 00:00:00.000000 thaifin-1.0.0/PKG-INFO
```

### Comparing `thaifin-0.2.2/LICENSE.md` & `thaifin-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `thaifin-0.2.2/README.md` & `thaifin-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -67,53 +67,54 @@
 # [11 rows x 35 columns]
 
 ```
 
 ### Columns Data
 
 ```python
-class FinancialSheet(BaseModel):
-    SecurityID: Optional[int]
-    Fiscal: Optional[int]
-    Quarter: Optional[int]
-    Cash: Optional[float]
-    DA: Optional[float]
-    DebtToEquity: Optional[float]
-    Equity: Optional[float]
-    EarningPerShare: Optional[float]
-    EarningPerShareYoY: Optional[float]
-    EarningPerShareQoQ: Optional[float]
-    GPM: Optional[float]
-    GrossProfit: Optional[float]
-    NetProfit: Optional[float]
-    NetProfitYoY: Optional[float]
-    NetProfitQoQ: Optional[float]
-    NPM: Optional[float]
-    Revenue: Optional[float]
-    RevenueYoY: Optional[float]
-    RevenueQoQ: Optional[float]
-    ROA: Optional[float]
-    ROE: Optional[float]
-    SGA: Optional[float]
-    SGAPerRevenue: Optional[float]
-    TotalDebt: Optional[float]
-    DividendYield: Optional[float]
-    BookValuePerShare: Optional[float]
-    Close: Optional[float]
-    MKTCap: Optional[float]
-    PriceEarningRatio: Optional[float]
-    PriceBookValue: Optional[float]
-    EVPerEbitDA: Optional[float]
-    EbitDATTM: Optional[float]
-    PaidUpCapital: Optional[float]
-    CashCycle: Optional[float]
-    OperatingActivities: Optional[float]
-    InvestingActivities: Optional[float]
-    FinancingActivities: Optional[float]
-    Asset: Optional[float]
+class QuarterFinancialSheetDatum(BaseModel):
+    security_id: str
+    fiscal: int
+    quarter: int
+    cash: Optional[str]
+    da: Optional[str]
+    debt_to_equity: Optional[str]
+    equity: Optional[str]
+    earning_per_share: Optional[str]
+    earning_per_share_yoy: Optional[str]
+    earning_per_share_qoq: Optional[str]
+    gpm: Optional[str]
+    gross_profit: Optional[str]
+    net_profit: Optional[str]
+    net_profit_yoy: Optional[str]
+    net_profit_qoq: Optional[str]
+    npm: Optional[str]
+    revenue: Optional[str]
+    revenue_yoy: Optional[str]
+    revenue_qoq: Optional[str]
+    roa: Optional[str]
+    roe: Optional[str]
+    sga: Optional[str]
+    sga_per_revenue: Optional[str]
+    total_debt: Optional[str]
+    dividend_yield: Optional[str]
+    book_value_per_share: Optional[str]
+    close: Optional[str]
+    mkt_cap: Optional[str]
+    price_earning_ratio: Optional[str]
+    price_book_value: Optional[str]
+    ev_per_ebit_da: Optional[str]
+    ebit_dattm: Optional[str]
+    paid_up_capital: Optional[str]
+    cash_cycle: Optional[str]
+    operating_activities: Optional[str]
+    investing_activities: Optional[str]
+    financing_activities: Optional[str]
+    asset: Optional[str]
+    end_of_year_date: Optional[str]
 ```
 
 ## Disclaimer
 
 เราไม่รับประกันความเสียหายใดๆทั้งสิ้นที่เกิดจาก แหล่งข้อมูล, library, source code,sample code, documentation, library dependencies และอื่นๆ
 
 ## FAQ
```

### Comparing `thaifin-0.2.2/pyproject.toml` & `thaifin-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "thaifin"
-version = "0.2.2"
+version = "1.0.0"
 description = "A Python library for access thai stock fundamental data up to 10+ years."
 authors = ["Nutchanon Ninyawee <me@nutchanon.org>"]
 license = "ISC"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.11"
 beautifulsoup4 = "^4.9.1"
 requests = "^2.24.0"
 lxml = "^4.5.1"
 furl = "^2.1.0"
-pydantic = "^1.6.1"
 arrow = "^0.16.0"
 fuzzywuzzy = "^0.18.0"
 python-Levenshtein = { version = "^0.12.0", optional = true }
 pandas = "^1.0.5"
 numpy = "^1.19.5"
 cachetools = "^4.2.1"
 tenacity = "^6.3.1"
+httpx = "^0.27.0"
+pydantic = "^2.7.1"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.extras]
+full = ["python-levenshtein"]
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.2.0"
 jupyter = "^1.0.0"
-pytest = "^5.4.3"
 tqdm = "^4.47.0"
 openpyxl = "^3.0.4"
 lxml = "^4.5.1"
-datamodel-code-generator = "^0.5.30"
 pdoc = "^3.0.1"
 
-[tool.poetry.extras]
-full = ["python-levenshtein"]
-
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `thaifin-0.2.2/thaifin/sources/set.py` & `thaifin-1.0.0/thaifin/sources/set.py`

 * *Files identical despite different names*

### Comparing `thaifin-0.2.2/PKG-INFO` & `thaifin-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: thaifin
-Version: 0.2.2
+Version: 1.0.0
 Summary: A Python library for access thai stock fundamental data up to 10+ years.
 License: ISC
 Author: Nutchanon Ninyawee
 Author-email: me@nutchanon.org
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: full
 Requires-Dist: arrow (>=0.16.0,<0.17.0)
 Requires-Dist: beautifulsoup4 (>=4.9.1,<5.0.0)
 Requires-Dist: cachetools (>=4.2.1,<5.0.0)
 Requires-Dist: furl (>=2.1.0,<3.0.0)
 Requires-Dist: fuzzywuzzy (>=0.18.0,<0.19.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: lxml (>=4.5.1,<5.0.0)
 Requires-Dist: numpy (>=1.19.5,<2.0.0)
 Requires-Dist: pandas (>=1.0.5,<2.0.0)
-Requires-Dist: pydantic (>=1.6.1,<2.0.0)
-Requires-Dist: python-Levenshtein (>=0.12.0,<0.13.0); extra == "full"
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
+Requires-Dist: python-Levenshtein (>=0.12.0,<0.13.0) ; extra == "full"
 Requires-Dist: requests (>=2.24.0,<3.0.0)
 Requires-Dist: tenacity (>=6.3.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 # thaifin: ข้อมูลพื้นฐานหุ้น ง่ายแค่สามบรรทัด
 
 > The same author as [PythaiNAV](https://github.com/CircleOnCircles/pythainav)
@@ -94,53 +95,54 @@
 # [11 rows x 35 columns]
 
 ```
 
 ### Columns Data
 
 ```python
-class FinancialSheet(BaseModel):
-    SecurityID: Optional[int]
-    Fiscal: Optional[int]
-    Quarter: Optional[int]
-    Cash: Optional[float]
-    DA: Optional[float]
-    DebtToEquity: Optional[float]
-    Equity: Optional[float]
-    EarningPerShare: Optional[float]
-    EarningPerShareYoY: Optional[float]
-    EarningPerShareQoQ: Optional[float]
-    GPM: Optional[float]
-    GrossProfit: Optional[float]
-    NetProfit: Optional[float]
-    NetProfitYoY: Optional[float]
-    NetProfitQoQ: Optional[float]
-    NPM: Optional[float]
-    Revenue: Optional[float]
-    RevenueYoY: Optional[float]
-    RevenueQoQ: Optional[float]
-    ROA: Optional[float]
-    ROE: Optional[float]
-    SGA: Optional[float]
-    SGAPerRevenue: Optional[float]
-    TotalDebt: Optional[float]
-    DividendYield: Optional[float]
-    BookValuePerShare: Optional[float]
-    Close: Optional[float]
-    MKTCap: Optional[float]
-    PriceEarningRatio: Optional[float]
-    PriceBookValue: Optional[float]
-    EVPerEbitDA: Optional[float]
-    EbitDATTM: Optional[float]
-    PaidUpCapital: Optional[float]
-    CashCycle: Optional[float]
-    OperatingActivities: Optional[float]
-    InvestingActivities: Optional[float]
-    FinancingActivities: Optional[float]
-    Asset: Optional[float]
+class QuarterFinancialSheetDatum(BaseModel):
+    security_id: str
+    fiscal: int
+    quarter: int
+    cash: Optional[str]
+    da: Optional[str]
+    debt_to_equity: Optional[str]
+    equity: Optional[str]
+    earning_per_share: Optional[str]
+    earning_per_share_yoy: Optional[str]
+    earning_per_share_qoq: Optional[str]
+    gpm: Optional[str]
+    gross_profit: Optional[str]
+    net_profit: Optional[str]
+    net_profit_yoy: Optional[str]
+    net_profit_qoq: Optional[str]
+    npm: Optional[str]
+    revenue: Optional[str]
+    revenue_yoy: Optional[str]
+    revenue_qoq: Optional[str]
+    roa: Optional[str]
+    roe: Optional[str]
+    sga: Optional[str]
+    sga_per_revenue: Optional[str]
+    total_debt: Optional[str]
+    dividend_yield: Optional[str]
+    book_value_per_share: Optional[str]
+    close: Optional[str]
+    mkt_cap: Optional[str]
+    price_earning_ratio: Optional[str]
+    price_book_value: Optional[str]
+    ev_per_ebit_da: Optional[str]
+    ebit_dattm: Optional[str]
+    paid_up_capital: Optional[str]
+    cash_cycle: Optional[str]
+    operating_activities: Optional[str]
+    investing_activities: Optional[str]
+    financing_activities: Optional[str]
+    asset: Optional[str]
+    end_of_year_date: Optional[str]
 ```
 
 ## Disclaimer
 
 เราไม่รับประกันความเสียหายใดๆทั้งสิ้นที่เกิดจาก แหล่งข้อมูล, library, source code,sample code, documentation, library dependencies และอื่นๆ
 
 ## FAQ
```

