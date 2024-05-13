# Comparing `tmp/pancakeswap-lottery-2.0.1.tar.gz` & `tmp/pancakeswap_lottery-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pancakeswap-lottery-2.0.1.tar", max compression
+gzip compressed data, was "pancakeswap_lottery-2.1.0.tar", max compression
```

## Comparing `pancakeswap-lottery-2.0.1.tar` & `pancakeswap_lottery-2.1.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1073 2021-07-08 10:14:05.893680 pancakeswap-lottery-2.0.1/LICENSE
--rw-r--r--   0        0        0     6814 2021-07-14 19:09:08.623332 pancakeswap-lottery-2.0.1/README.md
--rw-r--r--   0        0        0       61 2021-07-14 18:38:05.938297 pancakeswap-lottery-2.0.1/pancakeswap_lottery/__init__.py
--rw-r--r--   0        0        0    10696 2021-07-14 18:38:05.946298 pancakeswap-lottery-2.0.1/pancakeswap_lottery/assets/CakeToken.abi
--rw-r--r--   0        0        0    11600 2021-07-14 18:38:05.946298 pancakeswap-lottery-2.0.1/pancakeswap_lottery/assets/LotteryNFT.abi
--rw-r--r--   0        0        0    14380 2021-07-14 18:38:05.954297 pancakeswap-lottery-2.0.1/pancakeswap_lottery/assets/LotteryUpgradeProxy.abi
--rw-r--r--   0        0        0    17256 2021-07-14 18:38:05.958297 pancakeswap-lottery-2.0.1/pancakeswap_lottery/assets/PancakeSwapLottery.abi
--rw-r--r--   0        0        0     7956 2021-07-14 18:38:05.962298 pancakeswap-lottery-2.0.1/pancakeswap_lottery/lottery.py
--rw-r--r--   0        0        0    11447 2021-07-14 19:11:23.360381 pancakeswap-lottery-2.0.1/pancakeswap_lottery/lotteryv2.py
--rw-r--r--   0        0        0     1298 2021-07-14 18:38:05.966297 pancakeswap-lottery-2.0.1/pancakeswap_lottery/utils.py
--rw-r--r--   0        0        0     1077 2021-07-14 19:11:02.512218 pancakeswap-lottery-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     7928 2021-07-14 19:13:30.893236 pancakeswap-lottery-2.0.1/setup.py
--rw-r--r--   0        0        0     7770 2021-07-14 19:13:30.893700 pancakeswap-lottery-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-13 18:53:56.072886 pancakeswap_lottery-2.1.0/LICENSE
+-rw-r--r--   0        0        0     6814 2024-05-13 18:53:56.073116 pancakeswap_lottery-2.1.0/README.md
+-rw-r--r--   0        0        0       61 2024-05-13 18:53:56.077678 pancakeswap_lottery-2.1.0/pancakeswap_lottery/__init__.py
+-rw-r--r--   0        0        0    10696 2024-05-13 18:53:56.078013 pancakeswap_lottery-2.1.0/pancakeswap_lottery/assets/CakeToken.abi
+-rw-r--r--   0        0        0    11600 2024-05-13 18:53:56.078238 pancakeswap_lottery-2.1.0/pancakeswap_lottery/assets/LotteryNFT.abi
+-rw-r--r--   0        0        0    14380 2024-05-13 18:53:56.078443 pancakeswap_lottery-2.1.0/pancakeswap_lottery/assets/LotteryUpgradeProxy.abi
+-rw-r--r--   0        0        0    17256 2024-05-13 18:53:56.078614 pancakeswap_lottery-2.1.0/pancakeswap_lottery/assets/PancakeSwapLottery.abi
+-rw-r--r--   0        0        0     7958 2024-05-13 21:38:46.128086 pancakeswap_lottery-2.1.0/pancakeswap_lottery/lottery.py
+-rw-r--r--   0        0        0    11445 2024-05-13 21:38:46.128779 pancakeswap_lottery-2.1.0/pancakeswap_lottery/lotteryv2.py
+-rw-r--r--   0        0        0     1298 2024-05-13 21:38:46.129394 pancakeswap_lottery-2.1.0/pancakeswap_lottery/utils.py
+-rw-r--r--   0        0        0     1486 2024-05-13 21:38:51.968550 pancakeswap_lottery-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7916 1970-01-01 00:00:00.000000 pancakeswap_lottery-2.1.0/PKG-INFO
```

### Comparing `pancakeswap-lottery-2.0.1/LICENSE` & `pancakeswap_lottery-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pancakeswap-lottery-2.0.1/README.md` & `pancakeswap_lottery-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pancakeswap-lottery-2.0.1/pancakeswap_lottery/assets/CakeToken.abi` & `pancakeswap_lottery-2.1.0/pancakeswap_lottery/assets/CakeToken.abi`

 * *Files identical despite different names*

### Comparing `pancakeswap-lottery-2.0.1/pancakeswap_lottery/assets/LotteryNFT.abi` & `pancakeswap_lottery-2.1.0/pancakeswap_lottery/assets/LotteryNFT.abi`

 * *Files identical despite different names*

### Comparing `pancakeswap-lottery-2.0.1/pancakeswap_lottery/assets/LotteryUpgradeProxy.abi` & `pancakeswap_lottery-2.1.0/pancakeswap_lottery/assets/LotteryUpgradeProxy.abi`

 * *Files identical despite different names*

### Comparing `pancakeswap-lottery-2.0.1/pancakeswap_lottery/assets/PancakeSwapLottery.abi` & `pancakeswap_lottery-2.1.0/pancakeswap_lottery/assets/PancakeSwapLottery.abi`

 * *Files identical despite different names*

### Comparing `pancakeswap-lottery-2.0.1/pancakeswap_lottery/lottery.py` & `pancakeswap_lottery-2.1.0/pancakeswap_lottery/lottery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from datetime import datetime
+
 from web3 import Web3
