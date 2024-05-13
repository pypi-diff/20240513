# Comparing `tmp/sonatoki-0.1.5.tar.gz` & `tmp/sonatoki-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonatoki-0.1.5.tar", last modified: Sat May 11 17:49:31 2024, max compression
+gzip compressed data, was "sonatoki-0.2.0.tar", last modified: Mon May 13 20:21:36 2024, max compression
```

## Comparing `sonatoki-0.1.5.tar` & `sonatoki-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0    34523 2024-05-11 17:49:19.493311 sonatoki-0.1.5/LICENSE
--rw-r--r--   0        0        0     4765 2024-05-11 17:49:19.493311 sonatoki-0.1.5/README.md
--rw-r--r--   0        0        0     2013 2024-05-11 17:49:31.721320 sonatoki-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1160 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/Cleaners.py
--rw-r--r--   0        0        0     1935 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/Configs.py
--rw-r--r--   0        0        0     4470 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/Filters.py
--rw-r--r--   0        0        0     4441 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/Preprocessors.py
--rw-r--r--   0        0        0     3658 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/Scorers.py
--rw-r--r--   0        0        0     2310 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/Tokenizers.py
--rw-r--r--   0        0        0        0 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/__init__.py
--rw-r--r--   0        0        0       82 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/__main__.py
--rw-r--r--   0        0        0     4883 2024-05-11 17:49:19.493311 sonatoki-0.1.5/src/sonatoki/constants.py
--rw-r--r--   0        0        0     3849 2024-05-11 17:49:19.497311 sonatoki-0.1.5/src/sonatoki/ilo.py
--rw-r--r--   0        0        0   271013 2024-05-11 17:49:19.497311 sonatoki-0.1.5/src/sonatoki/linku.json
--rw-r--r--   0        0        0    77650 2024-05-11 17:49:19.497311 sonatoki-0.1.5/src/sonatoki/sandbox.json
--rw-r--r--   0        0        0        0 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      680 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/test_cleaners.py
--rw-r--r--   0        0        0     2315 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/test_filters.py
--rw-r--r--   0        0        0     4029 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/test_ilo.py
--rw-r--r--   0        0        0     4145 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/test_preprocessors.py
--rw-r--r--   0        0        0     1062 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/test_scorers.py
--rw-r--r--   0        0        0     3039 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/test_tokenize.py
--rw-r--r--   0        0        0      821 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/test_utils.py
--rw-r--r--   0        0        0      151 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/tokenize_cases/tokenize_sentences.yml
--rw-r--r--   0        0        0     1112 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/tokenize_cases/tokenize_sentences_tok.yml
--rw-r--r--   0        0        0      440 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/tokenize_cases/tokenize_words.yml
--rw-r--r--   0        0        0     1522 2024-05-11 17:49:19.497311 sonatoki-0.1.5/tests/tokenize_cases/tokenize_words_tok.yml
--rw-r--r--   0        0        0     5225 1970-01-01 00:00:00.000000 sonatoki-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-13 20:21:23.730103 sonatoki-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4765 2024-05-13 20:21:23.730103 sonatoki-0.2.0/README.md
+-rw-r--r--   0        0        0     1983 2024-05-13 20:21:36.578233 sonatoki-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1744 2024-05-13 20:21:23.730103 sonatoki-0.2.0/src/sonatoki/Cleaners.py
+-rw-r--r--   0        0        0     1929 2024-05-13 20:21:23.730103 sonatoki-0.2.0/src/sonatoki/Configs.py
+-rw-r--r--   0        0        0     5276 2024-05-13 20:21:23.730103 sonatoki-0.2.0/src/sonatoki/Filters.py
+-rw-r--r--   0        0        0     4441 2024-05-13 20:21:23.730103 sonatoki-0.2.0/src/sonatoki/Preprocessors.py
+-rw-r--r--   0        0        0     3643 2024-05-13 20:21:23.734104 sonatoki-0.2.0/src/sonatoki/Scorers.py
+-rw-r--r--   0        0        0     3326 2024-05-13 20:21:23.734104 sonatoki-0.2.0/src/sonatoki/Tokenizers.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:21:23.734104 sonatoki-0.2.0/src/sonatoki/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-13 20:21:23.734104 sonatoki-0.2.0/src/sonatoki/__main__.py
+-rw-r--r--   0        0        0    30942 2024-05-13 20:21:23.734104 sonatoki-0.2.0/src/sonatoki/constants.py
+-rw-r--r--   0        0        0     3849 2024-05-13 20:21:23.734104 sonatoki-0.2.0/src/sonatoki/ilo.py
+-rw-r--r--   0        0        0   271013 2024-05-13 20:21:23.734104 sonatoki-0.2.0/src/sonatoki/linku.json
+-rw-r--r--   0        0        0    77650 2024-05-13 20:21:23.734104 sonatoki-0.2.0/src/sonatoki/sandbox.json
+-rw-r--r--   0        0        0     2660 2024-05-13 20:21:23.734104 sonatoki-0.2.0/src/sonatoki/utils.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:21:23.734104 sonatoki-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      983 2024-05-13 20:21:23.734104 sonatoki-0.2.0/tests/test_cleaners.py
+-rw-r--r--   0        0        0     2982 2024-05-13 20:21:23.734104 sonatoki-0.2.0/tests/test_filters.py
+-rw-r--r--   0        0        0     4029 2024-05-13 20:21:23.734104 sonatoki-0.2.0/tests/test_ilo.py
+-rw-r--r--   0        0        0     4145 2024-05-13 20:21:23.734104 sonatoki-0.2.0/tests/test_preprocessors.py
+-rw-r--r--   0        0        0     1066 2024-05-13 20:21:23.734104 sonatoki-0.2.0/tests/test_scorers.py
+-rw-r--r--   0        0        0     3434 2024-05-13 20:21:23.734104 sonatoki-0.2.0/tests/test_tokenize.py
+-rw-r--r--   0        0        0      821 2024-05-13 20:21:23.734104 sonatoki-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1327 2024-05-13 20:21:23.734104 sonatoki-0.2.0/tests/tokenize_cases/tokenize_sentences_tok.yml
+-rw-r--r--   0        0        0     2784 2024-05-13 20:21:23.734104 sonatoki-0.2.0/tests/tokenize_cases/tokenize_words_tok.yml
+-rw-r--r--   0        0        0     5160 1970-01-01 00:00:00.000000 sonatoki-0.2.0/PKG-INFO
```

### Comparing `sonatoki-0.1.5/LICENSE` & `sonatoki-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.5/README.md` & `sonatoki-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.5/pyproject.toml` & `sonatoki-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sonatoki"
-version = "0.1.5"
+version = "0.2.0"
 description = "ilo li moku e toki li pana e sona ni: ni li toki ala toki pona?"
 authors = [
     { name = "jan Kekan San (@gregdan3)", email = "gregory.danielson3@gmail.com" },
 ]
 dependencies = [
     "unidecode>=1.3.6",
     "regex>=2023.12.25",
@@ -13,17 +13,14 @@
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "AGPL-3.0-or-later"
 
 [project.optional-dependencies]
-nltk = [
-    "nltk>=3.8.1",
-]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `sonatoki-0.1.5/src/sonatoki/Cleaners.py` & `sonatoki-0.2.0/src/sonatoki/Cleaners.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,24 +19,47 @@
 
     @classmethod
     @override
     def clean(cls, token: str) -> str:
         return re.sub(cls.pattern, cls.replace, token)
 
 
-class ConsecutiveDuplicates(RegexCleaner):
+class ConsecutiveDuplicates(Cleaner):
     """Remove consecutive duplicates from an input string, ignoring case.
 
     The first match of any 2+ will become `\\1`, preserving initial case.
     For example, `FfFoo` will reduce to `Foo`, and `bBAR` will reduce to `bAR`.
 
     This is desirable for Toki Pona written with the Latin alphabet because strings
     may be altered for emphasis or effect, such as in "sonaaaa" or "AAAAAA".
 
     This may be undesirable for moraic scripts like Hiragana, where `わわ` would be
     incorrectly reduced to `わ`. This does preserve phonotactic validity, though."""
 
+    @classmethod
+    @override
+    def clean(cls, token: str) -> str:
+        if not token:
+            return token
+
+        output = token[0]
+
+        last_output = output.lower()  # ignore case in comparison
+        for i in range(1, len(token)):
+            cur_char = token[i].lower()
+            if cur_char == last_output:
+                continue
+            output += token[i]  # preserve case of string
+            last_output = cur_char
+        return output
+
+
+class ConsecutiveDuplicatesRe(RegexCleaner):
+    """Reference implementation for `ConsecutiveDuplicates`."""
+
     pattern = re.compile(r"(.)\1+", flags=re.IGNORECASE)
     replace = r"\1"
 
 
-__all__ = ["ConsecutiveDuplicates"]
+__all__ = [
+    "ConsecutiveDuplicates",
+]
```

### Comparing `sonatoki-0.1.5/src/sonatoki/Configs.py` & `sonatoki-0.2.0/src/sonatoki/Configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ProperName,
     Phonotactic,
     Punctuation,
     NimiLinkuAle,
 )
 from sonatoki.Scorers import Number, Scorer, PassFail, SoftScaling, SoftPassFail
 from sonatoki.Cleaners import Cleaner, ConsecutiveDuplicates
