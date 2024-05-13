# Comparing `tmp/hal9-2.0.4.tar.gz` & `tmp/hal9-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hal9-2.0.4.tar", max compression
+gzip compressed data, was "hal9-2.0.5.tar", max compression
```

## Comparing `hal9-2.0.4.tar` & `hal9-2.0.5.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0     2896 2024-05-10 21:00:10.665875 hal9-2.0.4/README.md
--rw-r--r--   0        0        0       86 2024-05-10 21:00:10.593875 hal9-2.0.4/hal9/__init__.py
--rw-r--r--   0        0        0     1033 2024-05-10 21:00:10.593875 hal9-2.0.4/hal9/cli.py
--rw-r--r--   0        0        0      634 2024-05-10 21:00:10.593875 hal9-2.0.4/hal9/create.py
--rw-r--r--   0        0        0      719 2024-05-10 21:00:10.593875 hal9-2.0.4/hal9/deploy.py
--rw-r--r--   0        0        0      531 2024-05-10 21:00:10.593875 hal9-2.0.4/hal9/run.py
--rw-r--r--   0        0        0       70 2024-05-10 21:00:10.597875 hal9-2.0.4/hal9/templates/openai/app.py
--rw-r--r--   0        0        0      403 2024-05-10 21:00:10.597875 hal9-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 hal9-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2951 2024-05-13 20:08:58.664846 hal9-2.0.5/README.md
+-rw-r--r--   0        0        0       86 2024-05-13 20:08:58.596845 hal9-2.0.5/hal9/__init__.py
+-rw-r--r--   0        0        0     1127 2024-05-13 20:08:58.596845 hal9-2.0.5/hal9/cli.py
+-rw-r--r--   0        0        0      634 2024-05-13 20:08:58.596845 hal9-2.0.5/hal9/create.py
+-rw-r--r--   0        0        0      482 2024-05-13 20:08:58.596845 hal9-2.0.5/hal9/deploy.py
+-rw-r--r--   0        0        0      531 2024-05-13 20:08:58.596845 hal9-2.0.5/hal9/run.py
+-rw-r--r--   0        0        0      342 2024-05-13 20:08:58.596845 hal9-2.0.5/hal9/targets/docker.py
+-rw-r--r--   0        0        0      467 2024-05-13 20:08:58.600845 hal9-2.0.5/hal9/targets/hal9.py
+-rw-r--r--   0        0        0       42 2024-05-13 20:08:58.600845 hal9-2.0.5/hal9/templates/docker/Dockerfile
+-rw-r--r--   0        0        0       70 2024-05-13 20:08:58.600845 hal9-2.0.5/hal9/templates/openai/app.py
+-rw-r--r--   0        0        0      434 2024-05-13 20:08:58.600845 hal9-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 hal9-2.0.5/PKG-INFO
```

### Comparing `hal9-2.0.4/README.md` & `hal9-2.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Hal9: Create and Share Generative Apps
 
 [![Hal9 PyPi Downloads](https://img.shields.io/pypi/dm/hal9?label=PyPI)](https://pypi.org/project/hal9/)
 
 Create and deploy generative (LLMs and [difussers](https://github.com/huggingface/diffusers)) applications (chatbots and APIs) in seconds.
 - **Open:** Use any model (OpenAI, Llama, Groq, Midjourney) and any library like (LangChainl, DSPy).
-- **Intuitive:** No need to learn an app framework (streamlit, flask), simply use stdin and stdout.
-- **Scalable:** Engineers can esily integrate your app with Docker or use Hal9's self-service enterprise cloud.
+- **Intuitive:** No need to learn app frameworks (flask), simply use stdin and stdout, or write file to disk.
+- **Scalable:** Engineers can integrate your app with scalable technilogies (Docker, Kubernetes, etc)
+- **Powerful:** Using an OS process (stdin, stdout, files) as our app contract, enables long-running agents, multiple programming languages, and complex system dependencies.
 
 Focus on AI (RAG, fine-tuning, aligment, training) and skip engineering tasks (frontend development, backend integration, deployment, operations).
 
 ## Getting started
 
-To create and deploy a chatbot in 10 seconds run the following:
+To create and share a chatbot in seconds by running the following commands:
 
 ```bash
 pip install hal9
 
 hal9 create chatbot
 hal9 deploy chatbot
 ```
@@ -31,16 +32,14 @@
 hal9 create my-project --template midjourney
 hal9 create my-project --template groq
 hal9 create my-project --template langchain
 ```
 
 A template provides ready to use code with specific technologies and use cases. If you already have code, you can skip this step.
 
-Send a PR if you want to add additional templates.
-
 ## Development
 
 To make changes to your project, open `my-project/` in your IDE and modify `my-project/app.py`.
 
 You can then run your project as follows:
 
 ```bash
@@ -49,51 +48,41 @@
 pip install -r requirements.txt
 
 export OPENAI_KEY=YOUR_OPENAI_KEY
 ```
 
 If you customized your template with `--template` make sure to set the correct key, for example `export GROQ_KEY=YOUR_GROQ_KEY`.
 
-## Runtime
-
-Run your application as follows,
+You can then run your application locally with:
 
-```python
-python app.py
+```bash
+hal9 run .
 ```
 
-Use the command line tool to enter prompts, type `<enter>` twice to send the prompt to your code. Replies will be streamed back to console.
-
-From the parent folder, you can also run your application as follows:
+or
 
 ```bash
+cd ..
 hal9 run my-project
 ```
 
-## Deployment
+This command is just a convenience wrapper over `python app.py`
 
-We currently support Docker and `hal9.com`. Developers can send PR's with additional technologies or providers.
+## Deployment
 
-### Docker
+The deploy command will prepare for deployment your generative app.
 
-To deploy your project through Docker run:
+For example, you can prepare deployment as a generative app (Hal9), an API (Flask), a data app (Streamlit), or a container (Docker).
 
 ```bash
-docker build .
-docker run .
+hal9 deploy my-project --target hal9
+hal9 deploy my-project --target docker
 ```
 
-Your backend and frontend engineers can then easily consume this as an API. You can share the `my-project/` path as a GitHub repo with your infrastructure team for them to deploy to your cloud provider. There are GitHub actions available to build and deploy Docker images.
+Eeach command is tasked with preparing the deployment of your project folder. For example, `--target docker` will create a `Dockerfile` file that gets this project ready to run in cloud containers.
 
-### Hal9
+For personal use, `--target hal9` supports a free tier at `hal9.com`; enterprise support is also available to deploy with `--target hal9 --url hal9.yourcompany.com`
 
-To deploy to `hal9.com` run:
+## Contributing
 
-```bash
-hal9 deploy my-project --target hal9.com
-```
-
-When Hal9 runs in your own cloud you can replace `--target hal9.com` with the correct domain, for example:
+Pull Requests are welcomed to consider additional application templates or deployment targets. See [CONTIBUTE.md](CONTIBUTE.md).
 
-```bash
-hal9 deploy my-project --target hal9.acme.com
-```
```

### Comparing `hal9-2.0.4/hal9/cli.py` & `hal9-2.0.5/hal9/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,41 +12,42 @@
     Use this tool to create apps from templates that use Generative AI,
     run them locally and deploy them to the cloud.
     """
     pass
 
 @click.command()
 @click.argument('path')
-def create(path):
+def create(path :str):
     """
     Create Project
 
     PATH: The path for the new project. Required argument.
     """
     api_create(path, "openai")
 
 @click.command()
 @click.argument('path')
-def run(path):
+def run(path :str):
     """
     Run Project
 
     PATH: The path to the project. Required argument.
     """
     api_run(path)
 
 @click.command()
 @click.argument('path')
-def deploy(path):
+@click.option('--target', default="hal9", help='Deployment target')
+def deploy(path :str, target :str):
     """
     Deploy Project
 
     PATH: The path to the project. Required argument.
     """
-    print(f'Deploying {path}')
+    api_deploy(path, target)
 
 cli.add_command(create)
 cli.add_command(run)
 cli.add_command(deploy)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `hal9-2.0.4/hal9/create.py` & `hal9-2.0.5/hal9/create.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     ----------
     path : str 
             Path to the application.
     template : str 
             The template to use.
     """
 
-    current_dir = Path(__file__).parent
-    template_path = current_dir / "templates" / template
+    package_dir = Path(__file__).parent
+    template_path = package_dir / "templates" / template
 
     os.makedirs(path, exist_ok=True)
 
     for item in template_path.iterdir():
         dest = Path(path) / item.name
         if item.is_dir():
             shutil.copytree(item, dest)
```

### Comparing `hal9-2.0.4/hal9/run.py` & `hal9-2.0.5/hal9/run.py`

 * *Files identical despite different names*

