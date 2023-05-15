# Comparing `tmp/jupyterlab_language_pack_pt_br-3.6.post0.tar.gz` & `tmp/jupyterlab_language_pack_pt_br-3.6.post1.tar.gz`

## Comparing `jupyterlab_language_pack_pt_br-3.6.post0.tar` & `jupyterlab_language_pack_pt_br-3.6.post1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/.copier-answers.yml
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/CONTRIBUTORS.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/dask_labextension.po
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyter_archive.po
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyter_resource_usage.po
--rw-r--r--   0        0        0   192858 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab.po
--rw-r--r--   0        0        0    96287 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_git.po
--rw-r--r--   0        0        0    37177 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_lsp.po
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_search_replace.po
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_tour.po
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_widgets.po
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupytext.po
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/retrolab.po
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/spellchecker.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/LICENSE.txt
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/README.md
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/pyproject.toml
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post0/PKG-INFO
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/.copier-answers.yml
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/dask_labextension.po
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyter_archive.po
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyter_resource_usage.po
+-rw-r--r--   0        0        0   195399 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab.po
+-rw-r--r--   0        0        0    96287 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_git.po
+-rw-r--r--   0        0        0    42091 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_lsp.po
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_search_replace.po
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_tour.po
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_widgets.po
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupytext.po
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/retrolab.po
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/spellchecker.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/LICENSE.txt
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/README.md
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/pyproject.toml
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 jupyterlab_language_pack_pt_br-3.6.post1/PKG-INFO
```

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/CONTRIBUTORS.md` & `jupyterlab_language_pack_pt_br-3.6.post1/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/dask_labextension.po` & `jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/dask_labextension.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyter_archive.po` & `jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyter_archive.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab.po` & `jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: pt-BR\n"
 "X-Crowdin-File: /main/jupyterlab/locale/jupyterlab.pot\n"
 "X-Crowdin-File-ID: 191\n"
 "Language-Team: Portuguese, Brazilian\n"
 "Language: pt_BR\n"
-"PO-Revision-Date: 2023-02-07 18:30\n"
+"PO-Revision-Date: 2023-03-22 15:51\n"
 
 #: /examples/federated/md_package/schema/plugin.json:/description /packages/markdownviewer-extension/schema/plugin.json:/description
 msgctxt "schema"
 msgid "Markdown viewer settings."
 msgstr "Configurações da visualização do Markdown."
 
 #: /examples/federated/md_package/schema/plugin.json:/jupyter.lab.setting-icon-label /packages/markdownviewer-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
@@ -228,30 +228,30 @@
 msgctxt "schema"
 msgid "Application Context Menu"
 msgstr "Menu de contexto do aplicativo"
 
 #: /packages/application-extension/schema/shell.json:/description
 msgctxt "schema"
 msgid "JupyterLab Shell layout settings."
-msgstr ""
+msgstr "Configurações de layout do Shell JupyterLab."
 
 #: /packages/application-extension/schema/shell.json:/properties/hiddenMode/description
 msgctxt "settings"
 msgid "The method for hiding widgets in the main dock panel. Using `scale` will increase performance on Firefox but don't use it with Chrome, Chromium or Edge. Similar performance gains are seen with `contentVisibility` which is only available in Chromium-based browsers."
 msgstr "O método para ocultar widgets no painel principal do dock. Usar `scale` aumentará o desempenho no Firefox, mas não use-o com o Chrome, Chromium ou Edge. Ganhos de desempenho similares são vistos com `contentVisibility` que só estão disponíveis em navegadores baseados no Chromium."
 
 #: /packages/application-extension/schema/shell.json:/properties/hiddenMode/title
 msgctxt "settings"
 msgid "Hidden mode of main panel widgets"
-msgstr ""
+msgstr "Modo oculto de widgets do painel principal"
 
 #: /packages/application-extension/schema/shell.json:/title
 msgctxt "schema"
 msgid "JupyterLab Shell"
-msgstr ""
+msgstr "Shell do JupyterLab"
 
 #: /packages/application-extension/schema/sidebar.json:/description
 msgctxt "schema"
 msgid "Sidebar layout settings."
 msgstr "Configurações de layout da barra lateral."
 
 #: /packages/application-extension/schema/sidebar.json:/jupyter.lab.setting-icon-label
@@ -285,25 +285,25 @@
 msgctxt "settings"
 msgid "Whether to check for newer version of JupyterLab or not. It requires `fechNews` to be `true` to be active. If `true`, it will make a request to a website."
 msgstr ""
 
 #: /packages/apputils-extension/schema/notification.json:/properties/checkForUpdates/title
 msgctxt "settings"
 msgid "Check for JupyterLab updates"
-msgstr ""
+msgstr "Verificar se há atualizações do JupyterLab"
 
 #: /packages/apputils-extension/schema/notification.json:/properties/doNotDisturbMode/description
 msgctxt "settings"
 msgid "If `true`, no toast notifications will be automatically displayed."
-msgstr ""
+msgstr "Se `true`, nenhuma notificação toast será exibida automaticamente."
 
 #: /packages/apputils-extension/schema/notification.json:/properties/doNotDisturbMode/title
 msgctxt "settings"
 msgid "Silence all notifications"
-msgstr ""
+msgstr "Silenciar todas as notificações"
 
 #: /packages/apputils-extension/schema/notification.json:/properties/fetchNews/description
 msgctxt "settings"
 msgid "Whether to fetch news from Jupyter news feed. If `true`, it will make a request to a website."
 msgstr ""
 
 #: /packages/apputils-extension/schema/notification.json:/properties/fetchNews/title
@@ -480,15 +480,15 @@
 msgctxt "settings"
 msgid "An item is defined by a 'name', a 'command' name, and an 'icon' name"
 msgstr ""
 
 #: /packages/cell-toolbar-extension/schema/plugin.json:/properties/toolbar/title
 msgctxt "settings"
 msgid "List of toolbar items"
-msgstr ""
+msgstr "Lista de itens da barra de ferramentas"
 
 #: /packages/cell-toolbar-extension/schema/plugin.json:/title
 msgctxt "schema"
 msgid "Cell Toolbar"
 msgstr ""
 
 #: /packages/codemirror-extension/schema/commands.json:/description
@@ -530,30 +530,30 @@
 msgctxt "settings"
 msgid "When enabled, which is the default, doing copy or cut when there is no selection will copy or cut the whole lines that have cursors on them."
 msgstr "Quando habilitado, que é o comportamento padrão, ao copiar ou cortar quando nada estiver selecionado irá copiar ou cortar todas as linhas que tiverem cursores."
 
 #: /packages/codemirror-extension/schema/commands.json:/properties/lineWiseCopyCut/title /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/lineWiseCopyCut/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/lineWiseCopyCut/title
 msgctxt "settings"
 msgid "Line-wise Ctrl-C"
-msgstr ""
+msgstr "Ctrl-C por linha"
 
 #: /packages/codemirror-extension/schema/commands.json:/properties/scrollPastEnd/description
 msgctxt "settings"
 msgid "Whether to scroll past the end of text document"
 msgstr "Se deve rolar após o final do documento de texto"
 
 #: /packages/codemirror-extension/schema/commands.json:/properties/scrollPastEnd/title
 msgctxt "settings"
 msgid "Scroll behavior"
 msgstr "Comportamento da rolagem"
 
 #: /packages/codemirror-extension/schema/commands.json:/properties/selectionPointer/description
 msgctxt "settings"
 msgid "Control the mouse cursor appearance when hovering over the selection. Value is boolean or string, e.g. 'pointer'."
-msgstr ""
+msgstr "Controle a aparência do cursor do mouse ao passá-lo sobre a seleção. O valor é um booleano ou uma string, por exemplo, 'pointer'."
 
 #: /packages/codemirror-extension/schema/commands.json:/properties/selectionPointer/oneOf[0]/title
 msgctxt "settings"
 msgid "Use default"
 msgstr "Usar padrão"
 
 #: /packages/codemirror-extension/schema/commands.json:/properties/selectionPointer/oneOf[1]/title
@@ -570,15 +570,15 @@
 msgctxt "settings"
 msgid "Highlight active line. Value is boolean, or { nonEmpty: boolean }."
 msgstr ""
 
 #: /packages/codemirror-extension/schema/commands.json:/properties/styleActiveLine/oneOf[0]/title
 msgctxt "settings"
 msgid "Boolean"
-msgstr ""
+msgstr "Boolean"
 
 #: /packages/codemirror-extension/schema/commands.json:/properties/styleActiveLine/oneOf[1]/title
 msgctxt "settings"
 msgid "Object"
 msgstr "Objeto"
 
 #: /packages/codemirror-extension/schema/commands.json:/properties/styleActiveLine/title
@@ -602,15 +602,15 @@
 msgctxt "settings"
 msgid "Theme"
 msgstr "Tema"
 
 #: /packages/codemirror-extension/schema/commands.json:/title
 msgctxt "schema"
 msgid "CodeMirror"
-msgstr ""
+msgstr "CodeMirror"
 
 #: /packages/completer-extension/schema/consoles.json:/description
 msgctxt "schema"
 msgid "Console completer settings."
 msgstr "Configurações da função Autocompletar do Console."
 
 #: /packages/completer-extension/schema/consoles.json:/title
@@ -637,40 +637,40 @@
 msgctxt "schema"
 msgid "Notebook Completer"
 msgstr "Função Autocompletar do Notebook"
 
 #: /packages/console-extension/schema/foreign.json:/description
 msgctxt "schema"
 msgid "Code Console Foreign plugin settings."
-msgstr ""
+msgstr "Configurações de plugin externo do console de código."
 
 #: /packages/console-extension/schema/foreign.json:/title
 msgctxt "schema"
 msgid "Code Console Foreign plugin"
-msgstr ""
+msgstr "Plugin externo do console de código"
 
 #: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/autoClosingBrackets/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/autoClosingBrackets/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/autoClosingBrackets/title
 msgctxt "settings"
 msgid "Auto Closing Brackets"
-msgstr ""
+msgstr "Fechamento automático de parênteses"
 
 #: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/codeFolding/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/codeFolding/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/codeFolding/title
 msgctxt "settings"
 msgid "Code Folding"
 msgstr "Ocultação de código"
 
 #: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/cursorBlinkRate/description /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/cursorBlinkRate/description /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/cursorBlinkRate/description
 msgctxt "settings"
 msgid "Half-period in milliseconds used for cursor blinking. The default blink rate is 530ms. By setting this to zero, blinking can be disabled. A negative value hides the cursor entirely."
 msgstr ""
 
 #: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/cursorBlinkRate/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/cursorBlinkRate/title
 msgctxt "settings"
 msgid "Cursor Blinking Rate"
-msgstr ""
+msgstr "Taxa de piscagem do cursor"
 
 #: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/insertSpaces/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/insertSpaces/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/insertSpaces/title
 msgctxt "settings"
 msgid "Insert Spaces"
 msgstr "Inserir espaços"
 
 #: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/lineNumbers/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/lineNumbers/title
@@ -682,15 +682,15 @@
 msgctxt "settings"
 msgid "Line Wrap"
 msgstr "Quebras de linha"
 
 #: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/matchBrackets/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/matchBrackets/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/matchBrackets/title
 msgctxt "settings"
 msgid "Match Brackets"
-msgstr ""
+msgstr "Correspondência de parênteses"
 
 #: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/readOnly/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/readOnly/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/readOnly/title
 msgctxt "settings"
 msgid "Read Only"
 msgstr "Somente leitura"
 
 #: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/rulers/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/rulers/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/rulers/title
@@ -702,15 +702,15 @@
 msgctxt "settings"
 msgid "Tab Size"
 msgstr "Tamanho da tabulação"
 
 #: /packages/console-extension/schema/tracker.json:/definitions/editorConfig/properties/wordWrapColumn/title /packages/fileeditor-extension/schema/plugin.json:/definitions/editorConfig/properties/wordWrapColumn/title /packages/notebook-extension/schema/tracker.json:/definitions/editorConfig/properties/wordWrapColumn/title
 msgctxt "settings"
 msgid "Word Wrap Column"
-msgstr ""
+msgstr "Coluna Quebra de Linha"
 
 #: /packages/console-extension/schema/tracker.json:/description
 msgctxt "schema"
 msgid "Code Console settings."
 msgstr "Configurações do console de código."
 
 #: /packages/console-extension/schema/tracker.json:/jupyter.lab.menus/main[1]/items[1]/submenu/label
@@ -744,15 +744,16 @@
 msgid "Prompt Cell Configuration"
 msgstr "Configuração de célula prompt"
 
 #: /packages/console-extension/schema/tracker.json:/properties/showAllKernelActivity/description
 msgctxt "settings"
 msgid "Whether the console defaults to showing all\n"
 "kernel activity or just kernel activity originating from itself."
-msgstr ""
+msgstr "Se o console mostra todas as atividades do kernel\n"
+"ou apenas as atividades do kernel originárias de si mesmo."
 
 #: /packages/console-extension/schema/tracker.json:/properties/showAllKernelActivity/title
 msgctxt "settings"
 msgid "Show All Kernel Activity"
 msgstr "Mostrar todas as atividades do kernel"
 
 #: /packages/console-extension/schema/tracker.json:/title
@@ -764,15 +765,15 @@
 msgctxt "schema"
 msgid "CSV Viewer settings."
 msgstr "Configurações do visualizador CSV."
 
 #: /packages/csvviewer-extension/schema/csv.json:/jupyter.lab.setting-icon-label
 msgctxt "settings"
 msgid "CSV Viewer"
-msgstr ""
+msgstr "Visualizador de CSV"
 
 #: /packages/csvviewer-extension/schema/csv.json:/properties/toolbar/description /packages/csvviewer-extension/schema/tsv.json:/properties/toolbar/description
 msgctxt "settings"
 msgid "Note: To disable a toolbar item,\n"
 "copy it to User Preferences and add the\n"
 "\"disabled\" key. The following example will disable the delimiter selector item:\n"
 "{\n"
@@ -2167,15 +2168,15 @@
 msgid "Information"
 msgstr ""
 
 #: packages/application-extension/src/index.tsx:990
 msgid "Context menu customization has changed. You will need to reload JupyterLab to see the changes."
 msgstr ""
 
-#: packages/application-extension/src/index.tsx:995 packages/apputils/src/toolbar/factory.ts:34 packages/docmanager-extension/src/index.tsx:654 packages/mainmenu-extension/src/index.ts:948
+#: packages/application-extension/src/index.tsx:995 packages/apputils/src/toolbar/factory.ts:34 packages/docmanager-extension/src/index.tsx:654 packages/docprovider/src/yprovider.ts:135 packages/mainmenu-extension/src/index.ts:948
 msgid "Reload"
 msgstr "Recarregar"
 
 #: packages/application/src/connectionlost.ts:19
 msgid "Server Connection Error"
 msgstr "Erro de conexão ao servidor"
 
@@ -2395,23 +2396,23 @@
 msgid "Use Theme: %1"
 msgstr "Usar Tema: %1"
 
 #: packages/apputils-extension/src/workspacesplugin.ts:189
 msgid "Workspace loader"
 msgstr "Carregador da área de trabalho"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:274 packages/apputils-extension/src/workspacesplugin.ts:280 packages/docmanager/src/widgetmanager.ts:438 packages/docregistry/src/context.ts:1035 packages/docregistry/src/context.ts:1042
+#: packages/apputils-extension/src/workspacesplugin.ts:274 packages/apputils-extension/src/workspacesplugin.ts:280 packages/docmanager/src/widgetmanager.ts:438 packages/docregistry/src/context.ts:1035 packages/docregistry/src/context.ts:1042 packages/docregistry/src/context.ts:1101 packages/docregistry/src/context.ts:1108
 msgid "Save"
 msgstr "Salvar"
 
 #: packages/apputils-extension/src/workspacesplugin.ts:276 packages/apputils-extension/src/workspacesplugin.ts:82
 msgid "Save Current Workspace As…"
 msgstr ""
 
-#: packages/apputils-extension/src/workspacesplugin.ts:278 packages/apputils/src/sessioncontext.tsx:1292 packages/debugger-extension/src/index.ts:625 packages/debugger/src/panels/breakpoints/index.ts:66 packages/docmanager-extension/src/index.tsx:653 packages/docmanager-extension/src/index.tsx:703 packages/docmanager-extension/src/index.tsx:994 packages/docmanager/src/dialogs.ts:115 packages/docmanager/src/dialogs.ts:52 packages/docmanager/src/widgetmanager.ts:444 packages/extensionmanager/src/companions.tsx:216 packages/filebrowser/src/listing.ts:415 packages/filebrowser/src/model.ts:456 packages/filebrowser/src/opendialog.ts:87 packages/notebook/src/actions.tsx:1911 packages/running/src/index.tsx:232 packages/settingeditor/src/plugineditor.ts:137 packages/shortcuts-extension/src/components/ShortcutItem.tsx:247 packages/translation-extension/src/index.ts:138
+#: packages/apputils-extension/src/workspacesplugin.ts:278 packages/apputils/src/sessioncontext.tsx:1292 packages/debugger-extension/src/index.ts:625 packages/debugger/src/panels/breakpoints/index.ts:66 packages/docmanager-extension/src/index.tsx:1015 packages/docmanager-extension/src/index.tsx:653 packages/docmanager-extension/src/index.tsx:703 packages/docmanager-extension/src/index.tsx:994 packages/docmanager/src/dialogs.ts:115 packages/docmanager/src/dialogs.ts:52 packages/docmanager/src/widgetmanager.ts:444 packages/extensionmanager/src/companions.tsx:216 packages/filebrowser/src/listing.ts:415 packages/filebrowser/src/model.ts:456 packages/filebrowser/src/opendialog.ts:87 packages/notebook/src/actions.tsx:1911 packages/running/src/index.tsx:232 packages/settingeditor/src/plugineditor.ts:137 packages/shortcuts-extension/src/components/ShortcutItem.tsx:247 packages/translation-extension/src/index.ts:138
 msgid "Cancel"
 msgstr "Cancelar"
 
 #: packages/apputils-extension/src/workspacesplugin.ts:75
 msgid "JupyterLab workspace File"
 msgstr "Arquivo de área de trabalho do JupyterLab"
 
@@ -2535,23 +2536,23 @@
 msgid "Kernel Name:"
 msgstr "Nome do Kernel:"
 
 #: packages/apputils/src/sessioncontext.tsx:1714
 msgid "Kernel Id:"
 msgstr "Id do Kernel:"
 
-#: packages/apputils/src/thememanager.ts:362
+#: packages/apputils/src/thememanager.ts:362 packages/apputils/src/thememanager.ts:373
 msgid "Neither theme %1 nor default %2 loaded."
 msgstr "Nem o tema %1 nem o padrão %2 foram carregados."
 
-#: packages/apputils/src/thememanager.ts:446
+#: packages/apputils/src/thememanager.ts:446 packages/apputils/src/thememanager.ts:457
 msgid "Error Loading Theme"
 msgstr "Erro ao carregar o tema"
 
-#: packages/apputils/src/thememanager.ts:448 packages/docmanager-extension/src/index.tsx:406 packages/extensionmanager/src/companions.tsx:218 packages/extensionmanager/src/dialog.tsx:39 packages/extensionmanager/src/widget.tsx:354 packages/extensionmanager/src/widget.tsx:355
+#: packages/apputils/src/thememanager.ts:448 packages/apputils/src/thememanager.ts:459 packages/docmanager-extension/src/index.tsx:406 packages/extensionmanager/src/companions.tsx:218 packages/extensionmanager/src/dialog.tsx:39 packages/extensionmanager/src/widget.tsx:354 packages/extensionmanager/src/widget.tsx:355
 msgid "OK"
 msgstr "Ok"
 
 #: packages/apputils/src/toolbar/factory.ts:29
 msgid "Toolbar customization has changed. You will need to reload JupyterLab to see the changes."
 msgstr ""
 
@@ -2929,27 +2930,39 @@
 msgid "Scope"
 msgstr ""
 
 #: packages/debugger/src/panels/variables/tree.tsx:282
 msgid "Render variable"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:1009
+#: packages/docmanager-extension/src/index.tsx:1002 packages/docmanager-extension/src/index.tsx:981
+msgid "Delete %1"
+msgstr "Excluir %1"
+
+#: packages/docmanager-extension/src/index.tsx:1009 packages/docmanager-extension/src/index.tsx:1030
 msgid "Show in File Browser"
 msgstr "Mostrar no gerenciador de arquivos"
 
-#: packages/docmanager-extension/src/index.tsx:1075
+#: packages/docmanager-extension/src/index.tsx:1012 packages/docmanager-extension/src/index.tsx:1016 packages/docmanager-extension/src/index.tsx:991 packages/docmanager-extension/src/index.tsx:995 packages/filebrowser-extension/src/index.ts:819 packages/filebrowser/src/listing.ts:412 packages/filebrowser/src/listing.ts:416
+msgid "Delete"
+msgstr "Excluir"
+
+#: packages/docmanager-extension/src/index.tsx:1013 packages/docmanager-extension/src/index.tsx:992
+msgid "Are you sure you want to delete %1"
+msgstr "Você tem certeza que você quer excluir '%1'"
+
+#: packages/docmanager-extension/src/index.tsx:1075 packages/docmanager-extension/src/index.tsx:1096
 msgid "Are you sure you want to revert the %1 to the latest checkpoint? "
 msgstr "Tem certeza que deseja reverter o %1 para o último ponto de verificação? "
 
-#: packages/docmanager-extension/src/index.tsx:1081
+#: packages/docmanager-extension/src/index.tsx:1081 packages/docmanager-extension/src/index.tsx:1102
 msgid "This cannot be undone."
 msgstr "Essa ação não poderá ser desfeita."
 
-#: packages/docmanager-extension/src/index.tsx:1088
+#: packages/docmanager-extension/src/index.tsx:1088 packages/docmanager-extension/src/index.tsx:1109
 msgid "The checkpoint was last updated at: "
 msgstr "O ponto de verificação foi atualizado em: "
 
 #: packages/docmanager-extension/src/index.tsx:271
 msgid "Overrides for the default viewers for file types.\n"
 "Specify a mapping from file type name to document viewer name, for example:\n\n"
 "defaultViewers: {\n"
@@ -3032,15 +3045,15 @@
 msgid "Cannot Revert"
 msgstr "Impossível Reverter"
 
 #: packages/docmanager-extension/src/index.tsx:700
 msgid "Revert %1 to checkpoint"
 msgstr "Reverter %1 para o ponto de verificação"
 
-#: packages/docmanager-extension/src/index.tsx:704 packages/docregistry/src/context.ts:851 packages/docregistry/src/context.ts:869
+#: packages/docmanager-extension/src/index.tsx:704 packages/docregistry/src/context.ts:851 packages/docregistry/src/context.ts:869 packages/docregistry/src/context.ts:874 packages/docregistry/src/context.ts:892
 msgid "Revert"
 msgstr "Reverter"
 
 #: packages/docmanager-extension/src/index.tsx:725
 msgid "In collaborative mode, the document is saved automatically after every change"
 msgstr ""
 
@@ -3092,47 +3105,35 @@
 msgid "Save %1 As…"
 msgstr "Salvar %1 como…"
 
 #: packages/docmanager-extension/src/index.tsx:864
 msgid "Save with new path"
 msgstr "Salvar com novo caminho"
 
-#: packages/docmanager-extension/src/index.tsx:883
+#: packages/docmanager-extension/src/index.tsx:883 packages/docmanager-extension/src/index.tsx:904
 msgid "Autosave Documents"
 msgstr "Salvar documentos automaticamente"
 
-#: packages/docmanager-extension/src/index.tsx:943
+#: packages/docmanager-extension/src/index.tsx:943 packages/docmanager-extension/src/index.tsx:964
 msgid "New View for %1"
 msgstr "Nova Visualização para %1"
 
-#: packages/docmanager-extension/src/index.tsx:967
+#: packages/docmanager-extension/src/index.tsx:967 packages/docmanager-extension/src/index.tsx:988
 msgid "Rename%1…"
 msgstr ""
 
-#: packages/docmanager-extension/src/index.tsx:981
-msgid "Delete %1"
-msgstr "Excluir %1"
-
-#: packages/docmanager-extension/src/index.tsx:991 packages/docmanager-extension/src/index.tsx:995 packages/filebrowser-extension/src/index.ts:819 packages/filebrowser/src/listing.ts:412 packages/filebrowser/src/listing.ts:416
-msgid "Delete"
-msgstr "Excluir"
-
-#: packages/docmanager-extension/src/index.tsx:992
-msgid "Are you sure you want to delete %1"
-msgstr "Você tem certeza que você quer excluir '%1'"
-
 #: packages/docmanager/src/dialogs.ts:112
 msgid "Overwrite file?"
 msgstr "Sobrescrever o arquivo?"
 
 #: packages/docmanager/src/dialogs.ts:113
 msgid "\"%1\" already exists, overwrite?"
 msgstr "\"%1\" já existe, substituir?"
 
-#: packages/docmanager/src/dialogs.ts:116 packages/docregistry/src/context.ts:853 packages/docregistry/src/context.ts:865 packages/docregistry/src/context.ts:887 packages/docregistry/src/context.ts:898 packages/shortcuts-extension/src/components/ShortcutInput.tsx:499 packages/shortcuts-extension/src/components/ShortcutItem.tsx:254
+#: packages/docmanager/src/dialogs.ts:116 packages/docregistry/src/context.ts:853 packages/docregistry/src/context.ts:865 packages/docregistry/src/context.ts:876 packages/docregistry/src/context.ts:887 packages/docregistry/src/context.ts:888 packages/docregistry/src/context.ts:898 packages/docregistry/src/context.ts:910 packages/docregistry/src/context.ts:921 packages/shortcuts-extension/src/components/ShortcutInput.tsx:499 packages/shortcuts-extension/src/components/ShortcutItem.tsx:254
 msgid "Overwrite"
 msgstr "Sobrescrever"
 
 #: packages/docmanager/src/dialogs.ts:180
 msgid "File Path"
 msgstr "Caminho do arquivo"
 
@@ -3218,41 +3219,49 @@
 msgid "Save changes in \"%1\" before closing?"
 msgstr "Salvar alterações em \"%1\" antes de fechar?"
 
 #: packages/docmanager/src/widgetmanager.ts:445
 msgid "Discard"
 msgstr "Descartar"
 
-#: packages/docregistry/src/context.ts:1037
+#: packages/docprovider/src/yprovider.ts:131
+msgid "Session expired"
+msgstr "Sessão expirada"
+
+#: packages/docprovider/src/yprovider.ts:132
+msgid "The document session expired. You need to reload this browser tab."
+msgstr "A sessão do documento expirou. Você precisa recarregar esta aba do navegador."
+
+#: packages/docregistry/src/context.ts:1037 packages/docregistry/src/context.ts:1103
 msgid "Save File As.."
 msgstr "Salvar arquivo como.."
 
-#: packages/docregistry/src/context.ts:642
+#: packages/docregistry/src/context.ts:642 packages/docregistry/src/context.ts:665 packages/docregistry/src/context.ts:958
 msgid "File Save Error for %1"
 msgstr "Erro ao Salvar Arquivo para %1"
 
-#: packages/docregistry/src/context.ts:686 packages/docregistry/src/context.ts:744
+#: packages/docregistry/src/context.ts:686 packages/docregistry/src/context.ts:709 packages/docregistry/src/context.ts:744 packages/docregistry/src/context.ts:767
 msgid "File Load Error for %1"
 msgstr "Erro ao Carregar Arquivo para %1"
 
-#: packages/docregistry/src/context.ts:845
+#: packages/docregistry/src/context.ts:845 packages/docregistry/src/context.ts:868
 msgid "\"%1\" has changed on disk since the last time it was opened or saved.\n"
 "Do you want to overwrite the file on disk with the version open here,\n"
 "or load the version on disk (revert)?"
 msgstr ""
 
-#: packages/docregistry/src/context.ts:857
+#: packages/docregistry/src/context.ts:857 packages/docregistry/src/context.ts:880
 msgid "File Changed"
 msgstr "Arquivo modificado"
 
-#: packages/docregistry/src/context.ts:882
+#: packages/docregistry/src/context.ts:882 packages/docregistry/src/context.ts:905
 msgid "\"%1\" already exists. Do you want to replace it?"
 msgstr "\"%1\" já existe. Deseja substituir?"
 
-#: packages/docregistry/src/context.ts:890
+#: packages/docregistry/src/context.ts:890 packages/docregistry/src/context.ts:913
 msgid "File Overwrite?"
 msgstr "Sobrescrever arquivo?"
 
 #: packages/docregistry/src/mimedocument.ts:174 packages/docregistry/src/mimedocument.ts:70 packages/markdownviewer/src/widget.ts:201
 msgid "Renderer Failure: %1"
 msgstr "Falha no Renderizador: %1"
```

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_git.po` & `jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_git.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_lsp.po` & `jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_lsp.po`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: pt-BR\n"
 "X-Crowdin-File: /main/extensions/jupyterlab_lsp/locale/jupyterlab_lsp.pot\n"
 "X-Crowdin-File-ID: 199\n"
 "Language-Team: Portuguese, Brazilian\n"
 "Language: pt_BR\n"
-"PO-Revision-Date: 2022-12-09 17:13\n"
+"PO-Revision-Date: 2023-03-16 08:13\n"
 
 #: /packages/jupyterlab-lsp/schema/completion.json:/description
 msgctxt "schema"
 msgid "LSP Completion settings."
 msgstr "Configurações de preenchimento automático."
 
 #: /packages/jupyterlab-lsp/schema/completion.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/diagnostics.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/highlights.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/hover.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/jump_to.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/plugin.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/rename.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/signature.json:/jupyter.lab.setting-icon-label /packages/jupyterlab-lsp/schema/syntax_highlighting.json:/jupyter.lab.setting-icon-label
@@ -260,24 +260,44 @@
 msgstr ""
 
 #: /packages/jupyterlab-lsp/schema/hover.json:/description
 msgctxt "schema"
 msgid "LSP Hover over the code tooltip settings."
 msgstr ""
 
+#: /packages/jupyterlab-lsp/schema/hover.json:/properties/autoActivate/description
+msgctxt "settings"
+msgid "Automatic activation of hover without pressing a key. It will still be possible to show up tooltips with the modifier key."
+msgstr ""
+
+#: /packages/jupyterlab-lsp/schema/hover.json:/properties/autoActivate/title
+msgctxt "settings"
+msgid "Automatic hover"
+msgstr ""
+
 #: /packages/jupyterlab-lsp/schema/hover.json:/properties/cacheSize/description
 msgctxt "settings"
 msgid "Up to how many hover responses should be cached at any given time. The cache being is invalidated after any change in the editor."
 msgstr ""
 
 #: /packages/jupyterlab-lsp/schema/hover.json:/properties/cacheSize/title
 msgctxt "settings"
 msgid "Cache size"
 msgstr ""
 
+#: /packages/jupyterlab-lsp/schema/hover.json:/properties/delay/description
+msgctxt "settings"
+msgid "Number of milliseconds after which the hover tooltip should be shown. Ignored if 'Automatic hover' is off."
+msgstr ""
+
+#: /packages/jupyterlab-lsp/schema/hover.json:/properties/delay/title
+msgctxt "settings"
+msgid "Hover delay"
+msgstr ""
+
 #: /packages/jupyterlab-lsp/schema/hover.json:/properties/modifierKey/description
 msgctxt "settings"
 msgid "Keyboard key which activates the tooltip on hover. The allowed keys are Alt, Control, Shift, and AltGraph. Linux user: Meta key is also supported. Safari users: Meta key is also supported, AltGraph is not supported. To see which physical keys are mapped, visit: https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/getModifierState"
 msgstr ""
 
 #: /packages/jupyterlab-lsp/schema/hover.json:/properties/modifierKey/title /packages/jupyterlab-lsp/schema/jump_to.json:/properties/modifierKey/title
 msgctxt "settings"
@@ -470,58 +490,58 @@
 msgstr ""
 
 #: /packages/jupyterlab-lsp/schema/syntax_highlighting.json:/title
 msgctxt "schema"
 msgid "Code Syntax"
 msgstr ""
 
-#: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:236 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:238 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:243
+#: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:236 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:238 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:243 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:259
 msgid "Failed to load language server spec finder `{}`: \n"
 "{}"
 msgstr ""
 
 #: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:248
 msgid "Skipping non-installed server: `{}`"
 msgstr "Ignorando servidor não instalado: `{}`"
 
-#: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:254 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:259
+#: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:254 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:259 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:275
 msgid "Failed to fetch commands from language server spec finder `{}`:\n"
 "{}"
 msgstr ""
 
-#: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:267 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:272
+#: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:267 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:272 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:288
 msgid "Failed to validate commands from language server spec finder `{}`:\n"
 "{}"
 msgstr ""
 
-#: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:279 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:284
+#: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:279 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:284 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:300
 msgid "Skipped non-installed server(s): {}"
 msgstr ""
 
-#: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:41 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:46
+#: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:41 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:46 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:54
 msgid "extra language server specs, keyed by implementation, from conf.d"
 msgstr ""
 
-#: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:46 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:51
+#: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:46 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:51 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:59
 msgid "a dict of language server specs, keyed by implementation"
 msgstr ""
 
-#: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:52 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:57
+#: /python_packages/jupyter_lsp/jupyter_lsp/manager.py:52 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:57 /python_packages/jupyter_lsp/jupyter_lsp/manager.py:65
 msgid "try to find known language servers in sys.prefix (and elsewhere)"
 msgstr ""
 
-#: /python_packages/jupyter_lsp/jupyter_lsp/types.py:193 /python_packages/jupyter_lsp/jupyter_lsp/types.py:196
+#: /python_packages/jupyter_lsp/jupyter_lsp/types.py:193 /python_packages/jupyter_lsp/jupyter_lsp/types.py:196 /python_packages/jupyter_lsp/jupyter_lsp/types.py:198
 msgid "path to nodejs executable"
 msgstr ""
 
-#: /python_packages/jupyter_lsp/jupyter_lsp/types.py:195 /python_packages/jupyter_lsp/jupyter_lsp/types.py:198
+#: /python_packages/jupyter_lsp/jupyter_lsp/types.py:195 /python_packages/jupyter_lsp/jupyter_lsp/types.py:198 /python_packages/jupyter_lsp/jupyter_lsp/types.py:200
 msgid "absolute paths in which to seek node_modules"
 msgstr ""
 
-#: /python_packages/jupyter_lsp/jupyter_lsp/types.py:200 /python_packages/jupyter_lsp/jupyter_lsp/types.py:203
+#: /python_packages/jupyter_lsp/jupyter_lsp/types.py:200 /python_packages/jupyter_lsp/jupyter_lsp/types.py:203 /python_packages/jupyter_lsp/jupyter_lsp/types.py:205
 msgid "additional absolute paths to seek node_modules first"
 msgstr ""
 
 #: packages/completion-theme/src/about.tsx:47
 msgid " (current)"
 msgstr ""
 
@@ -529,144 +549,180 @@
 msgid "Licence: "
 msgstr ""
 
 #: packages/completion-theme/src/about.tsx:60
 msgid "Includes dedicated dark mode icons set"
 msgstr ""
 
-#: packages/completion-theme/src/index.ts:152 packages/completion-theme/src/index.ts:154
+#: packages/completion-theme/src/index.ts:152 packages/completion-theme/src/index.ts:154 packages/completion-theme/src/index.ts:155
 msgid "LSP Completer Themes"
 msgstr ""
 
-#: packages/completion-theme/src/index.ts:158 packages/completion-theme/src/index.ts:160
+#: packages/completion-theme/src/index.ts:158 packages/completion-theme/src/index.ts:160 packages/completion-theme/src/index.ts:161
 msgid "OK"
 msgstr ""
 
-#: packages/completion-theme/src/index.ts:189 packages/completion-theme/src/index.ts:190 packages/completion-theme/src/index.ts:192
+#: packages/completion-theme/src/index.ts:189 packages/completion-theme/src/index.ts:190 packages/completion-theme/src/index.ts:191 packages/completion-theme/src/index.ts:192
 msgid "Display the completer themes"
 msgstr ""
 
+#: packages/completion-theme/src/index.ts:197
+msgid "Language server protocol"
+msgstr ""
+
 #: packages/jupyterlab-lsp/src/adapters/adapter.ts:388 packages/jupyterlab-lsp/src/adapters/adapter.ts:397 packages/jupyterlab-lsp/src/adapters/adapter.ts:409 packages/jupyterlab-lsp/src/adapters/adapter.ts:412 packages/jupyterlab-lsp/src/adapters/adapter.ts:418 packages/jupyterlab-lsp/src/adapters/adapter.ts:435
 msgid "Message from "
 msgstr ""
 
 #: packages/jupyterlab-lsp/src/adapters/adapter.ts:432
 msgid "Dismiss"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:150
+#: packages/jupyterlab-lsp/src/components/serverSettings.tsx:103
+msgid "allowed values: %1"
+msgstr ""
+
+#: packages/jupyterlab-lsp/src/components/serverSettings.tsx:114
+msgid "Language servers"
+msgstr ""
+
+#: packages/jupyterlab-lsp/src/components/serverSettings.tsx:119
+msgid "Validation of user settings for language server failed"
+msgstr ""
+
+#: packages/jupyterlab-lsp/src/components/serverSettings.tsx:124
+msgid "Your language server settings do not follow current schema. The LSP configuration graphical interface will run in schema-free mode to enable you to continue using the current settings as-is (in case if the schema is outdated). If this is however an earlier configuration mistake (settings were not validated in earlier versions of jupyterlab-lsp), please correct the following validation errors in JSON Settings Editor, save, and reload application:"
+msgstr ""
+
+#: packages/jupyterlab-lsp/src/components/serverSettings.tsx:225
+msgid "Default values set programatically for: "
+msgstr ""
+
+#: packages/jupyterlab-lsp/src/components/serverSettings.tsx:242 packages/jupyterlab-lsp/src/components/statusbar.tsx:343 packages/jupyterlab-lsp/src/components/statusbar.tsx:352
+msgid "Available"
+msgstr ""
+
+#: packages/jupyterlab-lsp/src/components/serverSettings.tsx:247
+msgid "Not installed"
+msgstr ""
+
+#: packages/jupyterlab-lsp/src/components/serverSettings.tsx:55
+msgid "Multiple distinct values detected for:"
+msgstr ""
+
+#: packages/jupyterlab-lsp/src/components/serverSettings.tsx:57
+msgid "Retaining the last value for each of the settings. Please remove the additional values in JSON Settings Editor."
+msgstr ""
+
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:141 packages/jupyterlab-lsp/src/components/statusbar.tsx:150
 msgid "Troubleshooting"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:154
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:145 packages/jupyterlab-lsp/src/components/statusbar.tsx:154
 msgid "In case of issues with installation feel welcome to ask a question on GitHub."
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:158
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:149 packages/jupyterlab-lsp/src/components/statusbar.tsx:158
 msgid "Installation"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:168
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:159 packages/jupyterlab-lsp/src/components/statusbar.tsx:168
 msgid "No installation instructions were provided with this specification."
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:183
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:174 packages/jupyterlab-lsp/src/components/statusbar.tsx:183
 msgid "No language server for %1 detected"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:192
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:183 packages/jupyterlab-lsp/src/components/statusbar.tsx:192
 msgid "There is %1 language server you can easily install that supports %2."
 msgid_plural "There are %1 language servers you can easily install that supports %2."
 msgstr[0] ""
 msgstr[1] ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:211
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:202 packages/jupyterlab-lsp/src/components/statusbar.tsx:211
 msgid "We do not have an auto-detection ready for a language servers supporting %1 yet."
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:217
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:208 packages/jupyterlab-lsp/src/components/statusbar.tsx:217
 msgid "You may contribute a specification for auto-detection as described in our "
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:225
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:216 packages/jupyterlab-lsp/src/components/statusbar.tsx:225
 msgid "documentation"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:347
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:338 packages/jupyterlab-lsp/src/components/statusbar.tsx:347
 msgid "LSP servers"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:352
-msgid "Available"
-msgstr ""
-
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:362
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:353 packages/jupyterlab-lsp/src/components/statusbar.tsx:362
 msgid "Running"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:371
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:362 packages/jupyterlab-lsp/src/components/statusbar.tsx:371
 msgid "Missing"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:380
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:371 packages/jupyterlab-lsp/src/components/statusbar.tsx:380
 msgid "Documentation:"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:388
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:379 packages/jupyterlab-lsp/src/components/statusbar.tsx:388
 msgid "Language Servers"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:417 packages/jupyterlab-lsp/src/components/statusbar.tsx:418 packages/jupyterlab-lsp/src/components/statusbar.tsx:419
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:408 packages/jupyterlab-lsp/src/components/statusbar.tsx:417 packages/jupyterlab-lsp/src/components/statusbar.tsx:418 packages/jupyterlab-lsp/src/components/statusbar.tsx:419
 msgid "LSP status"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:467 packages/jupyterlab-lsp/src/components/statusbar.tsx:468 packages/jupyterlab-lsp/src/components/statusbar.tsx:469
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:458 packages/jupyterlab-lsp/src/components/statusbar.tsx:467 packages/jupyterlab-lsp/src/components/statusbar.tsx:468 packages/jupyterlab-lsp/src/components/statusbar.tsx:469
 msgid "LSP Code Intelligence"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:486 packages/jupyterlab-lsp/src/components/statusbar.tsx:487 packages/jupyterlab-lsp/src/components/statusbar.tsx:488
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:479 packages/jupyterlab-lsp/src/components/statusbar.tsx:486 packages/jupyterlab-lsp/src/components/statusbar.tsx:487 packages/jupyterlab-lsp/src/components/statusbar.tsx:488
 msgid "LSP server extension not found"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:813 packages/jupyterlab-lsp/src/components/statusbar.tsx:815 packages/jupyterlab-lsp/src/components/statusbar.tsx:816 packages/jupyterlab-lsp/src/components/statusbar.tsx:818 packages/jupyterlab-lsp/src/components/statusbar.tsx:824 packages/jupyterlab-lsp/src/components/statusbar.tsx:826 packages/jupyterlab-lsp/src/components/statusbar.tsx:827 packages/jupyterlab-lsp/src/components/statusbar.tsx:829
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:809 packages/jupyterlab-lsp/src/components/statusbar.tsx:813 packages/jupyterlab-lsp/src/components/statusbar.tsx:815 packages/jupyterlab-lsp/src/components/statusbar.tsx:816 packages/jupyterlab-lsp/src/components/statusbar.tsx:818 packages/jupyterlab-lsp/src/components/statusbar.tsx:820 packages/jupyterlab-lsp/src/components/statusbar.tsx:824 packages/jupyterlab-lsp/src/components/statusbar.tsx:826 packages/jupyterlab-lsp/src/components/statusbar.tsx:827 packages/jupyterlab-lsp/src/components/statusbar.tsx:829
 msgid "not initialized"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:829 packages/jupyterlab-lsp/src/components/statusbar.tsx:831 packages/jupyterlab-lsp/src/components/statusbar.tsx:832 packages/jupyterlab-lsp/src/components/statusbar.tsx:834
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:825 packages/jupyterlab-lsp/src/components/statusbar.tsx:829 packages/jupyterlab-lsp/src/components/statusbar.tsx:831 packages/jupyterlab-lsp/src/components/statusbar.tsx:832 packages/jupyterlab-lsp/src/components/statusbar.tsx:834
 msgid "Waiting for documents initialization..."
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:831 packages/jupyterlab-lsp/src/components/statusbar.tsx:833 packages/jupyterlab-lsp/src/components/statusbar.tsx:834 packages/jupyterlab-lsp/src/components/statusbar.tsx:836
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:827 packages/jupyterlab-lsp/src/components/statusbar.tsx:831 packages/jupyterlab-lsp/src/components/statusbar.tsx:833 packages/jupyterlab-lsp/src/components/statusbar.tsx:834 packages/jupyterlab-lsp/src/components/statusbar.tsx:836
 msgid "Fully connected & initialized (%2 virtual document)"
 msgid_plural "Fully connected & initialized (%2 virtual document)"
 msgstr[0] ""
 msgstr[1] ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:845 packages/jupyterlab-lsp/src/components/statusbar.tsx:848
-msgid "Fully connected, but %2/%3 virtual document stuck uninitialized: %4"
-msgstr ""
-
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:847 packages/jupyterlab-lsp/src/components/statusbar.tsx:850
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:841 packages/jupyterlab-lsp/src/components/statusbar.tsx:847 packages/jupyterlab-lsp/src/components/statusbar.tsx:850
 msgctxt "pluralized"
 msgid "Fully connected, but %2/%3 virtual document stuck uninitialized: %4"
 msgid_plural "Fully connected, but %2/%3 virtual documents stuck uninitialized: %4"
 msgstr[0] ""
 msgstr[1] ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:859 packages/jupyterlab-lsp/src/components/statusbar.tsx:862
-msgid "%2/%3 virtual document connected (%4 connections; waiting for: %5)"
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:845 packages/jupyterlab-lsp/src/components/statusbar.tsx:848
+msgid "Fully connected, but %2/%3 virtual document stuck uninitialized: %4"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/components/statusbar.tsx:862 packages/jupyterlab-lsp/src/components/statusbar.tsx:865
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:856 packages/jupyterlab-lsp/src/components/statusbar.tsx:862 packages/jupyterlab-lsp/src/components/statusbar.tsx:865
 msgctxt "pluralized"
 msgid "%2/%3 virtual document connected (%4 connections; waiting for: %5)"
 msgid_plural "%2/%3 virtual documents connected (%4 connections; waiting for: %5)"
 msgstr[0] ""
 msgstr[1] ""
 
+#: packages/jupyterlab-lsp/src/components/statusbar.tsx:859 packages/jupyterlab-lsp/src/components/statusbar.tsx:862
+msgid "%2/%3 virtual document connected (%4 connections; waiting for: %5)"
+msgstr ""
+
 #: packages/jupyterlab-lsp/src/components/utils.tsx:54
 msgid "cell %1"
 msgstr ""
 
 #: packages/jupyterlab-lsp/src/components/utils.tsx:55
 msgid "cells: %1-%2"
 msgstr ""
@@ -767,26 +823,42 @@
 msgid "Highlight references"
 msgstr ""
 
 #: packages/jupyterlab-lsp/src/features/highlights.ts:47 packages/jupyterlab-lsp/src/features/highlights.ts:49
 msgid "Highlight type definition"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/features/jump_to.ts:128 packages/jupyterlab-lsp/src/features/jump_to.ts:129 packages/jupyterlab-lsp/src/features/jump_to.ts:141
+#: packages/jupyterlab-lsp/src/features/jump_to.ts:128 packages/jupyterlab-lsp/src/features/jump_to.ts:129 packages/jupyterlab-lsp/src/features/jump_to.ts:141 packages/jupyterlab-lsp/src/features/jump_to.ts:236
 msgid "No jump targets found"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/features/jump_to.ts:258 packages/jupyterlab-lsp/src/features/jump_to.ts:260 packages/jupyterlab-lsp/src/features/jump_to.ts:284 packages/jupyterlab-lsp/src/features/jump_to.ts:288
+#: packages/jupyterlab-lsp/src/features/jump_to.ts:188
+msgid "Choose the jump target"
+msgstr ""
+
+#: packages/jupyterlab-lsp/src/features/jump_to.ts:189
+msgid "Jump"
+msgstr ""
+
+#: packages/jupyterlab-lsp/src/features/jump_to.ts:258 packages/jupyterlab-lsp/src/features/jump_to.ts:260 packages/jupyterlab-lsp/src/features/jump_to.ts:284 packages/jupyterlab-lsp/src/features/jump_to.ts:288 packages/jupyterlab-lsp/src/features/jump_to.ts:399
 msgid "Jump to definition"
 msgstr ""
 
-#: packages/jupyterlab-lsp/src/features/jump_to.ts:268 packages/jupyterlab-lsp/src/features/jump_to.ts:270 packages/jupyterlab-lsp/src/features/jump_to.ts:295 packages/jupyterlab-lsp/src/features/jump_to.ts:299
+#: packages/jupyterlab-lsp/src/features/jump_to.ts:268 packages/jupyterlab-lsp/src/features/jump_to.ts:270 packages/jupyterlab-lsp/src/features/jump_to.ts:295 packages/jupyterlab-lsp/src/features/jump_to.ts:299 packages/jupyterlab-lsp/src/features/jump_to.ts:444
 msgid "Jump back"
 msgstr ""
 
+#: packages/jupyterlab-lsp/src/features/jump_to.ts:377 packages/jupyterlab-lsp/src/features/jump_to.ts:408
+msgid "Connection not found for jump"
+msgstr ""
+
+#: packages/jupyterlab-lsp/src/features/jump_to.ts:430
+msgid "Jump to references"
+msgstr ""
+
 #: packages/jupyterlab-lsp/src/features/rename.ts:103 packages/jupyterlab-lsp/src/features/rename.ts:104 packages/jupyterlab-lsp/src/features/rename.ts:109
 msgid "Rename symbol"
 msgstr ""
 
 #: packages/jupyterlab-lsp/src/features/rename.ts:127 packages/jupyterlab-lsp/src/features/rename.ts:128 packages/jupyterlab-lsp/src/features/rename.ts:133 packages/jupyterlab-lsp/src/features/rename.ts:68 packages/jupyterlab-lsp/src/features/rename.ts:69
 msgid "Rename failed: %1"
 msgstr ""
```

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_search_replace.po` & `jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_search_replace.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po` & `jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_spreadsheet_editor.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_tour.po` & `jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_tour.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_widgets.po` & `jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupyterlab_widgets.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupytext.po` & `jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/jupytext.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/retrolab.po` & `jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/retrolab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/spellchecker.po` & `jupyterlab_language_pack_pt_br-3.6.post1/jupyterlab_language_pack_pt_BR/locale/pt_BR/LC_MESSAGES/spellchecker.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/.gitignore` & `jupyterlab_language_pack_pt_br-3.6.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/LICENSE.txt` & `jupyterlab_language_pack_pt_br-3.6.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/pyproject.toml` & `jupyterlab_language_pack_pt_br-3.6.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_pt_br-3.6.post0/PKG-INFO` & `jupyterlab_language_pack_pt_br-3.6.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-language-pack-pt-BR
-Version: 3.6.post0
+Version: 3.6.post1
 Summary: JupyterLab Portuguese (Brazil) Language Pack
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2023 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

