# Comparing `tmp/codemeta-server-0.3.1.tar.gz` & `tmp/codemeta-server-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codemeta-server-0.3.1.tar", last modified: Thu Mar  2 14:25:28 2023, max compression
+gzip compressed data, was "codemeta-server-0.4.0.tar", last modified: Mon May 15 16:35:29 2023, max compression
```

## Comparing `codemeta-server-0.3.1.tar` & `codemeta-server-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 14:25:28.588590 codemeta-server-0.3.1/
--rw-r--r--   0 proycon   (1000) users      (100)    35147 2022-03-25 20:45:56.000000 codemeta-server-0.3.1/LICENSE
--rw-r--r--   0 proycon   (1000) users      (100)      996 2023-03-02 14:25:28.588590 codemeta-server-0.3.1/PKG-INFO
--rw-r--r--   0 proycon   (1000) users      (100)     3206 2023-03-02 12:39:39.000000 codemeta-server-0.3.1/README.md
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 14:25:28.588590 codemeta-server-0.3.1/codemeta_server/
--rw-r--r--   0 proycon   (1000) users      (100)        0 2022-03-25 12:57:53.000000 codemeta-server-0.3.1/codemeta_server/__init__.py
--rw-r--r--   0 proycon   (1000) users      (100)    23715 2023-03-02 13:14:27.000000 codemeta-server-0.3.1/codemeta_server/main.py
-drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-03-02 14:25:28.588590 codemeta-server-0.3.1/codemeta_server.egg-info/
--rw-r--r--   0 proycon   (1000) users      (100)      996 2023-03-02 14:25:28.000000 codemeta-server-0.3.1/codemeta_server.egg-info/PKG-INFO
--rw-r--r--   0 proycon   (1000) users      (100)      331 2023-03-02 14:25:28.000000 codemeta-server-0.3.1/codemeta_server.egg-info/SOURCES.txt
--rw-r--r--   0 proycon   (1000) users      (100)        1 2023-03-02 14:25:28.000000 codemeta-server-0.3.1/codemeta_server.egg-info/dependency_links.txt
--rw-r--r--   0 proycon   (1000) users      (100)       62 2023-03-02 14:25:28.000000 codemeta-server-0.3.1/codemeta_server.egg-info/entry_points.txt
--rw-r--r--   0 proycon   (1000) users      (100)       42 2023-03-02 14:25:28.000000 codemeta-server-0.3.1/codemeta_server.egg-info/requires.txt
--rw-r--r--   0 proycon   (1000) users      (100)       16 2023-03-02 14:25:28.000000 codemeta-server-0.3.1/codemeta_server.egg-info/top_level.txt
--rw-r--r--   0 proycon   (1000) users      (100)       44 2022-10-21 19:42:18.000000 codemeta-server-0.3.1/requirements.txt
--rw-r--r--   0 proycon   (1000) users      (100)       38 2023-03-02 14:25:28.588590 codemeta-server-0.3.1/setup.cfg
--rwxr-xr-x   0 proycon   (1000) users      (100)     1416 2023-03-02 09:14:58.000000 codemeta-server-0.3.1/setup.py
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-15 16:35:29.659861 codemeta-server-0.4.0/
+-rw-r--r--   0 proycon   (1000) users      (100)    35147 2022-03-25 20:45:56.000000 codemeta-server-0.4.0/LICENSE
+-rw-r--r--   0 proycon   (1000) users      (100)     1047 2023-05-15 16:35:29.659861 codemeta-server-0.4.0/PKG-INFO
+-rw-r--r--   0 proycon   (1000) users      (100)     4457 2023-05-15 13:28:06.000000 codemeta-server-0.4.0/README.md
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-15 16:35:29.659861 codemeta-server-0.4.0/codemeta_server/
+-rw-r--r--   0 proycon   (1000) users      (100)        0 2022-03-25 12:57:53.000000 codemeta-server-0.4.0/codemeta_server/__init__.py
+-rw-r--r--   0 proycon   (1000) users      (100)    26806 2023-05-15 15:57:35.000000 codemeta-server-0.4.0/codemeta_server/main.py
+drwxr-xr-x   0 proycon   (1000) users      (100)        0 2023-05-15 16:35:29.659861 codemeta-server-0.4.0/codemeta_server.egg-info/
+-rw-r--r--   0 proycon   (1000) users      (100)     1047 2023-05-15 16:35:29.000000 codemeta-server-0.4.0/codemeta_server.egg-info/PKG-INFO
+-rw-r--r--   0 proycon   (1000) users      (100)      331 2023-05-15 16:35:29.000000 codemeta-server-0.4.0/codemeta_server.egg-info/SOURCES.txt
+-rw-r--r--   0 proycon   (1000) users      (100)        1 2023-05-15 16:35:29.000000 codemeta-server-0.4.0/codemeta_server.egg-info/dependency_links.txt
+-rw-r--r--   0 proycon   (1000) users      (100)       62 2023-05-15 16:35:29.000000 codemeta-server-0.4.0/codemeta_server.egg-info/entry_points.txt
+-rw-r--r--   0 proycon   (1000) users      (100)       70 2023-05-15 16:35:29.000000 codemeta-server-0.4.0/codemeta_server.egg-info/requires.txt
+-rw-r--r--   0 proycon   (1000) users      (100)       16 2023-05-15 16:35:29.000000 codemeta-server-0.4.0/codemeta_server.egg-info/top_level.txt
+-rw-r--r--   0 proycon   (1000) users      (100)       76 2023-05-15 16:32:23.000000 codemeta-server-0.4.0/requirements.txt
+-rw-r--r--   0 proycon   (1000) users      (100)       38 2023-05-15 16:35:29.659861 codemeta-server-0.4.0/setup.cfg
+-rwxr-xr-x   0 proycon   (1000) users      (100)     1466 2023-05-10 09:42:42.000000 codemeta-server-0.4.0/setup.py
```

### Comparing `codemeta-server-0.3.1/LICENSE` & `codemeta-server-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codemeta-server-0.3.1/PKG-INFO` & `codemeta-server-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codemeta-server
-Version: 0.3.1
+Version: 0.4.0
 Summary: Web API serving codemeta software metadata using codemeta and schema.org, provides a SPARQL endpoint and also offers a human web-interface
 Home-page: https://github.com/proycon/codemeta-server
 Author: Maarten van Gompel
 Author-email: proycon@anaproy.nl
 License: GPL-3.0-only
 Project-URL: Issues, https://github.com/proycon/codemeta-server/issues
 Project-URL: Source Code, https://github.com/proycon/codemeta-server
