# Comparing `tmp/assistant-fulfillment-helper-1.0.5.tar.gz` & `tmp/assistant-fulfillment-helper-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assistant-fulfillment-helper-1.0.5.tar", last modified: Fri Apr 28 19:22:46 2023, max compression
+gzip compressed data, was "assistant-fulfillment-helper-1.0.6.tar", last modified: Mon May 15 13:21:59 2023, max compression
```

## Comparing `assistant-fulfillment-helper-1.0.5.tar` & `assistant-fulfillment-helper-1.0.6.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.858353 assistant-fulfillment-helper-1.0.5/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     1101 2023-04-19 19:03:45.000000 assistant-fulfillment-helper-1.0.5/LICENSE
--rw-rw-r--   0 alisson   (1000) alisson   (1000)    12826 2023-04-28 19:22:46.858353 assistant-fulfillment-helper-1.0.5/PKG-INFO
--rw-rw-r--   0 alisson   (1000) alisson   (1000)    10584 2023-04-28 18:57:58.000000 assistant-fulfillment-helper-1.0.5/README.md
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      186 2023-04-27 13:22:02.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/__init__.py
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/controllers/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     1097 2023-04-27 19:23:01.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/controllers/auth_controller.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     4725 2023-04-28 18:04:35.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/controllers/webhook_controller.py
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/data/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      815 2023-04-27 19:34:51.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/data/token_data.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     2930 2023-04-27 19:55:12.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/data/webhook_data.py
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/exceptions/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      376 2023-04-26 22:02:12.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/exceptions/__init__.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      392 2023-04-26 21:14:54.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/exceptions/duplicated_intent_node_exception.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      443 2023-04-26 21:41:14.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/exceptions/intent_callback_not_found_exception.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      421 2023-04-26 21:48:21.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/exceptions/intent_response_instance_exception.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      428 2023-04-26 21:41:29.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/exceptions/invalid_webhook_token_exception.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      379 2023-04-26 20:40:51.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/exceptions/webhook_not_found_exception.py
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/models/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      274 2023-04-28 18:03:40.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/models/intent_model.py
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/responses/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      384 2023-04-27 19:56:30.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/responses/fulfillment_helper_response.py
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.858353 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/server/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      187 2023-04-27 17:57:58.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/server/__init__.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      777 2023-04-27 20:04:17.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/server/fulfillment_server.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     1052 2023-04-27 20:08:21.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/server/routes.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     3289 2023-04-28 18:04:06.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/fulfillment_helper.py
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)    12826 2023-04-28 19:22:46.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/PKG-INFO
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     1465 2023-04-28 19:22:46.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 alisson   (1000) alisson   (1000)        1 2023-04-28 19:22:46.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      353 2023-04-28 19:22:46.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/requires.txt
--rw-rw-r--   0 alisson   (1000) alisson   (1000)       29 2023-04-28 19:22:46.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/top_level.txt
--rw-rw-r--   0 alisson   (1000) alisson   (1000)       38 2023-04-28 19:22:46.858353 assistant-fulfillment-helper-1.0.5/setup.cfg
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     1543 2023-04-28 19:21:30.000000 assistant-fulfillment-helper-1.0.5/setup.py
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.858353 assistant-fulfillment-helper-1.0.5/test/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     2261 2023-04-27 18:53:31.000000 assistant-fulfillment-helper-1.0.5/test/test_fulfillment_helper.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     1430 2023-04-19 19:03:45.000000 assistant-fulfillment-helper-1.0.5/test/test_fulfillment_helper_response.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)    10126 2023-04-28 18:09:38.000000 assistant-fulfillment-helper-1.0.5/test/test_webhook_request.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-05-15 13:21:59.466055 assistant-fulfillment-helper-1.0.6/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     1101 2023-04-19 19:03:45.000000 assistant-fulfillment-helper-1.0.6/LICENSE
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)    13202 2023-05-15 13:21:59.466055 assistant-fulfillment-helper-1.0.6/PKG-INFO
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)    10928 2023-05-09 13:59:23.000000 assistant-fulfillment-helper-1.0.6/README.md
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-05-15 13:21:59.462055 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      251 2023-05-09 14:24:33.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/__init__.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-05-15 13:21:59.462055 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-05-15 13:21:59.462055 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/controllers/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     1097 2023-04-27 19:23:01.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/controllers/auth_controller.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     4725 2023-05-09 15:20:08.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/controllers/webhook_controller.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-05-15 13:21:59.462055 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/data/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      815 2023-05-09 14:09:36.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/data/token_data.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     3076 2023-05-15 12:30:36.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/data/webhook_data.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-05-15 13:21:59.466055 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/exceptions/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      376 2023-04-26 22:02:12.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/exceptions/__init__.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      392 2023-04-26 21:14:54.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/exceptions/duplicated_intent_node_exception.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      443 2023-04-26 21:41:14.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/exceptions/intent_callback_not_found_exception.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      421 2023-04-26 21:48:21.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/exceptions/intent_response_instance_exception.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      428 2023-04-26 21:41:29.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/exceptions/invalid_webhook_token_exception.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      379 2023-04-26 20:40:51.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/exceptions/webhook_not_found_exception.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-05-15 13:21:59.466055 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/models/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      274 2023-04-28 18:03:40.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/models/intent_model.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-05-15 13:21:59.466055 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/responses/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      384 2023-04-27 19:56:30.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/responses/fulfillment_helper_response.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-05-15 13:21:59.466055 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/server/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      187 2023-04-27 17:57:58.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/server/__init__.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      817 2023-05-15 12:38:47.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/server/fulfillment_server.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     1037 2023-05-09 15:07:00.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/server/routes.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     3942 2023-05-15 12:25:04.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/fulfillment_helper.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     1857 2023-05-09 14:26:36.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/fulfillment_helper_context.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-05-15 13:21:59.462055 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper.egg-info/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)    13202 2023-05-15 13:21:59.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     1564 2023-05-15 13:21:59.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)        1 2023-05-15 13:21:59.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      353 2023-05-15 13:21:59.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper.egg-info/requires.txt
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)       29 2023-05-15 13:21:59.000000 assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper.egg-info/top_level.txt
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)       38 2023-05-15 13:21:59.466055 assistant-fulfillment-helper-1.0.6/setup.cfg
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     1543 2023-05-15 13:21:47.000000 assistant-fulfillment-helper-1.0.6/setup.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-05-15 13:21:59.466055 assistant-fulfillment-helper-1.0.6/test/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     2253 2023-05-09 15:27:27.000000 assistant-fulfillment-helper-1.0.6/test/test_fulfillment_helper.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     2273 2023-05-09 15:28:26.000000 assistant-fulfillment-helper-1.0.6/test/test_fulfillment_helper_context.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     1430 2023-04-19 19:03:45.000000 assistant-fulfillment-helper-1.0.6/test/test_fulfillment_helper_response.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)    10125 2023-05-09 14:02:31.000000 assistant-fulfillment-helper-1.0.6/test/test_webhook_request.py
```

### Comparing `assistant-fulfillment-helper-1.0.5/LICENSE` & `assistant-fulfillment-helper-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `assistant-fulfillment-helper-1.0.5/PKG-INFO` & `assistant-fulfillment-helper-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistant-fulfillment-helper
-Version: 1.0.5
+Version: 1.0.6
 Summary: Assistant Fulfillment Helper Server
 Home-page: https://github.com/totvslabs/assistant-fulfillment-helper
 Author: TotvsLabs
 Author-email: info@totvslabs.com
 License: UNKNOWN
 Description: # Assistant Fulfillment Helper
         Esta biblioteta tem como objetivo facilitar a criação de *webhooks* para os nós de intenção da [Assistente TOTVS](https://produtos.totvs.com/ficha-tecnica/tudo-sobre-o-totvs-carol-assistente/). Com poucas linhas de código, é possivel criar uma regra de negócio customizada em sua própria estrutura de servidor.
@@ -55,14 +55,15 @@
         
         **Parâmetros:**
         | Parâmetro | Obrigatório? | Tipo | Descrição | 
         |-----------|--------------|------|-----------|
         | ``webhook`` | Sim | ``Str`` | Path do webhook, para o qual a Assistant requisitará nesse nó |
         | ``token`` | Sim | ``Str`` | Token disponibilizado pela Assistente na configuração do Nó de Intenção |
         | ``node`` | Sim | ``Str`` | Nome do Nó de Intenção cadastrado na Assistente |
+        | ``fallback_message`` | Não | ``Str`` | Mensagem padrão de retorno em caso de falha na execução do callback |
         
         ## Criando um callback
         Na chamada do callback, será passado uma variável do tipo ``Dict`` com alguns argumentos que poderão ser utilizados na regra de negócio como quiser. 
         Exemplo de um método para callback de um Nó de Intenção:
         ```python
         from assistant_fulfillment_helper import FulfillmentHelper, FulfillmentHelperResponse
         
