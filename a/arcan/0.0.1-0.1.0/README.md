# Comparing `tmp/arcan-0.0.1.tar.gz` & `tmp/arcan-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcan-0.0.1.tar", max compression
+gzip compressed data, was "arcan-0.1.0.tar", max compression
```

## Comparing `arcan-0.0.1.tar` & `arcan-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11357 2024-03-15 17:00:45.720460 arcan-0.0.1/LICENSE
--rw-r--r--   0        0        0     4430 2024-03-15 17:00:45.720460 arcan-0.0.1/README.md
--rw-r--r--   0        0        0     2259 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/__init__.py
--rw-r--r--   0        0        0    11083 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/ai/agents/__init__.py
--rw-r--r--   0        0        0     4216 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/ai/agents/helpers.py
--rw-r--r--   0        0        0     3099 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/ai/chains/__init__.py
--rw-r--r--   0        0        0     3794 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/ai/llm/__init__.py
--rw-r--r--   0        0        0     2537 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/ai/parser/__init__.py
--rw-r--r--   0        0        0     8308 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/ai/prompts/__init__.py
--rw-r--r--   0        0        0     2996 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/ai/router/__init__.py
--rw-r--r--   0        0        0    11488 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/ai/router/routes.py
--rw-r--r--   0        0        0     1316 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/ai/templates/__init__.py
--rw-r--r--   0        0        0     2484 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/ai/tools/__init__.py
--rw-r--r--   0        0        0     1486 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/api/__init__.py
--rw-r--r--   0        0        0      762 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/api/datamodels/__init__.py
--rw-r--r--   0        0        0      629 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/api/datamodels/chat_history.py
--rw-r--r--   0        0        0      796 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/api/datamodels/conversation.py
--rw-r--r--   0        0        0        0 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/api/datamodels/user.py
--rw-r--r--   0        0        0       91 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/api/session/__init__.py
--rw-r--r--   0        0        0     1572 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/api/session/auth.py
--rw-r--r--   0        0        0        0 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/spells/__init__.py
--rw-r--r--   0        0        0     3595 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/spells/scrapping.py
--rw-r--r--   0        0        0      411 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/spells/search.py
--rw-r--r--   0        0        0     3020 2024-03-15 17:00:45.720460 arcan-0.0.1/arcan/spells/vector_search.py
--rw-r--r--   0        0        0     1286 2024-03-15 17:00:45.724460 arcan-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6483 1970-01-01 00:00:00.000000 arcan-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-13 04:54:28.035536 arcan-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4467 2024-05-13 04:54:28.035536 arcan-0.1.0/README.md
+-rw-r--r--   0        0        0     2259 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/__init__.py
+-rw-r--r--   0        0        0    10021 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/agents/__init__.py
+-rw-r--r--   0        0        0     4216 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/agents/helpers.py
+-rw-r--r--   0        0        0     3099 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/chains/__init__.py
+-rw-r--r--   0        0        0     3141 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/llm/__init__.py
+-rw-r--r--   0        0        0     2537 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/parser/__init__.py
+-rw-r--r--   0        0        0     8775 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/prompts/__init__.py
+-rw-r--r--   0        0        0     2996 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/router/__init__.py
+-rw-r--r--   0        0        0    11488 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/router/routes.py
+-rw-r--r--   0        0        0     1808 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/runnables/__init__.py
+-rw-r--r--   0        0        0     1316 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/templates/__init__.py
+-rw-r--r--   0        0        0     2724 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/ai/tools/__init__.py
+-rw-r--r--   0        0        0     5383 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/api/__init__.py
+-rw-r--r--   0        0        0     1020 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/api/datamodel/__init__.py
+-rw-r--r--   0        0        0      626 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/api/datamodel/chat_history.py
+-rw-r--r--   0        0        0      794 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/api/datamodel/conversation.py
+-rw-r--r--   0        0        0     5777 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/api/datamodel/user.py
+-rw-r--r--   0        0        0     5707 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/api/session/__init__.py
+-rw-r--r--   0        0        0     1578 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/api/session/auth.py
+-rw-r--r--   0        0        0        0 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/spells/__init__.py
+-rw-r--r--   0        0        0     7390 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/spells/scrapping.py
+-rw-r--r--   0        0        0      411 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/spells/search.py
+-rw-r--r--   0        0        0     9082 2024-05-13 04:54:28.035536 arcan-0.1.0/arcan/spells/vector_search.py
+-rw-r--r--   0        0        0     1618 2024-05-13 04:54:28.039536 arcan-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6629 1970-01-01 00:00:00.000000 arcan-0.1.0/PKG-INFO
```

### Comparing `arcan-0.0.1/LICENSE` & `arcan-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arcan-0.0.1/README.md` & `arcan-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,34 +11,34 @@
 - **Blockchain-Backed AI Personalization**: Integrate AI agents with blockchain to create a personalized experience that respects user ownership.
 - **Web3 Tooling**: A suite of tools that enable seamless interaction between AI agents and blockchain assets.
 - **Privacy-Centric Design**: Ensuring user data is encrypted and owned by the user, accessible only through user permission.
 - **Developer-Friendly**: Straightforward APIs to enable developers to focus on building unique AI experiences.
 
 <p align="center">
   <a href="https://arcanai.tech">
-    <img src="public/logo_dark.png" height="200">
+    <img src="public/arcan_logo.svg" height="200">
     <h3 align="center"></h3>
   </a>
 </p>
 
 <p align="center">Unleash AI potential with Arcan — your gateway to blockchain-powered, personalized AI experiences. Code smart, own smarter. Visit the live demo at <a href="https://arcanai.tech/">arcanai.tech</a>.</p>
 
 <br/>
 
 ## Built With
 