-from sonatoki.Tokenizers import Tokenizer, WordTokenizerTok
+from sonatoki.Tokenizers import Tokenizer, WordTokenizer
 from sonatoki.Preprocessors import (
     URLs,
     Preprocessor,
     DiscordEmotes,
     DiscordSpecial,
     DiscordChannels,
     DiscordMentions,
@@ -45,15 +45,15 @@
 BaseConfig: IloConfig = {
     "preprocessors": [URLs],
     "cleaners": [ConsecutiveDuplicates],
     "ignoring_filters": [Numeric, Punctuation],
     "scoring_filters": [],
     "scorer": PassFail,
     "passing_score": 0.8,
-    "word_tokenizer": WordTokenizerTok,
+    "word_tokenizer": WordTokenizer,
 }
 
 
 PrefConfig: IloConfig = deepcopy(BaseConfig)
 PrefConfig["scoring_filters"].extend([NimiLinku, Syllabic, ProperName, Alphabetic])
 PrefConfig["scorer"] = SoftScaling
 
@@ -66,15 +66,15 @@
 DiscordConfig["preprocessors"].extend(
     [DiscordEmotes, DiscordMentions, DiscordChannels, DiscordSpecial]
 )
 TelegramConfig: IloConfig = deepcopy(PrefConfig)
 ForumConfig: IloConfig = deepcopy(PrefConfig)
 
 __all__ = [
-    "IloConfig",
     "BaseConfig",
-    "PrefConfig",
-    "LazyConfig",
     "DiscordConfig",
-    "TelegramConfig",
     "ForumConfig",
+    "IloConfig",
+    "LazyConfig",
+    "PrefConfig",
+    "TelegramConfig",
 ]
```

### Comparing `sonatoki-0.1.5/src/sonatoki/Filters.py` & `sonatoki-0.2.0/src/sonatoki/Filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 # PDM
 import regex
 from typing_extensions import override
 
 # LOCAL
 from sonatoki.constants import (
     VOWELS,
+    NIMI_PU,
+    ALPHABET,
+    ALLOWABLES,
     CONSONANTS,
-    NIMI_PU_SET,
-    ALPHABET_SET,
+    NIMI_LINKU,
+    NIMI_PU_ALE,
+    POSIX_PUNCT,
     UNICODE_PUNCT,
-    ALLOWABLES_SET,
-    NIMI_LINKU_SET,
-    NIMI_PU_ALE_SET,
-    NIMI_LINKU_ALE_SET,
-    PRUNED_POSIX_PUNCT,
-    NIMI_LINKU_SANDBOX_SET,
+    NIMI_LINKU_ALE,
+    ALL_PUNCT_RANGES,
+    NIMI_LINKU_SANDBOX,
 )
 
 regex.DEFAULT_VERSION = regex.VERSION1
 
 
 class Filter(ABC):
     @classmethod
@@ -50,26 +51,36 @@
     @classmethod
     @override
     @cache(maxsize=None)
     def filter(cls, token: str) -> bool:
         return not not regex.fullmatch(cls.pattern, token)
 
 
-class SetFilter(Filter):
+class MemberFilter(Filter):
     tokens: Set[str]
 
     @classmethod
     @override
     @cache(maxsize=None)
     def filter(cls, token: str) -> bool:
         return token.lower() in cls.tokens
 
 
-class Miscellaneous(SetFilter):
-    tokens = ALLOWABLES_SET
+class SubsetFilter(Filter):
+    tokens: Set[str]
+
+    @classmethod
+    @override
+    @cache(maxsize=None)
+    def filter(cls, token: str) -> bool:
+        return set(token.lower()).issubset(cls.tokens)
+
+
+class Miscellaneous(MemberFilter):
+    tokens = set(ALLOWABLES)
 
 
 class ProperName(Filter):
     """Determines if a given token is a valid name (also called a loan word).
     When Toki Pona is written with the Latin alphabet, names are generally
     capitalized at their start. This filter identifies those tokens.
 
@@ -79,34 +90,36 @@
     """
 
     @classmethod
     @override
     @cache(maxsize=None)
     def filter(cls, token: str) -> bool:
         return token == token.capitalize()
+        # TODO:  If the token is in a script which doesn't have a case distinction,
+        # this will errantly match.
 
 
-class NimiPu(SetFilter):
-    tokens = NIMI_PU_SET
+class NimiPu(MemberFilter):
+    tokens = set(NIMI_PU)
 
 
-class NimiPuAle(SetFilter):
-    tokens = NIMI_PU_ALE_SET
+class NimiPuAle(MemberFilter):
+    tokens = set(NIMI_PU_ALE)
 
 
-class NimiLinku(SetFilter):
-    tokens = NIMI_LINKU_SET
+class NimiLinku(MemberFilter):
+    tokens = set(NIMI_LINKU)
 
 
-class NimiLinkuAle(SetFilter):
-    tokens = NIMI_LINKU_ALE_SET
+class NimiLinkuAle(MemberFilter):
+    tokens = set(NIMI_LINKU_ALE)
 
 
-class NimiLinkuSandbox(SetFilter):
-    tokens = NIMI_LINKU_SANDBOX_SET
+class NimiLinkuSandbox(MemberFilter):
+    tokens = set(NIMI_LINKU_SANDBOX)
 
 
 class Phonotactic(RegexFilter):
     """Determines if a given token is phonotactically valid Toki Pona (or `n`).
     Excludes both consecutive nasals and the illegal syllables:
     - "nm", "nn"
     - "wu", "wo", "ji", "ti"
@@ -131,21 +144,20 @@
     # Alterative I was exploring takes ~15% more steps
     pattern = re.compile(
         rf"^(?:^[{VOWELS}]n?)?(?:[{CONSONANTS}][{VOWELS}]n?)*$|^n$",
         flags=re.IGNORECASE,
     )
 
 
-class Alphabetic(Filter):
-    @classmethod
-    @override
-    @cache(maxsize=None)
-    def filter(cls, token: str) -> bool:
-        # Faster than regex version
-        return set(token.lower()).issubset(ALPHABET_SET)
+class Alphabetic(SubsetFilter):
+    tokens = set(ALPHABET)
+
+
+class AlphabeticRe(RegexFilter):
+    pattern = re.compile(rf"[{ALPHABET}]+", flags=re.IGNORECASE)
 
 
 class Numeric(Filter):
     """Determine if a given token is entirely numeric.
     Covers all numeric symbols in Unicode.
 
     This will fail to find numeric tokens such as "1.111" or "-42",
@@ -156,22 +168,39 @@
     @classmethod
     @override
     @cache(maxsize=None)
     def filter(cls, msg: str) -> bool:
         return msg.isnumeric()
 
 
-class Punctuation(RegexFilter):
-    pattern = re.compile(rf"[{PRUNED_POSIX_PUNCT}{UNICODE_PUNCT}]+")
+class Punctuation(SubsetFilter):
+    """Identify whether a token is entirely punctuation. Fastest implementation."""
+
+    tokens = set(POSIX_PUNCT + UNICODE_PUNCT)
+
+
+class PunctuationRe(RegexFilter):
+    """Faster implementation of `PunctuationRe1`.
+    Goes out of date compared to the `regex` library if UNICODE_PUNCT is not updated."""
+
+    pattern = re.compile(rf"[{ALL_PUNCT_RANGES}]+")
+
+
+class PunctuationRe1(Regex1Filter):
+    """Reference implementation for identifying tokens made entirely of punctuation."""
+
+    pattern = regex.compile(r"[\p{Punctuation}\p{posix_punct}]+")
 
 
 __all__ = [
-    "NimiPu",
+    "Alphabetic",
     "NimiLinku",
     "NimiLinkuAle",
+    "NimiLinkuSandbox",
+    "NimiPu",
+    "NimiPuAle",
+    "Numeric",
     "Phonotactic",
-    "Syllabic",
-    "Alphabetic",
     "ProperName",
     "Punctuation",
-    "Numeric",
+    "Syllabic",
 ]
```

### Comparing `sonatoki-0.1.5/src/sonatoki/Preprocessors.py` & `sonatoki-0.2.0/src/sonatoki/Preprocessors.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -153,21 +153,21 @@
             ]
         ),
         flags=re.MULTILINE | re.DOTALL,
     )
 
 
 __all__ = [
+    "AllQuotes",
     "AngleBracketObject",
+    "ArrowQuote",
+    "Backticks",
     "DiscordChannels",
+    "DiscordEmotes",
     "DiscordMentions",
     "DiscordSpecial",
-    "DiscordEmotes",
-    "SingleQuotes",
     "DoubleQuotes",
-    "ArrowQuote",
-    "AllQuotes",
-    "Backticks",
     "Reference",
+    "SingleQuotes",
     "Spoilers",
     "URLs",
 ]