@@ -116,61 +117,62 @@
             
             return FulfillmentHelperResponse(
                 message = message,
                 short_message = "Boas vindas",
                 jump_to = "Pedidos",
                 options = [
                     "Criar Pedido", 
-                    "Consultar Pedido"
+                    "Consultar Pedido",
                     "Cancelar Pedido"
                 ],
                 logout = False,
                 parameters = { 'onboarding' : True }
             )
         ```
         
         ### Falha do Callback 
-        Se por algum motivo houver uma excessão na execução do callback, o servidor responderá uma mensagem de fallback padrão para a assentente ("Desculpe, não consegui processar seu pedido no momento."). Essa mensagem pode ser alteradas na definição da intenção. 
+        Se por algum motivo houver uma excessão na execução do callback, o servidor responderá uma mensagem de fallback padrão para a assistente ("Desculpe, não consegui processar seu pedido no momento."). Essa mensagem pode ser alterada na definição da intenção. 
         
         Por exemplo:
         ```python
         @fh.intent(webhook='login', node='Login', token='{token}', fallback_message='Estamos passando por alguns problemas.')
         def callback_login(params):
             resposta = 'lorem'*1/params # raises a TypeError Exception
             
             return FulfillmentHelperResponse(
                 message = resposta
             )
         ```
         
-        Na execução desse callback, a excessão TypeError será capturada pelo servidor o qual, por sua vez, retornará para o usuaŕio na Assistente a mensagem de fallback definida para esse callback e o detalhes do erro será disponibilizado no console do servidor. 
+        Na execução desse callback, a excessão `TypeError` será capturada pelo servidor. O qual, por sua vez, retornará para o usuário na Assistente a mensagem de fallback definida para esse callback e o detalhes do erro será disponibilizado no console do servidor. 
         
         ## Iniciando um servidor local
         Existem diferentes formas de executar o servidor webhook. A biblioteca disponibiliza o método ``start()`` para rodar o servidor diretamente pelo código e o método ``get_app_context()`` para poder executar externamente por outra biblioteca (ex: gunicorn) e executar testes.
         
         ### get_app_context()
-        O método ``get_app_context()`` retornará o contexto do servidor em uma variavel, o que é util para rodar testes e rodar a aplicação utilizando bibliotecas externas.
+        O método ``get_app_context()`` retornará o contexto do servidor em uma variável, o que é util para executar testes e rodar a aplicação utilizando bibliotecas externas e deixar pronto para receber requisições como um Webhook.
         
         Por exemplo:
         ```python
         fh = FulfillmentHelper()
         
         application = fh.get_app_context()
         ```
         
         Agora a aplicação pode ser executada com o comando:
         ```sh
         gunicorn my_app
         ```
         
-        > NOTA: nesse exemplo a variável ``application`` poderá ser acessada por bibliotecas de testes.
+        > NOTA: nesse exemplo a variável ``application`` poderá ser utilizada por bibliotecas de testes também.
         
         ### start()
-        O método ``start()`` é responsável por iniciar um servidor local e deixar pronto para receber requisições como um Webhook. O servidor local pode ser configurado passando algumas propriedades no momento da chamada. Por exemplo:
+        O método ``start()`` é responsável por iniciar um servidor e deixar pronto para receber requisições como um Webhook. Por esse método, o servidor pode ser configurado passando algumas propriedades no momento da chamada. 
         
+        Por exemplo:
         ```python
         fh = FulfillmentHelper()
         
         fh.start(
             debug = True
         )
         ```
@@ -181,15 +183,15 @@
         |-----------|--------------|------|---------|-----------|
         | ``debug`` | Não | ``Bool`` | ``False`` | O Debug ativo habilita verbosidade e reinicia o servidor em cada alteração de código |
         | ``host`` | Não | ``Str`` | ``0.0.0.0`` | Nome ou IP do host local |
         | ``port`` | Não | ``Int`` | ``5052`` | Porta do host local |
         
         
         ## Exceções 
-        Os possíveis erros são tratados pelas exceções do módulo. Aqui está a lista das exceções existentes:
+        Os possíveis erros são tratados pelas exceções da biblioteca. Aqui está a lista das exceções existentes:
         
         
         | Exceção | Problema | 
         |-----------|--------|
         | ``DuplicatedIntentNodeException()`` |  Foi tentado adicionar dois métodos de callback para o mesmo Nó de Intenção |
         | ``IntentCallbackNotFoundException()`` | O WebHook recebeu uma chamada para um Nó de Intenção indefinido |
         | ``IntentResponseInstanceException()`` | O Callback invocado não retornou a classe de resposta esperada (``FulfillmentHelperResponse()``) |
@@ -215,27 +217,29 @@
         
         fh = FulfillmentHelper()
         ...
         
         application = fh.get_app_context()
         ```
         