@@ -12,9 +12,10 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7.0
 License-File: LICENSE
```

### Comparing `codemeta-server-0.3.1/codemeta_server/main.py` & `codemeta-server-0.4.0/codemeta_server/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import sys
 import os.path
 import json
 import traceback
 import glob
 import re
-from typing import Union, Optional
+from typing import Union, Optional, List
 from os import environ
 from collections import defaultdict
 from packaging.version import Version
 from rdflib_endpoint import SparqlEndpoint
 from rdflib import Graph, ConjunctiveGraph, URIRef, Literal
 from fastapi import FastAPI, Request, Response
 from fastapi.responses import JSONResponse
 from fastapi.staticfiles import StaticFiles
-from codemeta import __path__ as CODEMETAPATH
 from codemeta.codemeta import serialize
 from codemeta.validation import get_validation_report
 from codemeta.common import getstream, init_graph, AttribDict, SDO, RDF, CODEMETAPY, urijoin
 from codemeta.parsers.jsonld import parse_jsonld
+from codemeta2html import __path__ as CODEMETA2HTMLPATH
+from codemeta2html.html import serialize_to_html
 import argparse
 
-VERSION = "0.3.1" #also adapt in setup.py and codemeta.json
+VERSION = "0.4.0" #also adapt in setup.py and codemeta.json
 
