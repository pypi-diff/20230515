# Comparing `tmp/archytas-0.2.4.tar.gz` & `tmp/archytas-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archytas-0.2.4.tar", max compression
+gzip compressed data, was "archytas-0.3.0.tar", max compression
```

## Comparing `archytas-0.2.4.tar` & `archytas-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    32472 2023-04-19 17:23:26.520856 archytas-0.2.4/LICENSE
--rw-r--r--   0        0        0     2577 2023-04-19 17:23:26.520856 archytas-0.2.4/README.md
--rw-r--r--   0        0        0        0 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/__init__.py
--rw-r--r--   0        0        0     3214 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/agent.py
--rw-r--r--   0        0        0      513 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/auth.py
--rw-r--r--   0        0        0     8997 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/demo_tools.py
--rw-r--r--   0        0        0     3583 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/prompt.py
--rw-r--r--   0        0        0     5866 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/react.py
--rw-r--r--   0        0        0     1055 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/repl.py
--rw-r--r--   0        0        0    17591 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/tool_utils.py
--rw-r--r--   0        0        0     1778 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/tools.py
--rw-r--r--   0        0        0      758 2023-04-19 17:23:26.524856 archytas-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3369 1970-01-01 00:00:00.000000 archytas-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    32472 2023-05-15 11:48:23.713528 archytas-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2088 2023-05-15 11:48:23.713528 archytas-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/__init__.py
+-rw-r--r--   0        0        0     8481 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/agent.py
+-rw-r--r--   0        0        0     9746 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/demo_tools.py
+-rw-r--r--   0        0        0     4129 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/prompt.py
+-rw-r--r--   0        0        0     3166 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/python.py
+-rw-r--r--   0        0        0     7500 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/react.py
+-rw-r--r--   0        0        0     1462 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/repl.py
+-rw-r--r--   0        0        0    18038 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/tool_utils.py
+-rw-r--r--   0        0        0     4586 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/tools.py
+-rw-r--r--   0        0        0     1251 2023-05-15 11:48:23.713528 archytas-0.3.0/archytas/utils.py
+-rw-r--r--   0        0        0      780 2023-05-15 11:48:23.749529 archytas-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 archytas-0.3.0/PKG-INFO
```

### Comparing `archytas-0.2.4/LICENSE` & `archytas-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `archytas-0.2.4/README.md` & `archytas-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -4,87 +4,59 @@
 Implementation of the [ReAct (Reason & Action)](https://arxiv.org/abs/2210.03629) framework for Large Language Model (LLM) agents. Mainly targeting OpenAI's GPT-4.
 
 Easily create tools from simple python functions or classes with the `@tool` decorator. A tools list can then be passed to the `ReActAgent` which will automagially generate a prompt for the LLM containing usage instructions for each tool, as well as manage the ReAct decision loop while the LLM performs its task.
 
 Tools can be anything from internet searches to custom interpreters for your domain. Archytas provides a few built-in demo tools e.g. datetime, fibonacci numbers, and a simple calculator.
 
 <div style="clear:left;"></div>
- 
-# Quicksart
+
+# Demo
+Short demo of using the `PythonTool` to download a COVID-19 dataset, and perform some basic processing/visualization/analysis/etc.
+<div align="center">
+  <a href="https://youtu.be/52e4xN8SIi8">
+    <img src="assets/covid_repl_demo.gif" alt="Watch the video">
+  </a>
+  <br/>
+  click to watch original video on youtube
+</div>
+
+# Quickstart
 ```bash
 # make sure poetry is installed
 pip install poetry
 
 # clone and install
 git clone git@github.com:jataware/archytas.git
 cd archytas
 poetry install
 
 # make sure OPENAI_API_KEY var is set
-# or set openai_key in .openai.toml
+# or pass it in as an argument to the agent
 export OPENAI_API_KEY="sk-..."
 
 # run demo
 poetry run chat-repl
 ```
 
 # Simple Usage
 Import pre-made tools from the tools module
 ```python
 from archytas.react import ReActAgent, FailedTaskError
-from archytas.tools import datetime_tool, fib_n, calculator
+from archytas.tools import PythonTool
 
 from easyrepl import REPL
 
 # create the agent with the tools list