```

### Comparing `sonatoki-0.1.5/src/sonatoki/Scorers.py` & `sonatoki-0.2.0/src/sonatoki/Scorers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # STL
 import math
-import logging
 from abc import ABC, abstractmethod
 from typing import Dict, List, Type, Union
 
 # PDM
 from typing_extensions import override
 
 # LOCAL
```

### Comparing `sonatoki-0.1.5/src/sonatoki/Tokenizers.py` & `sonatoki-0.2.0/src/sonatoki/Tokenizers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,36 @@
 # STL
 import re
 from abc import ABC, abstractmethod
-from typing import List
+from typing import Set, List
 
 # PDM
 import regex
 from typing_extensions import override
 
 # LOCAL
-from sonatoki.constants import UNICODE_PUNCT, PRUNED_POSIX_PUNCT
-
-try:
-    # PDM
-    import nltk
-    from nltk.tokenize import sent_tokenize as __sent_tokenize_nltk
-    from nltk.tokenize import word_tokenize as __word_tokenize_nltk
-except ImportError as e:
-    nltk = e
-
+from sonatoki.utils import regex_escape
+from sonatoki.constants import (
+    POSIX_PUNCT,
+    UNICODE_PUNCT,
+    SENTENCE_PUNCT,
+    ALL_PUNCT_RANGES,
+)
 
 regex.DEFAULT_VERSION = regex.VERSION1
 
 
 class Tokenizer(ABC):
     @classmethod
     @abstractmethod
     def tokenize(cls, s: str) -> List[str]: ...
 
 
