# Comparing `tmp/safraPyFunctions-2.2.6.tar.gz` & `tmp/safraPyFunctions-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/safraPyFunctions-2.2.6.tar", last modified: Thu Jan  5 17:43:43 2023, max compression
+gzip compressed data, was "dist/safraPyFunctions-3.0.0.tar", last modified: Mon May 15 14:15:48 2023, max compression
```

## Comparing `safraPyFunctions-2.2.6.tar` & `safraPyFunctions-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-01-05 17:43:43.000000 safraPyFunctions-2.2.6/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1384 2023-01-05 17:43:43.000000 safraPyFunctions-2.2.6/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      810 2023-01-05 10:44:36.000000 safraPyFunctions-2.2.6/README.md
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-01-05 17:43:43.000000 safraPyFunctions-2.2.6/safraPyFunctions/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        0 2023-01-04 15:24:42.000000 safraPyFunctions-2.2.6/safraPyFunctions/__init__.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)    57411 2023-01-05 10:52:26.000000 safraPyFunctions-2.2.6/safraPyFunctions/safraPyFunctions.py
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-01-05 17:43:43.000000 safraPyFunctions-2.2.6/safraPyFunctions.egg-info/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1384 2023-01-05 17:43:42.000000 safraPyFunctions-2.2.6/safraPyFunctions.egg-info/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      293 2023-01-05 17:43:43.000000 safraPyFunctions-2.2.6/safraPyFunctions.egg-info/SOURCES.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-01-05 17:43:43.000000 safraPyFunctions-2.2.6/safraPyFunctions.egg-info/dependency_links.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-01-05 17:43:43.000000 safraPyFunctions-2.2.6/safraPyFunctions.egg-info/requires.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       17 2023-01-05 17:43:43.000000 safraPyFunctions-2.2.6/safraPyFunctions.egg-info/top_level.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      106 2023-01-05 17:43:43.000000 safraPyFunctions-2.2.6/setup.cfg
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      587 2023-01-05 10:45:20.000000 safraPyFunctions-2.2.6/setup.py
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-05-15 14:15:48.000000 safraPyFunctions-3.0.0/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1384 2023-05-15 14:15:48.000000 safraPyFunctions-3.0.0/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      810 2023-01-05 10:44:36.000000 safraPyFunctions-3.0.0/README.md
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-05-15 14:15:47.000000 safraPyFunctions-3.0.0/safraPyFunctions/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        0 2023-01-04 15:24:42.000000 safraPyFunctions-3.0.0/safraPyFunctions/__init__.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)    56538 2023-05-15 14:15:35.000000 safraPyFunctions-3.0.0/safraPyFunctions/safraPyFunctions.py
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-05-15 14:15:48.000000 safraPyFunctions-3.0.0/safraPyFunctions.egg-info/
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-05-15 14:15:48.000000 safraPyFunctions-3.0.0/safraPyFunctions.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1384 2023-03-17 13:23:09.000000 safraPyFunctions-3.0.0/safraPyFunctions.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      293 2023-01-05 17:43:43.000000 safraPyFunctions-3.0.0/safraPyFunctions.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-01-05 17:43:43.000000 safraPyFunctions-3.0.0/safraPyFunctions.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-01-05 17:43:43.000000 safraPyFunctions-3.0.0/safraPyFunctions.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       17 2023-01-05 17:43:43.000000 safraPyFunctions-3.0.0/safraPyFunctions.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1384 2023-05-15 14:15:47.000000 safraPyFunctions-3.0.0/safraPyFunctions.egg-info/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      642 2023-05-15 14:15:47.000000 safraPyFunctions-3.0.0/safraPyFunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-05-15 14:15:47.000000 safraPyFunctions-3.0.0/safraPyFunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-05-15 14:15:47.000000 safraPyFunctions-3.0.0/safraPyFunctions.egg-info/requires.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       17 2023-05-15 14:15:47.000000 safraPyFunctions-3.0.0/safraPyFunctions.egg-info/top_level.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      106 2023-05-15 14:15:48.000000 safraPyFunctions-3.0.0/setup.cfg
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      587 2023-03-17 13:22:50.000000 safraPyFunctions-3.0.0/setup.py
```

### Comparing `safraPyFunctions-2.2.6/PKG-INFO` & `safraPyFunctions-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safraPyFunctions
-Version: 2.2.6
+Version: 3.0.0
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.safra.com.br/dados-migracao/safraPyFunctions
 Author: Carlos Piveta
 Author-email: carlos.piveta@safra.com.br
 License: MIT License
 Description: # safraPyFunctions
