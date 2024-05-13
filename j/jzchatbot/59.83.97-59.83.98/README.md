# Comparing `tmp/jzchatbot-59.83.97.tar.gz` & `tmp/jzchatbot-59.83.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzchatbot-59.83.97.tar", last modified: Sun May 12 10:06:12 2024, max compression
+gzip compressed data, was "jzchatbot-59.83.98.tar", last modified: Sun May 12 23:39:41 2024, max compression
```

## Comparing `jzchatbot-59.83.97.tar` & `jzchatbot-59.83.98.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 10:06:12.180890 jzchatbot-59.83.97/
--rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.83.97/LICENSE
--rw-rw-rw-   0        0        0      343 2024-05-12 10:06:12.178787 jzchatbot-59.83.97/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-10 01:46:29.000000 jzchatbot-59.83.97/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 10:06:12.159952 jzchatbot-59.83.97/jzchatbot/
--rw-rw-rw-   0        0        0     5955 2024-05-12 10:05:47.000000 jzchatbot-59.83.97/jzchatbot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 10:06:12.176406 jzchatbot-59.83.97/jzchatbot.egg-info/
--rw-rw-rw-   0        0        0      343 2024-05-12 10:06:12.000000 jzchatbot-59.83.97/jzchatbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-12 10:06:12.000000 jzchatbot-59.83.97/jzchatbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 10:06:12.000000 jzchatbot-59.83.97/jzchatbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-12 10:06:12.000000 jzchatbot-59.83.97/jzchatbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-12 10:06:12.000000 jzchatbot-59.83.97/jzchatbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 10:06:12.180890 jzchatbot-59.83.97/setup.cfg
--rw-rw-rw-   0        0        0      530 2024-05-12 10:05:32.000000 jzchatbot-59.83.97/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:39:41.183115 jzchatbot-59.83.98/
+-rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.83.98/LICENSE
+-rw-rw-rw-   0        0        0      343 2024-05-12 23:39:41.183115 jzchatbot-59.83.98/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-10 01:46:29.000000 jzchatbot-59.83.98/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 23:39:41.132255 jzchatbot-59.83.98/jzchatbot/
+-rw-rw-rw-   0        0        0     5316 2024-05-12 23:39:31.000000 jzchatbot-59.83.98/jzchatbot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:39:41.178771 jzchatbot-59.83.98/jzchatbot.egg-info/
+-rw-rw-rw-   0        0        0      343 2024-05-12 23:39:40.000000 jzchatbot-59.83.98/jzchatbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-12 23:39:40.000000 jzchatbot-59.83.98/jzchatbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 23:39:40.000000 jzchatbot-59.83.98/jzchatbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-12 23:39:40.000000 jzchatbot-59.83.98/jzchatbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-12 23:39:40.000000 jzchatbot-59.83.98/jzchatbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 23:39:41.183115 jzchatbot-59.83.98/setup.cfg
+-rw-rw-rw-   0        0        0      530 2024-05-12 23:38:00.000000 jzchatbot-59.83.98/setup.py
```

### Comparing `jzchatbot-59.83.97/LICENSE` & `jzchatbot-59.83.98/LICENSE`

 * *Files identical despite different names*

### Comparing `jzchatbot-59.83.97/jzchatbot/__init__.py` & `jzchatbot-59.83.98/jzchatbot/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,82 +36,67 @@
         best_response = None
         try:
             for entry in self.conversations:
                 question = entry["question"]
                 question_tokens = self.preprocess_text(question)
                 user_input_tokens = self.preprocess_text(user_input)
                 common_tokens = set(question_tokens) & set(user_input_tokens)