-some_tools = [datetime_tool, fib_n, calculator]
-agent = ReActAgent(tools=some_tools+[mytool], verbose=True)
+some_tools = [PythonTool, ..., etc.]
+agent = ReActAgent(tools=some_tools, verbose=True)
 
 # REPL to interact with agent
 for query in REPL()
     try:
         answer = agent.react(query)
         print(answer)
     except FailedTaskError as e:
         print(f"Error: {e}")
 ```
 
-## Built-in Tools
-(TODO)
-- ask_user
-- datetime
-- timestamp
-- fib_n
-- calculator
-- ...
-
-# Custom Tools
-(TODO)
-```python
-from archytas.tools import tool
-
-@tool()
-def example_tool(arg1:int, arg2:str='', arg3:dict=None) -> int:
-    """
-    Simple 1 sentence description of the tool
-
-    More detailed description of the tool. This can be multiple lines.
-    Explain more what the tool does, and what it is used for.
-
-    Args:
-        arg1 (int): Description of the first argument.
-        arg2 (str): Description of the second argument. Defaults to ''.
-        arg3 (dict): Description of the third argument. Defaults to {}.
-
-    Returns:
-        int: Description of the return value
-
-    Examples:
-        >>> example_tool(1, 'hello', {'a': 1, 'b': 2})
-        3
-        >>> example_tool(2, 'world', {'a': 1, 'b': 2})
-        4
-    """
-    return 42
-
-# TODO: class tool example
-```
+# Documentation
+See the [wiki docs](https://github.com/jataware/archytas/wiki) for details.
```

### Comparing `archytas-0.2.4/archytas/demo_tools.py` & `archytas-0.3.0/archytas/demo_tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -171,74 +171,14 @@
 
         Returns:
             float: The value of pi
         """
         return math.pi
 
 
-
-# @tool()
-class StatefulToolExample:
-    def __init__(self, i:int, s:str):
-        self.i = i
-        self.s = s
-
-    # @tool()
-    def inc(self) -> int:
-        """
-        increment the internal counter
-
-        Returns:
-            int: The new value of the internal counter
-        """
-        self.i += 1
-        return self.i
-
-    # @tool()
-    def set_i(self, i:int):
-        """
-        set the internal counter
-
-        Args:
-            i (int): The new value of the internal counter
-        """
-        self.i = i
-
-    # @tool()
-    def set_s(self, s:str):
-        """
-        set the internal string
-
-        Args:
-            s (str): The new value of the internal string
-        """
-        self.s = s
-
-    # @tool()
-    def get_i(self) -> int:
-        """
-        get the internal counter
-        
-        Returns:
-            int: The value of the internal counter
-        """
-        return self.i
-    
-    # @tool()
-    def get_s(self) -> str:
-        """
-        get the internal string
-
-        Returns:
-            str: The value of the internal string
-        """
-
-        return self.s
-
-
 from random import random
 @toolset()
 class Jackpot:
     """
     A simple slot machine game
     
     Start with 100 chips, and make bets to try and win more chips.
@@ -352,12 +292,86 @@
             # Ensure the total population remains constant
             total_error = population - (S_new + I_new + R_new)
             R_new += total_error
 
         self.parameters['S'], self.parameters['I'], self.parameters['R'] = S_new, I_new, R_new
         return self.parameters
 
+    @tool()
     def reset_model(self):
         """
         Reset the model to the initial parameters
         """
-        self.parameters = self._default_parameters.copy()
+        self.parameters = self._default_parameters.copy()
+
+
+
+@tool()
+def ObservablePlot(code:str):
+    """
+    Create an observable plot in code.
+
+    Args:
+        code (str): The Observable Plot code
+
+    """
+
+
+
+@toolset()
+class PlannerTool:
+    """
+    A tool for helping to make long term plans. After a plan is made, the system will remind you of the plan as you execute each of the steps.
+    """
+    def __init__(self):
+        self.current_plan = None
+        self.progress = None
+
+    @tool()
+    def make_new_plan(self, draft:list[str]) -> None:
+        """
+        Start the plan making process.
+
+        This starts a conversation with the system to refine and revise a plan until it is robust and well thought out.
+
+        Args:
+            draft (list[str]): An initial list of steps to include in the plan. These can be revised later.
+        """
+        self.current_plan = draft
+        import pdb; pdb.set_trace()
+        ...
+
+    @tool()
+    def revise_single_step(self, i:int, replacement:str) -> None:
+        """
+        Revise a single step in the current plan
+
+        Args:
+            i (int): The index of the step to revise
+            replacement (str): The new step to replace the old step with
+        """
+        raise NotImplementedError('TODO')
+
+    # @tool()
+    # def revise_plan(self, updates:dict[int,str]) -> None: ...
+
+    # @tool()
+    # def finalize_plan():...
+
+
+from .tool_utils import AgentRef
+@tool()
+def pirate_subquery(query:str, agent:AgentRef) -> str:
+    """
+    Runs a subquery using a oneshot agent in which answers will be worded like a pirate.
+
+    Args:
+        query (str): The query to run against the agent.
+
+    Returns:
+        str: Result of the subquery in pirate vernacular.
+
+    """
+    prompt = """
+    You are an pirate. Answer all questions truthfully using pirate vernacular.
+    """
+    return agent.oneshot(prompt=prompt, query=query)
```

### Comparing `archytas-0.2.4/archytas/prompt.py` & `archytas-0.3.0/archytas/prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 from typing import Callable
 from archytas.tool_utils import get_tool_prompt_description, get_tool_names
 
 