-STATIC_DIR = os.path.join(CODEMETAPATH[0], "resources")
+STATIC_DIR = os.path.join(CODEMETA2HTMLPATH[0], "style")
 
 
 SPARQL_BINDS = """PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
 PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
 PREFIX schema: <http://schema.org/>
 PREFIX codemeta: <https://codemeta.github.io/terms/>
 PREFIX stype: <https://w3id.org/software-types#>
@@ -39,49 +40,52 @@
 PREFIX skos: <http://www.w3.org/2004/02/skos/core#>
 PREFIX dct: <http://purl.org/dc/terms/>
 PREFIX orcid: <http://orcid.org/>
 """
 
 NSPREFIXES = ('rdfs:', 'schema:','codemeta:','stype:','iodata:','repostatus:','trl:','nwo:','tadirah:','spdx:','skos:','dct:','orcid:')
     
-
 class CodemetaServer(FastAPI):
     def __init__(self, *args,
                  graph: str,
                  title: str = "Codemeta Server",
                  description: str = "Serves software metadata using codemeta and schema.org\n[Source code](https://github.com/proycon/codemeta-server/)",
-                 baseurl: str = "http://localhost:8080",
+                 baseurl: str = "http://localhost:8080/",
                  baseuri: str = "",
                  version: str = VERSION,
                  includecontext: bool = False,
                  addcontext: list = [],
+                 addcontextgraph: list = [],
                  **kwargs
                 ) -> None:
         """Constructor for the CodemetaServer"""
         self.baseurl = baseurl
         if baseuri:
             self.baseuri = baseuri
         else:
             self.baseuri = self.baseurl
 
         if self.baseuri[-1] not in ('/','#','?'):
             self.baseuri += "/"
+        if self.baseurl[-1] not in ('/','#','?'):
+            self.baseurl += "/"
 
         self.title = kwargs.get('title')
         if kwargs.get('css'):
             self.css = [ x.strip() for x in kwargs.get('css',"").split(",") if x.strip() ]
         else:
             self.css = []
 
         self.intro = kwargs.get('intro',"")
 
         print(f"Instantiating codemeta server: graph={graph}, baseuri={self.baseuri}, baseurl={self.baseurl}",file=sys.stderr)
 
         self.includecontext = includecontext
         self.addcontext = addcontext
+        self.addcontextgraph = addcontextgraph
         g, contextgraph = init_graph(self.get_args())
         parse_jsonld(g, None, getstream(graph), self.get_args())
         self.graph = g
         self.contextgraph = contextgraph
         if self.includecontext:
             self.graph += contextgraph #include context
         self.build_versionmap()
@@ -94,16 +98,38 @@
 
         #Instantiate sub API for SPARQL endpoint
         subapi = SparqlEndpoint(
             graph=self.graph,
             title="Codemeta Server SPARQL endpoint",
             description="A SPARQL endpoint to serve software metadata using codemeta and schema.org\n[Source code](https://github.com/proycon/codemeta-server/)",
             version=VERSION,
-            public_url=f"{self.baseurl}/api/sparql",
+            public_url=urijoin(self.baseurl,"api/"),
+            path="/",
             cors_enabled=True,
+            example_query="""PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
+PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
+PREFIX schema: <http://schema.org/>
+PREFIX codemeta: <https://codemeta.github.io/terms/>
+PREFIX softwaretypes: <https://w3id.org/software-types#>
+PREFIX softwareiodata: <https://w3id.org/software-iodata#>
+PREFIX trl: <https://w3id.org/research-technology-readiness-levels#>
+PREFIX repostatus: <https://www.repostatus.org/#>
+PREFIX nwo: <https://w3id.org/nwo-research-fields#>
+PREFIX tadirah: <https://vocabs.dariah.eu/tadirah/>
+PREFIX spdx: <http://spdx.org/licenses/>
+PREFIX skos: <http://www.w3.org/2004/02/skos/core#>
+
+SELECT ?name ?description ?repo ?status ?license WHERE {
+    ?sub schema:name ?name .
+    ?sub rdf:type schema:SoftwareSourceCode .
+    ?sub schema:license ?license .
+    ?sub codemeta:developmentStatus ?status .
+    ?sub schema:codeRepository ?repo .
+} LIMIT 25
+"""
         )
         self.mount("/api", subapi)
 
         #Serve static files
         self.mount("/static", StaticFiles(directory=STATIC_DIR))
 
         @self.get("/",
@@ -152,15 +178,15 @@
                               "application/json": {},
                               "text/turtle": {},
                           }
                       },
                   }
                 )
         async def table(request: Request, res: Optional[str] = None, q: Optional[str] = None, sparql: Optional[str] = None):