-class NoOpTokenizer(Tokenizer):
-    """This is a special case that you do not want or need."""
-
-    @classmethod
-    @override
-    def tokenize(cls, s: str) -> List[str]:
-        return [s]
+class SetTokenizer(Tokenizer):
+    delimiters: Set[str]
 
 
 class RegexTokenizer(Tokenizer):
     pattern: "re.Pattern[str]"
 
     @classmethod
     @override
@@ -53,39 +45,95 @@
     @override
     def tokenize(cls, s: str) -> List[str]:
         return [
             clean for word in regex.split(cls.pattern, s) if (clean := word.strip())
         ]
 
 
-class WordTokenizerTok(RegexTokenizer):
-    pattern = re.compile(rf"""([{PRUNED_POSIX_PUNCT}{UNICODE_PUNCT}]+|\s+)""")
+class WordTokenizer(SetTokenizer):
+    delimiters = set(POSIX_PUNCT + UNICODE_PUNCT)
 
+    @classmethod
+    @override
+    def tokenize(cls, s: str) -> List[str]:
+        if not s:
+            return []
 
-class SentTokenizerTok(RegexTokenizer):
-    pattern = re.compile(r"""(?<=[.?!:;·…“”"'()\[\]\-])|$""", flags=re.MULTILINE)
-    # TODO: are <> or {} that common as *sentence* delims? [] are already a stretch
-    # TODO: do the typography characters matter?
-    # NOTE: | / and , are *not* sentence delimiters for my purpose
+        tokens: List[str] = []
+
+        last_match = 0
+        last_membership = s[0] in cls.delimiters
+        for i, char in enumerate(s):
+            mem = char in cls.delimiters
+            if mem == last_membership:
+                continue
+
+            match = s[last_match:i].split()
+            # TODO: kinda sucks? what about unicode whitespace?
+            last_match = i
+            last_membership = mem
+            [tokens.append(t) for t in match if t]
+
+        match = s[last_match:].strip().split()
+        if match:
+            tokens.extend(match)
+
+        return tokens
 
 
 class WordTokenizerRe(RegexTokenizer):