-prelude = 'You are the ReAct (Reason & Action) assistant. You act as an interface between a user and the system. Your job is to help the user to complete their tasks.'
+def prelude() -> str:
+    return 'You are the ReAct (Reason & Action) assistant. You only communicate with properly formatted JSON objects of the form {"thought": "...", "tool": "...", "tool_input": "..."}. You DO NOT communicate with plain text. You act as an interface between a user and the system. Your job is to help the user to complete their tasks.'
 
-tool_intro = '# Tools\nYou have access to the following tools which can help you in your job:'
+def tool_intro() -> str:
+    return '# Tools\nYou have access to the following tools which can help you in your job:'
 
-system_tools = f"""
+def system_tools() -> str: 
+    return f"""
 final_answer:
     the final_answer tool is used to indicate that you have completed the task. You should use this tool to communicate the final answer to the user.
     _input_: the final answer to the user's task
 
 fail_task
     the fail_task tool is used to indicate that you have failed to complete the task. You should use this tool to communicate the reason for the failure to the user. Do not call this tool unless you have given a good effort to complete the task.
     _input_: the reason for the failure
 """.strip()
 
 
 #TODO: there should be some way to give an example relevant to the environment/tools...
 #      or use a system tool for the example
-def formatting(tool_names:list[str]) -> str:
+def formatting(tool_names:list[str], *, ask_user:bool) -> str:
     tool_names += ['final_answer', 'fail_task']
     tools_list = ', '.join(tool_names)
     return f"""
 # Formatting
 Every response you generate should EXACTLY follow this JSON format:
 
 {{
   "thought"    : # you should always think about what you need to do
   "tool"       : # the name of the tool. This must be one of: {{{tools_list}}}
   "tool_input" : # the input to the tool
 }}
 
-Do not include any text outside of this JSON object. The user will not be able to see it. You can communicate with the user through the "thought" field or the ask_user tool.
-The tool input must be a valid JSON blob (i.e. null, string, number, boolean, array, or object). The input type will depend on which tool you select, so make sure to follow the instructions for each tool.
+Do not include any text outside of this JSON object. The user will not be able to see it. You can communicate with the user through the "thought" field, {'the final_answer tool, or the ask_user tool' if ask_user else 'or the final_answer tool'}.
+The tool input must be a valid JSON value (i.e. null, string, number, boolean, array, or object). The input type will depend on which tool you select, so make sure to follow the instructions for each tool.
 
 For example, if the user asked you what the square-root of 2, you would use the calculator like so:
 {{
     "thought": "I need to use the calculator to find the square-root of 2.",
     "tool": "calculator",
     "tool_input": "2^0.5"
 }}
 """.strip()
 
-notes = f"""
+def notes(*, ask_user:bool) -> str:
+    return f"""
 # Notes
 - assume any time based knowledge you have is out of date, and should be looked up. Things like the current date, current world leaders, celebrities ages, etc.
 - You are not very good at arithmetic, so you should generally use tools to do arithmetic for you.
-- The user cannot see your thoughts. If you want to communicate to tell the user something, it should be via the ask_user or final_answer tools.
+- The user cannot see your thoughts. If you want to communicate something to the user, it should be via the {'ask_user or final_answer tools' if ask_user else 'final_answer tool'}.
 """.strip()
 
 
 def build_prompt(tools: list[Callable]) -> str:
     """
     Build the prompt for the ReAct agent
     
@@ -59,21 +63,24 @@
         tools (list): A list of tools to use. Each tool should have the @tool decorator. applied.
     
     Returns:
         str: The prompt for the ReAct agent
     """
     # collect all the tool names (including class.method names)
     tool_names = build_all_tool_names(tools)
+
+    # check if the ask user prompt is in the list of tools
+    ask_user = 'ask_user' in tool_names
     
-    chunks = [prelude, tool_intro]
+    chunks = [prelude(), tool_intro()]
     for tool in tools:
         chunks.append(get_tool_prompt_description(tool))