-            return self.get_index(request,res,q,sparql, "index.html")
+            return self.get_index(request,res,q,sparql, "tableindex.html")
 
         @self.get("/data.json",
                   name="Full data download (JSON-LD)",
                   description="Returns all data as JSON-LD",
                   responses= {
                       200: {
                           "description": "Full dump of the knowledge graph",
@@ -169,15 +195,15 @@
                               "application/json": {},
                           }
                       },
                   }
                 )
         async def data_json():
             return self.respond( "json",
-                                  serialize(self.graph, None, self.get_args("json"), contextgraph=self.contextgraph )
+                                 self.serialize(None, "json")
                                )
 
         @self.get("/data.ttl",
                   name="Full data download (Turtle)",
                   description="Returns all data as Turtle",
                   responses= {
                       200: {
@@ -186,15 +212,15 @@
                               "text/turtle": {},
                           }
                       },
                   }
                 )
         async def data_turtle():
             return self.respond( "turtle",
-                                  serialize(self.graph, None, self.get_args("turtle"), contextgraph=self.contextgraph )
+                                 self.serialize(None, "turtle")
                                )
 
         @self.get("/validation/{resource:path}",
                   name="Validation report",
                   description="Returns a specific validation log",
                   responses= {
                       200: {
@@ -225,68 +251,101 @@
                               "application/json+ld": {},
                               "application/json": {},
                               "text/turtle": {},
                           }
                       },
                   }
                  )
+        @self.get("/{resource:path}/",
+                  name="Resource",
+                  description="Returns the selected resource",
+                  responses= {
+                      200: {
+                          "description": "Visualisation of the resource (html) or the linked data of the resource (json-ld/turtle)",
+                          "content": {
+                              "text/html": {},
+                              "application/json+ld": {},
+                              "application/json": {},
+                              "text/turtle": {},
+                          }
+                      },
+                  }
+                 )
         async def get_resource(resource: str, request: Request):
-            if resource.endswith(".json"):
+            if resource.endswith("data.json"):
+                resource = resource[:-(len("data.json") + 1)]
+                output_type = "json"
+            elif resource.endswith("data.ttl"):
+                resource = resource[:-(len("data.ttl") + 1)]
+                output_type = "ttl"
+            elif resource.endswith(".json"):
                 resource = resource[:-5]
                 output_type = "json"
             elif resource.endswith(".ttl"):
                 resource = resource[:-4]
-                output_type = "turtle"
+                output_type = "ttl"
             else:
                 output_type = self.get_output_type(request)
             res = URIRef(urijoin(self.baseuri, resource))
             if (res,None,None) in self.graph:
                 return self.respond( output_type,
-                             serialize(self.graph, res, self.get_args(output_type), contextgraph=self.contextgraph, title=self.title )
+                             self.serialize(res, output_type)
                             )
             else:
                 #if the resource does not exist, a version qualifier may be missing, attempt to find the latest version
                 versions = self.versionmap.get(resource.strip("/"),[])
                 if versions:
                     res = URIRef(urijoin(self.baseuri, resource,versions[0])) #first version is the latest one
                     if (res,None,None) in self.graph:
                         return self.respond( output_type,
-                                     serialize(self.graph, res, self.get_args(output_type), contextgraph=self.contextgraph, title=self.title )
+                                     self.serialize(res, output_type)
                                     )
             return self.respond404(output_type)
 
 
+
+
+    def serialize(self, res: Union[Optional[URIRef],List[URIRef]], output_type: str, **kwargs) -> str:
+        if output_type == "html":
+             return serialize_to_html(self.graph, res, self.get_args(output_type), contextgraph=self.contextgraph, title=self.title, **kwargs )
+        else:
+             return serialize(self.graph, res, self.get_args(output_type), contextgraph=self.contextgraph, title=self.title, **kwargs )
+
+
     def get_index(self, request: Request, res: Optional[str] = None, q: Optional[str] = None, sparql: Optional[str] = None, indextemplate: str  = "cardindex.html"):
         output_type = self.get_output_type(request)
         if q:
             sparql = self.formulate_query(q)
         if res: res = [ URIRef(self.baseuri + x) for x in res.split(";") ]
         try:
-            response = serialize(self.graph, res, self.get_args(output_type), contextgraph=self.contextgraph, sparql_query=sparql, indextemplate=indextemplate, title=self.title, q=q if q else "")
+            response = self.serialize(res, output_type, sparql_query=sparql, indextemplate=indextemplate, q=q if q else "")
         except Exception as e:
             msg = str(e)
-            if sparql: msg += "<pre>SPARQL query was: f{sparql}\n</pre>"
+            if sparql: msg += f"<pre>SPARQL query was: {sparql}\n</pre>"
             exc_type, exc_value, exc_traceback = sys.exc_info()
             msg += "<pre>" + "\n".join(traceback.format_exception(exc_type, exc_value, exc_traceback)) + "</pre>"
             print(msg,file=sys.stderr)
             return self.respond400( output_type, msg)
         return self.respond( output_type, response)
 
     def get_args(self, output_type: str = "json") -> AttribDict:
         return AttribDict({
             "baseuri": self.baseuri,
             "baseurl": self.baseurl,
+            "styledir": "static",
             "graph": True,
             "output": output_type,
-            "toolstore": True,
-            "no_cache": True,
+            "buildsite": True,
+            "serverside": True,
+            "no_cache": False,
             "includecontext": self.includecontext,
             "addcontext": self.addcontext,
+            "addcontextgraph": self.addcontextgraph,
             "intro": self.intro,
-            "css": [ urijoin(self.baseurl,"static/codemeta.css") , urijoin(self.baseurl,"static/fontawesome.css") ] + self.css
+            "css": [ f"codemeta.css?v={VERSION}" , f"fontawesome.css?v={VERSION}" ] + self.css #cache busting
         })
 
     def respond(self, output_type: str, content: Union[str,bytes, None]) -> Response:
         if content is None: content = ""
         if output_type == 'json':
             return Response( content=content, media_type="application/json+ld")
         elif output_type == "turtle":
@@ -353,21 +412,31 @@
                 key, value = clause.split('=',1)
                 value = value.strip()
                 if value and value[0] == '=': #== operator for exact match
                     value = value[1:]
                     exact = True
                 else:
                     exact = False
-                if not (value.startswith(NSPREFIXES) or value.isnumeric()):
-                    value = f"\"{value}\"" #string literal
-                i = len(conditions) + 1
-                if exact:
-                    conditions.append(f"?res {key} {value} .")
+                if value.find('|') > 0:
+                    values = []
+                    for value in value.split('|'): #disjunction
+                        if not (value.startswith(NSPREFIXES) or value.isnumeric()):
+                            value = f"\"{value}\"" #string literal
+                        values.append(f"{value} .")
+                    if values:
+                        i = len(conditions) + 1
+                        conditions.append("{{ VALUES ?values{i} {{ " + ", ".join(values)  + f" }} ?res {key} ?values{i}.")
                 else:
-                    conditions.append(f"?res {key} ?v{i} FILTER regex(str(?v{i}), {value}, \"i\") .") #last i is for case-insensitive
+                    if not (value.startswith(NSPREFIXES) or value.isnumeric()):
+                        value = f"\"{value}\"" #string literal
+                    i = len(conditions) + 1
+                    if exact:
+                        conditions.append(f"?res {key} {value} .")
+                    else:
+                        conditions.append(f"?res {key} ?v{i} FILTER regex(str(?v{i}), {value}, \"i\") .") #last i is for case-insensitive
             else:
                 value = clause.strip()
                 i = len(conditions) + 1
                 #broad search on names, descriptions and keywords
                 conditions.append(f"{{ ?res schema:name ?v{i}a FILTER regex(str(?v{i}a), \"{value}\", \"i\") . }} UNION {{ ?res schema:description ?v{i}b FILTER regex(str(?v{i}b), \"{value}\", \"i\") . }} UNION {{ ?res schema:keywords ?v{i}c FILTER regex(str(?v{i}c), \"{value}\", \"i\") . }}")
 
         conditions = "\n".join(conditions)