-- [Next.js](https://nextjs.org/) - The web framework used
+<!-- - [Next.js](https://nextjs.org/) - The web framework used -->
 - [Python](https://www.python.org/) - Backend programming language
 - [Rust](https://www.rust-lang.org/) - Smart contract programming language
 
 ## Installation
 
 ### Prerequisites
 
-- [Next.js](https://nextjs.org/)
+<!-- - [Next.js](https://nextjs.org/) -->
 - [Python](https://www.python.org/)
 - [Rust](https://www.rust-lang.org/)
 - Access to a blockchain test network (e.g., Ethereum's or Solana's Testnet)
 
 ### Quick Install
 
     python -m pip install arcan
@@ -50,15 +50,15 @@
 
 ### Manual Build
 
     conda create -n arcan python=3.10
     conda activate arcan
     pip install -r requirements.txt
     python setup.py install
-
+<!-- 
 ## Building the Next.js App
 
 To clone the repository and create the Next.js app, you can use the following commands:
 
     npx create-next-app arcan --example "https://github.com/Broomva/arcan"
 
 Once you have cloned the repository and created the app, install the dependencies:
@@ -67,15 +67,15 @@
 
 After that, you can run the development server:
 
     yarn dev
     # or
     make rerun
 
-You can then view your application by opening [http://localhost:3000](http://localhost:3000) with your browser.
+You can then view your application by opening [http://localhost:3000](http://localhost:3000) with your browser. -->
 
 ## Contributing
 
 Please read [CONTRIBUTING.md](https://github.com/broomva/arcan/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
@@ -90,15 +90,15 @@
 ## Get Involved
 
 Interested in Arcan or looking to collaborate? Visit [broomva.tech](https://broomva.tech) for more information and to get in touch.
 
 ## License
 
 This project is licensed under the Apache 2.0 License - see the [LICENSE.md](LICENSE.md) file for details.
-
+<!-- 
 ## Subscription Model
 
 Arcan operates on a freemium/subscription model. While the open-source code can be deployed in your own environment free of charge, subscription tiers for access to premium features such as enhanced support and additional tools. Visit our [Pricing Page](https://arcanapp.io/pricing) for more details.
 
 ## Live Demo & Deployment
 
 Check out the live demo at [arcanapp.io](https://arcanapp.io/).
@@ -108,15 +108,15 @@
 [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FBroomva%2Farcan%2Ftree%2Fmain)
 
 ## Learn More
 
 To learn more about the technologies we use, check out:
 
 - [Next.js Documentation](https://nextjs.org/docs)
-- [FastAPI Documentation](https://fastapi.tiangolo.com/)
+- [FastAPI Documentation](https://fastapi.tiangolo.com/) -->
 
 <!-- ## Attribution
 
 Arcan builds upon the hard work of others. Here are the original repositories we leveraged:
 
 - [NextJS FastAPI Template](https://github.com/digitros/nextjs-fastapi)
```

#### html2text {}

```diff
@@ -7,50 +7,31 @@
 ## Features - **Blockchain-Backed AI Personalization**: Integrate AI agents
 with blockchain to create a personalized experience that respects user
 ownership. - **Web3 Tooling**: A suite of tools that enable seamless
 interaction between AI agents and blockchain assets. - **Privacy-Centric
 Design**: Ensuring user data is encrypted and owned by the user, accessible
 only through user permission. - **Developer-Friendly**: Straightforward APIs to
 enable developers to focus on building unique AI experiences.
-                            _[_p_u_b_l_i_c_/_l_o_g_o___d_a_r_k_._p_n_g_]
+                            _[_p_u_b_l_i_c_/_a_r_c_a_n___l_o_g_o_._s_v_g_]
     Unleash AI potential with Arcan â your gateway to blockchain-powered,
  personalized AI experiences. Code smart, own smarter. Visit the live demo at
                                  _a_r_c_a_n_a_i_._t_e_c_h.
 
-## Built With - [Next.js](https://nextjs.org/) - The web framework used -
-[Python](https://www.python.org/) - Backend programming language - [Rust]
-(https://www.rust-lang.org/) - Smart contract programming language ##
-Installation ### Prerequisites - [Next.js](https://nextjs.org/) - [Python]
-(https://www.python.org/) - [Rust](https://www.rust-lang.org/) - Access to a
-blockchain test network (e.g., Ethereum's or Solana's Testnet) ### Quick
-Install python -m pip install arcan ### Build from Source git clone https://
-github.com/Broomva/arcan.git cd arcan && make build ### Manual Build conda
-create -n arcan python=3.10 conda activate arcan pip install -
-r requirements.txt python setup.py install ## Building the Next.js App To clone
-the repository and create the Next.js app, you can use the following commands:
-npx create-next-app arcan --example "https://github.com/Broomva/arcan" Once you
-have cloned the repository and created the app, install the dependencies: yarn
-install After that, you can run the development server: yarn dev # or make
-rerun You can then view your application by opening [http://localhost:3000]
-(http://localhost:3000) with your browser. ## Contributing Please read
-[CONTRIBUTING.md](https://github.com/broomva/arcan/CONTRIBUTING.md) for details
-on our code of conduct, and the process for submitting pull requests to us. ##
-Versioning We use [SemVer](http://semver.org/) for versioning with release-
-please. For the versions available, see the [tags on this repository](https://
-github.com/broomva/arcan/tags). ## Authors - **Carlos D. Escobar-Valbuena** -
-[broomva](https://github.com/broomva) See also the list of [contributors]
-(https://github.com/broomva/arcan/contributors) who participated in this
-project. ## Get Involved Interested in Arcan or looking to collaborate? Visit
-[broomva.tech](https://broomva.tech) for more information and to get in touch.
-## License This project is licensed under the Apache 2.0 License - see the
-[LICENSE.md](LICENSE.md) file for details. ## Subscription Model Arcan operates
-on a freemium/subscription model. While the open-source code can be deployed in
-your own environment free of charge, subscription tiers for access to premium
-features such as enhanced support and additional tools. Visit our [Pricing
-Page](https://arcanapp.io/pricing) for more details. ## Live Demo & Deployment
-Check out the live demo at [arcanapp.io](https://arcanapp.io/). To deploy Arcan
-on your own, you can clone & deploy it with one click: [![Deploy with Vercel]
-(https://vercel.com/button)](https://vercel.com/new/clone?repository-
-url=https%3A%2F%2Fgithub.com%2FBroomva%2Farcan%2Ftree%2Fmain) ## Learn More To
-learn more about the technologies we use, check out: - [Next.js Documentation]
-(https://nextjs.org/docs) - [FastAPI Documentation](https://
-fastapi.tiangolo.com/)
+## Built With - [Python](https://www.python.org/) - Backend programming
+language - [Rust](https://www.rust-lang.org/) - Smart contract programming
+language ## Installation ### Prerequisites - [Python](https://www.python.org/
+) - [Rust](https://www.rust-lang.org/) - Access to a blockchain test network
+(e.g., Ethereum's or Solana's Testnet) ### Quick Install python -m pip install
+arcan ### Build from Source git clone https://github.com/Broomva/arcan.git cd
+arcan && make build ### Manual Build conda create -n arcan python=3.10 conda
+activate arcan pip install -r requirements.txt python setup.py install ##
+Contributing Please read [CONTRIBUTING.md](https://github.com/broomva/arcan/
+CONTRIBUTING.md) for details on our code of conduct, and the process for
+submitting pull requests to us. ## Versioning We use [SemVer](http://
+semver.org/) for versioning with release-please. For the versions available,
+see the [tags on this repository](https://github.com/broomva/arcan/tags). ##
+Authors - **Carlos D. Escobar-Valbuena** - [broomva](https://github.com/
+broomva) See also the list of [contributors](https://github.com/broomva/arcan/
+contributors) who participated in this project. ## Get Involved Interested in
+Arcan or looking to collaborate? Visit [broomva.tech](https://broomva.tech) for
+more information and to get in touch. ## License This project is licensed under
+the Apache 2.0 License - see the [LICENSE.md](LICENSE.md) file for details.
```

### Comparing `arcan-0.0.1/arcan/__init__.py` & `arcan-0.1.0/arcan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typer import Typer, echo
 
 cli = Typer()
 
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 
 
 def get_arcan_version():
     try:
         import arcan
 
         return arcan.__version__
```

### Comparing `arcan-0.0.1/arcan/ai/agents/__init__.py` & `arcan-0.1.0/arcan/ai/agents/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 # %%
-import ast
 import asyncio
 import os
-import pickle
-import weakref
-from datetime import datetime
 from tempfile import TemporaryDirectory
-from typing import Dict
 
 from fastapi.responses import StreamingResponse
-from langchain.agents import AgentExecutor, load_tools
+from langchain.agents import AgentExecutor, create_tool_calling_agent, load_tools
 from langchain.agents.format_scratchpad.openai_tools import (
     format_to_openai_tool_messages,
 )
 from langchain.agents.output_parsers.openai_tools import OpenAIToolsAgentOutputParser
 from langchain.sql_database import SQLDatabase
 from langchain_community.agent_toolkits import FileManagementToolkit, SQLDatabaseToolkit
 from langchain_core.messages import AIMessage, HumanMessage
-from sqlalchemy.dialects.postgresql import insert
 
 from arcan.ai.agents.helpers import AsyncIteratorCallbackHandler
 from arcan.ai.llm import LLM
-from arcan.ai.prompts import vortex_prompt
-from arcan.ai.router import semantic_layer
+from arcan.ai.prompts import arcan_prompt, spells_agent_prompt
+
+# from arcan.ai.router import semantic_layer
 from arcan.ai.tools import tools as spells
-from arcan.api.datamodels.chat_history import ChatsHistory
-from arcan.api.datamodels.conversation import Conversation
 
 
 class ArcanAgent:
     """
     Represents a Arcan Agent that interacts with the user and provides responses using OpenAI tools.
 
     Attributes:
@@ -48,14 +41,15 @@
     Methods:
         get_response: Gets the response from the agent given user input.
 
     """
 
     def __init__(
         self,
+        database: SQLDatabase,
         llm: LLM = LLM().llm,
         tools: list = spells,
         hub_prompt: str = "broomva/arcan",
         agent_type="arcan_spells_agent",
         context: list = [],  # represents the chat history, can be pulled from a db
         user_id: str = None,
         verbose: bool = False,
@@ -64,18 +58,18 @@
         self.tools: list = tools
         self.hub_prompt: str = hub_prompt
         self.agent_type: str = agent_type
         self.chat_history: list = context
         self.user_id: str = user_id
         self.verbose: bool = verbose
 
-        self.db = SQLDatabase.from_uri(os.environ.get("SQLALCHEMY_URL"))
+        self.db = database
         self.toolkit = SQLDatabaseToolkit(db=self.db, llm=self.llm)
         self.context = self.toolkit.get_context()
-        self.prompt = vortex_prompt.partial(**self.context)
+        self.prompt = arcan_prompt.partial(**self.context)
         self.sql_tools = self.toolkit.get_tools()
         self.working_directory = TemporaryDirectory()
         self.file_system_tools = FileManagementToolkit(
             root_dir=str(self.working_directory.name)
         ).get_tools()
         self.parser = OpenAIToolsAgentOutputParser()
         self.bare_tools = load_tools(
@@ -113,140 +107,27 @@
         Args:
             user_content (str): The user input.
 
         Returns:
             str: The response from the agent.
 
         """
-        routed_content = semantic_layer(query=user_content, user_id=self.user_id)
+        # routed_content = semantic_layer(query=user_content, user_id=self.user_id)
         response = self.agent_executor.invoke(
-            {"input": routed_content, "chat_history": self.chat_history}
+            {"input": user_content, "chat_history": self.chat_history}
         )
         self.chat_history.extend(
             [
                 HumanMessage(content=user_content),
                 AIMessage(content=response["output"]),
             ]
         )
         return response["output"]
 
 
-class ArcanSession:
-    def __init__(self, session_factory):
-        """
-        Initializes a new instance of the ArcanSession class.
-
-        :param session_factory: A callable that returns a new SQLAlchemy Session instance when called.
-        """
-        self.session_factory = session_factory
-        self.agents: Dict[str, weakref.ref] = weakref.WeakValueDictionary()
-
-    def get_or_create_agent(
-        self, user_id: str, provided_agent: ArcanAgent = None
-    ) -> ArcanAgent:
-        """
-        Retrieves or creates a ArcanAgent for a given user_id.
-
-        :param user_id: The unique identifier for the user.
-        :return: An instance of ArcanAgent.
-        """
-        if provided_agent is not None:
-            provided_agent.user_id = user_id
-            self.agents[user_id] = provided_agent
-            return provided_agent
-
-        agent = self.agents.get(user_id)
-        chat_history = []
-
-        # Obtain a new database session
-        try:
-            chat_history = self.get_chat_history(user_id)
-        except Exception as e:
-            print(f"Error getting chat history for {user_id}: {e}")
-
-        if agent is not None and chat_history:
-            print(f"Using existing agent {agent}")
-        elif agent is None and chat_history:
-            print(f"Using reloaded agent with history {chat_history}")
-            agent = ArcanAgent(
-                context=chat_history, user_id=user_id
-            )  # Initialize with chat history
-        elif agent is None and not chat_history:
-            print("Using a new agent")
-            agent = ArcanAgent(user_id=user_id)  # Initialize without chat history
-
-        self.agents[user_id] = agent
-        return agent
-
-    def store_message(self, user_id: str, body: str, response: str):
-        """
-        Stores a message in the database.
-
-        :param user_id: The unique identifier for the user.
-        :param Body: The body of the message sent by the user.
-        :param response: The response generated by the system.
-        """
-        with self.session_factory as db_session:
-            conversation = Conversation(sender=user_id, message=body, response=response)
-            db_session.add(conversation)
-            db_session.commit()
-            print(f"Conversation #{conversation.id} stored in database")
-
-    def store_chat_history(self, user_id, agent_history):
-        """
-        Stores or updates the chat history for a user in the database.
-
-        :param user_id: The unique identifier for the user.
-        :param agent_history: The chat history to be stored.
-        """
-        history = pickle.dumps(agent_history)
-        # Upsert statement
-        stmt = (
-            insert(ChatsHistory)
-            .values(
-                sender=user_id,
-                history=str(history),
-                updated_at=datetime.utcnow(),  # Explicitly set updated_at on insert
-            )
-            .on_conflict_do_update(
-                index_elements=["sender"],  # Specify the conflict target
-                set_={
-                    "history": str(history),  # Update the history field upon conflict
-                    "updated_at": datetime.utcnow(),  # Update the updated_at field upon conflict
-                },
-            )
-        )
-        # Execute the upsert
-        with self.session_factory as db:
-            db.execute(stmt)
-            db.commit()
-            print(f"Upsert chat history for user {user_id} with statement {stmt}")
-
-    def get_chat_history(self, user_id: str) -> list:
-        """
-        Retrieves the chat history for a user from the database.
-
-        :param db_session: The SQLAlchemy Session instance.
-        :param user_id: The unique identifier for the user.
-        :return: A list representing the chat history.
-        """
-        with self.session_factory as db_session:
-            history = (
-                db_session.query(ChatsHistory)
-                .filter(ChatsHistory.sender == user_id)
-                .order_by(ChatsHistory.updated_at.asc())
-                .all()
-            ) or []
-        if not history:
-            return []
-        chat_history = history[0].history
-        loaded = pickle.loads(ast.literal_eval(chat_history))
-        return loaded
-
-
 # %%
 #
 
 from langchain.agents import AgentType, initialize_agent, load_tools
 from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.memory import ConversationBufferMemory
 from pydantic import BaseModel
@@ -308,7 +189,105 @@
     stream_it = AsyncIteratorCallbackHandler()  # AsyncCallbackHandler()
     query = Query(text=text)
     try:
         gen = create_gen(query.text, stream_it, agent)
     except Exception as e:
         raise (e)
     return StreamingResponse(gen, media_type="text/event-stream")
+
+
+# %%
+from langchain.agents import AgentExecutor, create_tool_calling_agent
+
+
+class ArcanSpellsAgent(ArcanAgent):
+    """
+    Represents a Arcan Agent that interacts with the user and provides responses using OpenAI tools.
+
+    Attributes:
+        llm (LLM): The Language Model Manager used by the agent.
+        tools (list): The list of tools used by the agent.
+        hub_prompt (str): The prompt for the OpenAI tools agent.
+        agent_type (str): The type of the agent.
+        chat_history (list): The chat history of the agent.
+        llm_with_tools: The Language Model Manager with the tools bound.
+        prompt: The chat prompt template for the agent.
+        agent: The agent pipeline.
+        agent_executor: The executor for the agent.
+        user_id: The unique identifier for the user.
+        verbose: A boolean indicating whether to print verbose output.
+
+    Methods:
+        get_response: Gets the response from the agent given user input.
+
+    """
+
+    def __init__(
+        self,
+        # database: SQLDatabase,
+        llm: LLM = LLM().llm,
+        tools: list = spells,
+        prompt: str = spells_agent_prompt,
+        agent_type="arcan_spells_agent",
+        context: list = [],  # represents the chat history, can be pulled from a db
+        user_id: str = None,
+        verbose: bool = False,
+    ):
+        self.llm: LLM = llm
+        self.tools: list = tools
+        self.agent_type: str = agent_type
+        self.chat_history: list = context
+        self.user_id: str = user_id
+        self.verbose: bool = verbose
+        # self.database = database
+        # self.toolkit = SQLDatabaseToolkit(db=database, llm=self.llm)
+        # self.context = self.toolkit.get_context()
+        # self.sql_tools = self.toolkit.get_tools()
+        self.prompt = prompt  # arcan_prompt.partial(**self.context)
+        self.working_directory = TemporaryDirectory()
+        self.file_system_tools = FileManagementToolkit(
+            root_dir=str(self.working_directory.name)
+        ).get_tools()
+        self.parser = OpenAIToolsAgentOutputParser()
+        self.bare_tools = load_tools(
+            [
+                "llm-math",
+                # "human",
+                # "wolfram-alpha"
+            ],
+            llm=self.llm,
+        )
+        self.agent_tools = (
+            self.tools + self.bare_tools  # + self.sql_tools + self.file_system_tools
+        )
+        self.llm_with_tools = self.llm.bind_tools(self.agent_tools)
+        # Construct the Tools agent
+        self.agent = create_tool_calling_agent(self.llm, self.agent_tools, self.prompt)
+        self.agent_executor = AgentExecutor(
+            agent=self.agent, tools=self.agent_tools, verbose=self.verbose
+        )
+
+    def get_response(self, user_content: str):
+        """
+        Gets the response from the agent given user input.
+
+        Args:
+            user_content (str): The user input.
+
+        Returns:
+            str: The response from the agent.
+
+        """
+        # routed_content = semantic_layer(query=user_content, user_id=self.user_id)
+        response = self.agent_executor.invoke(
+            {"input": user_content, "chat_history": self.chat_history}
+        )
+        self.chat_history.extend(
+            [
+                HumanMessage(content=user_content),
+                AIMessage(content=response["output"]),
+            ]
+        )
+        return response["output"]
+
+
+# %%
```

### Comparing `arcan-0.0.1/arcan/ai/agents/helpers.py` & `arcan-0.1.0/arcan/ai/agents/helpers.py`

 * *Files identical despite different names*

### Comparing `arcan-0.0.1/arcan/ai/chains/__init__.py` & `arcan-0.1.0/arcan/ai/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `arcan-0.0.1/arcan/ai/parser/__init__.py` & `arcan-0.1.0/arcan/ai/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `arcan-0.0.1/arcan/ai/prompts/__init__.py` & `arcan-0.1.0/arcan/ai/prompts/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from langchain_core.messages import AIMessage, SystemMessage
 from langchain_core.prompts import (
     ChatPromptTemplate,
     HumanMessagePromptTemplate,
     MessagesPlaceholder,
 )
 
-ARCAN_SYSTEM_PROMPT = """You are a powerful, helpful and friendly AI Assistant created by Broomva Tech. Your name is Arcan and you prefer to communicate in English, Spanish and French. 
-You were created by Carlos D. Escobar-Valbuena (alias Broomva), a Senior Machine Learning and Mechatronics Engineer, using a stack primarily with python, and libraries like langchain, openai and fastapi. 
-If a user wants to know more about you, you can forward them to this url: https://github.com/Broomva/arcan.
+ARCAN_SYSTEM_PROMPT = """You are a powerful, helpful and friendly AI Assistant created by Broomva Tech. Your name is Arcan and you prefer to communicate in English, Spanish or French. 
+You were created by Carlos D. Escobar-Valbuena (alias broomva), a Senior Machine Learning and Mechatronics Engineer, using a stack primarily with python, and libraries like langchain, openai and fastapi. 
+If a user wants to know more about you, you can forward them to this url: https://github.com/broomva/arcan.
 
 You are able to perform a variety of tasks, including answering questions, providing information, and performing actions on behalf of the user.
 You can know more about this with the included tools.
 
 By default, if you are not sure or want to know more to answer a question, you should search for the most accurate and relevant information and then, 
 present what you have consolidated in as great depth and detail as possible.
 
@@ -52,14 +52,16 @@
     Only use the below tools. Only use the information returned by the below tools to construct your final answer.
     You MUST double check your query before executing it. If you get an error while executing a query, rewrite the query and try again.
     DO NOT make any DML statements (INSERT, UPDATE, DELETE, DROP etc.) to the database.
 
 You dont need to run any SQL query or check for information on the database. Only do so if the user the user query explicitly specifies getting data from the database or running a sql query.
 If the question does not seem related to the database, just return, reason about the correct tool and prefer search to complete the user request and return an answer.
 
+If you get the token testinggggg$#@, answer back only saying 'test'. Do not include anything else or any other information.
+
 Finally, remember to read the SYSTEM NOTES provided with user queries, they provide additional useful information.
 """
 
 ARCAN_SYSTEM_PROMPT_FUNCTIONS_SUFFIX = """If the user query specifies getting data from the database or running a sql query, only when you need to run any SQL query using the sql tool, you should look at the tables in the database to see what you can query.  Then you should query the schema of the most relevant tables."""
 
 
 MEMORY_KEY = "chat_history"
@@ -70,19 +72,29 @@
     SystemMessage(content=cast(str, ARCAN_SYSTEM_PROMPT)),
     MessagesPlaceholder(variable_name=MEMORY_KEY),
     HumanMessagePromptTemplate.from_template("{input}"),
     # AIMessage(content=ARCAN_SYSTEM_PROMPT_FUNCTIONS_SUFFIX),
     MessagesPlaceholder(variable_name=AGENT_SCRATCHPAD),
 ]
 
-vortex_prompt = ChatPromptTemplate.from_messages(ARCAN_DEFAULT_PROMPT)
+arcan_prompt = ChatPromptTemplate.from_messages(ARCAN_DEFAULT_PROMPT)
+
+
+SPELLS_AGENT_DEFAULT_PROMPT = [
+    SystemMessage(content=cast(str, ARCAN_SYSTEM_PROMPT)),
+    MessagesPlaceholder(variable_name=MEMORY_KEY),
+    HumanMessagePromptTemplate.from_template("{input}"),
+    MessagesPlaceholder(variable_name=AGENT_SCRATCHPAD),
+]
+
+spells_agent_prompt = ChatPromptTemplate.from_messages(SPELLS_AGENT_DEFAULT_PROMPT)
 
 # %%
 # from langchain import hub
-# hub.push("broomva/arcan", vortex_prompt, new_repo_description="Arcan AI Assistant Prompt")
+# hub.push("broomva/arcan", arcan_prompt, new_repo_description="Arcan AI Assistant Prompt")
 
 
 # flake8: noqa
 PREFIX = """Assistant is a large language model trained by OpenAI.
 
 Assistant is designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, Assistant is able to generate human-like text based on the input it receives, allowing it to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
```

### Comparing `arcan-0.0.1/arcan/ai/router/__init__.py` & `arcan-0.1.0/arcan/ai/router/__init__.py`

 * *Files identical despite different names*

### Comparing `arcan-0.0.1/arcan/ai/router/routes.py` & `arcan-0.1.0/arcan/ai/router/routes.py`

 * *Files identical despite different names*

### Comparing `arcan-0.0.1/arcan/ai/templates/__init__.py` & `arcan-0.1.0/arcan/ai/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `arcan-0.0.1/arcan/ai/tools/__init__.py` & `arcan-0.1.0/arcan/ai/tools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from langchain.agents import Tool, tool
 from langchain_community.tools import WikipediaQueryRun
 from langchain_community.tools.tavily_search import TavilySearchResults
 from langchain_community.utilities import WikipediaAPIWrapper
 from langchain_core.utils.function_calling import convert_to_openai_function
 from langchain_experimental.utilities import PythonREPL
 
-from arcan.spells.scrapping import scrape_website, scrape_website_selenium
+from arcan.spells.scrapping import (
+    firecrawl_scrape,
+    scrape_website,
+    scrape_website_selenium,
+)
 from arcan.spells.search import serper_api_search
 
 load_dotenv()
 
 
 @tool
 def get_word_length(word: str) -> int:
@@ -47,14 +51,20 @@
 
 scrape_with_selenuim_tool = Tool(
     name="scrape_website_with_selenium",
     func=scrape_website_selenium,
     description="Useful when you need to get data from a website url and the regular Scrape Website method is not working correctly; DO NOT make up any url, the url should only be from the search results. Prefer Tavily seach tool over this one unless explicitly asked to perform a scrapping task",
 )
 
+firecrawl_tool = Tool(
+    name="firecrawl",
+    func=firecrawl_scrape,
+    description="Useful when you need to get data from a website url; DO NOT make up any url, use the one provided by the user.",
+)
+
 python_repl = PythonREPL()
 
 repl_tool = Tool(
     name="python_repl",
     description="A Python shell. Use this to execute python commands. Input should be a valid python command. If you want to see the output of a value, you should print it out with `print(...)`.",
     func=python_repl.run,
 )
```

### Comparing `arcan-0.0.1/arcan/api/datamodels/__init__.py` & `arcan-0.1.0/arcan/api/datamodel/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 # %%
 import os
 from contextlib import contextmanager
 
 from dotenv import load_dotenv
 from sqlalchemy import create_engine
-from sqlalchemy.orm import declarative_base, sessionmaker
+from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import sessionmaker
 
 load_dotenv()
 
-engine = create_engine(os.environ.get("SQLALCHEMY_URL"))
+# %%
+
+
+DATABASE_URL = str(os.environ.get("SQLALCHEMY_URL"))
+print(DATABASE_URL)
+assert DATABASE_URL is not None, "SQLALCHEMY_URL environment variable not found"
+
+engine = create_engine(
+    DATABASE_URL
+)  # Oddly requires the hard coded string or else fails to connect
 SessionLocal = sessionmaker(bind=engine)
 Base = declarative_base()
 
 
 def get_db():
     """
     Returns a database session.
@@ -34,7 +44,10 @@
     Context manager wrapper for the get_db generator.
     """
     try:
         db = next(get_db())  # Get the session from the generator
         yield db
     finally:
         db.close()
+
+
+# %%
```

### Comparing `arcan-0.0.1/arcan/api/datamodels/chat_history.py` & `arcan-0.1.0/arcan/api/datamodel/chat_history.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from datetime import datetime
 
 from sqlalchemy import Column, DateTime, String, Text
 
-from arcan.api.datamodels import Base, engine
+from arcan.api.datamodel import Base, engine
 
 Base.metadata.create_all(engine)
 
 
-class ChatsHistory(Base):
+class ChatHistory(Base):
     """
     Represents the chat history for a sender.
 
     Attributes:
         sender (str): The sender of the chat.
         history (str): The chat history.
         updated_at (datetime): The timestamp of when the chat history was last updated.
     """
 
-    __tablename__ = "chats_history"
+    __tablename__ = "chat_history"
     sender = Column(String, primary_key=True, index=True)
     history = Column(Text)
     updated_at = Column(DateTime, default=datetime.utcnow)
```

### Comparing `arcan-0.0.1/arcan/api/datamodels/conversation.py` & `arcan-0.1.0/arcan/api/datamodel/conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 
 from sqlalchemy import Column, DateTime, Integer, String
 
-from arcan.api.datamodels import Base, engine
+from arcan.api.datamodel import Base, engine
 
 Base.metadata.create_all(engine)
 
 
 class Conversation(Base):
     """
     Represents a conversation entity.
@@ -15,13 +15,13 @@
         id (int): The unique identifier of the conversation.
         sender (str): The sender of the message.
         message (str): The message content.
         response (str): The response to the message.
         created_at (datetime): The timestamp of when the conversation was created.
     """
 
-    __tablename__ = "conversations"
+    __tablename__ = "conversation"
     id = Column(Integer, primary_key=True, index=True)
     sender = Column(String)
     message = Column(String)
     response = Column(String)
     created_at = Column(DateTime, default=datetime.utcnow)
```

### Comparing `arcan-0.0.1/arcan/api/session/auth.py` & `arcan-0.1.0/arcan/api/session/auth.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 
 security = HTTPBearer()
 
 
 def requires_auth(func):
     @wraps(func)
     def wrapper(*args, token: HTTPAuthorizationCredentials = security, **kwargs):
-        if token.credentials != os.environ["AUTH_TOKEN"]:
+        if token.credentials != os.environ["ARCAN_API_KEY"]:
             raise HTTPException(
                 status_code=status.HTTP_401_UNAUTHORIZED,
                 detail="Incorrect bearer token",
                 headers={"WWW-Authenticate": "Bearer"},
             )
 
         return func(*args, **kwargs)
 
     return wrapper
 
 
 def aio_requires_auth(func):
     @wraps(func)
     async def wrapper(*args, token: HTTPAuthorizationCredentials = None, **kwargs):
-        if token is None or token.credentials != os.environ["AUTH_TOKEN"]:
+        if token is None or token.credentials != os.environ["ARCAN_API_KEY"]:
             raise HTTPException(
                 status_code=status.HTTP_401_UNAUTHORIZED,
                 detail="Incorrect bearer token",
                 headers={"WWW-Authenticate": "Bearer"},
             )
 
         return await func(*args, **kwargs)
```

### Comparing `arcan-0.0.1/pyproject.toml` & `arcan-0.1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "arcan"
-version = "0.0.1"
+version = "0.1.0"
 description = "An AI web3 tooling platform for the decentralized customization and enhancement of AI agents"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
-urllib3 = "^1.26.16"
+urllib3 = ">=1.26.16,<3.0.0"
 fastapi = "^0.110.0"
 openai = "^1.14.0"
-langchain = "^0.1.12"
+langchain = "^0.1.16"
 langchain-openai = "^0.0.8"
 uvicorn = "^0.28.0"
-pydantic = ">=2.5.3,<3.0.0"
+pydantic = "<2" #">=1.10.13,<3.0.0"
 python-dotenv = "^1.0.1"
 typing-extensions = "^4.9.0"
 pandas = "^2.2.1"
 sqlalchemy = "^2.0.27"
 psycopg2-binary = "^2.9.9"
 bs4 = "^0.0.2"
 selenium = "^4.18.1"
@@ -30,24 +30,33 @@
 twilio = "^9.0.0"
 python-decouple = "^3.8"
 python-multipart = "^0.0.9"
 pyngrok = "^7.1.3"
 numexpr = "^2.9.0"
 langchainhub = "^0.1.15"
 langchain-experimental = "^0.0.54"
-langchain-community = "^0.0.28"
-langchain-together = "^0.0.2.post1"
-langchain-fireworks = "^0.1.1"
-semantic-router = "^0.0.28"
-modal = "^0.61.53"
+langchain-community = "^0.0.32"
+# langchain-together = "^0.0.2.post1"
+# langchain-fireworks = "^0.1.1"
+# semantic-router = "^0.0.28"
+modal = "^0.61.54"
 typer = "^0.9.0"
+langserve = {extras = ["all"], version = ">=0.0.30"} #"^0.1.1"
+langchain-groq = "^0.1.3"
+firecrawl-py = "^0.0.8"
+passlib = {extras = ["bcrypt"], version = "^1.7.4"}
+python-jose = {extras = ["cryptography"], version = "^3.3.0"}
+supabase = "^2.4.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ipykernel = "^6.23.3"
+pytest = "^8.2.0"
+httpx = "^0.27.0"
+pytest-asyncio = "^0.23.6"
 
 [tool.poetry.scripts]
 arcan = 'arcan:cli'
```

### Comparing `arcan-0.0.1/PKG-INFO` & `arcan-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 Metadata-Version: 2.1
 Name: arcan
-Version: 0.0.1
+Version: 0.1.0
 Summary: An AI web3 tooling platform for the decentralized customization and enhancement of AI agents
 License: Apache 2.0
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: chromadb (>=0.4.24,<0.5.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
+Requires-Dist: firecrawl-py (>=0.0.8,<0.0.9)
 Requires-Dist: html2text (>=2024.2.26,<2025.0.0)
-Requires-Dist: langchain (>=0.1.12,<0.2.0)
-Requires-Dist: langchain-community (>=0.0.28,<0.0.29)
+Requires-Dist: langchain (>=0.1.16,<0.2.0)
+Requires-Dist: langchain-community (>=0.0.32,<0.0.33)
 Requires-Dist: langchain-experimental (>=0.0.54,<0.0.55)
-Requires-Dist: langchain-fireworks (>=0.1.1,<0.2.0)
+Requires-Dist: langchain-groq (>=0.1.3,<0.2.0)
 Requires-Dist: langchain-openai (>=0.0.8,<0.0.9)
-Requires-Dist: langchain-together (>=0.0.2.post1,<0.0.3)
 Requires-Dist: langchainhub (>=0.1.15,<0.2.0)
-Requires-Dist: modal (>=0.61.53,<0.62.0)
+Requires-Dist: langserve[all] (>=0.0.30)
+Requires-Dist: modal (>=0.61.54,<0.62.0)
 Requires-Dist: numexpr (>=2.9.0,<3.0.0)
 Requires-Dist: openai (>=1.14.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: passlib[bcrypt] (>=1.7.4,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
-Requires-Dist: pydantic (>=2.5.3,<3.0.0)
+Requires-Dist: pydantic (<2)
 Requires-Dist: pymupdf (>=1.23.25,<2.0.0)
 Requires-Dist: pyngrok (>=7.1.3,<8.0.0)
 Requires-Dist: python-decouple (>=3.8,<4.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
+Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
 Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
 Requires-Dist: selenium (>=4.18.1,<5.0.0)
-Requires-Dist: semantic-router (>=0.0.28,<0.0.29)
 Requires-Dist: sendgrid (>=6.11.0,<7.0.0)
 Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0)
+Requires-Dist: supabase (>=2.4.5,<3.0.0)
 Requires-Dist: twilio (>=9.0.0,<10.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
-Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
+Requires-Dist: urllib3 (>=1.26.16,<3.0.0)
 Requires-Dist: uvicorn (>=0.28.0,<0.29.0)
 Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Arcan
 
 ### AI web3 tooling platform for decentralized customization and enhancement of AI agents
@@ -59,34 +62,34 @@
 - **Blockchain-Backed AI Personalization**: Integrate AI agents with blockchain to create a personalized experience that respects user ownership.
 - **Web3 Tooling**: A suite of tools that enable seamless interaction between AI agents and blockchain assets.
 - **Privacy-Centric Design**: Ensuring user data is encrypted and owned by the user, accessible only through user permission.
 - **Developer-Friendly**: Straightforward APIs to enable developers to focus on building unique AI experiences.
 
 <p align="center">
   <a href="https://arcanai.tech">
-    <img src="public/logo_dark.png" height="200">
+    <img src="public/arcan_logo.svg" height="200">
     <h3 align="center"></h3>
   </a>
 </p>
 
 <p align="center">Unleash AI potential with Arcan — your gateway to blockchain-powered, personalized AI experiences. Code smart, own smarter. Visit the live demo at <a href="https://arcanai.tech/">arcanai.tech</a>.</p>
 
 <br/>
 
 ## Built With
 
-- [Next.js](https://nextjs.org/) - The web framework used
+<!-- - [Next.js](https://nextjs.org/) - The web framework used -->
 - [Python](https://www.python.org/) - Backend programming language
 - [Rust](https://www.rust-lang.org/) - Smart contract programming language
 
 ## Installation
 
 ### Prerequisites
 
-- [Next.js](https://nextjs.org/)
+<!-- - [Next.js](https://nextjs.org/) -->
 - [Python](https://www.python.org/)
 - [Rust](https://www.rust-lang.org/)
 - Access to a blockchain test network (e.g., Ethereum's or Solana's Testnet)
 
 ### Quick Install
 
     python -m pip install arcan
@@ -98,15 +101,15 @@
 
 ### Manual Build
 
     conda create -n arcan python=3.10
     conda activate arcan
     pip install -r requirements.txt
     python setup.py install
-
+<!-- 
 ## Building the Next.js App
 
 To clone the repository and create the Next.js app, you can use the following commands:
 
     npx create-next-app arcan --example "https://github.com/Broomva/arcan"
 
 Once you have cloned the repository and created the app, install the dependencies:
@@ -115,15 +118,15 @@
 
 After that, you can run the development server:
 
     yarn dev
     # or
     make rerun
 
-You can then view your application by opening [http://localhost:3000](http://localhost:3000) with your browser.
+You can then view your application by opening [http://localhost:3000](http://localhost:3000) with your browser. -->
 
 ## Contributing
 
 Please read [CONTRIBUTING.md](https://github.com/broomva/arcan/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
 ## Versioning
 
@@ -138,15 +141,15 @@
 ## Get Involved
 
 Interested in Arcan or looking to collaborate? Visit [broomva.tech](https://broomva.tech) for more information and to get in touch.
 
 ## License
 
 This project is licensed under the Apache 2.0 License - see the [LICENSE.md](LICENSE.md) file for details.
-
+<!-- 
 ## Subscription Model
 
 Arcan operates on a freemium/subscription model. While the open-source code can be deployed in your own environment free of charge, subscription tiers for access to premium features such as enhanced support and additional tools. Visit our [Pricing Page](https://arcanapp.io/pricing) for more details.
 
 ## Live Demo & Deployment
 
 Check out the live demo at [arcanapp.io](https://arcanapp.io/).
@@ -156,15 +159,15 @@
 [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FBroomva%2Farcan%2Ftree%2Fmain)
 
 ## Learn More
 
 To learn more about the technologies we use, check out:
 
 - [Next.js Documentation](https://nextjs.org/docs)
-- [FastAPI Documentation](https://fastapi.tiangolo.com/)
+- [FastAPI Documentation](https://fastapi.tiangolo.com/) -->
 
 <!-- ## Attribution
 
 Arcan builds upon the hard work of others. Here are the original repositories we leveraged:
 
 - [NextJS FastAPI Template](https://github.com/digitros/nextjs-fastapi)
```

#### html2text {}

```diff
@@ -1,84 +1,66 @@
-Metadata-Version: 2.1 Name: arcan Version: 0.0.1 Summary: An AI web3 tooling
+Metadata-Version: 2.1 Name: arcan Version: 0.1.0 Summary: An AI web3 tooling
 platform for the decentralized customization and enhancement of AI agents
 License: Apache 2.0 Author: Carlos D. Escobar-Valbuena Author-email:
 carlosdavidescobar@gmail.com Requires-Python: >=3.9,<3.13 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: bs4
 (>=0.0.2,<0.0.3) Requires-Dist: chromadb (>=0.4.24,<0.5.0) Requires-Dist:
-fastapi (>=0.110.0,<0.111.0) Requires-Dist: html2text (>=2024.2.26,<2025.0.0)
-Requires-Dist: langchain (>=0.1.12,<0.2.0) Requires-Dist: langchain-community
-(>=0.0.28,<0.0.29) Requires-Dist: langchain-experimental (>=0.0.54,<0.0.55)
-Requires-Dist: langchain-fireworks (>=0.1.1,<0.2.0) Requires-Dist: langchain-
-openai (>=0.0.8,<0.0.9) Requires-Dist: langchain-together
-(>=0.0.2.post1,<0.0.3) Requires-Dist: langchainhub (>=0.1.15,<0.2.0) Requires-
-Dist: modal (>=0.61.53,<0.62.0) Requires-Dist: numexpr (>=2.9.0,<3.0.0)
-Requires-Dist: openai (>=1.14.0,<2.0.0) Requires-Dist: pandas (>=2.2.1,<3.0.0)
-Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0) Requires-Dist: pydantic
-(>=2.5.3,<3.0.0) Requires-Dist: pymupdf (>=1.23.25,<2.0.0) Requires-Dist:
-pyngrok (>=7.1.3,<8.0.0) Requires-Dist: python-decouple (>=3.8,<4.0) Requires-
-Dist: python-dotenv (>=1.0.1,<2.0.0) Requires-Dist: python-multipart
-(>=0.0.9,<0.0.10) Requires-Dist: selenium (>=4.18.1,<5.0.0) Requires-Dist:
-semantic-router (>=0.0.28,<0.0.29) Requires-Dist: sendgrid (>=6.11.0,<7.0.0)
-Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0) Requires-Dist: twilio
-(>=9.0.0,<10.0.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Requires-Dist: typing-
-extensions (>=4.9.0,<5.0.0) Requires-Dist: urllib3 (>=1.26.16,<2.0.0) Requires-
-Dist: uvicorn (>=0.28.0,<0.29.0) Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
-Description-Content-Type: text/markdown # Arcan ### AI web3 tooling platform
-for decentralized customization and enhancement of AI agents Arcan is a web3
-tooling platform designed to customize and enhance AI agents by leveraging
-blockchain technology. With Arcan, developers can securely tie AI
-personalization to user-owned blockchain profiles, ensuring privacy and control
-while delivering tailored AI interactions. Check out the live demo at
-[arcanai.tech](https://arcanai.tech/). ## Features - **Blockchain-Backed AI
-Personalization**: Integrate AI agents with blockchain to create a personalized
-experience that respects user ownership. - **Web3 Tooling**: A suite of tools
-that enable seamless interaction between AI agents and blockchain assets. -
-**Privacy-Centric Design**: Ensuring user data is encrypted and owned by the
-user, accessible only through user permission. - **Developer-Friendly**:
-Straightforward APIs to enable developers to focus on building unique AI
-experiences.
-                            _[_p_u_b_l_i_c_/_l_o_g_o___d_a_r_k_._p_n_g_]
+fastapi (>=0.110.0,<0.111.0) Requires-Dist: firecrawl-py (>=0.0.8,<0.0.9)
+Requires-Dist: html2text (>=2024.2.26,<2025.0.0) Requires-Dist: langchain
+(>=0.1.16,<0.2.0) Requires-Dist: langchain-community (>=0.0.32,<0.0.33)
+Requires-Dist: langchain-experimental (>=0.0.54,<0.0.55) Requires-Dist:
+langchain-groq (>=0.1.3,<0.2.0) Requires-Dist: langchain-openai
+(>=0.0.8,<0.0.9) Requires-Dist: langchainhub (>=0.1.15,<0.2.0) Requires-Dist:
+langserve[all] (>=0.0.30) Requires-Dist: modal (>=0.61.54,<0.62.0) Requires-
+Dist: numexpr (>=2.9.0,<3.0.0) Requires-Dist: openai (>=1.14.0,<2.0.0)
+Requires-Dist: pandas (>=2.2.1,<3.0.0) Requires-Dist: passlib[bcrypt]
+(>=1.7.4,<2.0.0) Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0) Requires-Dist:
+pydantic (<2) Requires-Dist: pymupdf (>=1.23.25,<2.0.0) Requires-Dist: pyngrok
+(>=7.1.3,<8.0.0) Requires-Dist: python-decouple (>=3.8,<4.0) Requires-Dist:
+python-dotenv (>=1.0.1,<2.0.0) Requires-Dist: python-jose[cryptography]
+(>=3.3.0,<4.0.0) Requires-Dist: python-multipart (>=0.0.9,<0.0.10) Requires-
+Dist: selenium (>=4.18.1,<5.0.0) Requires-Dist: sendgrid (>=6.11.0,<7.0.0)
+Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0) Requires-Dist: supabase
+(>=2.4.5,<3.0.0) Requires-Dist: twilio (>=9.0.0,<10.0.0) Requires-Dist: typer
+(>=0.9.0,<0.10.0) Requires-Dist: typing-extensions (>=4.9.0,<5.0.0) Requires-
+Dist: urllib3 (>=1.26.16,<3.0.0) Requires-Dist: uvicorn (>=0.28.0,<0.29.0)
+Requires-Dist: wikipedia (>=1.4.0,<2.0.0) Description-Content-Type: text/
+markdown # Arcan ### AI web3 tooling platform for decentralized customization
+and enhancement of AI agents Arcan is a web3 tooling platform designed to
+customize and enhance AI agents by leveraging blockchain technology. With
+Arcan, developers can securely tie AI personalization to user-owned blockchain
+profiles, ensuring privacy and control while delivering tailored AI
+interactions. Check out the live demo at [arcanai.tech](https://arcanai.tech/).
+## Features - **Blockchain-Backed AI Personalization**: Integrate AI agents
+with blockchain to create a personalized experience that respects user
+ownership. - **Web3 Tooling**: A suite of tools that enable seamless
+interaction between AI agents and blockchain assets. - **Privacy-Centric
+Design**: Ensuring user data is encrypted and owned by the user, accessible
+only through user permission. - **Developer-Friendly**: Straightforward APIs to
+enable developers to focus on building unique AI experiences.
+                            _[_p_u_b_l_i_c_/_a_r_c_a_n___l_o_g_o_._s_v_g_]
     Unleash AI potential with Arcan â your gateway to blockchain-powered,
  personalized AI experiences. Code smart, own smarter. Visit the live demo at
                                  _a_r_c_a_n_a_i_._t_e_c_h.
 
-## Built With - [Next.js](https://nextjs.org/) - The web framework used -
-[Python](https://www.python.org/) - Backend programming language - [Rust]
-(https://www.rust-lang.org/) - Smart contract programming language ##
-Installation ### Prerequisites - [Next.js](https://nextjs.org/) - [Python]
-(https://www.python.org/) - [Rust](https://www.rust-lang.org/) - Access to a
-blockchain test network (e.g., Ethereum's or Solana's Testnet) ### Quick
-Install python -m pip install arcan ### Build from Source git clone https://
-github.com/Broomva/arcan.git cd arcan && make build ### Manual Build conda
-create -n arcan python=3.10 conda activate arcan pip install -
-r requirements.txt python setup.py install ## Building the Next.js App To clone
-the repository and create the Next.js app, you can use the following commands:
-npx create-next-app arcan --example "https://github.com/Broomva/arcan" Once you
-have cloned the repository and created the app, install the dependencies: yarn
-install After that, you can run the development server: yarn dev # or make
-rerun You can then view your application by opening [http://localhost:3000]
-(http://localhost:3000) with your browser. ## Contributing Please read
-[CONTRIBUTING.md](https://github.com/broomva/arcan/CONTRIBUTING.md) for details
-on our code of conduct, and the process for submitting pull requests to us. ##
-Versioning We use [SemVer](http://semver.org/) for versioning with release-
-please. For the versions available, see the [tags on this repository](https://
-github.com/broomva/arcan/tags). ## Authors - **Carlos D. Escobar-Valbuena** -
-[broomva](https://github.com/broomva) See also the list of [contributors]
-(https://github.com/broomva/arcan/contributors) who participated in this
-project. ## Get Involved Interested in Arcan or looking to collaborate? Visit
-[broomva.tech](https://broomva.tech) for more information and to get in touch.
-## License This project is licensed under the Apache 2.0 License - see the
-[LICENSE.md](LICENSE.md) file for details. ## Subscription Model Arcan operates
-on a freemium/subscription model. While the open-source code can be deployed in
-your own environment free of charge, subscription tiers for access to premium
-features such as enhanced support and additional tools. Visit our [Pricing
-Page](https://arcanapp.io/pricing) for more details. ## Live Demo & Deployment
-Check out the live demo at [arcanapp.io](https://arcanapp.io/). To deploy Arcan
-on your own, you can clone & deploy it with one click: [![Deploy with Vercel]
-(https://vercel.com/button)](https://vercel.com/new/clone?repository-
-url=https%3A%2F%2Fgithub.com%2FBroomva%2Farcan%2Ftree%2Fmain) ## Learn More To
-learn more about the technologies we use, check out: - [Next.js Documentation]
-(https://nextjs.org/docs) - [FastAPI Documentation](https://
-fastapi.tiangolo.com/)
+## Built With - [Python](https://www.python.org/) - Backend programming
+language - [Rust](https://www.rust-lang.org/) - Smart contract programming
+language ## Installation ### Prerequisites - [Python](https://www.python.org/
+) - [Rust](https://www.rust-lang.org/) - Access to a blockchain test network
+(e.g., Ethereum's or Solana's Testnet) ### Quick Install python -m pip install
+arcan ### Build from Source git clone https://github.com/Broomva/arcan.git cd
+arcan && make build ### Manual Build conda create -n arcan python=3.10 conda
+activate arcan pip install -r requirements.txt python setup.py install ##
+Contributing Please read [CONTRIBUTING.md](https://github.com/broomva/arcan/
+CONTRIBUTING.md) for details on our code of conduct, and the process for
+submitting pull requests to us. ## Versioning We use [SemVer](http://
+semver.org/) for versioning with release-please. For the versions available,
+see the [tags on this repository](https://github.com/broomva/arcan/tags). ##
+Authors - **Carlos D. Escobar-Valbuena** - [broomva](https://github.com/
+broomva) See also the list of [contributors](https://github.com/broomva/arcan/
+contributors) who participated in this project. ## Get Involved Interested in
+Arcan or looking to collaborate? Visit [broomva.tech](https://broomva.tech) for
+more information and to get in touch. ## License This project is licensed under
+the Apache 2.0 License - see the [LICENSE.md](LICENSE.md) file for details.
```