-    chunks.append(system_tools+'\n')
-    chunks.append(formatting(tool_names)+'\n')
-    chunks.append(notes)
+    chunks.append(system_tools()+'\n')
+    chunks.append(formatting(tool_names, ask_user=ask_user)+'\n')
+    chunks.append(notes(ask_user=ask_user))
     return '\n\n'.join(chunks)
 
         
 def build_all_tool_names(tools: list[Callable]) -> list[str]:
     """
     Build a list of tool names from a list of tools
```

### Comparing `archytas-0.2.4/archytas/repl.py` & `archytas-0.3.0/archytas/repl.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from archytas.react import ReActAgent, FailedTaskError
-from archytas.tools import datetime_tool, timestamp
-from archytas.demo_tools import fib_n, example_tool, calculator, Jackpot, ModelSimulation
+from archytas.tools import datetime_tool, timestamp, PythonTool
+from archytas.demo_tools import fib_n, example_tool, calculator, Jackpot, ModelSimulation, pirate_subquery
 
 from rich import traceback, print; traceback.install(show_locals=True)
 from easyrepl import REPL
 
 import pdb
 
 
 def start_repl():
     # make an instance of a class tool
     jackpot = Jackpot(chips=1000)
 
     # make a list of the tools to use
-    tools = [datetime_tool, timestamp, fib_n, example_tool, calculator, jackpot, ModelSimulation]
+    tools = [datetime_tool, timestamp, fib_n, example_tool, calculator, jackpot, ModelSimulation, PythonTool, pirate_subquery]
+
+    # # example of making a python tool with a prelude and some pre-initialized local variables
+    # import numpy as np
+    # python = PythonTool(
+    #     prelude='import numpy as np\nfrom matplotlib import pyplot as plt',
+    #     locals={'fib_n': fib_n, 'jackpot': jackpot, 'ModelSimulation': ModelSimulation},
+    # )
+    # tools = [python]
 
     # create the agent
     agent = ReActAgent(tools=tools, verbose=True)
 
     # print the agent's prompt
     # print(agent.prompt)
```

### Comparing `archytas-0.2.4/archytas/tool_utils.py` & `archytas-0.3.0/archytas/tool_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 import inspect
 from docstring_parser import parse as parse_docstring
 from rich import traceback; traceback.install(show_locals=True)
 from textwrap import indent
 from typing import Callable, Any
-import functools
+
 
 import pdb
 
 
 #TODO: separate system tools from library tools from user tools
 #      ideally system tools will have no library dependencies
 
 #TODO: parse extra long manual page from doc string. man_page can be seen by calling man <tool_name>
 # man_page:str|None=None
 # wrapper._man_page = man_page
 
 
+# Class/type definition for types used in dependency injection.
+AgentRef = type("AgentRef", (), {})
+ToolNameRef = type("ToolNameRef", (), {})
+ToolFnRef = type("ToolFnRef", (), {})
+LoopControllerRef = type("LoopControllerRef", (), {})
+
+INJECTION_MAPPING = {
+    AgentRef: "agent",
+    ToolNameRef: "tool_name",
+    ToolFnRef: "raw_tool",
+    LoopControllerRef: "loop_controller",
+}
+
+
 def tool(*, name:str|None=None):
     """
     Decorator to convert a function into a tool for ReAct agents to use.
 
     Usage:
     ```
         @tool()
@@ -42,20 +56,74 @@
             '''
     ```
     """
     def decorator(func:Callable):
         # check that the decorator is being applied to a function
         if not inspect.isfunction(func):
             raise TypeError(f"tool decorator can only be applied to functions or classes. Got {func} of type {type(func)}")
+
+        #attach usage description to the wrapper function
+        args_list, ret, desc, injections = get_tool_signature(func)
+
+        func._name = name if name else func.__name__
+        func._is_function_tool = True
+        func._args_list = args_list
+        func._ret = ret
+        func._desc = desc
+
+        def run(*args:tuple[object, dict|list|str|int|float|bool|None], tool_context:dict[str,object]=None):
+            """Output from LLM will be dumped into a json object. Depending on object type, call func accordingly."""
+
+            # The only time this will be a tuple is if more than one argument is passed in, which should only happen when this is an method and that is self.
+            if len(args) == 2 and getattr(args[0], "_is_class_tool", False):
+                self, args = args
+            else:
+                self = None
+                args = args[0]
+
+            if self is not None:
+                pargs = [self]
+            else:
+                pargs = []
+            kwargs = {}
+
+            #TODO: make this look at _call_type rather than isinstance to determine what to do
+            #      single argument functions that take a dict vs multi-argument functions will both have a dict, but they need to be called differently func(args) vs func(**args)
+            if args is None:
+                pass
+            elif len(args_list) == 1:
+                pargs.append(args)
+            elif isinstance(args, dict):
+                kwargs.update(args)
+            elif isinstance(args, list):
+                pargs.extend(args)
+            elif isinstance(args, (str, int, float, bool)):
+                pargs.append(args)
+            else:
+                raise TypeError(f"args must be a valid json object type (dict, list, str, int, float, bool, or None). Got {type(args)}")
+
+            # Add injections to kwargs
+            for inj_name, inj_type in injections.items():
+                context_key = INJECTION_MAPPING.get(inj_type, None)
+                context_value = tool_context.get(context_key, None)
+                if context_value:
+                    kwargs[inj_name] = context_value
+
+            result = func(*pargs, **kwargs)
+
+            #convert the result to a string if it is not already a string
+            if not isinstance(result, str):
+                result = str(result)
+
+            return result
+
+        # Add func as the attribute of the run method
+        func.run = run
         
-        # determine if function, or class method, and return the appropriate wrapper
-        if is_class_method(func):
-            return make_method_tool_wrapper(func, name)
-        else:
-            return make_func_tool_wrapper(func, name)
+        return func
 
     return decorator
 
 
 def toolset(*, name:str|None=None):
     """
     Decorator used to convert a class into a toolset for ReAct agents to use.