-        Ou simplesmente importar a "application" diretamente:
-        
+        2. Importando a `application` (contexto da aplicação) diretamente:
         ```python
         from assistant_fulfillment_helper import FulfillmentHelper, application
         
         fh = FulfillmentHelper()
         ...
         ```
         
         Agora é só iniciar o servidor com [Gunicorn](https://gunicorn.org/):
         ```
         gunicorn -w 4 main
         ```
         
+        > NOTA: `main` deve ser o nome do arquivo raíz da sua aplicação, o qual possui o contexto do app acessível (`application`).
+        
         ## Licença
         MIT (LICENSE)
+        
 Keywords: assistant fulfillment helper carol totvs carolina carolapp
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `assistant-fulfillment-helper-1.0.5/README.md` & `assistant-fulfillment-helper-1.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 **Parâmetros:**
 | Parâmetro | Obrigatório? | Tipo | Descrição | 
 |-----------|--------------|------|-----------|
 | ``webhook`` | Sim | ``Str`` | Path do webhook, para o qual a Assistant requisitará nesse nó |
 | ``token`` | Sim | ``Str`` | Token disponibilizado pela Assistente na configuração do Nó de Intenção |
 | ``node`` | Sim | ``Str`` | Nome do Nó de Intenção cadastrado na Assistente |
+| ``fallback_message`` | Não | ``Str`` | Mensagem padrão de retorno em caso de falha na execução do callback |
 
 ## Criando um callback
 Na chamada do callback, será passado uma variável do tipo ``Dict`` com alguns argumentos que poderão ser utilizados na regra de negócio como quiser. 
 Exemplo de um método para callback de um Nó de Intenção:
 ```python
 from assistant_fulfillment_helper import FulfillmentHelper, FulfillmentHelperResponse
 
@@ -108,61 +109,62 @@
     
     return FulfillmentHelperResponse(
         message = message,
         short_message = "Boas vindas",
         jump_to = "Pedidos",
         options = [
             "Criar Pedido", 
-            "Consultar Pedido"
+            "Consultar Pedido",
             "Cancelar Pedido"
         ],
         logout = False,
         parameters = { 'onboarding' : True }
     )
 ```
 
 ### Falha do Callback 
-Se por algum motivo houver uma excessão na execução do callback, o servidor responderá uma mensagem de fallback padrão para a assentente ("Desculpe, não consegui processar seu pedido no momento."). Essa mensagem pode ser alteradas na definição da intenção. 
+Se por algum motivo houver uma excessão na execução do callback, o servidor responderá uma mensagem de fallback padrão para a assistente ("Desculpe, não consegui processar seu pedido no momento."). Essa mensagem pode ser alterada na definição da intenção. 
 
 Por exemplo:
 ```python
 @fh.intent(webhook='login', node='Login', token='{token}', fallback_message='Estamos passando por alguns problemas.')
 def callback_login(params):
     resposta = 'lorem'*1/params # raises a TypeError Exception
     
     return FulfillmentHelperResponse(
         message = resposta
     )
 ```
 
-Na execução desse callback, a excessão TypeError será capturada pelo servidor o qual, por sua vez, retornará para o usuaŕio na Assistente a mensagem de fallback definida para esse callback e o detalhes do erro será disponibilizado no console do servidor. 
+Na execução desse callback, a excessão `TypeError` será capturada pelo servidor. O qual, por sua vez, retornará para o usuário na Assistente a mensagem de fallback definida para esse callback e o detalhes do erro será disponibilizado no console do servidor. 
 
 ## Iniciando um servidor local
 Existem diferentes formas de executar o servidor webhook. A biblioteca disponibiliza o método ``start()`` para rodar o servidor diretamente pelo código e o método ``get_app_context()`` para poder executar externamente por outra biblioteca (ex: gunicorn) e executar testes.
 
 ### get_app_context()
-O método ``get_app_context()`` retornará o contexto do servidor em uma variavel, o que é util para rodar testes e rodar a aplicação utilizando bibliotecas externas.
+O método ``get_app_context()`` retornará o contexto do servidor em uma variável, o que é util para executar testes e rodar a aplicação utilizando bibliotecas externas e deixar pronto para receber requisições como um Webhook.
 
 Por exemplo:
 ```python
 fh = FulfillmentHelper()
 
 application = fh.get_app_context()
 ```
 
 Agora a aplicação pode ser executada com o comando:
 ```sh
 gunicorn my_app
 ```
 
-> NOTA: nesse exemplo a variável ``application`` poderá ser acessada por bibliotecas de testes.
+> NOTA: nesse exemplo a variável ``application`` poderá ser utilizada por bibliotecas de testes também.
 
 ### start()
-O método ``start()`` é responsável por iniciar um servidor local e deixar pronto para receber requisições como um Webhook. O servidor local pode ser configurado passando algumas propriedades no momento da chamada. Por exemplo:
+O método ``start()`` é responsável por iniciar um servidor e deixar pronto para receber requisições como um Webhook. Por esse método, o servidor pode ser configurado passando algumas propriedades no momento da chamada. 
 
+Por exemplo:
 ```python
 fh = FulfillmentHelper()
 
 fh.start(
     debug = True
 )
 ```
@@ -173,15 +175,15 @@
 |-----------|--------------|------|---------|-----------|
 | ``debug`` | Não | ``Bool`` | ``False`` | O Debug ativo habilita verbosidade e reinicia o servidor em cada alteração de código |
 | ``host`` | Não | ``Str`` | ``0.0.0.0`` | Nome ou IP do host local |
 | ``port`` | Não | ``Int`` | ``5052`` | Porta do host local |
 
 
 ## Exceções 
-Os possíveis erros são tratados pelas exceções do módulo. Aqui está a lista das exceções existentes:
+Os possíveis erros são tratados pelas exceções da biblioteca. Aqui está a lista das exceções existentes:
 
 
 | Exceção | Problema | 
 |-----------|--------|
 | ``DuplicatedIntentNodeException()`` |  Foi tentado adicionar dois métodos de callback para o mesmo Nó de Intenção |
 | ``IntentCallbackNotFoundException()`` | O WebHook recebeu uma chamada para um Nó de Intenção indefinido |
 | ``IntentResponseInstanceException()`` | O Callback invocado não retornou a classe de resposta esperada (``FulfillmentHelperResponse()``) |
@@ -207,23 +209,24 @@
 
 fh = FulfillmentHelper()
 ...
 
 application = fh.get_app_context()
 ```
 
-Ou simplesmente importar a "application" diretamente:
-
+2. Importando a `application` (contexto da aplicação) diretamente:
 ```python
 from assistant_fulfillment_helper import FulfillmentHelper, application
 
 fh = FulfillmentHelper()
 ...
 ```
 
 Agora é só iniciar o servidor com [Gunicorn](https://gunicorn.org/):
 ```
 gunicorn -w 4 main
 ```
 
+> NOTA: `main` deve ser o nome do arquivo raíz da sua aplicação, o qual possui o contexto do app acessível (`application`).
+
 ## Licença
-MIT (LICENSE)
+MIT (LICENSE)
```

### Comparing `assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/controllers/auth_controller.py` & `assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/controllers/auth_controller.py`

 * *Files identical despite different names*

### Comparing `assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/controllers/webhook_controller.py` & `assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/controllers/webhook_controller.py`

 * *Files identical despite different names*

### Comparing `assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/data/token_data.py` & `assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/data/token_data.py`

 * *Files identical despite different names*

### Comparing `assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/data/webhook_data.py` & `assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/data/webhook_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,37 +16,43 @@
 
         Returns:
             list(IntentModel) : List of intentions declared to the webhook
 
         Raises:
             WebhookNotFoundException: when the webhook is not found in the known webhook list
         """
+        if webhook == None:
+            webhook = ""
+            
         if webhook in WebhookData.__webhooks:
             return WebhookData.__webhooks.get(webhook)
         raise WebhookNotFoundException(webhook)
     
     @staticmethod
     def set_intent(webhook: str, intent: IntentModel):
         """ Set an intent definition ti a webhook
 
         Args:
             webhook (str) : Webhook path to receive the intent
             intent (IntentModel) : Intent to be added on the webhook context
         """
+        if webhook == None:
+            webhook = ""
+            
         if webhook not in WebhookData.__webhooks:
             WebhookData.__webhooks[webhook] = []
         WebhookData.__validate_webhook_intent(webhook, intent)
         WebhookData.__webhooks[webhook].append(intent)
 
     @staticmethod
     def load_intent(_webhook, intent_name, intent_token):
         """ Load an intent definition from a webhook context
 
         Args:
-            _webhook (str) : Webhook path to get the intent definition
+            _webhook (list(MultipleDict)) : Multiple dict of intentions in a Webhook
             intent_name (str) : Name of the intent to be loaded
             intent_token (str) : Token of the intent
 
         Returns:
             IntentModel : Intent definitions
 
         Raises:
```

### Comparing `assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/server/routes.py` & `assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/app/server/routes.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 @server_bp.route('/', methods=['POST'])
 @auth.validate_auth
 def default():
     """ Default route to handle deprecated Assistant request
     
     .. versionadded:: 0.0.1
     """
-    return WebhookController('fh_default_path').process_request()
+    return WebhookController('').process_request()
 
 
 @server_bp.route('/<webhook>', methods=['POST'])
 @auth.validate_auth
 def main(webhook):
     """ Default route to handle Assistant request
```

### Comparing `assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/fulfillment_helper.py` & `assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper/fulfillment_helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .app.server.fulfillment_server import FulfillmentServer
 from .app.models.intent_model import IntentModel
 from .app.data.webhook_data import WebhookData
 from .app.data.token_data import TokenData
+from .fulfillment_helper_context import FulfillmentHelperContext
 
 class FulfillmentHelper(FulfillmentServer):
     """Interface class to instance the module
     """
 
     def intent(self, webhook:str, token:str, node:str, fallback_message:str = None) -> any:
         """ @decorator_method
@@ -20,14 +21,15 @@
                     message="Hello, It's your webhook response"
                 )
 
         Args:
             webhook (str): The path for webhook server that will receive requests
             token (str): The webhook token provided by Assistant UI
             node (str): The name of node created on Asisstant
+            fallback_message (str): Fallback client message in case of callback error
         """
         def wrapper_intent(f):
             self.__register(
                 callback=f,
                 webhook_token=token,
                 node_name=node,
                 webhook_path=webhook,
@@ -49,26 +51,38 @@
             node_name (str): The name of node created on Asisstant
         """
         self.__register(
             callback=callback,
             webhook_token=webhook_token,
             node_name=node_name
         )
+        
+    def registerContext(self, Context: FulfillmentHelperContext):
+        for intent in Context.get_intents():
+            self.__register(
+                callback=intent.get('callback'),
+                webhook_token=intent.get('webhook_token'),
+                node_name=intent.get('node_name'),
+                webhook_path=intent.get('webhook_path'),
+                fallback_message=intent.get('fallback_message')
+            )
 
-    def __register(self, callback:callable, webhook_token:str, node_name:str, webhook_path:str = 'fh_default_path', fallback_message:str = None) -> None:
+    def __register(self, callback:callable, webhook_token:str, node_name:str, webhook_path:str = '', fallback_message:str = None) -> None:
         """ Privated method to storage the intents and webhooks from intent() and registerIntent()
 
         .. versionadded:: 1.0.5
 
         Args:
             callback (callable): Method to be called for requests in this intent 
             webhook (str): The path for webhook server that will receive requests
             node_name (str): The name of node created on Asisstant
             webhook_token (str): The webhook token provided by Assistant UI
         """
+        webhook_path = '' if webhook_path == None else webhook_path
+        
         intent = IntentModel(
             callback = callback,
             webhook_token = webhook_token,
             node_name = node_name,
             fallback_message = fallback_message
         )
         WebhookData.set_intent(webhook=webhook_path, intent=intent)
@@ -82,10 +96,7 @@
 
         Args:
             host (str): Host defined to the application
             port (int): Port defined to the application
             debug (bool): Run the webhook in debug mode
         """
         self.run(host, port, debug)
-
-
-
```

### Comparing `assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/PKG-INFO` & `assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistant-fulfillment-helper
-Version: 1.0.5
+Version: 1.0.6
 Summary: Assistant Fulfillment Helper Server
 Home-page: https://github.com/totvslabs/assistant-fulfillment-helper
 Author: TotvsLabs
 Author-email: info@totvslabs.com
 License: UNKNOWN
 Description: # Assistant Fulfillment Helper
         Esta biblioteta tem como objetivo facilitar a criação de *webhooks* para os nós de intenção da [Assistente TOTVS](https://produtos.totvs.com/ficha-tecnica/tudo-sobre-o-totvs-carol-assistente/). Com poucas linhas de código, é possivel criar uma regra de negócio customizada em sua própria estrutura de servidor.
@@ -55,14 +55,15 @@
         
         **Parâmetros:**
         | Parâmetro | Obrigatório? | Tipo | Descrição | 
         |-----------|--------------|------|-----------|
         | ``webhook`` | Sim | ``Str`` | Path do webhook, para o qual a Assistant requisitará nesse nó |
         | ``token`` | Sim | ``Str`` | Token disponibilizado pela Assistente na configuração do Nó de Intenção |
         | ``node`` | Sim | ``Str`` | Nome do Nó de Intenção cadastrado na Assistente |
+        | ``fallback_message`` | Não | ``Str`` | Mensagem padrão de retorno em caso de falha na execução do callback |
         
         ## Criando um callback
         Na chamada do callback, será passado uma variável do tipo ``Dict`` com alguns argumentos que poderão ser utilizados na regra de negócio como quiser. 
         Exemplo de um método para callback de um Nó de Intenção:
         ```python
         from assistant_fulfillment_helper import FulfillmentHelper, FulfillmentHelperResponse
         
@@ -116,61 +117,62 @@
             
             return FulfillmentHelperResponse(
                 message = message,
                 short_message = "Boas vindas",
                 jump_to = "Pedidos",
                 options = [
                     "Criar Pedido", 
-                    "Consultar Pedido"
+                    "Consultar Pedido",
                     "Cancelar Pedido"
                 ],
                 logout = False,
                 parameters = { 'onboarding' : True }
             )
         ```
         
         ### Falha do Callback 
-        Se por algum motivo houver uma excessão na execução do callback, o servidor responderá uma mensagem de fallback padrão para a assentente ("Desculpe, não consegui processar seu pedido no momento."). Essa mensagem pode ser alteradas na definição da intenção. 
+        Se por algum motivo houver uma excessão na execução do callback, o servidor responderá uma mensagem de fallback padrão para a assistente ("Desculpe, não consegui processar seu pedido no momento."). Essa mensagem pode ser alterada na definição da intenção. 
         
         Por exemplo:
         ```python
         @fh.intent(webhook='login', node='Login', token='{token}', fallback_message='Estamos passando por alguns problemas.')
         def callback_login(params):
             resposta = 'lorem'*1/params # raises a TypeError Exception
             
             return FulfillmentHelperResponse(
                 message = resposta
             )
         ```
         
-        Na execução desse callback, a excessão TypeError será capturada pelo servidor o qual, por sua vez, retornará para o usuaŕio na Assistente a mensagem de fallback definida para esse callback e o detalhes do erro será disponibilizado no console do servidor. 
+        Na execução desse callback, a excessão `TypeError` será capturada pelo servidor. O qual, por sua vez, retornará para o usuário na Assistente a mensagem de fallback definida para esse callback e o detalhes do erro será disponibilizado no console do servidor. 
         
         ## Iniciando um servidor local
         Existem diferentes formas de executar o servidor webhook. A biblioteca disponibiliza o método ``start()`` para rodar o servidor diretamente pelo código e o método ``get_app_context()`` para poder executar externamente por outra biblioteca (ex: gunicorn) e executar testes.
         
         ### get_app_context()
-        O método ``get_app_context()`` retornará o contexto do servidor em uma variavel, o que é util para rodar testes e rodar a aplicação utilizando bibliotecas externas.
+        O método ``get_app_context()`` retornará o contexto do servidor em uma variável, o que é util para executar testes e rodar a aplicação utilizando bibliotecas externas e deixar pronto para receber requisições como um Webhook.
         
         Por exemplo:
         ```python
         fh = FulfillmentHelper()
         
         application = fh.get_app_context()
         ```
         
         Agora a aplicação pode ser executada com o comando:
         ```sh
         gunicorn my_app
         ```
         
-        > NOTA: nesse exemplo a variável ``application`` poderá ser acessada por bibliotecas de testes.
+        > NOTA: nesse exemplo a variável ``application`` poderá ser utilizada por bibliotecas de testes também.
         
         ### start()
-        O método ``start()`` é responsável por iniciar um servidor local e deixar pronto para receber requisições como um Webhook. O servidor local pode ser configurado passando algumas propriedades no momento da chamada. Por exemplo:
+        O método ``start()`` é responsável por iniciar um servidor e deixar pronto para receber requisições como um Webhook. Por esse método, o servidor pode ser configurado passando algumas propriedades no momento da chamada. 
         
+        Por exemplo:
         ```python
         fh = FulfillmentHelper()
         
         fh.start(
             debug = True
         )
         ```
@@ -181,15 +183,15 @@
         |-----------|--------------|------|---------|-----------|
         | ``debug`` | Não | ``Bool`` | ``False`` | O Debug ativo habilita verbosidade e reinicia o servidor em cada alteração de código |
         | ``host`` | Não | ``Str`` | ``0.0.0.0`` | Nome ou IP do host local |
         | ``port`` | Não | ``Int`` | ``5052`` | Porta do host local |
         
         
         ## Exceções 
-        Os possíveis erros são tratados pelas exceções do módulo. Aqui está a lista das exceções existentes:
+        Os possíveis erros são tratados pelas exceções da biblioteca. Aqui está a lista das exceções existentes:
         
         
         | Exceção | Problema | 
         |-----------|--------|
         | ``DuplicatedIntentNodeException()`` |  Foi tentado adicionar dois métodos de callback para o mesmo Nó de Intenção |
         | ``IntentCallbackNotFoundException()`` | O WebHook recebeu uma chamada para um Nó de Intenção indefinido |
         | ``IntentResponseInstanceException()`` | O Callback invocado não retornou a classe de resposta esperada (``FulfillmentHelperResponse()``) |
@@ -215,27 +217,29 @@
         
         fh = FulfillmentHelper()
         ...
         
         application = fh.get_app_context()
         ```
         
-        Ou simplesmente importar a "application" diretamente:
-        
+        2. Importando a `application` (contexto da aplicação) diretamente:
         ```python
         from assistant_fulfillment_helper import FulfillmentHelper, application
         
         fh = FulfillmentHelper()
         ...
         ```
         
         Agora é só iniciar o servidor com [Gunicorn](https://gunicorn.org/):
         ```
         gunicorn -w 4 main
         ```
         
+        > NOTA: `main` deve ser o nome do arquivo raíz da sua aplicação, o qual possui o contexto do app acessível (`application`).
+        
         ## Licença
         MIT (LICENSE)
+        
 Keywords: assistant fulfillment helper carol totvs carolina carolapp
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/SOURCES.txt` & `assistant-fulfillment-helper-1.0.6/assistant_fulfillment_helper.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 assistant_fulfillment_helper/__init__.py
 assistant_fulfillment_helper/fulfillment_helper.py
+assistant_fulfillment_helper/fulfillment_helper_context.py
 assistant_fulfillment_helper.egg-info/PKG-INFO
 assistant_fulfillment_helper.egg-info/SOURCES.txt
 assistant_fulfillment_helper.egg-info/dependency_links.txt
 assistant_fulfillment_helper.egg-info/requires.txt
 assistant_fulfillment_helper.egg-info/top_level.txt
 assistant_fulfillment_helper/app/controllers/auth_controller.py
 assistant_fulfillment_helper/app/controllers/webhook_controller.py
@@ -20,9 +21,10 @@
 assistant_fulfillment_helper/app/exceptions/webhook_not_found_exception.py
 assistant_fulfillment_helper/app/models/intent_model.py
 assistant_fulfillment_helper/app/responses/fulfillment_helper_response.py
 assistant_fulfillment_helper/app/server/__init__.py
 assistant_fulfillment_helper/app/server/fulfillment_server.py
 assistant_fulfillment_helper/app/server/routes.py
 test/test_fulfillment_helper.py
+test/test_fulfillment_helper_context.py
 test/test_fulfillment_helper_response.py
 test/test_webhook_request.py
```

### Comparing `assistant-fulfillment-helper-1.0.5/setup.py` & `assistant-fulfillment-helper-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     'zope.event==4.6',
     'zope.interface==5.5.2'
 ]
 
 setup(
     name='assistant-fulfillment-helper',
     author="TotvsLabs",
-    version='1.0.5',
+    version='1.0.6',
     author_email='info@totvslabs.com',
     python_requires='>=3.7',
     description="Assistant Fulfillment Helper Server",
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requirements,
     include_package_data=True,
```

### Comparing `assistant-fulfillment-helper-1.0.5/test/test_fulfillment_helper.py` & `assistant-fulfillment-helper-1.0.6/test/test_fulfillment_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from assistant_fulfillment_helper.app.models.intent_model import IntentModel
 
 FulfillmentServer.run = MagicMock()
 
 class TestFulfillmentHelper:
 
     def test_recovery_intent(self):
-        node_name = 'test_define_new_intent'
+        node_name = 'test_recovery_intent'
         path_name = 'test_path'
 
         fh = FulfillmentHelper()
         @fh.intent(path_name, node=node_name, token=constants.FAKE_TOKEN)
         def callback_test(args:dict):
             return FulfillmentHelperResponse(
                 message=constants.FAKE_SUCCESS_MESSAGE
@@ -28,29 +28,29 @@
         ) == IntentModel(
             callback = callback_test,
             webhook_token = constants.FAKE_TOKEN,
             node_name = node_name
         )
 
     def test_recovery_intent_deprecated(self):
-        node_name = 'test_define_new_intent'
+        node_name = 'test_recovery_intent_deprecated'
         def callback_test(args:dict):
             return FulfillmentHelperResponse(
                 message=constants.FAKE_SUCCESS_MESSAGE
             )
         
         fh = FulfillmentHelper()
         fh.registerIntent(
             callback=callback_test,
             webhook_token=constants.FAKE_TOKEN,
             node_name=node_name
         )
     
         assert WebhookData.load_intent(
-            _webhook = WebhookData.get('fh_default_path'),
+            _webhook = WebhookData.get(''),
             intent_name=node_name,
             intent_token=constants.FAKE_TOKEN
         ) == IntentModel(
             callback = callback_test,
             webhook_token = constants.FAKE_TOKEN,
             node_name = node_name
         )
```

### Comparing `assistant-fulfillment-helper-1.0.5/test/test_fulfillment_helper_response.py` & `assistant-fulfillment-helper-1.0.6/test/test_fulfillment_helper_response.py`

 * *Files identical despite different names*

### Comparing `assistant-fulfillment-helper-1.0.5/test/test_webhook_request.py` & `assistant-fulfillment-helper-1.0.6/test/test_webhook_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import pytest
 from test.mocks import constants
 from assistant_fulfillment_helper.fulfillment_helper import FulfillmentHelper
 from assistant_fulfillment_helper.app.responses.fulfillment_helper_response import FulfillmentHelperResponse
 
 fh = FulfillmentHelper()
-
 class TestWebhookRequest:
 
     def test_health_check_success(self, client):
         response = client.get('/')
         assert response.json == dict(
             message = "This is a TOTVS Assistant Webhook Server. See https://pypi.org/project/assistant-fulfillment-helper/ for more details"
         )
```

