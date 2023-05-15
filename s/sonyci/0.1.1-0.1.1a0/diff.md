# Comparing `tmp/sonyci-0.1.1.tar.gz` & `tmp/sonyci-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonyci-0.1.1.tar", last modified: Mon May 15 19:57:02 2023, max compression
+gzip compressed data, was "sonyci-0.1.1a0.tar", last modified: Fri May 12 21:08:44 2023, max compression
```

## Comparing `sonyci-0.1.1.tar` & `sonyci-0.1.1a0.tar`

### file list

```diff
@@ -1,33 +1,29 @@
--rw-r--r--   0        0        0     3111 2023-05-15 19:56:33.188981 sonyci-0.1.1/README.md
--rw-r--r--   0        0        0     1538 2023-05-15 19:57:02.020951 sonyci-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      135 2023-05-15 19:56:33.188981 sonyci-0.1.1/sonyci/__init__.py
--rw-r--r--   0        0        0       34 2023-05-15 19:56:33.188981 sonyci-0.1.1/sonyci/__main__.py
--rw-r--r--   0        0        0       22 2023-05-15 19:56:33.188981 sonyci-0.1.1/sonyci/_version.py
--rw-r--r--   0        0        0     3696 2023-05-15 19:56:33.188981 sonyci-0.1.1/sonyci/cli.py
--rw-r--r--   0        0        0     1852 2023-05-15 19:56:33.188981 sonyci-0.1.1/sonyci/config.py
--rw-r--r--   0        0        0      232 2023-05-15 19:56:33.188981 sonyci-0.1.1/sonyci/log.py
--rw-r--r--   0        0        0     3510 2023-05-15 19:56:33.188981 sonyci-0.1.1/sonyci/sonyci.py
--rw-r--r--   0        0        0     1397 2023-05-15 19:56:33.192981 sonyci-0.1.1/sonyci/utils.py
--rw-r--r--   0        0        0        0 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1300 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/cli/test_cli_login.py
--rw-r--r--   0        0        0     1036 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/cli/test_cli_search.py
--rw-r--r--   0        0        0     2324 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0       40 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/sonyci/guid.toml
--rw-r--r--   0        0        0      179 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/sonyci/sonyci.toml
--rw-r--r--   0        0        0      135 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/sonyci/sonyci_different_key.toml
--rw-r--r--   0        0        0      119 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/sonyci/sonyci_no_key.toml
--rw-r--r--   0        0        0     1369 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/sonyci/test_config.py
--rw-r--r--   0        0        0     1881 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/test_sonyci.py
--rw-r--r--   0        0        0     1108 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/vhs/test_cli_login/test_bad_login.yaml
--rw-r--r--   0        0        0     1123 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/vhs/test_cli_login/test_login.yaml
--rw-r--r--   0        0        0     1199 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/vhs/test_cli_search/test_empty_search.yaml
--rw-r--r--   0        0        0     7201 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/vhs/test_cli_search/test_guid_search.yaml
--rw-r--r--   0        0        0     9586 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/vhs/tests.test_sonyci/test_asset.yaml
--rw-r--r--   0        0        0    10744 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/vhs/tests.test_sonyci/test_asset_download.yaml
--rw-r--r--   0        0        0     1123 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/vhs/tests.test_sonyci/test_token.yaml
--rw-r--r--   0        0        0     2442 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/vhs/tests.test_sonyci/test_workspace.yaml
--rw-r--r--   0        0        0     2559 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/vhs/tests.test_sonyci/test_workspace_contents.yaml
--rw-r--r--   0        0        0     2297 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/vhs/tests.test_sonyci/test_workspace_empty_search.yaml
--rw-r--r--   0        0        0     2669 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/vhs/tests.test_sonyci/test_workspace_search.yaml
--rw-r--r--   0        0        0     2547 2023-05-15 19:56:33.192981 sonyci-0.1.1/tests/vhs/tests.test_sonyci/test_workspaces.yaml
--rw-r--r--   0        0        0     4249 1970-01-01 00:00:00.000000 sonyci-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3111 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/README.md
+-rw-r--r--   0        0        0     1437 2023-05-12 21:08:44.095228 sonyci-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/sonyci/__init__.py
+-rw-r--r--   0        0        0       34 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/sonyci/__main__.py
+-rw-r--r--   0        0        0       23 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/sonyci/_version.py
+-rw-r--r--   0        0        0     3486 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/sonyci/cli.py
+-rw-r--r--   0        0        0     1852 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/sonyci/config.py
+-rw-r--r--   0        0        0      164 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/sonyci/log.py
+-rw-r--r--   0        0        0     3492 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/sonyci/sonyci.py
+-rw-r--r--   0        0        0     1397 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/sonyci/utils.py
+-rw-r--r--   0        0        0     1382 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/tests/conftest.py
+-rw-r--r--   0        0        0       40 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/tests/sonyci/guid.toml
+-rw-r--r--   0        0        0      179 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/tests/sonyci/sonyci.toml
+-rw-r--r--   0        0        0      135 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/tests/sonyci/sonyci_different_key.toml
+-rw-r--r--   0        0        0      119 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/tests/sonyci/sonyci_no_key.toml
+-rw-r--r--   0        0        0     1369 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/tests/sonyci/test_config.py
+-rw-r--r--   0        0        0     1626 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/tests/test_cli.py
+-rw-r--r--   0        0        0     1991 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/tests/test_sonyci.py
+-rw-r--r--   0        0        0     1108 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/tests/vhs/tests.test_cli/test_bad_login.yaml
+-rw-r--r--   0        0        0     1123 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/tests/vhs/tests.test_cli/test_login.yaml
+-rw-r--r--   0        0        0     9585 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_asset.yaml
+-rw-r--r--   0        0        0    10744 2023-05-12 21:08:13.314792 sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_asset_download.yaml
+-rw-r--r--   0        0        0     1123 2023-05-12 21:08:13.318792 sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_token.yaml
+-rw-r--r--   0        0        0     2404 2023-05-12 21:08:13.318792 sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_workspace.yaml
+-rw-r--r--   0        0        0     2559 2023-05-12 21:08:13.318792 sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_workspace_contents.yaml
+-rw-r--r--   0        0        0     2297 2023-05-12 21:08:13.318792 sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_workspace_empty_search.yaml
+-rw-r--r--   0        0        0     2669 2023-05-12 21:08:13.318792 sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_workspace_search.yaml
+-rw-r--r--   0        0        0     2469 2023-05-12 21:08:13.318792 sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_workspaces.yaml
+-rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 sonyci-0.1.1a0/PKG-INFO
```

### Comparing `sonyci-0.1.1/README.md` & `sonyci-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `sonyci-0.1.1/pyproject.toml` & `sonyci-0.1.1a0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,41 +4,39 @@
 authors = [
     { name = "WGBH-MLA", email = "ryan_harbert@wgbh.org" },
 ]
 dependencies = [
     "pydantic~=1.10",
     "requests-oauth2client~=1.1",
     "loguru~=0.7",
+    "rich~=13.3",
 ]
 requires-python = ">=3.7"
 readme = "README.md"
 dynamic = []
-version = "0.1.1"
+version = "0.1.1a"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 ci = "sonyci.__main__:app"
 
 [project.optional-dependencies]
 test = [
-    "pytest~=7.3",
-    "vcrpy~=4.2",
-    "pytest-vcr~=1.0",
-    "pytest-cov~=4.0",
-    "pytest-sugar~=0.9",
-    "pytest-xdist~=3.2",
+    "pytest>=7.3.1",
+    "vcrpy>=4.2.1",
+    "pytest-vcr>=1.0.2",
+    "pytest-cov>=4.0.0",
+    "pytest-sugar>=0.9.7",
+    "pytest-xdist>=3.2.1",
     "urllib3~=1.26",
 ]
 cli = [
-    "typer[all]>=0.9.0",
-]
-cli-ci = [
-    "typer>=0.9.0",
+    "typer[all]>=0.7.0",
 ]
 docs = [
     "mkdocs~=1.4",
     "mkdocs-material~=9.1",
     "mkdocs-git-revision-date-localized-plugin~=1.2",
     "mike",
     "mkdocstrings[python]~=0.21",
@@ -55,29 +53,21 @@
 source = "file"
 path = "sonyci/_version.py"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "ruff~=0.0",
     "black~=23.3",
-    "pre-commit~=2.21",
+    "pre-commit>=2.21.0",
 ]
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
-markers = [
-    "no_ci: marks tests to skip on CI",
-]
-
-[tool.coverage.run]
-omit = [
-    "tests/*",
-]
 
 [tool.ruff]
 select = [
     "B",
     "C4",
     "C90",
     "E",
```

### Comparing `sonyci-0.1.1/sonyci/cli.py` & `sonyci-0.1.1a0/sonyci/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,36 +18,38 @@
         print(f'v{__version__}')
 
         raise Exit()
 
 
 @app.command()
 def login(
-    ctx: Context,
     username: str = Option(
         ..., '--username', '-u', help='Sony CI username.', envvar='CI_USERNAME'
     ),
     password: str = Option(
         ..., '--password', '-p', help='Sony CI password.', envvar='CI_PASSWORD'
     ),
-    test: bool = Option(False, '--test', '-t', help='Skips saving the token.'),
+    client_id: str = Option(
+        ..., '--client-id', '-c', help='Sony CI client ID.', envvar='CI_CLIENT_ID'
+    ),
+    client_secret: str = Option(
+        ...,
+        '--client-secret',
+        '-s',
+        help='Sony CI client secret.',
+        envvar='CI_CLIENT_SECRET',
+    ),
 ):
     """Login to Sony CI."""
     from sonyci.utils import get_token
 