-    pattern = re.compile(r"""(?<=[.?!;:'"-])""")
+    pattern = re.compile(rf"""([{ALL_PUNCT_RANGES}]+|\s+)""")
+
+
+class WordTokenizerRe1(Regex1Tokenizer):
+    """Reference implementation for WorkTokenizer."""
+
+    pattern = regex.compile(r"""([\p{posix_punct}\p{Punctuation}]+|\s+)""")
+
+
+class SentTokenizer(SetTokenizer):
+    delimiters = set(SENTENCE_PUNCT + "\n")  # regex does \n with a flag
+
+    @classmethod
+    @override
+    def tokenize(cls, s: str) -> List[str]:
+        if not s:
+            return []
+
+        tokens: List[str] = []
+        last_match = 0
+        for i, char in enumerate(s):
+            if char not in cls.delimiters:
+                continue
+
+            match = s[last_match : i + 1].strip()
+            last_match = i + 1  # newlines can strip but idc
+            if not match:
+                continue
+            tokens.append(match)
+
+        match = s[last_match:].strip()
+        if match:
+            tokens.append(match)
+
+        return tokens
 
 
 class SentTokenizerRe(RegexTokenizer):
-    pattern = re.compile(r"""(.*?[.?!;:])|(.+?$)""")
+    pattern = re.compile(
+        rf"""(?<=[{regex_escape(SENTENCE_PUNCT)}])|$""", flags=re.MULTILINE
+    )
+    # TODO: are <> or {} that common as *sentence* delims? [] are already a stretch
+    # TODO: do the typography characters matter?
+    # NOTE: | / and , are *not* sentence delimiters for my purpose
+
 