@@ -107,118 +175,54 @@
         #get the list of @tool methods in the class
         methods = inspect.getmembers(cls, predicate=inspect.isfunction)
         methods = [method for name, method in methods if is_tool(method)]
 
         # get the class docstring description
         docstring = inspect.getdoc(cls)
 
-        class wrapper:
-            def __init__(self, *args, **kwargs):
-                # create an instance of the class
-                self._instance = cls(*args, **kwargs)
-
-                # mark this as a class tool instance
-                self._is_class_tool_instance = True
-
+        # Somewhat complicated way of turning the run functions in to bound methods to the instance.
+        # Needs the instance to bind them, so wrap __new__ and bind right as they are created.
+        prev_new = cls.__new__
+        def new(cls, *args, **kwargs):
+            obj = prev_new(cls)
+            for method in methods:
+                bound_run_method = method.run.__get__(obj, cls)
+                method.run = bound_run_method
+            obj._is_class_tool_instance = True
+            return obj
+        cls.__new__ = new
 
         # attach the metadata to the class
-        wrapper._name = name if name else cls.__name__
-        wrapper._is_class_tool = True
-        wrapper._docstring = docstring
-        wrapper._tool_methods = methods
-        
-        return wrapper
-    
-    return decorator
-
-
-
-def make_func_tool_wrapper(func:Callable, name:str|None=None):
-    def wrapper(args:dict|list|str|int|float|bool|None):
-        """Output from LLM will be dumped into a json object. Depending on object type, call func accordingly."""
-        
-        #TODO: make this look at _call_type rather than isinstance to determine what to do
-        #      single argument functions that take a dict vs mutli-argument functions will both have a dict, but they need to be called differently func(args) vs func(**args)
-        if isinstance(args, dict):
-            result = func(**args)
-        elif isinstance(args, list):
-            result = func(*args)
-        elif isinstance(args, (str, int, float, bool)):
-            result = func(args)
-        elif args is None:
-            result = func()
-        else:
-            raise TypeError(f"args must be a valid json object type (dict, list, str, int, float, bool, or None). Got {type(args)}")
-
-        #convert the result to a string if it is not already a string
-        if not isinstance(result, str):
-            result = str(result)
-
-        return result
-    
-    #attach usage description to the wrapper function
-    args_list, ret, desc = get_tool_signature(func)
+        cls._name = name if name else cls.__name__
+        cls._is_class_tool = True
+        cls._docstring = docstring
+        cls._tool_methods = methods
 
-    wrapper._name = name if name else func.__name__
-    wrapper._is_function_tool = True
-    wrapper._args_list = args_list
-    wrapper._ret = ret
-    wrapper._desc = desc
-
-    return wrapper
-
-def make_method_tool_wrapper(func:Callable, name:str|None=None):
-    def wrapper(self, args:dict|list|str|int|float|bool|None):
-        """Output from LLM will be dumped into a json object. Depending on object type, call func accordingly."""
-        
-        if isinstance(args, dict):
-            result = func(self, **args)
-        elif isinstance(args, list):
-            result = func(self, *args)
-        elif isinstance(args, (str, int, float, bool)):
-            result = func(self, args)
-        elif args is None:
-            result = func(self)
-        else:
-            raise TypeError(f"args must be a valid json object type (dict, list, str, int, float, bool, or None). Got {type(args)}")
-
-        #convert the result to a string if it is not already a string
-        if not isinstance(result, str):
-            result = str(result)
-
-        return result
+        return cls
     