```

### Comparing `safraPyFunctions-2.2.6/README.md` & `safraPyFunctions-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `safraPyFunctions-2.2.6/safraPyFunctions/safraPyFunctions.py` & `safraPyFunctions-3.0.0/safraPyFunctions/safraPyFunctions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ =     "CARLOS PIVETA"
 __collaborators__ = "CARLOS PIVETA, LEONARDO BOTELHO, MATHEUS FELIX"
 __license__ =    "DADOS"
-__version__ =    "2.2.7"
+__version__ =    "3.0.0"
 __maintainer__ = "CARLOS PIVETA"
 __email__ =      "dados@safra.com.br"
 __status__ =     "Production"
 
 import os
 import re
 import sys
@@ -27,100 +27,45 @@
 warnings.filterwarnings("ignore")
 
 # -------------------------------------------------------------------------------------------------------------------------------
 # | CLASS CONN
 # -------------------------------------------------------------------------------------------------------------------------------
 class conn():   
     
-    """
-    import helpers.safraFunctions as sf
-    sc = sf.conn()
-    
-    A classe de funções uteis para trabalhar com os 
-    dados armazenados na cloudera
-    
-    Instances
-    -------
-    sandbox : str
-        Retorno da variavel de ambiente Sandbox
-    user : str
-        Usuário atual
-    passwd : str
-        Retorno da variavel de ambiente passwd (senha)
-    environment : str
-        Retorno da variavel de ambiente environment (ambiente)
-    
-    Methods
-    -------
-    spark = sc.getSpark([dPrint = False])
-        Função de conexão para consulta/execução de comandos SQL via Spark
-        
-    hive = sc.getHive([dPrint = False])
-        Função de conexão para consulta/execução de comandos SQL via Hive
-        
-    impala = sc.getImpala([dPrint = False])
-        Função de conexão para consulta/execução de comandos SQL via Impala
-        
-    tpConn = sc.getConn([dPrint =False])
-        Função que retorna a melhor conexão com base no ambiente que está sendo rodado
-        
-    dropSandbox(strTable = 'tabela',[dPrint =True])
-        Função para apagar uma tabela do sandbox
-        
-    [dtPartition] = getLastPartition(strSchema = 'abc',strTable ='tabela',[exportDataframe = True], [intLimit = 1000])
-        Função para pegar a ultima partição caso exista
-        
-    toSandBox(strSchema = 'abc',strTable = 'tabela',[ultimaParticao = False],[intLimit = 1000],[CampoDocumento = None],[tpDocumento = None])
-        Função para salvar uma tabela do ambiente produtivo no ambiente sandbox com id unico caso seja necessário
-    
-    df = readTable(strSchema = abc ,strTable = tabela, [bolSandbox = False])
-        Função para carregar uma tabela (sandbox ou corporativo) em um dataframe
-        
-    val = getResult(query = 'select max(valor) from tabela')
-        Função para trazer para uma variavel o valor de resultado de uma query
-        
-    saveSandbox(df = DFA,strTableName = 'nome da tabela')
-        Função salvar dataframe como tabela no sandbox
-        
-    DFA = setTmpView(df = DFA)
-        Função para criar uma tempview a partir de um dataframe
-        
-    DFA = setColumnsUp(df = DFA)
-        Função para transformar o nome de todas as tabelas de um dataframe Spark em Maiúscula
-        
-    DFA = setColumnsLow(df = DFA)
-        Função para transformar o nome de todas as tabelas de um dataframe Spark em Minúscula
-        
-    query = setQueryToSandbox(strQuery = strQ,listDbs = LISTADB,strAmbiente = 'DEV')
-        Função para transformar a query com origem no corporativo para o sandbox
-    """
-    
     def __init__(self,strEnv = None,strUser= None,strpassword= None,strSandbox = None):
         try:
-            self.sandbox = os.environ['WORKLOAD_SANDBOX']
             self.user  = os.environ['HADOOP_USER_NAME']
-            self.passwd = os.environ['WORKLOAD_PASSWORD']
-            
-            if strEnv == None:
-                self.environment = 'DEV'
+        except:
+            self.user  = 'PRD'
+        
+        if strEnv == None:
+            self.environment = 'DEV'
+        else:
+            self.environment = strEnv.upper()
+        
+        if strUser != None:
+            self.sandbox = strSandbox
+            self.user = strUser
+            self.passwd = strpassword
+        else:
+            if self.user  != 'PRD':
+                try:
+                    self.sandbox = os.environ['WORKLOAD_SANDBOX']
+                    self.passwd = os.environ['WORKLOAD_PASSWORD']
+                    self.environment = 'DEV'
+                except Exception as e:
+                    self.sandbox = None
+                    self.passwd = None
+                    self.environment = 'DEV'
+                    print('Criar variaveis de ambiente !!!!')
             else:
-                 self.environment = strEnv.upper()
-
-            if strUser != None:
-                self.sandbox = strSandbox
-                self.user = strUser
-                self.passwd = strpassword
-
-        except Exception as e:
-            self.sandbox = None
-            self.user  = None
-            self.passwd = None
-            self.environment = 'PROD'
-            print('Criar variaveis de ambiente !!!!')
-            
+                self.sandbox = None
+                self.passwd = None
+                self.environment = 'PROD'
+                
         #conexções
         self.spark = None
         self.impala = None
         self.hive = None
         self.tpConn = None
         
     def getSpark(self,dPrint = True, dist = False):
@@ -194,21 +139,35 @@
                 return self.spark
         else:
             self.tpConn = self.spark
             return self.spark
                 
     def getHive(self,dPrint = True):
         """
-        hive = sc.getHive([dPrint = False])
-        Função de conexão para consulta/execução de comandos SQL via Hive        
+        spark = s.getSpark([dPrint = False])
+        Função de conexão para consulta/execução de comandos SQL via Spark
+        
         Parameters
         ----------
         dPrint : bool (optional)
-            Define se será impresso a menssagem de retorno
-            
+            Define se será impresso a mensagem de retorno
+
+        Argumentos:
+        -----------
+        self: objeto
+            Objeto que chama a função.
+        dPrint : bool (opcional)
+            Define se a mensagem de retorno será impressa.
+        dist : bool (opcional)
+            Define se a sessão será distribuída ou local.
+
+        Retorna:
+        --------
+        spark : objeto
+            Sessão do Spark.
         """
         if self.hive == None:
             if self.spark == None:
                 self.getSpark()
                 
             try:
                 from pyspark_llap import HiveWarehouseSession
@@ -339,15 +298,15 @@
         """
         try:
             self.getImpala()
             impala = self.impala
             impala.execute(strQuery)
             df = as_pandas(impala)
             return df
-        except exception as e:
+        except Exception as e:
             print('ERRO!!! ')
             print(e) 
             
     def getLastPartition(self,strSchema,strTable,exportDataframe = False,intLimit = None):
         """
         [dtPartition] = getLastPartition(strSchema = 'abc',strTable ='tabela',[exportDataframe = True], [intLimit = 1000])
         Função para pegar a ultima partição caso exista 
@@ -408,16 +367,17 @@
             limitação de linhas de retorno
         CampoDocumento str(optional)
             Nome do campo com informação do numero de documento (cpf ou cnpj) para trazer as informações do id unico
         tpDocumento
             tipo do documento [Raiz ou Completo] a ser cruzado com a tabela pessoa.pessoa
         
         """
-        if self.tpConn == None:
-            self.getConn()
+        if self.impala == None:
+            if self.tpConn == None:
+                self.getConn()
             
         self.dropSandbox(strTable) 
         
         strLimit  = '' if intLimit == None else ' limit '+str(intLimit)
         
         try:
             if CampoDocumento == None:
@@ -472,14 +432,18 @@
         strSchema: str
             Nome do database aonde a tabela esta localizada
         strTable : str
             Nome da tabela a ser carregada
         bolSandbox bol (optional)
             marcação [True/False] se o retorno a base do ambiente produtivo [False] ou do Sandbox ['True']
         """
+        
+        if strSchema[:7].upper() == 'SANDBOX':
+            bolSandbox = True
+        
         if bolSandbox == True:
             self.getSpark()
         else:
             self.getConn()
             
         flagSandbox = True if self.environment != 'DEV' else bolSandbox
         schema = self.sandbox if flagSandbox == True else strSchema
@@ -494,15 +458,29 @@
             df = None
             print('ERRO! Tabela {} NÃO carragada !'.format(query))
             print(e)
             
         return df
         
         print(flagSandbox,schema)
-    
+        
+        
+    def execute(self,strQuery):
+        self.getConn()
+        conx = self.spark if [self.environment != 'DEV'] else self.hive
+        try:
+            df = conx.sql(strQuery)
+            print('querry {} executada !'.format(strQuery))
+        except Exception as e:
+            df = None
+            print('ERRO! querry {} NÃO executada !'.format(strQuery))
+            print(e)
+            
+        return df
+   
     def getResult(self,query):
         """
         val = getResult(query = 'select max(valor) from tabela')
         Função para trazer para uma variavel o valor de resultado de uma query
         Parameters
         ----------
         query : str
@@ -736,18 +714,18 @@
         else:
             print('Sem arquivos para serem carregados')
             
 # -------------------------------------------------------------------------------------------------------------------------------
 # | CLASS TOOLS
 # -------------------------------------------------------------------------------------------------------------------------------
 
-class tools():
+class tool():
     """
     import helpers.safraFunctions as sf
-    st = sf.tools()
+    st = sf.tool()
     
     A classe de funções uteis para trabalhar com python e dataframes 
     
     """
     def getToday(self) -> str:
         """
         getToday()
@@ -856,15 +834,15 @@
         exe = "pip install -i http://nexus-alm.safra.com.br/repository/pypi-repo/simple --trusted-host nexus-alm.safra.com.br "+strPacote
         os.system(exe)
     
     def fnCount(self,df,nmDF,dPrint=True):
         if(dPrint==True):
             print("{}:{}".format(nmDF,df.count()))
             
-    def zipFolder(self strPasta = './pastaorigem/' ,strSaida = './nomepasta/nomearquivodestino'):
+    def zipFolder(self,strPasta = './pastaorigem/' ,strSaida = './nomepasta/nomearquivodestino'):
         try:
             shutil.make_archive(strSaida, 'zip', strPasta)
         except Exception as e:
             print('ERRO! AO COMPACTAR A PASTA')
             print(e)
     
     def unzipFile(self,arquivo ="file.zip", pasta = 'targetdir'):
@@ -1076,14 +1054,15 @@
                     tables = list(set(tmptables))
                     tmpTxt = None     
                 #percorre todos as tabelas do script para pegar a ultima particao 
                 for tt in range(len(tables)):
                     try:
                         schema = tables[tt][1].lower().split('.')[0]
                         tabela = tables[tt][1].lower().split('.')[1]
+                        tabela = tabela.repalce(')','').repalce('(','').repalce('[','').repalce(']','')
                         hive_partition_pf = self.sc.getLastPartition(schema,tabela)
                         str_where_pf[tables[tt][1].lower().split('.')[1]] = "" + "'" + hive_partition_pf +"'"
                         if self.debugPrint == True : print(str_where_pf)
                     except Exception as e:  
                         continue
                 #percorre todas as datas informadas
                 
@@ -1185,15 +1164,15 @@
                                         strtable = tablenm.split('.')[-1].strip()
 
                                         if len(df.take(1)) > 0:
                                             if len(tablenm.split('.')) >= 2 :
                                                 if strtable[0:4] == 'TMP_':
                                                     df.createOrReplaceTempView(tablenm.upper().replace('.TMP_','_TMP_'))
                                                 else:
-                                                    df.write.format(self.strFormatoEscrita).mode(self.tipoEscrita).saveAsTable(tablenm)                                                                                        
+                                                    df.write.format('hive').mode(self.tipoEscrita).saveAsTable(tablenm)                                                                                        
     #                                         elif strtable[0:4] == 'TMP_':
     #                                             df.createOrReplaceTempView(tablenm)
     #                                         else:
     #                                             df.write.format('hive').mode(self.tipoEscrita).saveAsTable(self.db+tablenm)
     #                                         del df
                                 self._LoggingDB('STEP '+self.proc,table,'querie executada para a DATA REF '+ self.dtMesRef) 
                             except Exception as e:      
@@ -1222,8 +1201,15 @@
                                         queryf = queries.format(**str_where_pf)
                                         self._LoggingDB('QUERIE '+self.proc,table,queryf.replace('\n',' '))  
                                         self.sqlContext.executeUpdate(queryf.replace('\n',' '))
                                 self._LoggingDB('STEP '+self.proc,table,'querie executada para a DATA REF '+ self.dtMesRef) 
                             except Exception as e:
                                 exc_type, exc_obj, exc_tb = sys.exc_info()
                                 self._LoggingDB('ERRO NA LINHA '+str(exc_tb.tb_lineno)+' - '+self.proc,table,'Erro ao criar a base '+table+' '+str(e))
-                                print(e)
+                                print(e)
+                                
+                                
+# -------------------------------------------------------------------------------------------------------------------------------
+# | EASY IMPORTS
+# -------------------------------------------------------------------------------------------------------------------------------                                
+sqlConn =  conn()
+tools = tool()
```

### Comparing `safraPyFunctions-2.2.6/safraPyFunctions.egg-info/PKG-INFO` & `safraPyFunctions-3.0.0/safraPyFunctions.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safraPyFunctions
-Version: 2.2.6
+Version: 3.0.0
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.safra.com.br/dados-migracao/safraPyFunctions
 Author: Carlos Piveta
 Author-email: carlos.piveta@safra.com.br
 License: MIT License
 Description: # safraPyFunctions
```

### Comparing `safraPyFunctions-2.2.6/setup.py` & `safraPyFunctions-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(
     name='safraPyFunctions',
-    version='2.2.6',
+    version='3.0.0',
     url='https://gitlab.safra.com.br/dados-migracao/safraPyFunctions',
     license='MIT License',
     author='Carlos Piveta',
 	long_description=readme,
     long_description_content_type="text/markdown",
     author_email='carlos.piveta@safra.com.br',
     keywords='Pacote',
```