+class SentTokenizerRe1(Regex1Tokenizer):
+    pattern = regex.compile(
+        rf"""(?<=[{regex_escape(SENTENCE_PUNCT)}]|$)""", flags=regex.MULTILINE
+    )
 
-if not isinstance(nltk, ImportError):
 
-    class WordTokenizerNLTK(Tokenizer):
-        @classmethod
-        @override
-        def tokenize(cls, s: str) -> List[str]:
-            return __word_tokenize_nltk(text=s, language=LANGUAGE)
-
-    class SentTokenizerNLTK(Tokenizer):
-        @classmethod
-        @override
-        def tokenize(cls, s: str) -> List[str]:
-            return __sent_tokenize_nltk(text=s, language=LANGUAGE)
+__all__ = [
+    "WordTokenizer",
+    "SentTokenizer",
+]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sonatoki-0.1.5/src/sonatoki/ilo.py` & `sonatoki-0.2.0/src/sonatoki/ilo.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.5/src/sonatoki/linku.json` & `sonatoki-0.2.0/src/sonatoki/linku.json`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.5/src/sonatoki/sandbox.json` & `sonatoki-0.2.0/src/sonatoki/sandbox.json`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.5/tests/test_filters.py` & `sonatoki-0.2.0/tests/test_filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # STL
 import string
 
 # PDM
-import regex as re
 import hypothesis.strategies as st
-from hypothesis import HealthCheck, given, assume, example, settings
+from hypothesis import given, example
 
 # LOCAL
 from sonatoki.Filters import (
     NimiPu,
     Numeric,
     Syllabic,
     NimiLinku,
     Alphabetic,
     ProperName,
     Phonotactic,
     Punctuation,
+    AlphabeticRe,
+    PunctuationRe,
+    PunctuationRe1,
 )
 from sonatoki.Cleaners import ConsecutiveDuplicates
 from sonatoki.constants import NIMI_PU, NIMI_LINKU
 
 # FILESYSTEM
 from .test_utils import ALPHABETIC_RE, PROPER_NAME_RE
 
@@ -63,41 +65,62 @@
 @given(st.from_regex(Syllabic.pattern.pattern, fullmatch=True))
 @example("wuwojitiwunwonjintinmanna")
 def test_Syllabic(s: str):
     res = Syllabic.filter(s)
     assert res, repr(s)
 
 
-@given(st.from_regex(ALPHABETIC_RE, fullmatch=True))
+@given(st.from_regex(AlphabeticRe.pattern.pattern, fullmatch=True))
 @example("muems")
 @example("mpptp")
 @example("tptpt")
 def test_Alphabetic(s: str):
-    res = Alphabetic.filter(s)
-    assert res, repr(s)
+    res_fn = Alphabetic.filter(s)
+    res_re = AlphabeticRe.filter(s)
+    assert res_fn == res_re, repr(s)
+
+
+@given(st.from_regex(AlphabeticRe.pattern.pattern, fullmatch=True))
+def test_AlphabeticRe(s: str):
+    res_re = AlphabeticRe.filter(s)
+    assert res_re, repr(s)
 
 
 @given(st.from_regex(PROPER_NAME_RE, fullmatch=True))
 def test_ProperName(s: str):
     res = ProperName.filter(s)
     assert res, repr(s)
 
 
-@given(st.from_regex(Punctuation.pattern.pattern, fullmatch=True))
+@given(st.from_regex(PunctuationRe.pattern.pattern, fullmatch=True))
 @example("[]")
 @example(r"\\")
 @example(r"\"")
 @example("⟨·⟩")
 @example("…")
-@example("「」")  # `　`
+@example("「」")
 @example(string.punctuation)
-def test_Punctuation(s: str):
-    res = Punctuation.filter(s)
+def test_PunctuationRe1(s: str):
+    res = PunctuationRe1.filter(s)
     assert res, repr(s)
 
 