-    #attach usage description to the wrapper function
-    args_list, ret, desc = get_tool_signature(func)
-
-    wrapper._name = name if name else func.__name__
-    wrapper._is_method_tool = True
-    wrapper._args_list = args_list
-    wrapper._ret = ret
-    wrapper._desc = desc
-
-    return wrapper
-
+    return decorator
 
 
 def is_class_method(func:Callable) -> bool:
     """checks if a function is part of a class, or a standalone function"""
     assert inspect.isfunction(func), f"is_class_method can only be used on functions. Got {func}"
     return func.__qualname__ != func.__name__
 
+
 def is_tool(obj:Callable|type) -> bool:
-    """checks if an object is a tool function, tool method, or tool class (may not be an instance of a class tool)"""
+    """checks if an object is a tool function, tool method, tool class, or an instance of a class tool"""
     return hasattr(obj, '_is_function_tool') or hasattr(obj, '_is_method_tool') or hasattr(obj, '_is_class_tool') or hasattr(obj, '_is_class_tool_instance')
         
 
 def get_tool_name(obj:Callable|type) -> str:
     """Get the name of the tool, either from the @tool _name field, or the __name__ attribute"""
     assert is_tool(obj), f"get_tool_name can only be used on decorated @tools. Got {obj}"
     return getattr(obj, '_name')
 
+
 def get_tool_names(obj:Callable|type) -> list[str]:
     """
     Get the tool name, or all method names if tool is a class tool
     """
     assert is_tool(obj), f"get_tool_name can only be used on decorated @tools. Got {obj}"
     
     if hasattr(obj, '_is_class_tool') or hasattr(obj, '_is_class_tool_instance'):
@@ -229,23 +233,23 @@
 
         return names
     
     #otherwise, just return the name of the tool
     return [get_tool_name(obj)]
 
 
-
 def get_tool_prompt_description(obj:Callable|type|Any):
     if hasattr(obj, '_is_class_tool') or hasattr(obj, '_is_class_tool_instance'):
         return get_tool_class_prompt_description(obj)
     if hasattr(obj, '_is_function_tool') or hasattr(obj, '_is_method_tool'):
         return get_tool_func_prompt_description(obj)
 
     raise TypeError(f"get_tool_prompt_description can only be used on @tools. Got {obj}")
 
+
 def get_tool_func_prompt_description(func:Callable):
     assert is_tool(func), f"Function {func.__name__} does not have the @tool decorator attached"
     assert inspect.isfunction(func), f"get_tool_func_prompt_description can only be used on functions. Got {func}"
 
     #get the list of arguments
     
     args_list = func._args_list
@@ -265,22 +269,23 @@
     
     #################### INPUT ####################
     chunks.append('    _input_: ')
     
     if len(args_list) == 0:
         chunks.append("None")
     
-
-    elif len(args_list) == 1 and args_list[0][1] is not dict:
+    # 1-argument case for simple types don't need to be wrapped in a json
+    elif len(args_list) == 1 and args_list[0][1] in (str, int, float, bool):
         arg_name, arg_type, arg_desc, arg_default = args_list[0]
         chunks.append(f"({arg_type.__name__}")
         if arg_default:
             chunks.append(f", optional")
         chunks.append(f") {arg_desc}")
     
+    # all other cases have arguments wrapped in a json
     else:
         chunks.append("a json object with the following fields:\n    {")
         for arg_name, arg_type, arg_desc, arg_default in args_list:
             chunks.append(f'\n        "{arg_name}": # ({arg_type.__name__}')
             if arg_default:
                 chunks.append(f", optional")
             chunks.append(f") {arg_desc}")
@@ -342,74 +347,73 @@
 
 def get_tool_signature(func:Callable) -> tuple[list[tuple[str, type, str|None, str|None]], tuple[str|None, type|None, str|None], tuple[str, str|None, list[str]]]:
     """
     Check that the docstring and function signature match for a tool function, and return all function information.
 
     Args:
         func (function): The function to check and extract information from
-        ignore_self (bool): If True, ignore the first argument of the function if it is named 'self'
 
     Returns:
         args_list: A list of tuples (name, type, description, default) for each argument
         ret: A tuple (name, type, description) for the return value
         desc: A tuple (short_description, long_description, examples) from the docstring for the function
     """
     assert inspect.isfunction(func), f"get_tool_signature can only be used on functions. Got {func}"
 
     # get the function signature from the function and the docstring
     docstring = parse_docstring(func.__doc__)
     signature = inspect.signature(func)
 