+
 from .utils import generate_lottery_date, load_abi
 
 
 class Lottery:
     """Class for accessing PancakeSwap Lottery smart-contract information."""
 
     def __init__(self, provider="https://bsc-dataseed.binance.org:443"):
```

### Comparing `pancakeswap-lottery-2.0.1/pancakeswap_lottery/lotteryv2.py` & `pancakeswap_lottery-2.1.0/pancakeswap_lottery/lotteryv2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from datetime import datetime
+
 from web3 import Web3
+
 from .utils import load_abi
 
 
 class LotteryV2:
     """Class for accessing PancakeSwap Lottery V2 smart-contract information."""
 
     def __init__(self, provider="https://bsc-dataseed.binance.org"):
@@ -29,15 +31,15 @@
             address=contract_addresses["PancakeSwapLottery"],
         )
 
         self.token_contract = self._load_contract(
             abi_name="CakeToken", address=contract_addresses["CakeToken"]
         )
 
-        self.decimals = 10 ** 18
+        self.decimals = 10**18
 
     def _load_contract(self, abi_name, address):
         return self.w3.eth.contract(address=address, abi=load_abi(abi_name))
 
     def _status(self, statusid):
         status = {
             1: "Open",
@@ -288,21 +290,21 @@
         matchballs = [1, 2, 3, 4, 5, 6]
         probability_pct = {}
 
         if numbers_matched:
             if numbers_matched not in range(1, 7):
                 return "Pick a number between 1 and 6"
 
-            e = possible_numbers ** numbers_matched
+            e = possible_numbers**numbers_matched
             odds = 1 / e * 100
 
             return float(f"{odds:.4f}")
 
         for matchball in matchballs:
-            e = possible_numbers ** matchball
+            e = possible_numbers**matchball
             odds = 1 / e * 100
             probability_pct.update({f"match_{matchball}": float(f"{odds:.4f}")})
 
         return probability_pct
 
     def winning_numbers(self, lotteryround):
         """Get winning numbers for lottery round
@@ -344,23 +346,23 @@
 
         return winnings
 
     def address_winnings(self, address, lotteryround):
         """Get lottery winnings (CAKE) for a given address and round
 
         Args:
-            address (int): BSC address
+            address (str): BSC address
             lotteryround (int): Lottery round
 
         Examples:
             >>> lottery.address_winnings("0x621D6ee5FA9634d86396C13fAaD6A7827606A6d7", lotteryround=16)
             {'tickets': 8, 'ticketids': [634970, 634971, 634972, 634973, 634974, 634975, 634976, 634977], 'winning_tickets': [634970, 634971]}
         """
         userinfo = self.lottery_contract.functions.viewUserInfoForLotteryId(
-            self.w3.toChecksumAddress(address),
+            self.w3.to_checksum_address(address),
             lotteryround,
             0,
             100,
         ).call()
 
         count = 0
         winning_tickets = []
```

### Comparing `pancakeswap-lottery-2.0.1/pancakeswap_lottery/utils.py` & `pancakeswap_lottery-2.1.0/pancakeswap_lottery/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import os
 import json
+import os
 from datetime import datetime, timedelta, timezone
 
 
 def load_abi(abi_name):
     path = f"{os.path.dirname(os.path.abspath(__file__))}/assets/"
     with open(os.path.abspath(path + f"{abi_name}.abi")) as f:
         abi: str = json.load(f)
```

### Comparing `pancakeswap-lottery-2.0.1/setup.py` & `pancakeswap_lottery-2.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,292 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pancakeswap-lottery
+Version: 2.1.0
+Summary: A Python client for accessing PancakeSwap Lottery smart contract information through Web3.py
+Home-page: https://github.com/frefrik/pancakeswap-lottery
+License: MIT
+Keywords: pancakeswap,cake,lottery,bsc,web3
+Author: Fredrik Haarstad
+Author-email: codemonkey@zomg.no
+Requires-Python: >=3.9,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: web3 (>=6.18.0,<7.0.0)
+Project-URL: Repository, https://github.com/frefrik/pancakeswap-lottery
+Description-Content-Type: text/markdown
 
-packages = \
-['pancakeswap_lottery']
+# PancakeSwap Lottery 🥞 - Web3 client
 
-package_data = \
-{'': ['*'], 'pancakeswap_lottery': ['assets/*']}
+![PyPI version](https://img.shields.io/pypi/v/pancakeswap-lottery)
+![PyPI downloads](https://img.shields.io/pypi/dm/pancakeswap-lottery)
+![Licence](https://img.shields.io/github/license/frefrik/pancakeswap-lottery)
+![Python version](https://img.shields.io/pypi/pyversions/pancakeswap-lottery)
 
-install_requires = \
-['web3>=5.18.0,<6.0.0']
-
-setup_kwargs = {
-    'name': 'pancakeswap-lottery',
-    'version': '2.0.1',
-    'description': 'A Python client for accessing PancakeSwap Lottery smart contract information through Web3.py',
-    'long_description': '# PancakeSwap Lottery 🥞 - Web3 client\n\n![PyPI version](https://img.shields.io/pypi/v/pancakeswap-lottery)\n![PyPI downloads](https://img.shields.io/pypi/dm/pancakeswap-lottery)\n![Licence](https://img.shields.io/github/license/frefrik/pancakeswap-lottery)\n![Python version](https://img.shields.io/pypi/pyversions/pancakeswap-lottery)\n\nA Python client for accessing [PancakeSwap Lottery](https://pancakeswap.finance/lottery) smart contract information through [Web3.py](https://github.com/ethereum/web3.py).\n\n---\n\n**Documentation**: https://frefrik.github.io/pancakeswap-lottery\n\n**Examples**: https://frefrik.github.io/pancakeswap-lottery/guide/examples\n\n**Source Code**: https://github.com/frefrik/pancakeswap-lottery\n\n**PyPI**: https://pypi.org/project/pancakeswap-lottery\n\n---\n\n## Installation\nInstall from [PyPI](https://pypi.org/project/pancakeswap-lottery/):\n```\npip install pancakeswap-lottery\n```\n\n## Usage\n```python\nfrom pancakeswap_lottery import LotteryV2\n\nlottery = LotteryV2()\n\n# Current lottery round number\ncurrent_round = lottery.current_round()\n\n# Current ticket id\nticketid = lottery.current_ticket()\n\n# Status of lottery round\nstatus = lottery.status()\n\n# Lottery draw date and time of lottery round\ndraw_date = lottery.draw_date()\n\n# Ticket price in CAKE\nticket_price = lottery.ticket_price()\n\n# Total prize pool of lottery round in CAKE\nprize_pool = lottery.prize_pool()\n\n# Prize pool allocation in CAKE\nallocation = lottery.prize_pool_allocation()\n\n# Total number of tickets in lottery round\ntotal_tickets = lottery.total_tickets(lotteryround=23)\n\n# Winning numbers for lottery round\nwinning_numbers = lottery.winning_numbers(lotteryround=16)\n\n# Get lottery winnings (CAKE) for a given address and round\naddress_winnings = lottery.address_winnings(address="0x621D6ee5FA9634d86396C13fAaD6A7827606A6d7", lotteryround=16)\n\n# Get lottery winnings (CAKE) for a given ticket and round\nticket_winnings = lottery.ticket_winnings(lotteryround=10, ticketid=158408)\n\n# Number of winners per prize bracket\nwinners = lottery.winners_per_bracket(lotteryround=16)\n\n# Amount of CAKE won per ticket in each prize bracket\ncake_per_bracket = lottery.cake_per_bracket(lotteryround=16)\n\n# Percentage probability of winning the lottery\nwinning_probability = lottery.winning_probability()\n\n# Data from historic lottery rounds can also be pulled\nstatus = lottery.status(lotteryround=10)\ndraw_date = lottery.draw_date(lotteryround=10)\nticket_price = lottery.ticket_price(lotteryround=10)\nprize_pool = lottery.prize_pool(lotteryround=10)\nallocation = lottery.prize_pool_allocation(lotteryround=10)\n```\n\n### Response previews\n```python\n>>> lottery.current_round()\n20\n\n>>> lottery.current_ticket()\n1124981\n\n>>> lottery.status()\nOpen\n\n>>> lottery.draw_date()\n2021-07-12 20:00:00\n\n>>> lottery.ticket_price()\n0.32\n\n>>> lottery.prize_pool()\n63024\n\n>>> lottery.prize_pool_allocation()\n{\'match_1\': 630, \'match_2\': 1891, \'match_3\': 3781, \'match_4\': 6302, \'match_5\': 12605, \'match_6\': 25210, \'burn\': 12605}\n\n>>> lottery.total_tickets(lotteryround=23)\n14253\n\n>>> lottery.ticket_winnings(lotteryround=15, ticketid=567093)\n865.536634168\n\n>>> lottery.address_winnings("0x621D6ee5FA9634d86396C13fAaD6A7827606A6d7", lotteryround=16)\n{\'tickets\': 8, \'ticketids\': [634970, 634971, 634972, 634973, 634974, 634975, 634976, 634977], \'winning_tickets\': [634970, 634971]}\n\n >>> lottery.winning_numbers(lotteryround=16)\n743350\n\n>>> lottery.winners_per_bracket(lotteryround=16)\n{\'match_1\': 19133, \'match_2\': 1921, \'match_3\': 188, \'match_4\': 21, \'match_5\': 1, \'match_6\': 1}\n\n>>> lottery.cake_per_bracket(lotteryround=16)\n{\'match_1\': 0, \'match_2\': 3, \'match_3\': 62, \'match_4\': 925, \'match_5\': 38843, \'match_6\': 77687}\n\n>>> lottery.winning_probability()\n{\'match_1\': 10.0, \'match_2\': 1.0, \'match_3\': 0.1, \'match_4\': 0.01, \'match_5\': 0.001, \'match_6\': 0.0001}\n```\n\n<details>\n<summary>Lottery V1</summary>\n\n## Usage (Lottery V1)\n```python\nfrom pancakeswap_lottery import Lottery\n\nlottery = Lottery()\n\n# Current lottery round\nissue_index = lottery.get_issue_index()\n\n# Total pot (CAKE) of current lottery round\ntotal_amount = lottery.get_total_amount()\n\n# Prize pool allocation (percent)\nallocation = lottery.get_allocation()\n\n# Total addresses\ntotal_addresses = lottery.get_total_addresses()\n\n# Drawed \ndrawed = lottery.get_drawed()\n\n# Drawing phase\ndrawing_phase = lottery.get_drawing_phase()\n\n# Last timestamp\ntimestamp = lottery.get_last_timestamp(epoch=False)\n\n# Date and time of lottery round\nlottery_date = lottery.get_lottery_date(432)\n\n# Total rewards of lottery round\ntotal_rewards = lottery.get_total_rewards(432)\n\n# Winning numbers of lottery round\nhistory_numbers = lottery.get_history_numbers(432)\n\n# Numbers of tickets matched\nhistory_amount = lottery.get_history_amount(432)\n\n# Numers of tickets matched a specified number\nmatching_reward_amount = lottery.get_matching_reward_amount(432, 3)\n\n# Lottery numbers for a given ticket\nlottery_numbers = lottery.get_lottery_numbers(1328060)\n\n# Rewards for a given ticket\nreward_view = lottery.get_reward_view(1328060)\n\n# Max number\nmax_number = lottery.get_max_number()\n\n# CAKE contract address\ncake_contract = lottery.get_cake()\n\n# PLT-token contract address\nlottery_contract = lottery.get_lotteryNFT()\n\n# Total number of tickets bought by a given address\nbalance = lottery.get_balance_of("0xc13456A34305e9265E907F70f76B1BA6E2055c8B")\n```\n\n### Response previews (Lottery V1)\n```python\n>>> lottery.get_issue_index()\n435\n\n>>> lottery.get_total_amount()\n34977.25\n\n>>> lottery.get_allocation()\n{\'1\': 50, \'2\': 20, \'3\': 10}\n\n>>> lottery.get_total_addresses()\n200\n\n>>> lottery.get_drawed()\nFalse\n\n>>> lottery.get_drawing_phase()\nFalse\n\n>>> lottery.get_last_timestamp(epoch=False)\n2021-03-27 11:38:49\n\n>>> lottery.get_lottery_date(432)\n2021-03-26 02:00:00+00:00\n\n>>> lottery.get_total_rewards(432)\n51384.125\n\n>>> lottery.get_history_numbers(432)\n[2, 13, 7, 3]\n\n>>> lottery.get_history_amount(432)\n{\'4\': 1, \'3\': 34, \'2\': 718}\n\n>>> lottery.get_matching_reward_amount(432, 3)\n34\n\n>>> lottery.get_lottery_numbers(1328060)\n[11, 5, 14, 6]\n\n>>> lottery.get_reward_view(1328060)\n0\n\n>>> lottery.get_max_number()\n14\n\n>>> lottery.get_min_price()\n1\n\n>>> lottery.get_cake()\n0x0E09FaBB73Bd3Ade0a17ECC321fD13a19e81cE82\n\n>>> lottery.get_lotteryNFT()\n0x5e74094Cd416f55179DBd0E45b1a8ED030e396A1\n\n>>> lottery.get_balance_of("0xc13456A34305e9265E907F70f76B1BA6E2055c8B")\n2673\n```\n</details>\n\n## Donate\nIf you found this library useful and want to support my work feel free to donate a small amount 🙏🏻\n\n- 🥞 CAKE: 0xCFad66049e2C9Bc28647B2e2e3449B6B7C602d42\n- Ξ ETH: 0x7E916c46157f012Fb8dece4A042Dc603e8d627Df\n- ₿ BTC: bc1qgn2mdf5wsxft33s3ea8sh060y85mzntzs8cuu7\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n\n## Disclaimer\n\nThis project is not affiliated with the PancakeSwap team.',
-    'author': 'Fredrik Haarstad',
-    'author_email': 'codemonkey@zomg.no',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/frefrik/pancakeswap-lottery',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+A Python client for accessing [PancakeSwap Lottery](https://pancakeswap.finance/lottery) smart contract information through [Web3.py](https://github.com/ethereum/web3.py).
 
+---
 
-setup(**setup_kwargs)
+**Documentation**: https://frefrik.github.io/pancakeswap-lottery
+
+**Examples**: https://frefrik.github.io/pancakeswap-lottery/guide/examples
+
+**Source Code**: https://github.com/frefrik/pancakeswap-lottery
+
+**PyPI**: https://pypi.org/project/pancakeswap-lottery
+
+---
+
+## Installation
+Install from [PyPI](https://pypi.org/project/pancakeswap-lottery/):
+```
+pip install pancakeswap-lottery
+```
+
+## Usage
+```python
+from pancakeswap_lottery import LotteryV2
+
+lottery = LotteryV2()
+
+# Current lottery round number
+current_round = lottery.current_round()
+
+# Current ticket id
+ticketid = lottery.current_ticket()
+
+# Status of lottery round
+status = lottery.status()
+
+# Lottery draw date and time of lottery round
+draw_date = lottery.draw_date()
+
+# Ticket price in CAKE
+ticket_price = lottery.ticket_price()
+
+# Total prize pool of lottery round in CAKE
+prize_pool = lottery.prize_pool()
+
+# Prize pool allocation in CAKE
+allocation = lottery.prize_pool_allocation()
+
+# Total number of tickets in lottery round
+total_tickets = lottery.total_tickets(lotteryround=23)
+
+# Winning numbers for lottery round
+winning_numbers = lottery.winning_numbers(lotteryround=16)
+
+# Get lottery winnings (CAKE) for a given address and round
+address_winnings = lottery.address_winnings(address="0x621D6ee5FA9634d86396C13fAaD6A7827606A6d7", lotteryround=16)
+
+# Get lottery winnings (CAKE) for a given ticket and round
+ticket_winnings = lottery.ticket_winnings(lotteryround=10, ticketid=158408)
+
+# Number of winners per prize bracket
+winners = lottery.winners_per_bracket(lotteryround=16)
+
+# Amount of CAKE won per ticket in each prize bracket
+cake_per_bracket = lottery.cake_per_bracket(lotteryround=16)
+
+# Percentage probability of winning the lottery
+winning_probability = lottery.winning_probability()
+
+# Data from historic lottery rounds can also be pulled
+status = lottery.status(lotteryround=10)
+draw_date = lottery.draw_date(lotteryround=10)
+ticket_price = lottery.ticket_price(lotteryround=10)
+prize_pool = lottery.prize_pool(lotteryround=10)
+allocation = lottery.prize_pool_allocation(lotteryround=10)
+```
+
+### Response previews
+```python
+>>> lottery.current_round()
+20
+
+>>> lottery.current_ticket()
+1124981
+
+>>> lottery.status()
+Open
+
+>>> lottery.draw_date()
+2021-07-12 20:00:00
+
+>>> lottery.ticket_price()
+0.32
+
+>>> lottery.prize_pool()
+63024
+
+>>> lottery.prize_pool_allocation()
+{'match_1': 630, 'match_2': 1891, 'match_3': 3781, 'match_4': 6302, 'match_5': 12605, 'match_6': 25210, 'burn': 12605}
+
+>>> lottery.total_tickets(lotteryround=23)
+14253
+
+>>> lottery.ticket_winnings(lotteryround=15, ticketid=567093)
+865.536634168
+
+>>> lottery.address_winnings("0x621D6ee5FA9634d86396C13fAaD6A7827606A6d7", lotteryround=16)
+{'tickets': 8, 'ticketids': [634970, 634971, 634972, 634973, 634974, 634975, 634976, 634977], 'winning_tickets': [634970, 634971]}
+
+ >>> lottery.winning_numbers(lotteryround=16)
+743350
+
+>>> lottery.winners_per_bracket(lotteryround=16)
+{'match_1': 19133, 'match_2': 1921, 'match_3': 188, 'match_4': 21, 'match_5': 1, 'match_6': 1}
+
+>>> lottery.cake_per_bracket(lotteryround=16)
+{'match_1': 0, 'match_2': 3, 'match_3': 62, 'match_4': 925, 'match_5': 38843, 'match_6': 77687}
+
+>>> lottery.winning_probability()
+{'match_1': 10.0, 'match_2': 1.0, 'match_3': 0.1, 'match_4': 0.01, 'match_5': 0.001, 'match_6': 0.0001}
+```
+
+<details>
+<summary>Lottery V1</summary>
+
+## Usage (Lottery V1)
+```python
+from pancakeswap_lottery import Lottery
+
+lottery = Lottery()
+
+# Current lottery round
+issue_index = lottery.get_issue_index()
+
+# Total pot (CAKE) of current lottery round
+total_amount = lottery.get_total_amount()
+
+# Prize pool allocation (percent)
+allocation = lottery.get_allocation()
+
+# Total addresses
+total_addresses = lottery.get_total_addresses()
+
+# Drawed 
+drawed = lottery.get_drawed()
+
+# Drawing phase
+drawing_phase = lottery.get_drawing_phase()
+
+# Last timestamp
+timestamp = lottery.get_last_timestamp(epoch=False)
+
+# Date and time of lottery round
+lottery_date = lottery.get_lottery_date(432)
+
+# Total rewards of lottery round
+total_rewards = lottery.get_total_rewards(432)
+
+# Winning numbers of lottery round
+history_numbers = lottery.get_history_numbers(432)
+
+# Numbers of tickets matched
+history_amount = lottery.get_history_amount(432)
+
+# Numers of tickets matched a specified number
+matching_reward_amount = lottery.get_matching_reward_amount(432, 3)
+
+# Lottery numbers for a given ticket
+lottery_numbers = lottery.get_lottery_numbers(1328060)
+
+# Rewards for a given ticket
+reward_view = lottery.get_reward_view(1328060)
+
+# Max number
+max_number = lottery.get_max_number()
+
+# CAKE contract address
+cake_contract = lottery.get_cake()
+
+# PLT-token contract address
+lottery_contract = lottery.get_lotteryNFT()
+
+# Total number of tickets bought by a given address
+balance = lottery.get_balance_of("0xc13456A34305e9265E907F70f76B1BA6E2055c8B")
+```
+
+### Response previews (Lottery V1)
+```python
+>>> lottery.get_issue_index()
+435
+
+>>> lottery.get_total_amount()
+34977.25
+
+>>> lottery.get_allocation()
+{'1': 50, '2': 20, '3': 10}
+
+>>> lottery.get_total_addresses()
+200
+
+>>> lottery.get_drawed()
+False
+
+>>> lottery.get_drawing_phase()
+False
+
+>>> lottery.get_last_timestamp(epoch=False)
+2021-03-27 11:38:49
+
+>>> lottery.get_lottery_date(432)
+2021-03-26 02:00:00+00:00
+
+>>> lottery.get_total_rewards(432)
+51384.125
+
+>>> lottery.get_history_numbers(432)
+[2, 13, 7, 3]
+
+>>> lottery.get_history_amount(432)
+{'4': 1, '3': 34, '2': 718}
+
+>>> lottery.get_matching_reward_amount(432, 3)
+34
+
+>>> lottery.get_lottery_numbers(1328060)
+[11, 5, 14, 6]
+
+>>> lottery.get_reward_view(1328060)
+0
+
+>>> lottery.get_max_number()
+14
+
+>>> lottery.get_min_price()
+1
+
+>>> lottery.get_cake()
+0x0E09FaBB73Bd3Ade0a17ECC321fD13a19e81cE82
+
+>>> lottery.get_lotteryNFT()
+0x5e74094Cd416f55179DBd0E45b1a8ED030e396A1
+
+>>> lottery.get_balance_of("0xc13456A34305e9265E907F70f76B1BA6E2055c8B")
+2673
+```
+</details>
+
+## Donate
+If you found this library useful and want to support my work feel free to donate a small amount 🙏🏻
+
+- 🥞 CAKE: 0xCFad66049e2C9Bc28647B2e2e3449B6B7C602d42
+- Ξ ETH: 0x7E916c46157f012Fb8dece4A042Dc603e8d627Df
+- ₿ BTC: bc1qgn2mdf5wsxft33s3ea8sh060y85mzntzs8cuu7
+
+## License
+
+This project is licensed under the terms of the MIT license.
+
+## Disclaimer
+
+This project is not affiliated with the PancakeSwap team.
```