+@given(st.from_regex(PunctuationRe.pattern.pattern, fullmatch=True))
+def test_PunctuationRe(s: str):
+    res_re = PunctuationRe.filter(s)
+    res_re1 = PunctuationRe1.filter(s)
+    assert res_re == res_re1, repr(s)
+
+
+@given(st.from_regex(PunctuationRe.pattern.pattern, fullmatch=True))
+def test_Punctuation(s: str):
+    res_fn = Punctuation.filter(s)
+    res_re1 = PunctuationRe1.filter(s)
+    assert res_fn == res_re1, repr(s)
+
+
 @given(st.from_regex(r"\d+", fullmatch=True))
 @example("124125")
 @example("99990000")
 def test_Numeric(s: str):
     res = Numeric.filter(s)
     assert res, repr(s)
```

### Comparing `sonatoki-0.1.5/tests/test_ilo.py` & `sonatoki-0.2.0/tests/test_ilo.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.5/tests/test_preprocessors.py` & `sonatoki-0.2.0/tests/test_preprocessors.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.5/tests/test_scorers.py` & `sonatoki-0.2.0/tests/test_scorers.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,30 +12,30 @@
     NimiPu,
     Numeric,
     Syllabic,
     NimiLinku,
     Alphabetic,
     ProperName,
     Phonotactic,
-    Punctuation,
+    PunctuationRe,
 )
 from sonatoki.Scorers import Scorer, Scaling, PassFail, SoftScaling, SoftPassFail
 
 # FILESYSTEM
 from .test_utils import token_strategy
 
 FILTERS = [
     NimiPu,
     Numeric,
     Syllabic,
     NimiLinku,
     Alphabetic,
     ProperName,
     Phonotactic,
-    Punctuation,
+    PunctuationRe,
 ]
 
 SCORERS = [
     PassFail,
     SoftPassFail,
     Scaling,
     SoftScaling,
```

### Comparing `sonatoki-0.1.5/tests/test_tokenize.py` & `sonatoki-0.2.0/tests/test_tokenize.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,31 +3,22 @@
 
 # PDM
 import yaml
 import pytest
 
 # LOCAL
 from sonatoki.Tokenizers import (
+    SentTokenizer,
+    WordTokenizer,
     SentTokenizerRe,
     WordTokenizerRe,
-    SentTokenizerTok,
-    WordTokenizerTok,
+    SentTokenizerRe1,
+    WordTokenizerRe1,
 )
 
-try:
-    # PDM
-    import nltk
-
-    # LOCAL
-    from sonatoki.Tokenizers import SentTokenizerNLTK, WordTokenizerNLTK
-
-except ImportError as e:
-    nltk = e
-    # TODO: warn user
-
 
 class TokenizerTest(TypedDict):
     name: str
     input: str
     output: List[str]
     should_be_equal: bool
     xfail: bool
@@ -52,60 +43,81 @@
             )
         )
 
     return formatted_tests
 
 
 @pytest.mark.parametrize(
-    "test", load_tokenizer_tests("tests/tokenize_cases/tokenize_sentences.yml")
+    "test", load_tokenizer_tests("tests/tokenize_cases/tokenize_sentences_tok.yml")
 )
-def test_sentences_re(test: TokenizerTest):
-    if isinstance(nltk, ImportError):
-        pytest.skip("nltk not installed")
+def test_SentTokenizer(test: TokenizerTest):
     if test["xfail"]:
         pytest.xfail()
 
-    transformed_re = SentTokenizerRe.tokenize(test["input"])
-    transformed_nltk = SentTokenizerNLTK.tokenize(test["input"])
-    assert (transformed_re == transformed_nltk) == test["should_be_equal"], test["name"]
+    fn_tokenized = SentTokenizer.tokenize(test["input"])
+    re1_tokenized = SentTokenizerRe1.tokenize(test["input"])
+    assert fn_tokenized == re1_tokenized, test["name"]
 
 
 @pytest.mark.parametrize(
-    "test", load_tokenizer_tests("tests/tokenize_cases/tokenize_words.yml")
+    "test", load_tokenizer_tests("tests/tokenize_cases/tokenize_sentences_tok.yml")
 )
-def test_word_tokenize_re(test: TokenizerTest):
-    if isinstance(nltk, ImportError):
-        pytest.skip("nltk not installed")
+def test_SentTokenizerRe(test: TokenizerTest):
     if test["xfail"]:
         pytest.xfail()
 
-    transformed_re = WordTokenizerRe.tokenize(test["input"])
-    transformed_nltk = WordTokenizerNLTK.tokenize(test["input"])
-    assert (transformed_re == transformed_nltk) == test["should_be_equal"], test["name"]
+    re_tokenized = SentTokenizerRe.tokenize(test["input"])
+    re1_tokenized = SentTokenizerRe1.tokenize(test["input"])
+    assert re_tokenized == re1_tokenized, test["name"]
 
 
 @pytest.mark.parametrize(
     "test", load_tokenizer_tests("tests/tokenize_cases/tokenize_sentences_tok.yml")
 )