-    token: BearerToken = get_token(
-        username,
-        password,
-        ctx.parent.params.get('client_id'),
-        ctx.parent.params.get('client_secret'),
-    )
-    if not test:
-        with open('.token', 'w') as f:
-            f.write(BearerTokenSerializer().dumps(token))
-    log.success('logged in to Sony CI!')
+    token: BearerToken = get_token(username, password, client_id, client_secret)
+    with open('.token', 'w') as f:
+        f.write(BearerTokenSerializer().dumps(token))
+        log.success('logged in to Sony CI!')
 
 
 @app.command()
 def get(ctx: Context, path: Annotated[str, Argument(..., help='The path to GET')]):
     """Make a GET request to Sony CI."""
     ci = SonyCi(t=ctx.parent.params['token'])
     log.trace(f'GET {path}')
@@ -100,24 +102,14 @@
     workspace_id: str = Option(
         None,
         '--workspace-id',
         '-w',
         help='Sony CI workspace ID.',
         envvar='CI_WORKSPACE_ID',
     ),
-    client_id: str = Option(
-        None, '--client-id', '-c', help='Sony CI client ID.', envvar='CI_CLIENT_ID'
-    ),
-    client_secret: str = Option(
-        None,
-        '--client-secret',
-        '-s',
-        help='Sony CI client secret.',
-        envvar='CI_CLIENT_SECRET',
-    ),
 ):
     if not verbose:
         log.remove()
     if not token:  # and if command is not login
         log.debug('no token provided, trying to load from .token')
         try:
             with open('.token') as f:
```

### Comparing `sonyci-0.1.1/sonyci/config.py` & `sonyci-0.1.1a0/sonyci/config.py`

 * *Files identical despite different names*

### Comparing `sonyci-0.1.1/sonyci/sonyci.py` & `sonyci-0.1.1a0/sonyci/sonyci.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,18 +60,18 @@
         Example:
             ```py
             ci.client.get('workspaces')
             ```
         """
         return ApiClient(self.base_url, auth=self.auth)
 
-    def workspaces(self) -> list:
+    def workspaces(self):
         return self.get('workspaces')['items']
 
-    def workspace(self) -> dict:
+    def workspace(self):
         """Return response of /workspaces/{workspace_id}"""
         return self.get(f'workspaces/{self.workspace_id}')
 
     def workspace_contents(self, **kwargs) -> list:
         """Returns items form the workspace"""
         return self.get(f'workspaces/{self.workspace_id}/contents', params=kwargs)[
             'items'
@@ -85,18 +85,18 @@
             kwargs['query'] = query
         if not kwargs.get('kind'):
             kwargs['kind'] = 'asset'
         return self.get(f'workspaces/{self.workspace_id}/search', params=kwargs)[
             'items'
         ]
 
-    def asset(self, asset_id: str, **kwargs) -> dict:
+    def asset(self, asset_id: str = None, **kwargs):
         return self.get(f'/assets/{asset_id}', params=kwargs)
 
-    def asset_download(self, asset_id: str, **kwargs) -> dict:
+    def asset_download(self, asset_id: str = None, **kwargs):
         return self.get(f'/assets/{asset_id}/download', params=kwargs)
 
     @json
     def get(self, *args, **kwargs):
         log.debug(f'GET {args} {kwargs}')
         return self.client.get(*args, **kwargs)
```

### Comparing `sonyci-0.1.1/sonyci/utils.py` & `sonyci-0.1.1a0/sonyci/utils.py`

 * *Files identical despite different names*

### Comparing `sonyci-0.1.1/tests/cli/test_cli_login.py` & `sonyci-0.1.1a0/tests/test_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,79 @@
-from pytest import mark
+from pytest import fixture, mark
+from typer.testing import CliRunner
 
+from sonyci import Config
 from sonyci.cli import app
 
 
+@fixture
+def runner():
+    return CliRunner()
+
+
+@fixture
+def error_runner():
+    return CliRunner(mix_stderr=False)
+
+
+@fixture
+def config(pytestconfig):
+    if pytestconfig.getoption('record'):
+        return Config.from_toml('./ci.toml')
+    return Config.from_toml('./tests/sonyci/sonyci.toml')
+
+
 @mark.vcr()
 def test_login(runner, config):
     result = runner.invoke(
         app,
         [
-            '--client-id',
-            config['client_id'],
-            '--client-secret',
-            config['client_secret'],
             'login',
             '--username',
             config['username'],
             '--password',
             config['password'],
-            '--test',
+            '--client-id',
+            config['client_id'],
+            '--client-secret',
+            config['client_secret'],
         ],
     )
     assert result.exit_code == 0
     assert not result.stdout
 
 
 @mark.vcr()
-def test_bad_login(error_runner):
-    result = error_runner.invoke(
+def test_bad_login(runner):
+    result = runner.invoke(
         app,
         [
-            '--client-id',
-            'test',
-            '--client-secret',
-            'test',
             'login',
             '--username',
             'test',
             '--password',
             'test',
-            '--test',
+            '--client-id',
+            'test',
+            '--client-secret',
+            'test',
         ],
     )
     assert result.exit_code == 1
     assert 'invalid_client' in str(result.exception)
 
 
-def test_missing_username(runner):
-    result = runner.invoke(
+def test_missing_username(error_runner):
+    result = error_runner.invoke(
         app,
         [
+            'login',
+            '--password',
+            'test',
             '--client-id',
             'test',
             '--client-secret',
             'test',
-            'login',
-            '--password',
-            'test',
         ],
     )
     assert result.exit_code == 2
-    assert '--username' in result.stdout
+    assert '--username' in result.stderr
```

### Comparing `sonyci-0.1.1/tests/sonyci/test_config.py` & `sonyci-0.1.1a0/tests/sonyci/test_config.py`

 * *Files identical despite different names*

### Comparing `sonyci-0.1.1/tests/test_sonyci.py` & `sonyci-0.1.1a0/tests/test_sonyci.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from pytest import fixture, mark
 
 from sonyci import Config, SonyCi
 
 
 @fixture(scope='module')
+def guid() -> str:
+    return Config.from_toml('./tests/sonyci/guid.toml')['guid']
+
+
+@fixture(scope='module')
 def asset_id():
     return '554544ceaf6b4c94a4a06cee5bc1f39f'
 
 
 @fixture(scope='module')
 def ci_config(pytestconfig):
     if pytestconfig.getoption('record'):
```

### Comparing `sonyci-0.1.1/tests/vhs/test_cli_login/test_bad_login.yaml` & `sonyci-0.1.1a0/tests/vhs/tests.test_cli/test_bad_login.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
       Connection:
       - keep-alive
       Content-Length:
       - '97'
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Thu, 11 May 2023 17:28:02 GMT
+      - Tue, 09 May 2023 17:18:47 GMT
       Expires:
       - '-1'
       Pragma:
       - no-cache
       Strict-Transport-Security:
       - max-age=86400; includeSubDomains
       X-Frame-Options:
```

### Comparing `sonyci-0.1.1/tests/vhs/test_cli_login/test_login.yaml` & `sonyci-0.1.1a0/tests/vhs/tests.test_cli/test_login.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
       Connection:
       - keep-alive
       Content-Length:
       - '143'
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Thu, 11 May 2023 17:28:02 GMT
+      - Tue, 09 May 2023 17:18:47 GMT
       Expires:
       - '-1'
       Pragma:
       - no-cache
       Strict-Transport-Security:
       - max-age=86400; includeSubDomains
       X-Frame-Options:
```

### Comparing `sonyci-0.1.1/tests/vhs/test_cli_search/test_empty_search.yaml` & `sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_workspace_empty_search.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,54 @@
 interactions:
 - request:
+    body: grant_type=password&client_id=FAKE_CLIENT_ID&client_secret=FAKE_CLIENT_SECRET
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '109'
+      Content-Type:
+      - application/x-www-form-urlencoded
+      User-Agent:
+      - python-requests/2.30.0
+      authorization:
+      - Bearer DUMMY
+    method: POST
+    uri: https://api.cimediacloud.com/oauth2/token
+  response:
+    body:
+      string: '{"access_token": "DUMMY_ACCESS_TOKEN", "expires_in": 86400, "token_type":
+        "bearer", "refresh_token": "DUMMY_REFRESH_TOKEN"}'
+    headers:
+      Cache-Control:
+      - no-cache
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '143'
+      Content-Type:
+      - application/json; charset=utf-8
+      Date:
+      - Tue, 09 May 2023 21:15:37 GMT
+      Expires:
+      - '-1'
+      Pragma:
+      - no-cache
+      Strict-Transport-Security:
+      - max-age=86400; includeSubDomains
+      X-Frame-Options:
+      - deny
+    status:
+      code: 200
+      message: OK
+- request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
@@ -25,26 +70,26 @@
       Connection:
       - keep-alive
       Content-Length:
       - '144'
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Thu, 11 May 2023 17:26:36 GMT
+      - Tue, 09 May 2023 21:15:37 GMT
       Expires:
       - '-1'
       Pragma:
       - no-cache
       Strict-Transport-Security:
       - max-age=86400; includeSubDomains
       X-Frame-Options:
       - deny
       X-RateLimit-Limit:
       - '5000'
       X-RateLimit-Remaining:
-      - '4969'
+      - '4984'
       X-RateLimit-Reset:
-      - '1683826020'
+      - '1683666960'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `sonyci-0.1.1/tests/vhs/test_cli_search/test_guid_search.yaml` & `sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_asset.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,76 +1,119 @@
 interactions:
 - request:
+    body: grant_type=password&client_id=FAKE_CLIENT_ID&client_secret=FAKE_CLIENT_SECRET
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '109'
+      Content-Type:
+      - application/x-www-form-urlencoded
+      User-Agent:
+      - python-requests/2.30.0
+      authorization:
+      - Bearer DUMMY
+    method: POST
+    uri: https://api.cimediacloud.com/oauth2/token
+  response:
+    body:
+      string: '{"access_token": "DUMMY_ACCESS_TOKEN", "expires_in": 86400, "token_type":
+        "bearer", "refresh_token": "DUMMY_REFRESH_TOKEN"}'
+    headers:
+      Cache-Control:
+      - no-cache
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '143'
+      Content-Type:
+      - application/json; charset=utf-8
+      Date:
+      - Wed, 10 May 2023 14:39:29 GMT
+      Expires:
+      - '-1'
+      Pragma:
+      - no-cache
+      Strict-Transport-Security:
+      - max-age=86400; includeSubDomains
+      X-Frame-Options:
+      - deny
+    status:
+      code: 200
+      message: OK
+- request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
       - python-requests/2.30.0
       authorization:
       - Bearer DUMMY
     method: GET
-    uri: https://api.cimediacloud.com/workspaces/f44132c2393d470c88b9884f45877ebb/search?query=pb-aacip-e4308199588&kind=asset
+    uri: https://api.cimediacloud.com/assets/554544ceaf6b4c94a4a06cee5bc1f39f
   response:
     body:
-      string: '{"limit": 50, "offset": 0, "count": 1, "kind": "Asset", "type": "All",
-        "query": "pb-aacip-e4308199588", "items": [{"id": "554544ceaf6b4c94a4a06cee5bc1f39f",
-        "name": "cpb-aacip-e4308199588.txt", "size": 16, "createdOn": "2021-08-17T15:13:59.841Z",
-        "thumbnails": [{"type": "medium", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail-medium.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC1tZWRpdW0uanBnIiwiQ29uZGl0aW9uIjp7IklwQWRkcmVzcyI6eyJBV1M6U291cmNlSXAiOiIwLjAuMC4wLzAifSwiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3NDY4OTc5OTd9fX1dfQ__&Signature=SFtjecF7C~pWTCDz9wVqxcfJq~TQT2H7iMMC3i8QHyjTf5rrGlCnm1F3CENRsKMH0HsBY0BRb6IQlDzeEew~YWEFkYr4p2x5h2Sshzt2DoCrMN6a5klrqFdX~rGLwK3Q0d03Sow2HWn~RnR9tSFmEI5IwrVf7ye6k4~Zc6jxZzs_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+      string: '{"id": "554544ceaf6b4c94a4a06cee5bc1f39f", "name": "cpb-aacip-e4308199588.txt",
+        "size": 16, "createdBy": {"id": "16a555d05c60439a8243a3d6c349fd8b", "name":
+        "AAPB Notifications", "email": "aapb_notifications@wgbh.org"}, "createdOn":
+        "2021-08-17T15:13:59.841Z", "thumbnailUrl": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC5qcGciLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc0NjgwMTU2OX19fV19&Signature=GxhOdGcHEWUa0eqDL0NW3Zg959MV4l1KH2pGswLunyc7YLVZyTSuB8pS6rjekCpcoqN5kngg7baHXng4QRCn0sdFkaA2jsEKkbZnd4HSpEfhf-LVA1QZYDN0lR6IMPaAVzq0uVjZefKDmSduhO3~xaVXaWRBf~zAYqaQ8FN9Czw_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+        "proxyUrl": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/document-pdf.pdf?u=16a555d05c60439a8243a3d6c349fd8b&a=554544ceaf6b4c94a4a06cee5bc1f39f&ct=abb0668d5b054200b6a89c3826024e42&et=stream&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL2RvY3VtZW50LXBkZi5wZGY~dT0xNmE1NTVkMDVjNjA0MzlhODI0M2EzZDZjMzQ5ZmQ4YiZhPTU1NDU0NGNlYWY2YjRjOTRhNGEwNmNlZTViYzFmMzlmJmN0PWFiYjA2NjhkNWIwNTQyMDBiNmE4OWMzODI2MDI0ZTQyJmV0PXN0cmVhbSIsIkNvbmRpdGlvbiI6eyJJcEFkZHJlc3MiOnsiQVdTOlNvdXJjZUlwIjoiMC4wLjAuMC8wIn0sIkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNjgzNzcyNzY5fX19XX0_&Signature=JmoVYhXkUtnZkWG6X4IF8lVxMd8Iv4E6l-FfVjHOkteK7hoMhcwkUn8n4Q6rSibUKhAt8z05dCvpZRZmIyI3LnSjmoI0vkBCQlt2N6zf1NcLeali8cS2BxwCDRhm9Aj9X5eCkiRD6otzKfJwlLPZ3LCbvWW2oVkV9aMYa4nTMy8_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+        "type": "Document", "format": "txt", "status": "Complete", "folder": {"id":
+        "d870616520634dbc8eb8caec141188fa", "name": "Workspace"}, "modifiedOn": "2021-08-17T15:14:43.43Z",
+        "md5Checksum": "23211babeacb8adf336194eaca77f510", "clipSource": {}, "technicalMetadata":
+        {}, "archiveStatus": "Not archived", "restoreStatus": "Not restored", "isDeleted":
+        false, "isTrashed": false, "fileRequest": {}, "lastActivityOn": "2021-08-17T15:14:43.32Z",
+        "uploadCompleteDate": "2021-08-17T15:13:59.966Z", "uploadTransferType": "SinglepartHttp",
+        "thumbnails": [{"type": "medium", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail-medium.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC1tZWRpdW0uanBnIiwiQ29uZGl0aW9uIjp7IklwQWRkcmVzcyI6eyJBV1M6U291cmNlSXAiOiIwLjAuMC4wLzAifSwiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3NDY4MDE1Njl9fX1dfQ__&Signature=jlUaS2pF28BRI3cqoritBB8nt34eVxmN-tuW7PpAxsOYJWP0s~WWtPtLRSpc6UtS3YSB8eDPQvJAyv--MI2-EXtkZyFs9Q3izNwyHwEDdogsdRLppjnM7uX-j-i8X-CZnOIeIpEj6gTTySFkbQHixa69XuV5ealSi2xHCHJTmXs_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
         "size": 3554, "width": 433, "height": 560, "isExternal": false}, {"type":
-        "large", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail-large.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC1sYXJnZS5qcGciLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc0Njg5Nzk5N319fV19&Signature=fSG3h4wDG9nT-4IyWqa813ajZ7mVfsd677hFxhabtZN2UOnMOJ2QeGBUz6qWvkzmDydcRj380TKB6VH4r8nEkP3y8H92hymlNiSdXaAWYxa3SLmfVkeNOLEOp4OZwL0mXzSX~5S6e8Fi4Tok4jlL3p9svIhBY0kSVLvrhXW0e8Y_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+        "large", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail-large.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC1sYXJnZS5qcGciLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc0NjgwMTU2OX19fV19&Signature=CEcLgZg9xrHkG~Fj1KTC~YHJc~gTsVsJli0VW0rYxvzPX-yJ64PxH7y6Z72COl-ICKYv6qJ41IuPH2cjjYc6qtZBT0ZzTa6D4mSCDu8W17eKVMcYTYiLfj7bvITwC3yQVLBtXLvLtKoVml~iUBT7UmULDfbqodbXzoOaotHD1CM_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
         "size": 7208, "width": 612, "height": 792, "isExternal": false}, {"type":
-        "2000px", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail-2000px.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC0yMDAwcHguanBnIiwiQ29uZGl0aW9uIjp7IklwQWRkcmVzcyI6eyJBV1M6U291cmNlSXAiOiIwLjAuMC4wLzAifSwiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3NDY4OTc5OTd9fX1dfQ__&Signature=KS~a0qL5a-46kzduKyyeuZs3r6T6CugxvTbmxrWjjGNBrBx9r9wWQsQh-x4~c-w2U-Rw1UOX54pD3wyeDPxW8u0cJp3BNNrmUXaqIA65HcI167AaP42VDk5wnNDj0EZxQ1bKwQSYk8M3cxbOlRjX3092Cz2f1ak5qp4U34QfoVU_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+        "2000px", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail-2000px.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC0yMDAwcHguanBnIiwiQ29uZGl0aW9uIjp7IklwQWRkcmVzcyI6eyJBV1M6U291cmNlSXAiOiIwLjAuMC4wLzAifSwiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3NDY4MDE1Njl9fX1dfQ__&Signature=jia6vJ3tw0TUWThj-AlavAeufrs3hvUaSPwby86NoxBQnvtV~yZuKx4Yojcc9FZxa7BVkX0z7J3cBJ-3KUeEVjM4p6ljp7yjGQr-LrK4O-vlnYiR0TiuwKIL2sgXDzYnn1FlXLP38dI98~q0J5VwLOiJUe0u4HaQ5K6Oe9iAHio_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
         "size": 7208, "width": 612, "height": 792, "isExternal": false}, {"type":
-        "small", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC5qcGciLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc0Njg5Nzk5N319fV19&Signature=XImPzv3WB23Ug34HD8iFwd7ARCl1yom2pyXK-ML0QH5rxzW40oeY953-fsvLf9fxW79D5CtE7mIGYoUu3NVjLzscShXv83wdKeLp~ib9tCvsK~3o7mjSiZTM1Yrv8B2WPNYlMos8OJsyQqjdkpkFT1g5G3FQCt6bN3NS3jVPnBI_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+        "small", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC5qcGciLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc0NjgwMTU2OX19fV19&Signature=GxhOdGcHEWUa0eqDL0NW3Zg959MV4l1KH2pGswLunyc7YLVZyTSuB8pS6rjekCpcoqN5kngg7baHXng4QRCn0sdFkaA2jsEKkbZnd4HSpEfhf-LVA1QZYDN0lR6IMPaAVzq0uVjZefKDmSduhO3~xaVXaWRBf~zAYqaQ8FN9Czw_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
         "size": 1038, "width": 193, "height": 250, "isExternal": false}, {"type":
-        "standard", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC5qcGciLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc0Njg5Nzk5N319fV19&Signature=XImPzv3WB23Ug34HD8iFwd7ARCl1yom2pyXK-ML0QH5rxzW40oeY953-fsvLf9fxW79D5CtE7mIGYoUu3NVjLzscShXv83wdKeLp~ib9tCvsK~3o7mjSiZTM1Yrv8B2WPNYlMos8OJsyQqjdkpkFT1g5G3FQCt6bN3NS3jVPnBI_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+        "standard", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC5qcGciLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc0NjgwMTU2OX19fV19&Signature=GxhOdGcHEWUa0eqDL0NW3Zg959MV4l1KH2pGswLunyc7YLVZyTSuB8pS6rjekCpcoqN5kngg7baHXng4QRCn0sdFkaA2jsEKkbZnd4HSpEfhf-LVA1QZYDN0lR6IMPaAVzq0uVjZefKDmSduhO3~xaVXaWRBf~zAYqaQ8FN9Czw_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
         "size": 1038, "width": 193, "height": 250}], "proxies": [{"type": "document-pdf",
-        "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/document-pdf.pdf?u=16a555d05c60439a8243a3d6c349fd8b&a=554544ceaf6b4c94a4a06cee5bc1f39f&ct=abb0668d5b054200b6a89c3826024e42&et=stream&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL2RvY3VtZW50LXBkZi5wZGY~dT0xNmE1NTVkMDVjNjA0MzlhODI0M2EzZDZjMzQ5ZmQ4YiZhPTU1NDU0NGNlYWY2YjRjOTRhNGEwNmNlZTViYzFmMzlmJmN0PWFiYjA2NjhkNWIwNTQyMDBiNmE4OWMzODI2MDI0ZTQyJmV0PXN0cmVhbSIsIkNvbmRpdGlvbiI6eyJJcEFkZHJlc3MiOnsiQVdTOlNvdXJjZUlwIjoiMC4wLjAuMC8wIn0sIkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNjgzODY5MTk3fX19XX0_&Signature=boSX5Wi7lAvoC-hfX6E0oNIQtdOc7K6fTFMP9EhTjUjxxSZ3FFpT6dI31~RjC1sTVmEbeazVym2dMKBVphBHXdM-bGRB4ZbYNRFZqBrNKcco6o17CpD5cY72yQcpXHgZlXEmEUsP~S7LaFjQFGKAFz11odfHgzm5bmdrE-5t1iA_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
-        "size": 7172, "isExternal": false}], "type": "Document", "format": "txt",
-        "status": "Complete", "lastActivityOn": "2023-05-11T17:25:47.652Z", "modifiedOn":
-        "2021-08-17T15:14:43.43Z", "md5Checksum": "23211babeacb8adf336194eaca77f510",
-        "clipSource": {}, "technicalMetadata": {}, "archiveStatus": "Not archived",
-        "restoreStatus": "Not restored", "uploadCompleteDate": "2021-08-17T15:13:59.966Z",
-        "isTrashed": false, "isFavorite": false, "isExternal": false, "uploadTransferType":
-        "SinglepartHttp", "folder": {"id": "d870616520634dbc8eb8caec141188fa", "name":
-        "Workspace"}, "workspace": {"id": "f44132c2393d470c88b9884f45877ebb", "name":
+        "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/document-pdf.pdf?u=16a555d05c60439a8243a3d6c349fd8b&a=554544ceaf6b4c94a4a06cee5bc1f39f&ct=abb0668d5b054200b6a89c3826024e42&et=stream&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL2RvY3VtZW50LXBkZi5wZGY~dT0xNmE1NTVkMDVjNjA0MzlhODI0M2EzZDZjMzQ5ZmQ4YiZhPTU1NDU0NGNlYWY2YjRjOTRhNGEwNmNlZTViYzFmMzlmJmN0PWFiYjA2NjhkNWIwNTQyMDBiNmE4OWMzODI2MDI0ZTQyJmV0PXN0cmVhbSIsIkNvbmRpdGlvbiI6eyJJcEFkZHJlc3MiOnsiQVdTOlNvdXJjZUlwIjoiMC4wLjAuMC8wIn0sIkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNjgzNzcyNzY5fX19XX0_&Signature=JmoVYhXkUtnZkWG6X4IF8lVxMd8Iv4E6l-FfVjHOkteK7hoMhcwkUn8n4Q6rSibUKhAt8z05dCvpZRZmIyI3LnSjmoI0vkBCQlt2N6zf1NcLeali8cS2BxwCDRhm9Aj9X5eCkiRD6otzKfJwlLPZ3LCbvWW2oVkV9aMYa4nTMy8_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+        "size": 7172, "isExternal": false}], "acquisitionSource": {"name": "American
+        Archive"}, "workspace": {"id": "f44132c2393d470c88b9884f45877ebb", "name":
         "My Workspace", "class": "Personal"}, "network": {"id": "70c6959f648a428096c88906b6655773",
         "name": "AAPB''s Network", "class": "Personal"}, "filmstrips": [], "waveforms":
-        [], "mediaAnalyses": [], "acquisitionSource": {"name": "American Archive"},
-        "totalFolderCount": 1, "isTimedTextMatch": false, "kind": "Asset", "createdBy":
-        {"id": "16a555d05c60439a8243a3d6c349fd8b", "name": "AAPB Notifications", "email":
-        "aapb_notifications@wgbh.org"}}], "order": {"by": "Relevance", "direction":
-        "Desc"}}'
+        [], "mediaAnalyses": [], "isExternal": false, "isFavorite": false}'
     headers:
       Cache-Control:
       - no-cache
       Connection:
       - keep-alive
       Content-Length:
-      - '5785'
+      - '7152'
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Thu, 11 May 2023 17:26:37 GMT
+      - Wed, 10 May 2023 14:39:29 GMT
       Expires:
       - '-1'
       Pragma:
       - no-cache
       Strict-Transport-Security:
       - max-age=86400; includeSubDomains
       X-Frame-Options:
       - deny
       X-RateLimit-Limit:
       - '5000'
       X-RateLimit-Remaining:
-      - '4968'
+      - '4964'
       X-RateLimit-Reset:
-      - '1683826020'
+      - '1683729600'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `sonyci-0.1.1/tests/vhs/tests.test_sonyci/test_asset.yaml` & `sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_asset_download.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -28,15 +28,15 @@
       Connection:
       - keep-alive
       Content-Length:
       - '143'
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Fri, 12 May 2023 22:12:50 GMT
+      - Wed, 10 May 2023 15:02:37 GMT
       Expires:
       - '-1'
       Pragma:
       - no-cache
       Strict-Transport-Security:
       - max-age=86400; includeSubDomains
       X-Frame-Options:
@@ -54,66 +54,53 @@
       Connection:
       - keep-alive
       User-Agent:
       - python-requests/2.30.0
       authorization:
       - Bearer DUMMY
     method: GET
-    uri: https://api.cimediacloud.com/assets/554544ceaf6b4c94a4a06cee5bc1f39f
+    uri: https://api.cimediacloud.com/assets/554544ceaf6b4c94a4a06cee5bc1f39f/download
   response:
     body:
-      string: '{"id": "554544ceaf6b4c94a4a06cee5bc1f39f", "name": "cpb-aacip-e4308199588.txt",
-        "size": 16, "createdBy": {"id": "16a555d05c60439a8243a3d6c349fd8b", "name":
-        "AAPB Notifications", "email": "aapb_notifications@wgbh.org"}, "createdOn":
-        "2021-08-17T15:13:59.841Z", "thumbnailUrl": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC5qcGciLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc0NzAwMTU3MH19fV19&Signature=MpI2R-xeM2e63IE3a5S90hHfZFXU60yZ6YgEceJAZp9KZsfUZ3Sg5Mcgt1FtQ8sVAm5csSbp3HeHagpst9GHb8yUzQF7nKLWpWPGZWlCmS5nSV7gvmesfOalsdrnwYxBiYcFxqRhIp38sbp2RR6lIe802xRBSh-mboJpsScNRr8_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
-        "proxyUrl": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/document-pdf.pdf?u=16a555d05c60439a8243a3d6c349fd8b&a=554544ceaf6b4c94a4a06cee5bc1f39f&ct=abb0668d5b054200b6a89c3826024e42&et=stream&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL2RvY3VtZW50LXBkZi5wZGY~dT0xNmE1NTVkMDVjNjA0MzlhODI0M2EzZDZjMzQ5ZmQ4YiZhPTU1NDU0NGNlYWY2YjRjOTRhNGEwNmNlZTViYzFmMzlmJmN0PWFiYjA2NjhkNWIwNTQyMDBiNmE4OWMzODI2MDI0ZTQyJmV0PXN0cmVhbSIsIkNvbmRpdGlvbiI6eyJJcEFkZHJlc3MiOnsiQVdTOlNvdXJjZUlwIjoiMC4wLjAuMC8wIn0sIkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNjgzOTcyNzcwfX19XX0_&Signature=Lbi-O1peWq9x1qgsy2va8kygx4zYLxYeCrF5ChDtkmnCKgWVy8f7Qw84PDd2Nsz2PQiHraXaDWIvk6KNFcVSsEszkvCCId-CtzXc2-6qoP8wkApCUrtFynwMgoA9zU1JgyKc84AwVRttPZlca7ERL7cEItoz03Rl9IwR69X2MSE_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
-        "type": "Document", "format": "txt", "status": "Complete", "folder": {"id":
-        "d870616520634dbc8eb8caec141188fa", "name": "Workspace"}, "modifiedOn": "2021-08-17T15:14:43.43Z",
-        "md5Checksum": "23211babeacb8adf336194eaca77f510", "clipSource": {}, "technicalMetadata":
-        {}, "archiveStatus": "Not archived", "restoreStatus": "Not restored", "isDeleted":
-        false, "isTrashed": false, "fileRequest": {}, "lastActivityOn": "2023-05-12T22:11:52.587Z",
-        "uploadCompleteDate": "2021-08-17T15:13:59.966Z", "uploadTransferType": "SinglepartHttp",
-        "thumbnails": [{"type": "medium", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail-medium.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC1tZWRpdW0uanBnIiwiQ29uZGl0aW9uIjp7IklwQWRkcmVzcyI6eyJBV1M6U291cmNlSXAiOiIwLjAuMC4wLzAifSwiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3NDcwMDE1NzB9fX1dfQ__&Signature=CakYTxApCcot0MZHnzfnP~fhG200Kuj0A3IDylAtPMg~HIDY2POTDhoAs2xnQDffUY8WnH20vjdXcvBbmy7vFut-VbPlCDtb3FUZyv7pTMTrM7uG7ycR4l9Gzh7qXMv6H8GWM85pFbnPkTuxgUmerlYHlubFpq8uC32D6NdvHcM_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+      string: '{"location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/cpb-aacip-e4308199588.txt?response-content-disposition=attachment%3Bfilename%3D%22cpb-aacip-e4308199588.txt%22&u=16a555d05c60439a8243a3d6c349fd8b&a=554544ceaf6b4c94a4a06cee5bc1f39f&ct=abb0668d5b054200b6a89c3826024e42&et=download&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9jcGItYWFjaXAtZTQzMDgxOTk1ODgudHh0P3Jlc3BvbnNlLWNvbnRlbnQtZGlzcG9zaXRpb249YXR0YWNobWVudCUzQmZpbGVuYW1lJTNEJTIyY3BiLWFhY2lwLWU0MzA4MTk5NTg4LnR4dCUyMiZ1PTE2YTU1NWQwNWM2MDQzOWE4MjQzYTNkNmMzNDlmZDhiJmE9NTU0NTQ0Y2VhZjZiNGM5NGE0YTA2Y2VlNWJjMWYzOWYmY3Q9YWJiMDY2OGQ1YjA1NDIwMGI2YTg5YzM4MjYwMjRlNDImZXQ9ZG93bmxvYWQiLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTY4Mzc0MTc1N319fV19&Signature=Rm1BDupZhapmUTSc23l1aK0RtnbIYB3Pqci0xIBB9SKIGcHA6w3rfr6eFp6T2b6sjjBpgKjTFnjjtZveA4iS5geZzgurUaDwrBAqi6p3e0Zw6TAi2PF2SfSxlaal6c8QLOjOVTOn6T~1Q5~Oj6BUy57W2BpqcY-e-JdTbjcsyKs_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+        "id": "554544ceaf6b4c94a4a06cee5bc1f39f", "size": 16, "proxies": [{"type":
+        "document-pdf", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/document-pdf.pdf?response-content-disposition=attachment%3Bfilename%3D%22cpb-aacip-e4308199588-.pdf%22&u=16a555d05c60439a8243a3d6c349fd8b&a=554544ceaf6b4c94a4a06cee5bc1f39f&ct=abb0668d5b054200b6a89c3826024e42&et=download&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL2RvY3VtZW50LXBkZi5wZGY~cmVzcG9uc2UtY29udGVudC1kaXNwb3NpdGlvbj1hdHRhY2htZW50JTNCZmlsZW5hbWUlM0QlMjJjcGItYWFjaXAtZTQzMDgxOTk1ODgtLnBkZiUyMiZ1PTE2YTU1NWQwNWM2MDQzOWE4MjQzYTNkNmMzNDlmZDhiJmE9NTU0NTQ0Y2VhZjZiNGM5NGE0YTA2Y2VlNWJjMWYzOWYmY3Q9YWJiMDY2OGQ1YjA1NDIwMGI2YTg5YzM4MjYwMjRlNDImZXQ9ZG93bmxvYWQiLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTY4Mzc0MTc1N319fV19&Signature=SRW19usG1qPq9G4V9He09KokPUm8egdgB9g1H~KATi5kGQ2fw5p-Utl~CnyPxQ1sCA5jRjgsI~ElOQpofHnp8oVSxqLH9LdNIhGosNASdXzkyONPArbFHPI3tAQMJjQ9ffJ5UfpJQU6FSjj3j1UPXWWu2teMn5Zhh42IG1bEVFk_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+        "size": 7172, "isExternal": false}], "thumbnails": [{"type": "medium", "location":
+        "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail-medium.jpg?response-content-disposition=attachment%3Bfilename%3D%22cpb-aacip-e4308199588_433x560_thumbnail.jpg%22&u=16a555d05c60439a8243a3d6c349fd8b&a=554544ceaf6b4c94a4a06cee5bc1f39f&ct=abb0668d5b054200b6a89c3826024e42&et=download&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC1tZWRpdW0uanBnP3Jlc3BvbnNlLWNvbnRlbnQtZGlzcG9zaXRpb249YXR0YWNobWVudCUzQmZpbGVuYW1lJTNEJTIyY3BiLWFhY2lwLWU0MzA4MTk5NTg4XzQzM3g1NjBfdGh1bWJuYWlsLmpwZyUyMiZ1PTE2YTU1NWQwNWM2MDQzOWE4MjQzYTNkNmMzNDlmZDhiJmE9NTU0NTQ0Y2VhZjZiNGM5NGE0YTA2Y2VlNWJjMWYzOWYmY3Q9YWJiMDY2OGQ1YjA1NDIwMGI2YTg5YzM4MjYwMjRlNDImZXQ9ZG93bmxvYWQiLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTY4Mzc0MTc1N319fV19&Signature=XMSCoQAZHYPO47DfuAmHfU9C9P~P72dJJ31jSY35FwoOwoerhY~jIBYRoABOHyyI-9ZVjn5oTmP4PnMIkVj1q3BOHG01dkYc9IQjkY3pSVXRHuA7JHDNsi7WWURxMMii8O40RAgIWxqTnHj3Z5mCnqkS9N4njRxS1jAK1aEb8Mo_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
         "size": 3554, "width": 433, "height": 560, "isExternal": false}, {"type":
-        "large", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail-large.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC1sYXJnZS5qcGciLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc0NzAwMTU3MH19fV19&Signature=bX8zzuto4zztd9u8jfHjl837utXuAsPOUztqbclwG3dnIxfcy5YsFb76M-YwMZtVXElYLHzTS8bztOl~5dS~i7CqLorcgNPWiPChUqpEYDZYh309rNWRpCi-XcfpCwVJm8TtVvcCBGw2i1-nhSP2QRCff1sdQ9MUoBXzi3DJQBE_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+        "large", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail-large.jpg?response-content-disposition=attachment%3Bfilename%3D%22cpb-aacip-e4308199588_612x792_thumbnail.jpg%22&u=16a555d05c60439a8243a3d6c349fd8b&a=554544ceaf6b4c94a4a06cee5bc1f39f&ct=abb0668d5b054200b6a89c3826024e42&et=download&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC1sYXJnZS5qcGc~cmVzcG9uc2UtY29udGVudC1kaXNwb3NpdGlvbj1hdHRhY2htZW50JTNCZmlsZW5hbWUlM0QlMjJjcGItYWFjaXAtZTQzMDgxOTk1ODhfNjEyeDc5Ml90aHVtYm5haWwuanBnJTIyJnU9MTZhNTU1ZDA1YzYwNDM5YTgyNDNhM2Q2YzM0OWZkOGImYT01NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5ZiZjdD1hYmIwNjY4ZDViMDU0MjAwYjZhODljMzgyNjAyNGU0MiZldD1kb3dubG9hZCIsIkNvbmRpdGlvbiI6eyJJcEFkZHJlc3MiOnsiQVdTOlNvdXJjZUlwIjoiMC4wLjAuMC8wIn0sIkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNjgzNzQxNzU3fX19XX0_&Signature=BzxMTTlMxeksXAy3BRBZUomyXku21fy7w3Gso8xhhr8eSeFvU7CLoLWN~ApyLAPC7Bj-mRwpko18pwjiRrDcLovLvXk1rIxnjCWyCaXSK2K6eIHfdv9RwNv45M6uRNAF05Ib-xGYptaGACSJNR3~We2bPmXvDRdE8WOnQ7Z-RIw_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
         "size": 7208, "width": 612, "height": 792, "isExternal": false}, {"type":
-        "2000px", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail-2000px.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC0yMDAwcHguanBnIiwiQ29uZGl0aW9uIjp7IklwQWRkcmVzcyI6eyJBV1M6U291cmNlSXAiOiIwLjAuMC4wLzAifSwiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3NDcwMDE1NzB9fX1dfQ__&Signature=ikmYtDJB6sox8RU0aEqsRqD2fJYiB88fE8iZzAITg4EoKWbxG8sX1zWIwzVokcbypcJCHLyqqqYU1LinPAYmbGkhV7HXOl-joU0NPDKXsu9hcemeMtzkjvFvsQqQ4DNkgoT8mKTgonDBaXxv1wS1ULgtRwxdfHxq4Q1d9y0AyJk_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+        "2000px", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail-2000px.jpg?response-content-disposition=attachment%3Bfilename%3D%22cpb-aacip-e4308199588_612x792_thumbnail.jpg%22&u=16a555d05c60439a8243a3d6c349fd8b&a=554544ceaf6b4c94a4a06cee5bc1f39f&ct=abb0668d5b054200b6a89c3826024e42&et=download&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC0yMDAwcHguanBnP3Jlc3BvbnNlLWNvbnRlbnQtZGlzcG9zaXRpb249YXR0YWNobWVudCUzQmZpbGVuYW1lJTNEJTIyY3BiLWFhY2lwLWU0MzA4MTk5NTg4XzYxMng3OTJfdGh1bWJuYWlsLmpwZyUyMiZ1PTE2YTU1NWQwNWM2MDQzOWE4MjQzYTNkNmMzNDlmZDhiJmE9NTU0NTQ0Y2VhZjZiNGM5NGE0YTA2Y2VlNWJjMWYzOWYmY3Q9YWJiMDY2OGQ1YjA1NDIwMGI2YTg5YzM4MjYwMjRlNDImZXQ9ZG93bmxvYWQiLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTY4Mzc0MTc1N319fV19&Signature=YRC9J36S6PBIwKzW2SXaSZ6H9lhR0dhg09HvY5HOCSIK2KPt7mz5L0BOaNKkBR1cy2BoZduhe0v26r30GfKWEojcR9EcHZvC2PBFuixEWYAGc8uH6a5nOwWYomIXi-Vknn-0W7QXudSWf4zXy30fH-cxwNDgDix2MZTaTHI7NOQ_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
         "size": 7208, "width": 612, "height": 792, "isExternal": false}, {"type":
-        "small", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC5qcGciLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc0NzAwMTU3MH19fV19&Signature=MpI2R-xeM2e63IE3a5S90hHfZFXU60yZ6YgEceJAZp9KZsfUZ3Sg5Mcgt1FtQ8sVAm5csSbp3HeHagpst9GHb8yUzQF7nKLWpWPGZWlCmS5nSV7gvmesfOalsdrnwYxBiYcFxqRhIp38sbp2RR6lIe802xRBSh-mboJpsScNRr8_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+        "small", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail.jpg?response-content-disposition=attachment%3Bfilename%3D%22cpb-aacip-e4308199588_193x250_thumbnail.jpg%22&u=16a555d05c60439a8243a3d6c349fd8b&a=554544ceaf6b4c94a4a06cee5bc1f39f&ct=abb0668d5b054200b6a89c3826024e42&et=download&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC5qcGc~cmVzcG9uc2UtY29udGVudC1kaXNwb3NpdGlvbj1hdHRhY2htZW50JTNCZmlsZW5hbWUlM0QlMjJjcGItYWFjaXAtZTQzMDgxOTk1ODhfMTkzeDI1MF90aHVtYm5haWwuanBnJTIyJnU9MTZhNTU1ZDA1YzYwNDM5YTgyNDNhM2Q2YzM0OWZkOGImYT01NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5ZiZjdD1hYmIwNjY4ZDViMDU0MjAwYjZhODljMzgyNjAyNGU0MiZldD1kb3dubG9hZCIsIkNvbmRpdGlvbiI6eyJJcEFkZHJlc3MiOnsiQVdTOlNvdXJjZUlwIjoiMC4wLjAuMC8wIn0sIkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNjgzNzQxNzU3fX19XX0_&Signature=flDPudAOVIRKhzjj1OUlMYa3t1QVE~hoy0tDOv21jIonlPzX-ZNp4-VPncN0~iFlHL6qItyBrF5DvuGqEg~ymv~epW4LfYREcghQIWMRL~hlNQODeKGnJk~ddRvxibbXCCEcwPtogKk5J9z5MyA0moOAch2oRN--aCtsxXPjoV4_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
         "size": 1038, "width": 193, "height": 250, "isExternal": false}, {"type":
-        "standard", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail.jpg?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC5qcGciLCJDb25kaXRpb24iOnsiSXBBZGRyZXNzIjp7IkFXUzpTb3VyY2VJcCI6IjAuMC4wLjAvMCJ9LCJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc0NzAwMTU3MH19fV19&Signature=MpI2R-xeM2e63IE3a5S90hHfZFXU60yZ6YgEceJAZp9KZsfUZ3Sg5Mcgt1FtQ8sVAm5csSbp3HeHagpst9GHb8yUzQF7nKLWpWPGZWlCmS5nSV7gvmesfOalsdrnwYxBiYcFxqRhIp38sbp2RR6lIe802xRBSh-mboJpsScNRr8_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
-        "size": 1038, "width": 193, "height": 250}], "proxies": [{"type": "document-pdf",
-        "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/document-pdf.pdf?u=16a555d05c60439a8243a3d6c349fd8b&a=554544ceaf6b4c94a4a06cee5bc1f39f&ct=abb0668d5b054200b6a89c3826024e42&et=stream&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL2RvY3VtZW50LXBkZi5wZGY~dT0xNmE1NTVkMDVjNjA0MzlhODI0M2EzZDZjMzQ5ZmQ4YiZhPTU1NDU0NGNlYWY2YjRjOTRhNGEwNmNlZTViYzFmMzlmJmN0PWFiYjA2NjhkNWIwNTQyMDBiNmE4OWMzODI2MDI0ZTQyJmV0PXN0cmVhbSIsIkNvbmRpdGlvbiI6eyJJcEFkZHJlc3MiOnsiQVdTOlNvdXJjZUlwIjoiMC4wLjAuMC8wIn0sIkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNjgzOTcyNzcwfX19XX0_&Signature=Lbi-O1peWq9x1qgsy2va8kygx4zYLxYeCrF5ChDtkmnCKgWVy8f7Qw84PDd2Nsz2PQiHraXaDWIvk6KNFcVSsEszkvCCId-CtzXc2-6qoP8wkApCUrtFynwMgoA9zU1JgyKc84AwVRttPZlca7ERL7cEItoz03Rl9IwR69X2MSE_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
-        "size": 7172, "isExternal": false}], "acquisitionSource": {"name": "American
-        Archive"}, "workspace": {"id": "f44132c2393d470c88b9884f45877ebb", "name":
-        "My Workspace", "class": "Personal"}, "network": {"id": "70c6959f648a428096c88906b6655773",
-        "name": "AAPB''s Network", "class": "Personal"}, "filmstrips": [], "waveforms":
-        [], "mediaAnalyses": [], "isExternal": false, "isFavorite": false}'
+        "standard", "location": "https://cdn01.cimediacloud.com/cifiles/554544ceaf6b4c94a4a06cee5bc1f39f/renditions/thumbnail.jpg?response-content-disposition=attachment%3Bfilename%3D%22cpb-aacip-e4308199588_193x250_thumbnail.jpg%22&u=16a555d05c60439a8243a3d6c349fd8b&a=554544ceaf6b4c94a4a06cee5bc1f39f&ct=abb0668d5b054200b6a89c3826024e42&et=download&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiKjovL2NkbjAxLmNpbWVkaWFjbG91ZC5jb20vY2lmaWxlcy81NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5Zi9yZW5kaXRpb25zL3RodW1ibmFpbC5qcGc~cmVzcG9uc2UtY29udGVudC1kaXNwb3NpdGlvbj1hdHRhY2htZW50JTNCZmlsZW5hbWUlM0QlMjJjcGItYWFjaXAtZTQzMDgxOTk1ODhfMTkzeDI1MF90aHVtYm5haWwuanBnJTIyJnU9MTZhNTU1ZDA1YzYwNDM5YTgyNDNhM2Q2YzM0OWZkOGImYT01NTQ1NDRjZWFmNmI0Yzk0YTRhMDZjZWU1YmMxZjM5ZiZjdD1hYmIwNjY4ZDViMDU0MjAwYjZhODljMzgyNjAyNGU0MiZldD1kb3dubG9hZCIsIkNvbmRpdGlvbiI6eyJJcEFkZHJlc3MiOnsiQVdTOlNvdXJjZUlwIjoiMC4wLjAuMC8wIn0sIkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNjgzNzQxNzU3fX19XX0_&Signature=flDPudAOVIRKhzjj1OUlMYa3t1QVE~hoy0tDOv21jIonlPzX-ZNp4-VPncN0~iFlHL6qItyBrF5DvuGqEg~ymv~epW4LfYREcghQIWMRL~hlNQODeKGnJk~ddRvxibbXCCEcwPtogKk5J9z5MyA0moOAch2oRN--aCtsxXPjoV4_&Key-Pair-Id=APKAJNUSFH4IKQRZ44WA",
+        "size": 1038, "width": 193, "height": 250}]}'
     headers:
       Cache-Control:
       - no-cache
       Connection:
       - keep-alive
       Content-Length:
-      - '7153'
+      - '8482'
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Fri, 12 May 2023 22:12:50 GMT
+      - Wed, 10 May 2023 15:02:37 GMT
       Expires:
       - '-1'
       Pragma:
       - no-cache
       Strict-Transport-Security:
       - max-age=86400; includeSubDomains
       X-Frame-Options:
       - deny
       X-RateLimit-Limit:
       - '5000'
       X-RateLimit-Remaining:
-      - '4975'
+      - '4966'
       X-RateLimit-Reset:
-      - '1683929580'
+      - '1683730980'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `sonyci-0.1.1/tests/vhs/tests.test_sonyci/test_token.yaml` & `sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_token.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
       Connection:
       - keep-alive
       Content-Length:
       - '143'
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Fri, 12 May 2023 22:12:42 GMT
+      - Mon, 08 May 2023 20:34:35 GMT
       Expires:
       - '-1'
       Pragma:
       - no-cache
       Strict-Transport-Security:
       - max-age=86400; includeSubDomains
       X-Frame-Options:
```

### Comparing `sonyci-0.1.1/tests/vhs/tests.test_sonyci/test_workspace.yaml` & `sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_workspace.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         Connection:
           - keep-alive
         Content-Length:
           - '143'
         Content-Type:
           - application/json; charset=utf-8
         Date:
-          - Fri, 12 May 2023 22:12:45 GMT
+          - Mon, 08 May 2023 20:34:36 GMT
         Expires:
           - '-1'
         Pragma:
           - no-cache
         Strict-Transport-Security:
           - max-age=86400; includeSubDomains
         X-Frame-Options:
@@ -58,39 +58,37 @@
           - python-requests/2.30.0
         authorization:
           - Bearer DUMMY
       method: GET
       uri: https://api.cimediacloud.com/workspaces/f44132c2393d470c88b9884f45877ebb
     response:
       body:
-        string:
-          '{"name": "My Workspace", "id": "f44132c2393d470c88b9884f45877ebb",
-          "assetCount": 12}'
+        string: '{"name": "My Workspace", "id": "f44132c2393d470c88b9884f45877ebb"}'
       headers:
         Cache-Control:
           - no-cache
         Connection:
           - keep-alive
         Content-Length:
           - '3062'
         Content-Type:
           - application/json; charset=utf-8
         Date:
-          - Fri, 12 May 2023 22:12:46 GMT
+          - Mon, 08 May 2023 20:34:37 GMT
         Expires:
           - '-1'
         Pragma:
           - no-cache
         Strict-Transport-Security:
           - max-age=86400; includeSubDomains
         X-Frame-Options:
           - deny
         X-RateLimit-Limit:
           - '5000'
         X-RateLimit-Remaining:
-          - '4979'
+          - '4984'
         X-RateLimit-Reset:
-          - '1683929580'
+          - '1683578100'
       status:
         code: 200
         message: OK
 version: 1
```

### Comparing `sonyci-0.1.1/tests/vhs/tests.test_sonyci/test_workspace_contents.yaml` & `sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_workspaces.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         Connection:
           - keep-alive
         Content-Length:
           - '143'
         Content-Type:
           - application/json; charset=utf-8
         Date:
-          - Fri, 12 May 2023 22:12:46 GMT
+          - Mon, 08 May 2023 20:34:35 GMT
         Expires:
           - '-1'
         Pragma:
           - no-cache
         Strict-Transport-Security:
           - max-age=86400; includeSubDomains
         X-Frame-Options:
@@ -55,43 +55,42 @@
         Connection:
           - keep-alive
         User-Agent:
           - python-requests/2.30.0
         authorization:
           - Bearer DUMMY
       method: GET
-      uri: https://api.cimediacloud.com/workspaces/f44132c2393d470c88b9884f45877ebb/contents
+      uri: https://api.cimediacloud.com/workspaces
     response:
       body:
         string:
-          '{"limit": 50, "offset": 0, "count": 13, "kind": "All", "order": {"by":
-          "CreatedOn", "direction": "Asc"}, "items": [{"id": "d870616520634dbc8eb8caec141188fa",
-          "name": "Workspace"}]}'
+          '{"limit": 50, "offset": 0, "count": 2, "items": [{"name": "American
+          Archive of Public Broadcasting", "id": "051303c1c1d24da7988128e6d2f56aa9"}]}'
       headers:
         Cache-Control:
           - no-cache
         Connection:
           - keep-alive
         Content-Length:
-          - '119677'
+          - '7629'
         Content-Type:
           - application/json; charset=utf-8
         Date:
-          - Fri, 12 May 2023 22:12:47 GMT
+          - Mon, 08 May 2023 20:34:36 GMT
         Expires:
           - '-1'
         Pragma:
           - no-cache
         Strict-Transport-Security:
           - max-age=86400; includeSubDomains
         X-Frame-Options:
           - deny
         X-RateLimit-Limit:
           - '5000'
         X-RateLimit-Remaining:
-          - '4978'
+          - '4985'
         X-RateLimit-Reset:
-          - '1683929580'
+          - '1683578100'
       status:
         code: 200
         message: OK
 version: 1
```

### Comparing `sonyci-0.1.1/tests/vhs/tests.test_sonyci/test_workspace_empty_search.yaml` & `sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_workspace_search.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,95 +1,98 @@
 interactions:
-- request:
-    body: grant_type=password&client_id=FAKE_CLIENT_ID&client_secret=FAKE_CLIENT_SECRET
-    headers:
-      Accept:
-      - '*/*'
-      Accept-Encoding:
-      - gzip, deflate
-      Connection:
-      - keep-alive
-      Content-Length:
-      - '109'
-      Content-Type:
-      - application/x-www-form-urlencoded
-      User-Agent:
-      - python-requests/2.30.0
-      authorization:
-      - Bearer DUMMY
-    method: POST
-    uri: https://api.cimediacloud.com/oauth2/token
-  response:
-    body:
-      string: '{"access_token": "DUMMY_ACCESS_TOKEN", "expires_in": 86400, "token_type":
-        "bearer", "refresh_token": "DUMMY_REFRESH_TOKEN"}'
-    headers:
-      Cache-Control:
-      - no-cache
-      Connection:
-      - keep-alive
-      Content-Length:
-      - '143'
-      Content-Type:
-      - application/json; charset=utf-8
-      Date:
-      - Fri, 12 May 2023 22:12:48 GMT
-      Expires:
-      - '-1'
-      Pragma:
-      - no-cache
-      Strict-Transport-Security:
-      - max-age=86400; includeSubDomains
-      X-Frame-Options:
-      - deny
-    status:
-      code: 200
-      message: OK
-- request:
-    body: null
-    headers:
-      Accept:
-      - '*/*'
-      Accept-Encoding:
-      - gzip, deflate
-      Connection:
-      - keep-alive
-      User-Agent:
-      - python-requests/2.30.0
-      authorization:
-      - Bearer DUMMY
-    method: GET
-    uri: https://api.cimediacloud.com/workspaces/f44132c2393d470c88b9884f45877ebb/search?query=i+am+not+a+guid&kind=asset
-  response:
-    body:
-      string: '{"limit": 50, "offset": 0, "count": 0, "kind": "Asset", "type": "All",
-        "query": "i am not a guid", "items": [], "order": {"by": "Relevance", "direction":
-        "Desc"}}'
-    headers:
-      Cache-Control:
-      - no-cache
-      Connection:
-      - keep-alive
-      Content-Length:
-      - '144'
-      Content-Type:
-      - application/json; charset=utf-8
-      Date:
-      - Fri, 12 May 2023 22:12:48 GMT
-      Expires:
-      - '-1'
-      Pragma:
-      - no-cache
-      Strict-Transport-Security:
-      - max-age=86400; includeSubDomains
-      X-Frame-Options:
-      - deny
-      X-RateLimit-Limit:
-      - '5000'
-      X-RateLimit-Remaining:
-      - '4977'
-      X-RateLimit-Reset:
-      - '1683929580'
-    status:
-      code: 200
-      message: OK
+  - request:
+      body: grant_type=password&client_id=FAKE_CLIENT_ID&client_secret=FAKE_CLIENT_SECRET
+      headers:
+        Accept:
+          - '*/*'
+        Accept-Encoding:
+          - gzip, deflate
+        Connection:
+          - keep-alive
+        Content-Length:
+          - '109'
+        Content-Type:
+          - application/x-www-form-urlencoded
+        User-Agent:
+          - python-requests/2.30.0
+        authorization:
+          - Bearer DUMMY
+      method: POST
+      uri: https://api.cimediacloud.com/oauth2/token
+    response:
+      body:
+        string:
+          '{"access_token": "DUMMY_ACCESS_TOKEN", "expires_in": 86400, "token_type":
+          "bearer", "refresh_token": "DUMMY_REFRESH_TOKEN"}'
+      headers:
+        Cache-Control:
+          - no-cache
+        Connection:
+          - keep-alive
+        Content-Length:
+          - '143'
+        Content-Type:
+          - application/json; charset=utf-8
+        Date:
+          - Tue, 09 May 2023 21:15:38 GMT
+        Expires:
+          - '-1'
+        Pragma:
+          - no-cache
+        Strict-Transport-Security:
+          - max-age=86400; includeSubDomains
+        X-Frame-Options:
+          - deny
+      status:
+        code: 200
+        message: OK
+  - request:
+      body: null
+      headers:
+        Accept:
+          - '*/*'
+        Accept-Encoding:
+          - gzip, deflate
+        Connection:
+          - keep-alive
+        User-Agent:
+          - python-requests/2.30.0
+        authorization:
+          - Bearer DUMMY
+      method: GET
+      uri: https://api.cimediacloud.com/workspaces/f44132c2393d470c88b9884f45877ebb/search?query=pb-aacip-e4308199588&kind=asset
+    response:
+      body:
+        string:
+          '{"limit": 50, "offset": 0, "count": 1, "kind": "Asset", "type": "All",
+          "query": "pb-aacip-e4308199588", "items": [{"id": "554544ceaf6b4c94a4a06cee5bc1f39f",
+          "name": "cpb-aacip-e4308199588.txt"}], "order": {"by": "Relevance", "direction":
+          "Desc"}}'
+      headers:
+        Cache-Control:
+          - no-cache
+        Connection:
+          - keep-alive
+        Content-Length:
+          - '5784'
+        Content-Type:
+          - application/json; charset=utf-8
+        Date:
+          - Tue, 09 May 2023 21:15:38 GMT
+        Expires:
+          - '-1'
+        Pragma:
+          - no-cache
+        Strict-Transport-Security:
+          - max-age=86400; includeSubDomains
+        X-Frame-Options:
+          - deny
+        X-RateLimit-Limit:
+          - '5000'
+        X-RateLimit-Remaining:
+          - '4983'
+        X-RateLimit-Reset:
+          - '1683666960'
+      status:
+        code: 200
+        message: OK
 version: 1
```

### Comparing `sonyci-0.1.1/tests/vhs/tests.test_sonyci/test_workspace_search.yaml` & `sonyci-0.1.1a0/tests/vhs/tests.test_sonyci/test_workspace_contents.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         Connection:
           - keep-alive
         Content-Length:
           - '143'
         Content-Type:
           - application/json; charset=utf-8
         Date:
-          - Fri, 12 May 2023 22:12:49 GMT
+          - Tue, 09 May 2023 21:15:36 GMT
         Expires:
           - '-1'
         Pragma:
           - no-cache
         Strict-Transport-Security:
           - max-age=86400; includeSubDomains
         X-Frame-Options:
@@ -55,44 +55,43 @@
         Connection:
           - keep-alive
         User-Agent:
           - python-requests/2.30.0
         authorization:
           - Bearer DUMMY
       method: GET
-      uri: https://api.cimediacloud.com/workspaces/f44132c2393d470c88b9884f45877ebb/search?query=pb-aacip-e4308199588&kind=asset
+      uri: https://api.cimediacloud.com/workspaces/f44132c2393d470c88b9884f45877ebb/contents
     response:
       body:
         string:
-          '{"limit": 50, "offset": 0, "count": 1, "kind": "Asset", "type": "All",
-          "query": "pb-aacip-e4308199588", "items": [{"id": "554544ceaf6b4c94a4a06cee5bc1f39f",
-          "name": "cpb-aacip-e4308199588.txt"}], "order": {"by": "Relevance", "direction":
-          "Desc"}}'
+          '{"limit": 50, "offset": 0, "count": 13, "kind": "All", "order": {"by":
+          "CreatedOn", "direction": "Asc"}, "items": [{"id": "d870616520634dbc8eb8caec141188fa",
+          "name": "Workspace"}]}'
       headers:
         Cache-Control:
           - no-cache
         Connection:
           - keep-alive
         Content-Length:
-          - '5785'
+          - '119672'
         Content-Type:
           - application/json; charset=utf-8
         Date:
-          - Fri, 12 May 2023 22:12:49 GMT
+          - Tue, 09 May 2023 21:15:36 GMT
         Expires:
           - '-1'
         Pragma:
           - no-cache
         Strict-Transport-Security:
           - max-age=86400; includeSubDomains
         X-Frame-Options:
           - deny
         X-RateLimit-Limit:
           - '5000'
         X-RateLimit-Remaining:
-          - '4976'
+          - '4985'
         X-RateLimit-Reset:
-          - '1683929580'
+          - '1683666960'
       status:
         code: 200
         message: OK
 version: 1
```

### Comparing `sonyci-0.1.1/PKG-INFO` & `sonyci-0.1.1a0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: sonyci
-Version: 0.1.1
+Version: 0.1.1a0
 Summary: A Sony Ci api client
 Author-Email: WGBH-MLA <ryan_harbert@wgbh.org>
 License: MIT
 Requires-Python: >=3.7
 Requires-Dist: pydantic~=1.10
 Requires-Dist: requests-oauth2client~=1.1
 Requires-Dist: loguru~=0.7
-Requires-Dist: pytest~=7.3; extra == "test"
-Requires-Dist: vcrpy~=4.2; extra == "test"
-Requires-Dist: pytest-vcr~=1.0; extra == "test"
-Requires-Dist: pytest-cov~=4.0; extra == "test"
-Requires-Dist: pytest-sugar~=0.9; extra == "test"
-Requires-Dist: pytest-xdist~=3.2; extra == "test"
+Requires-Dist: rich~=13.3
+Requires-Dist: pytest>=7.3.1; extra == "test"
+Requires-Dist: vcrpy>=4.2.1; extra == "test"
+Requires-Dist: pytest-vcr>=1.0.2; extra == "test"
+Requires-Dist: pytest-cov>=4.0.0; extra == "test"
+Requires-Dist: pytest-sugar>=0.9.7; extra == "test"
+Requires-Dist: pytest-xdist>=3.2.1; extra == "test"
 Requires-Dist: urllib3~=1.26; extra == "test"
-Requires-Dist: typer[all]>=0.9.0; extra == "cli"
-Requires-Dist: typer>=0.9.0; extra == "cli-ci"
+Requires-Dist: typer[all]>=0.7.0; extra == "cli"
 Requires-Dist: mkdocs~=1.4; extra == "docs"
 Requires-Dist: mkdocs-material~=9.1; extra == "docs"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin~=1.2; extra == "docs"
 Requires-Dist: mike; extra == "docs"
 Requires-Dist: mkdocstrings[python]~=0.21; extra == "docs"
 Requires-Dist: mkdocs-jupyter~=0.24; extra == "docs"
 Provides-Extra: test
 Provides-Extra: cli
-Provides-Extra: cli-ci
 Provides-Extra: docs
 Description-Content-Type: text/markdown
 
 ![deploy](https://github.com/WGBH-MLA/sonyci/actions/workflows/CI.yml/badge.svg)
 [![codecov](https://codecov.io/gh/WGBH-MLA/sonyci/branch/main/graph/badge.svg?token=6J7UUYW9I9)](https://codecov.io/gh/WGBH-MLA/sonyci)
 <a href="https://codecov.io/gh/WGBH-MLA/sonyci"><img height=20 src="https://codecov.io/gh/WGBH-MLA/sonyci/branch/main/graphs/tree.svg?token=6J7UUYW9I9"></img></a>
```

#### html2text {}

```diff
@@ -1,34 +1,33 @@
-Metadata-Version: 2.1 Name: sonyci Version: 0.1.1 Summary: A Sony Ci api client
-Author-Email: WGBH-MLA
+Metadata-Version: 2.1 Name: sonyci Version: 0.1.1a0 Summary: A Sony Ci api
+client Author-Email: WGBH-MLA
 wgbh.org> License: MIT Requires-Python: >=3.7 Requires-Dist: pydantic~=1.10
 Requires-Dist: requests-oauth2client~=1.1 Requires-Dist: loguru~=0.7 Requires-
-Dist: pytest~=7.3; extra == "test" Requires-Dist: vcrpy~=4.2; extra == "test"
-Requires-Dist: pytest-vcr~=1.0; extra == "test" Requires-Dist: pytest-cov~=4.0;
-extra == "test" Requires-Dist: pytest-sugar~=0.9; extra == "test" Requires-
-Dist: pytest-xdist~=3.2; extra == "test" Requires-Dist: urllib3~=1.26; extra ==
-"test" Requires-Dist: typer[all]>=0.9.0; extra == "cli" Requires-Dist:
-typer>=0.9.0; extra == "cli-ci" Requires-Dist: mkdocs~=1.4; extra == "docs"
+Dist: rich~=13.3 Requires-Dist: pytest>=7.3.1; extra == "test" Requires-Dist:
+vcrpy>=4.2.1; extra == "test" Requires-Dist: pytest-vcr>=1.0.2; extra == "test"
+Requires-Dist: pytest-cov>=4.0.0; extra == "test" Requires-Dist: pytest-
+sugar>=0.9.7; extra == "test" Requires-Dist: pytest-xdist>=3.2.1; extra ==
+"test" Requires-Dist: urllib3~=1.26; extra == "test" Requires-Dist: typer
+[all]>=0.7.0; extra == "cli" Requires-Dist: mkdocs~=1.4; extra == "docs"
 Requires-Dist: mkdocs-material~=9.1; extra == "docs" Requires-Dist: mkdocs-git-
 revision-date-localized-plugin~=1.2; extra == "docs" Requires-Dist: mike; extra
 == "docs" Requires-Dist: mkdocstrings[python]~=0.21; extra == "docs" Requires-
 Dist: mkdocs-jupyter~=0.24; extra == "docs" Provides-Extra: test Provides-
-Extra: cli Provides-Extra: cli-ci Provides-Extra: docs Description-Content-
-Type: text/markdown ![deploy](https://github.com/WGBH-MLA/sonyci/actions/
-workflows/CI.yml/badge.svg) [![codecov](https://codecov.io/gh/WGBH-MLA/sonyci/
-branch/main/graph/badge.svg?token=6J7UUYW9I9)](https://codecov.io/gh/WGBH-MLA/
-sonyci) [https://codecov.io/gh/WGBH-MLA/sonyci/branch/main/graphs/
-tree.svg?token=6J7UUYW9I9] # sonyci A Sony Ci api client ## Install ```shell
-pdm install ``` ## Configure Create a file called `.cred` with the following
-contents, and add your credentials: ```shell export CI_USERNAME= export
-CI_PASSWORD= export CI_CLIENT_ID= export CI_CLIENT_SECRET= export
-CI_WORKSPACE_ID= ``` Activate the variables: ```shell source .cred ```
-Alternate notation: (May not be available in your terminal) ```shell . .cred
-``` ## Use Run the cli with `ci` ```shell $ ci -h Usage: ci [OPTIONS] COMMAND
-[ARGS]... â­â Options
+Extra: cli Provides-Extra: docs Description-Content-Type: text/markdown !
+[deploy](https://github.com/WGBH-MLA/sonyci/actions/workflows/CI.yml/badge.svg)
+[![codecov](https://codecov.io/gh/WGBH-MLA/sonyci/branch/main/graph/
+badge.svg?token=6J7UUYW9I9)](https://codecov.io/gh/WGBH-MLA/sonyci) [https://
+codecov.io/gh/WGBH-MLA/sonyci/branch/main/graphs/tree.svg?token=6J7UUYW9I9] #
+sonyci A Sony Ci api client ## Install ```shell pdm install ``` ## Configure
+Create a file called `.cred` with the following contents, and add your
+credentials: ```shell export CI_USERNAME= export CI_PASSWORD= export
+CI_CLIENT_ID= export CI_CLIENT_SECRET= export CI_WORKSPACE_ID= ``` Activate the
+variables: ```shell source .cred ``` Alternate notation: (May not be available
+in your terminal) ```shell . .cred ``` ## Use Run the cli with `ci` ```shell $
+ci -h Usage: ci [OPTIONS] COMMAND [ARGS]... â­â Options
 ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
 â --version -v Show the version and exit. â â --token -t TEXT Sony CI
 token. [env var: TOKEN] [default: None] â â --install-completion Install
 completion for the current shell. â â --show-completion Show completion for
 the current shell, to copy it or â â customize the installation. â â --
 help -h Show this message and exit. â
 â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
```