-                similarity = len(common_tokens) / max(len(question_tokens), len(user_input_tokens))
+            
+                # Check for division by zero
+                if len(question_tokens) == 0 or len(user_input_tokens) == 0:
+                    similarity = 0
+                else:
+                    similarity = len(common_tokens) / max(len(question_tokens), len(user_input_tokens))
 
                 if similarity > max_similarity:
                     max_similarity = similarity
                     best_response = entry.get("answers", ["I'm sorry, I don't have a response for that."])
 
             if best_response:
                 return random.choice(best_response)
             else:
                 if self.math_enabled and "math" in user_input.lower():
                     return self.handle_math_question(user_input)
                 else:
                     return "I'm sorry, I didn't understand your question."
 
-        except ZeroDivisionError:
-            return "Minimum of 4 characters and/or numbers."
-
         except BaseException as e:
             return f"Error: {e}"
 
     def handle_math_question(self, user_input):
-        math_functions = {
-            "sin": np.sin,
-            "cos": np.cos,
-            "tan": np.tan,
-            "asin": np.arcsin,
-            "acos": np.arccos,
-            "atan": np.arctan,
-            "sqrt": np.sqrt,
-            "log": np.log,
-            "exp": np.exp
-        }
-
-        operands = ["+", "-", "*", "/", "^", "%", "//"]
-
-        for function_name, function in math_functions.items():
-            if function_name in user_input:
-                argument = re.search(r'\d+', user_input).group()
-                try:
-                    result = function(float(argument))
-                    return f"The result of {user_input} is {result}."
-                except ValueError:
-                    return f"Invalid argument for {function_name}."
-
-        for operand in operands:
-            if operand in user_input:
-                numbers = re.findall(r'\d+', user_input)
-                if operand == "+":
-                    result = sum(map(int, numbers))
-                elif operand == "-":
-                    result = int(numbers[0]) - int(numbers[1])
-                elif operand == "*":
-                    result = int(numbers[0]) * int(numbers[1])
-                elif operand == "/":
-                    if int(numbers[1]) != 0:
-                        result = int(numbers[0]) / int(numbers[1])
-                    else:
-                        return "Division by zero is not allowed."
-                elif operand == "^":
-                    result = int(numbers[0]) ** int(numbers[1])
-                elif operand == "%":
-                    result = int(numbers[0]) % int(numbers[1])
-                elif operand == "//":
-                    result = int(numbers[0]) // int(numbers[1])
-
-                return f"The result of {user_input} is {result}."
+        # Regular expression to match mathematical expressions
+        math_expression = re.findall(r'(\d+\.?\d*)\s*([+\-*/^%])\s*(\d+\.?\d*)', user_input)
+    
+        if math_expression:
+            operand1, operator, operand2 = math_expression[0]
+            operand1 = float(operand1)
+            operand2 = float(operand2)
+
+            if operator == '+':
+                result = operand1 + operand2
+            elif operator == '-':
+                result = operand1 - operand2
+            elif operator == '*':
+                result = operand1 * operand2
+            elif operator == '/':
+                if operand2 != 0:
+                    result = operand1 / operand2
+                else:
+                    return "Division by zero is not allowed."
+            elif operator == '^':
+                result = operand1 ** operand2
+            elif operator == '%':
+                result = operand1 % operand2
+            else:
+                return "Invalid operator."
+        
+            return f"The result of {user_input} is {result}."
 
-        return "I'm sorry, I couldn't solve that math question."
+        else:
+            return "I'm sorry, I couldn't solve that math question."
 
     def speak(self, text):
         self.engine.say(text)
         self.engine.runAndWait()
 
     def load_conversations(self, file_path):
         with open(file_path, 'r') as file:
```

### Comparing `jzchatbot-59.83.97/setup.py` & `jzchatbot-59.83.98/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open("README.md", "r") as fh: 
 	description = fh.read() 
 
 setuptools.setup( 
 	name="jzchatbot", 
-	version="59.83.97", 
+	version="59.83.98", 
 	author="JZ Enterprises", 
 	packages=setuptools.find_packages(), 
 	description="A package that creates advanced AI chatbots", 
 	long_description=description, 
 	long_description_content_type="text/markdown", 
 	license='MIT', 
 	python_requires='>=3.8',
```