-def test_sentences_tok(test: TokenizerTest):
+def test_SentTokenizerRe1(test: TokenizerTest):
+    if test["xfail"]:
+        pytest.xfail()
+
+    re1_tokenized = SentTokenizerRe1.tokenize(test["input"])
+    assert re1_tokenized == test["output"], test["name"]
+
+
+###################
+# Word tokenizers #
+###################
+
+
+@pytest.mark.parametrize(
+    "test", load_tokenizer_tests("tests/tokenize_cases/tokenize_words_tok.yml")
+)
+def test_WordTokenizer(test: TokenizerTest):
+    if test["xfail"]:
+        pytest.xfail()
+
+    fn_tokenized = WordTokenizer.tokenize(test["input"])
+    re1_tokenized = WordTokenizerRe1.tokenize(test["input"])
+    assert fn_tokenized == re1_tokenized, test["name"]
+
+
+@pytest.mark.parametrize(
+    "test", load_tokenizer_tests("tests/tokenize_cases/tokenize_words_tok.yml")
+)
+def test_WordTokenizerRe(test: TokenizerTest):
     if test["xfail"]:
         pytest.xfail()
 
-    transformed_tok = SentTokenizerTok.tokenize(test["input"])
-    if test["should_be_equal"]:
-        assert transformed_tok == test["output"], test["name"]
-    else:
-        assert transformed_tok != test["output"], test["name"]
+    re_tokenized = WordTokenizerRe.tokenize(test["input"])
+    re1_tokenized = WordTokenizerRe1.tokenize(test["input"])
+    assert re_tokenized == re1_tokenized, test["name"]
 
 
 @pytest.mark.parametrize(
     "test", load_tokenizer_tests("tests/tokenize_cases/tokenize_words_tok.yml")
 )
-def test_word_tokenize_tok(test: TokenizerTest):
+def test_WordTokenizerRe1(test: TokenizerTest):
+    """This implementation will always exhibit the correct behavior, so long as `regex` is up to date
+    Thus, it is used as a reference implementation for all other tests"""
     if test["xfail"]:
         pytest.xfail()
 
-    transformed_tok = WordTokenizerTok.tokenize(test["input"])
-    if test["should_be_equal"]:
-        assert transformed_tok == test["output"], test["name"]
-    else:
-        assert transformed_tok != test["output"], test["name"]
+    re1_tokenized = WordTokenizerRe1.tokenize(test["input"])
+    assert re1_tokenized == test["output"], test["name"]
```

### Comparing `sonatoki-0.1.5/tests/test_utils.py` & `sonatoki-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.5/tests/tokenize_cases/tokenize_sentences_tok.yml` & `sonatoki-0.2.0/tests/tokenize_cases/tokenize_sentences_tok.yml`

 * *Files 25% similar despite different names*

```diff
@@ -49,7 +49,14 @@
 - name: "quotes"
   input: "toki li tan kulupu Kuko li ni: 'o ike ala!'"
   output: # expected; we split on right of all sentence-ending puncts
     - "toki li tan kulupu Kuko li ni:"
     - "'"
     - "o ike ala!"
     - "'"
+- name: "discovered case 1"
+  input: "ona li ken lukin e sitelen [_ike_nanpa_lete_ike]. ni li pona kin."
+  output:
+    - "ona li ken lukin e sitelen ["
+    - "_ike_nanpa_lete_ike]"
+    - "."
+    - "ni li pona kin."
```

### Comparing `sonatoki-0.1.5/PKG-INFO` & `sonatoki-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: sonatoki
-Version: 0.1.5
+Version: 0.2.0
 Summary: ilo li moku e toki li pana e sona ni: ni li toki ala toki pona?
 Author-Email: "jan Kekan San (@gregdan3)" <gregory.danielson3@gmail.com>
 License: AGPL-3.0-or-later
 Requires-Python: >=3.8
 Requires-Dist: unidecode>=1.3.6
 Requires-Dist: regex>=2023.12.25
 Requires-Dist: typing-extensions>=4.11.0
-Requires-Dist: nltk>=3.8.1; extra == "nltk"
-Provides-Extra: nltk
 Description-Content-Type: text/markdown
 
 # sona toki
 
 ## What is **sona toki**?
 
 This library, "Language Knowledge," helps you identify whether a message is in Toki Pona. No grammar checking, yet, which means this more checks whether a given message has enough Toki Pona words.
```