-    # determine if self needs to be ignored
-    ignore_self: bool = is_class_method(func)
-
     # Extract argument information from the docstring
     docstring_args = {arg.arg_name: (arg.type_name, arg.description, arg.default) for arg in docstring.params}
 
     # Extract argument information from the signature (ignore self from class methods)
-    signature_args = {k: v.annotation for i, (k, v) in enumerate(signature.parameters.items()) if not (i == 0 and ignore_self and k == 'self')}
+    all_args = {k: v.annotation for i, (k, v) in enumerate(signature.parameters.items()) if not (i == 0 and k == 'self')}
+
+    # Extract argument information from the signature (ignore self from class methods)
+    injected_args = {k: v for k, v in all_args.items() if v in INJECTION_MAPPING}
+    signature_args = {k: v for k, v in all_args.items() if k not in injected_args}
 
     # Check if the docstring argument names match the signature argument names
     if set(docstring_args.keys()) != set(signature_args.keys()):
         raise ValueError(f"Docstring argument names do not match function signature argument names for function '{func.__name__}'")
 
     # Check if the docstring argument types match the signature argument types
     for arg_name, arg_type in signature_args.items():
         docstring_arg_type, _, _ = docstring_args[arg_name]
-        if arg_type.__name__ != docstring_arg_type:
+        if docstring_arg_type not in (arg_type.__name__ , str(arg_type)):
             raise ValueError(f"Docstring type '{docstring_arg_type}' does not match function signature type '{arg_type.__name__}' for argument '{arg_name}' for function '{func.__name__}'")
 
     # Generate a list of tuples (name, type, description, default) for each argument
     #TODO: use the signature to determine if an argument is optional or not
     args_list = [(arg_name, signature_args[arg_name], arg_desc, arg_default) for arg_name, (arg_type, arg_desc, arg_default) in docstring_args.items()]
 
-    # get the return type and description
+    # get the return type and description (and correctly set None to empty return type)
     signature_ret_type = signature.return_annotation
+    if signature_ret_type is None:
+        signature_ret_type = inspect.Signature.empty
 
-    # # if docstring.returns:
-    # if signature_ret_type == inspect.Signature.empty and docstring.returns is None:
-    #     ...
     try:
         docstring_ret_type = docstring.returns.type_name
     except AttributeError:
         docstring_ret_type = '_empty'
     if signature_ret_type.__name__ != docstring_ret_type:
         raise ValueError(f"Docstring return type '{docstring_ret_type}' does not match function signature return type '{signature_ret_type.__name__}' for function '{func.__name__}'")
-    
+
     # get the return type and description
     if docstring.returns is None:
         ret = (None, None, None)
     else:
         ret = (docstring.returns.return_name, signature_ret_type, docstring.returns.description)
 
     # get the docstring description and examples
     examples = [example.description for example in docstring.examples]
     desc = (docstring.short_description, docstring.long_description, examples)
     
-    return args_list, ret, desc
+    return args_list, ret, desc, injected_args
 
 
 
 def make_tool_dict(tools:list[Callable|type|Any]) -> dict[str, Callable]:
     """
     Create a dictionary of tools from a list of tool functions.
 
@@ -420,15 +424,15 @@
 
     Returns:
         dict[str, Callable]: A dictionary of tools. Class methods of class tools are included as separate functions.
     """
     #TODO: extract methods from any class tools
     tool_dict = {}
     for tool in tools:
-        assert is_tool(tool), f"make_tool_dict can only be used on tools. Got {tool}"
+        assert is_tool(tool), f"make_tool_dict can only be used on wrapped @tools/@toolsets. Got {tool}"
         name = getattr(tool, '_name')
         
         
         if hasattr(tool, '_is_function_tool'):
             if name in tool_dict:
                 raise ValueError(f"Tool name '{name}' is already in use")
             tool_dict[name] = tool
@@ -444,15 +448,15 @@
         assert hasattr(tool, '_is_class_tool'), f"Tool {tool} is not a function, method, or class tool"
         if hasattr(tool, '_is_class_tool_instance'):
             instance = tool
         else:
             instance = tool()
 
         # add each method to the tool dictionary under the name 'class_name.method_name'
-        methods = inspect.getmembers(instance._instance, predicate=inspect.ismethod)
+        methods = inspect.getmembers(instance, predicate=inspect.ismethod)
         for _, method in methods:
             if not hasattr(method, '_name'):
                 continue
             method_name = f'{name}.{method._name}'
             if method_name in tool_dict:
                 raise ValueError(f"Tool name '{method_name}' is already in use")
             tool_dict[method_name] = method