@@ -463,29 +532,33 @@
         if 'CODEMETA_CSS' in environ:
             kwargs['css'] = environ['CODEMETA_CSS']
 
     if not kwargs.get('addcontext'):
         if 'CODEMETA_ADDCONTEXT' in environ:
             kwargs['addcontext'] = environ['CODEMETA_ADDCONTEXT'].split(" ")
 
+    if not kwargs.get('addcontextgraph'):
+        if 'CODEMETA_ADDCONTEXTGRAPH' in environ:
+            kwargs['addcontextgraph'] = environ['CODEMETA_ADDCONTEXTGRAPH'].split(" ")
+
     if not kwargs.get('includecontext'):
         if 'CODEMETA_INCLUDECONTEXT' in environ:
             kwargs['includecontext'] = environ['CODEMETA_INCLUDECONTEXT'].lower() in ("true","yes","1")
 
     return CodemetaServer(**kwargs)
 
 
 def main():
     import uvicorn
     parser = argparse.ArgumentParser(description="Codemeta Server", formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument('--host',type=str, help="Host to serve on", action='store', default="0.0.0.0")
     parser.add_argument('--port',type=int, help="Port to serve on", action='store', default=8080)
     parser.add_argument('--graph',type=str, help="JSON-LD graph to load (as produced by codemetapy --graph)", action='store', required=True)
     parser.add_argument('--baseuri',type=str, help="Base URI used in the IDs of all resources", action='store', required=True)
-    parser.add_argument('--baseurl',type=str, help="Base URL (only needed when distinct from base URI)", action='store')
+    parser.add_argument('--baseurl',type=str, help="Base URL", action='store')
     parser.add_argument('--inputlogdir',type=str, help="Directory where *.harvest.log can be found as generated by codemeta-harvester", action='store')
     parser.add_argument('--addcontext', help="Add the specified jsonld (must be a URL) to the context (and to the context graph). May be specified multiple times.", action='append',required=False)
     parser.add_argument('--includecontext', help="Include all context vocabularies in the main graph and express it verbosely in serialisations. This makes the resoluting codemeta.json richer without the need to query certain external vocabularies, at the cost of added redundancy.", action='store_true',required=False)
     parser.add_argument('--intro', type=str, help="Introductory text (html) to add to indices", action='store',required=False)
     parser.add_argument('--title',type=str, help="Title", action='store')
     parser.add_argument('--css',type=str, help="URLs to extra CSS stylesheets to use (comma separated list)", action='store')
     args = parser.parse_args() #parsed arguments can be accessed as attributes
```

### Comparing `codemeta-server-0.3.1/codemeta_server.egg-info/PKG-INFO` & `codemeta-server-0.4.0/codemeta_server.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codemeta-server
-Version: 0.3.1
+Version: 0.4.0
 Summary: Web API serving codemeta software metadata using codemeta and schema.org, provides a SPARQL endpoint and also offers a human web-interface
 Home-page: https://github.com/proycon/codemeta-server
 Author: Maarten van Gompel
 Author-email: proycon@anaproy.nl
 License: GPL-3.0-only
 Project-URL: Issues, https://github.com/proycon/codemeta-server/issues
 Project-URL: Source Code, https://github.com/proycon/codemeta-server
@@ -12,9 +12,10 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7.0
 License-File: LICENSE
```

### Comparing `codemeta-server-0.3.1/setup.py` & `codemeta-server-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(
-    version='0.3.1', #also adapt in main.py anmd codemeta.json
+    version='0.4.0', #also adapt in main.py anmd codemeta.json
     name='codemeta-server',
     license='GPL-3.0-only',
     description='Web API serving codemeta software metadata using codemeta and schema.org, provides a SPARQL endpoint and also offers a human web-interface',
     author='Maarten van Gompel',
     author_email='proycon@anaproy.nl',
     url='https://github.com/proycon/codemeta-server',
     packages=find_packages(),
@@ -17,14 +17,15 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     project_urls={
         "Issues": "https://github.com/proycon/codemeta-server/issues",
         "Source Code": "https://github.com/proycon/codemeta-server",
         "Releases": "https://github.com/proycon/codemeta-server/releases"
     },
     entry_points={
```