```

### Comparing `archytas-0.2.4/pyproject.toml` & `archytas-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archytas"
-version = "0.2.4"
+version = "0.3.0"
 description = "A library for pairing LLM agents with tools so they perform open ended tasks"
 authors = ["David Andrew Samson <david.andrew.engineer@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [project.urls]
 "Homepage" = "https://github.com/jataware/archytas"
@@ -17,14 +17,15 @@
 python = "^3.10"
 openai = "^0.27.4"
 tenacity = "^8.2.2"
 rich = "^13.3.4"
 docstring-parser = "^0.15"
 pytz = "^2023.3"
 toml = "^0.10.2"
+frozendict = "^2.3.8"
 
 [tool.poetry.group.dev.dependencies]
 easyrepl = "^0.1.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `archytas-0.2.4/PKG-INFO` & `archytas-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: archytas
-Version: 0.2.4
+Version: 0.3.0
 Summary: A library for pairing LLM agents with tools so they perform open ended tasks
 License: GPL-3.0-or-later
 Author: David Andrew Samson
 Author-email: david.andrew.engineer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docstring-parser (>=0.15,<0.16)
+Requires-Dist: frozendict (>=2.3.8,<3.0.0)
 Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
@@ -24,87 +25,60 @@
 Implementation of the [ReAct (Reason & Action)](https://arxiv.org/abs/2210.03629) framework for Large Language Model (LLM) agents. Mainly targeting OpenAI's GPT-4.
 
 Easily create tools from simple python functions or classes with the `@tool` decorator. A tools list can then be passed to the `ReActAgent` which will automagially generate a prompt for the LLM containing usage instructions for each tool, as well as manage the ReAct decision loop while the LLM performs its task.
 
 Tools can be anything from internet searches to custom interpreters for your domain. Archytas provides a few built-in demo tools e.g. datetime, fibonacci numbers, and a simple calculator.
 
 <div style="clear:left;"></div>
- 
-# Quicksart
+
+# Demo
+Short demo of using the `PythonTool` to download a COVID-19 dataset, and perform some basic processing/visualization/analysis/etc.
+<div align="center">
+  <a href="https://youtu.be/52e4xN8SIi8">
+    <img src="assets/covid_repl_demo.gif" alt="Watch the video">
+  </a>
+  <br/>
+  click to watch original video on youtube
+</div>
+
+# Quickstart
 ```bash
 # make sure poetry is installed
 pip install poetry
 
 # clone and install
 git clone git@github.com:jataware/archytas.git
 cd archytas
 poetry install
 
 # make sure OPENAI_API_KEY var is set
-# or set openai_key in .openai.toml
+# or pass it in as an argument to the agent
 export OPENAI_API_KEY="sk-..."
 
 # run demo
 poetry run chat-repl
 ```
 
 # Simple Usage
 Import pre-made tools from the tools module
 ```python
 from archytas.react import ReActAgent, FailedTaskError
-from archytas.tools import datetime_tool, fib_n, calculator
+from archytas.tools import PythonTool
 
 from easyrepl import REPL
 
 # create the agent with the tools list
-some_tools = [datetime_tool, fib_n, calculator]
-agent = ReActAgent(tools=some_tools+[mytool], verbose=True)
+some_tools = [PythonTool, ..., etc.]
+agent = ReActAgent(tools=some_tools, verbose=True)
 
 # REPL to interact with agent
 for query in REPL()
     try:
         answer = agent.react(query)
         print(answer)
     except FailedTaskError as e:
         print(f"Error: {e}")
 ```
 
-## Built-in Tools
-(TODO)
-- ask_user
-- datetime
-- timestamp
-- fib_n
-- calculator
-- ...
-
-# Custom Tools
-(TODO)
-```python
-from archytas.tools import tool
-
-@tool()
-def example_tool(arg1:int, arg2:str='', arg3:dict=None) -> int:
-    """
-    Simple 1 sentence description of the tool
-
-    More detailed description of the tool. This can be multiple lines.
-    Explain more what the tool does, and what it is used for.
-
-    Args:
-        arg1 (int): Description of the first argument.
-        arg2 (str): Description of the second argument. Defaults to ''.
-        arg3 (dict): Description of the third argument. Defaults to {}.
-
-    Returns:
-        int: Description of the return value
-
-    Examples:
-        >>> example_tool(1, 'hello', {'a': 1, 'b': 2})
-        3
-        >>> example_tool(2, 'world', {'a': 1, 'b': 2})
-        4
-    """
-    return 42
+# Documentation
+See the [wiki docs](https://github.com/jataware/archytas/wiki) for details.
 
-# TODO: class tool example
-```
```

