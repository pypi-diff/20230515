# Comparing `tmp/forust-0.2.6.tar.gz` & `tmp/forust-0.2.7.tar.gz`

## Comparing `forust-0.2.6.tar` & `forust-0.2.7.tar`

### file list

```diff
@@ -1,41 +1,44 @@
--rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 forust-0.2.6/local_dependencies/forust-ml/Cargo.toml
--rw-r--r--   0        0        0     5775 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/.github/workflows/CI.yml
--rw-r--r--   0        0        0      274 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/.gitignore
--rw-r--r--   0        0        0      334 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11542 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/LICENSE
--rw-r--r--   0        0        0    12996 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/README.md
--rw-r--r--   0        0        0     4213 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/benches/forust_benchmarks.rs
--rw-r--r--   0        0        0   390367 2023-05-09 02:05:58.000000 forust-0.2.6/local_dependencies/forust-ml/dist/forust-0.2.6-cp310-none-win_amd64.whl
--rw-r--r--   0        0        0   754317 2023-05-09 02:05:01.000000 forust-0.2.6/local_dependencies/forust-ml/dist/forust-0.2.6.tar.gz
--rw-r--r--   0        0        0    16121 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/resources/pdp_plot_age.png
--rw-r--r--   0        0        0    10758 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
--rw-r--r--   0        0        0    57910 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/resources/titanic.csv
--rw-r--r--   0        0        0   655700 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/resources/tree-image-crop.png
--rw-r--r--   0        0        0     2626 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/rs-example.md
--rw-r--r--   0        0        0     1226 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/scripts/make_resources.py
--rw-r--r--   0        0        0       56 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/scripts/run-python-tests.ps1
--rw-r--r--   0        0        0       56 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/scripts/run-python-tests.sh
--rw-r--r--   0        0        0     5772 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/src/binning.rs
--rw-r--r--   0        0        0      259 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/src/constraints.rs
--rw-r--r--   0        0        0     8706 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/src/data.rs
--rw-r--r--   0        0        0      602 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/src/errors.rs
--rw-r--r--   0        0        0    27532 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/src/gradientbooster.rs
--rw-r--r--   0        0        0     9621 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/src/histogram.rs
--rw-r--r--   0        0        0      336 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/src/lib.rs
--rw-r--r--   0        0        0     6268 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/src/node.rs
--rw-r--r--   0        0        0     4255 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/src/objective.rs
--rw-r--r--   0        0        0     4186 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/src/partial_dependence.rs
--rw-r--r--   0        0        0    35701 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/src/splitter.rs
--rw-r--r--   0        0        0    22389 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/src/tree.rs
--rw-r--r--   0        0        0    30292 2023-05-09 02:01:11.000000 forust-0.2.6/local_dependencies/forust-ml/src/utils.rs
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.6/Cargo.toml
--rw-r--r--   0        0        0      756 2023-05-09 02:01:11.000000 forust-0.2.6/.gitignore
--rw-r--r--   0        0        0    12996 2023-05-09 02:01:11.000000 forust-0.2.6/README.md
--rw-r--r--   0        0        0    21888 2023-05-09 02:01:11.000000 forust-0.2.6/forust/__init__.py
--rw-r--r--   0        0        0      816 2023-05-09 02:01:11.000000 forust-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     7624 2023-05-09 02:01:11.000000 forust-0.2.6/scratch.py
--rw-r--r--   0        0        0    10103 2023-05-09 02:01:11.000000 forust-0.2.6/src/lib.rs
--rw-r--r--   0        0        0    13133 2023-05-09 02:01:11.000000 forust-0.2.6/tests/test_booster.py
--rw-r--r--   0        0        0    11542 2023-05-09 02:01:11.000000 forust-0.2.6/LICENSE
--rw-r--r--   0        0        0    12996 2023-05-09 02:01:11.000000 forust-0.2.6/README.md
--rw-r--r--   0        0        0    13780 1970-01-01 00:00:00.000000 forust-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 forust-0.2.7/local_dependencies/forust-ml/Cargo.toml
+-rw-r--r--   0      501       20     5608 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      262 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/.gitignore
+-rw-r--r--   0      501       20      320 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/.pre-commit-config.yaml
+-rw-r--r--   0      501       20     3242 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/CONTRIBUTING.md
+-rw-r--r--   0      501       20    11341 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/LICENSE
+-rw-r--r--   0      501       20    15307 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/README.md
+-rw-r--r--   0      501       20     4228 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/benches/forust_benchmarks.rs
+-rw-r--r--   0      501       20   449752 2023-05-15 13:50:45.000000 forust-0.2.7/local_dependencies/forust-ml/dist/forust-0.2.7-cp311-cp311-macosx_10_7_x86_64.whl
+-rw-r--r--   0      501       20   763229 2023-05-15 13:49:15.000000 forust-0.2.7/local_dependencies/forust-ml/dist/forust-0.2.7.tar.gz
+-rw-r--r--   0      501       20    16121 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/resources/pdp_plot_age.png
+-rw-r--r--   0      501       20    10758 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
+-rw-r--r--   0      501       20    57018 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/resources/titanic.csv
+-rw-r--r--   0      501       20   655700 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/resources/tree-image-crop.png
+-rw-r--r--   0      501       20     2556 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/rs-example.md
+-rw-r--r--   0      501       20     1179 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/scripts/make_resources.py
+-rw-r--r--   0      501       20       53 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/scripts/run-python-tests.ps1
+-rw-r--r--   0      501       20       53 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/scripts/run-python-tests.sh
+-rw-r--r--   0      501       20     5610 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/binning.rs
+-rw-r--r--   0      501       20      248 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/constraints.rs
+-rw-r--r--   0      501       20     9944 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/data.rs
+-rw-r--r--   0      501       20      562 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/errors.rs
+-rw-r--r--   0      501       20    35446 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/gradientbooster.rs
+-rw-r--r--   0      501       20     9357 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/histogram.rs
+-rw-r--r--   0      501       20      355 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/lib.rs
+-rw-r--r--   0      501       20     8847 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/metric.rs
+-rw-r--r--   0      501       20     6060 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/node.rs
+-rw-r--r--   0      501       20     4868 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/objective.rs
+-rw-r--r--   0      501       20     4018 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/partial_dependence.rs
+-rw-r--r--   0      501       20     2276 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/sampler.rs
+-rw-r--r--   0      501       20    34685 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/splitter.rs
+-rw-r--r--   0      501       20    21677 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/tree.rs
+-rw-r--r--   0      501       20    29701 2023-05-15 13:45:36.000000 forust-0.2.7/local_dependencies/forust-ml/src/utils.rs
+-rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.7/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-05-15 13:45:36.000000 forust-0.2.7/.gitignore
+-rw-r--r--   0      501       20    15307 2023-05-15 13:46:19.000000 forust-0.2.7/README.md
+-rw-r--r--   0      501       20    26798 2023-05-15 13:45:36.000000 forust-0.2.7/forust/__init__.py
+-rw-r--r--   0      501       20      785 2023-05-15 13:45:36.000000 forust-0.2.7/pyproject.toml
+-rw-r--r--   0      501       20     7353 2023-05-15 13:45:36.000000 forust-0.2.7/scratch.py
+-rw-r--r--   0      501       20    12675 2023-05-15 13:45:36.000000 forust-0.2.7/src/lib.rs
+-rw-r--r--   0      501       20    14397 2023-05-15 13:45:36.000000 forust-0.2.7/tests/test_booster.py
+-rw-r--r--   0      501       20    11341 2023-05-15 13:46:19.000000 forust-0.2.7/LICENSE
+-rw-r--r--   0      501       20    15307 2023-05-15 13:46:19.000000 forust-0.2.7/README.md
+-rw-r--r--   0        0        0    16091 1970-01-01 00:00:00.000000 forust-0.2.7/PKG-INFO
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/.github/workflows/CI.yml` & `forust-0.2.7/local_dependencies/forust-ml/.github/workflows/CI.yml`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-name: Test and Deploy
-on: [pull_request, push]
-
-jobs:
-  windows-build-tests:
-    strategy:
-      matrix:
-        pyversion: ["3.8", "3.9", "3.10", "3.11"]
-    runs-on: "windows-latest"
-    steps:
-      - uses: actions/checkout@v2
-      - name: Install latests stable Rust
-        uses: actions-rs/toolchain@v1
-        with:
-          toolchain: stable
-          override: true
-      - uses: actions/setup-python@v2
-        with:
-          python-version: ${{ matrix.pyversion }}
-          architecture: x64
-      - name: Install deps
-        run: pip install numpy pandas seaborn xgboost=='1.6.1' scikit-learn
-      - run: |
-          cp README.md py-forust/README.md
-          cp LICENSE py-forust/LICENSE
-      - name: Build test data
-        run: python scripts/make_resources.py
-      - name: Run Cargo tests
-        uses: actions-rs/cargo@v1
-        with:
-          command: test
-      - name: Build Wheels with maturin
-        uses: messense/maturin-action@v1
-        with:
-          target: x86_64
-          command: build
-          args: --release --strip --interpreter python --manifest-path py-forust/Cargo.toml --out dist
-      - name: Install wheel
-        run: pip install forust --no-index --find-links dist --no-deps --force-reinstall
-      - name: Run Package Tests
-        run: |
-          pip install pytest
-          cd py-forust
-          pytest tests
-          cd ..
-      - name: Save Artifacts
-        uses: actions/upload-artifact@v2
-        with:
-          name: wheels
-          path: dist
-      - if: "startsWith(github.ref, 'refs/tags/')"
-        name: Publish Wheels
-        uses: messense/maturin-action@v1
-        with:
-          command: publish
-          args: --username ${{ secrets.PYPI_USERNAME }} --password ${{ secrets.PYPI_PASSWORD }} --interpreter python --skip-existing --manifest-path py-forust/Cargo.toml
-
-  macos-build-test:
-    strategy:
-      matrix:
-        pyversion: ["3.8", "3.9", "3.10", "3.11"]
-    runs-on: "macos-latest"
-    steps:
-      - uses: actions/checkout@v2
-      - name: Install latests stable Rust
-        uses: actions-rs/toolchain@v1
-        with:
-          toolchain: stable
-          override: true
-      - uses: actions/setup-python@v2
-        with:
-          python-version: ${{ matrix.pyversion }}
-          architecture: x64
-      - name: Install deps
-        run: pip install numpy pandas seaborn xgboost=='1.6.1' scikit-learn
-      - run: |
-          cp README.md py-forust/README.md
-          cp LICENSE py-forust/LICENSE
-      - name: Build test data
-        run: python scripts/make_resources.py
-      - name: Run Cargo tests
-        uses: actions-rs/cargo@v1
-        with:
-          command: test
-      - name: Build Wheels with maturin
-        uses: messense/maturin-action@v1
-        with:
-          target: x86_64
-          command: build
-          args: --release --strip --interpreter python --manifest-path py-forust/Cargo.toml --out dist
-      - name: Install wheel
-        run: pip install forust --no-index --find-links dist --no-deps --force-reinstall
-      - name: Run Package Tests
-        run: |
-          pip install pytest
-          cd py-forust
-          pytest tests
-          cd ..
-      - name: Save Artifacts
-        uses: actions/upload-artifact@v2
-        with:
-          name: wheels
-          path: dist
-      - if: "startsWith(github.ref, 'refs/tags/')"
-        name: Publish Wheels
-        uses: messense/maturin-action@v1
-        with:
-          command: publish
-          target: x86_64
-          args: --username ${{ secrets.PYPI_USERNAME }} --password ${{ secrets.PYPI_PASSWORD }} --interpreter python --skip-existing --manifest-path py-forust/Cargo.toml
-
-  linux-build-test:
-    runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        pyversion: ["3.8", "3.9", "3.10", "3.11"]
-        # target: [x86_64, i686]
-    steps:
-      - uses: actions/checkout@v2
-      - name: Install latests stable Rust
-        uses: actions-rs/toolchain@v1
-        with:
-          toolchain: stable
-          override: true
-      - uses: actions/setup-python@v2
-        with:
-          python-version: ${{ matrix.pyversion }}
-          architecture: x64
-      - name: Install deps
-        run: pip install numpy pandas seaborn xgboost=='1.6.1' scikit-learn
-      - run: |
-          cp README.md py-forust/README.md
-          cp LICENSE py-forust/LICENSE
-      - name: Build test data
-        run: python scripts/make_resources.py
-      - name: Run Cargo tests
-        uses: actions-rs/cargo@v1
-        with:
-          command: test
-      - name: Build Wheels with maturin
-        uses: messense/maturin-action@v1
-        with:
-          target: x86_64
-          manylinux: auto
-          command: build
-          args: --release --strip --interpreter python${{ matrix.pyversion }} --manifest-path py-forust/Cargo.toml --out dist
-      - name: Install wheel
-        run: pip install forust --no-index --find-links dist --no-deps --force-reinstall
-      - name: Run Package Tests
-        run: |
-          pip install pytest
-          cd py-forust
-          pytest tests
-          cd ..
-      - name: Save Artifacts
-        uses: actions/upload-artifact@v2
-        with:
-          name: wheels
-          path: dist
-      - if: "startsWith(github.ref, 'refs/tags/')"
-        name: Publish Wheels
-        uses: messense/maturin-action@v1
-        with:
-          command: publish
-          target: x86_64
-          manylinux: auto
-          args: --username ${{ secrets.PYPI_USERNAME }} --password ${{ secrets.PYPI_PASSWORD }} --interpreter python${{ matrix.pyversion }} --skip-existing --manifest-path py-forust/Cargo.toml
+name: Test and Deploy
+on: [pull_request, push]
+
+jobs:
+  windows-build-tests:
+    strategy:
+      matrix:
+        pyversion: ["3.8", "3.9", "3.10", "3.11"]
+    runs-on: "windows-latest"
+    steps:
+      - uses: actions/checkout@v2
+      - name: Install latests stable Rust
+        uses: actions-rs/toolchain@v1
+        with:
+          toolchain: stable
+          override: true
+      - uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.pyversion }}
+          architecture: x64
+      - name: Install deps
+        run: pip install numpy pandas seaborn xgboost=='1.6.1' scikit-learn
+      - run: |
+          cp README.md py-forust/README.md
+          cp LICENSE py-forust/LICENSE
+      - name: Build test data
+        run: python scripts/make_resources.py
+      - name: Run Cargo tests
+        uses: actions-rs/cargo@v1
+        with:
+          command: test
+      - name: Build Wheels with maturin
+        uses: messense/maturin-action@v1
+        with:
+          target: x86_64
+          command: build
+          args: --release --strip --interpreter python --manifest-path py-forust/Cargo.toml --out dist
+      - name: Install wheel
+        run: pip install forust --no-index --find-links dist --no-deps --force-reinstall
+      - name: Run Package Tests
+        run: |
+          pip install pytest
+          cd py-forust
+          pytest tests
+          cd ..
+      - name: Save Artifacts
+        uses: actions/upload-artifact@v2
+        with:
+          name: wheels
+          path: dist
+      - if: "startsWith(github.ref, 'refs/tags/')"
+        name: Publish Wheels
+        uses: messense/maturin-action@v1
+        with:
+          command: publish
+          args: --username ${{ secrets.PYPI_USERNAME }} --password ${{ secrets.PYPI_PASSWORD }} --interpreter python --skip-existing --manifest-path py-forust/Cargo.toml
+
+  macos-build-test:
+    strategy:
+      matrix:
+        pyversion: ["3.8", "3.9", "3.10", "3.11"]
+    runs-on: "macos-latest"
+    steps:
+      - uses: actions/checkout@v2
+      - name: Install latests stable Rust
+        uses: actions-rs/toolchain@v1
+        with:
+          toolchain: stable
+          override: true
+      - uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.pyversion }}
+          architecture: x64
+      - name: Install deps
+        run: pip install numpy pandas seaborn xgboost=='1.6.1' scikit-learn
+      - run: |
+          cp README.md py-forust/README.md
+          cp LICENSE py-forust/LICENSE
+      - name: Build test data
+        run: python scripts/make_resources.py
+      - name: Run Cargo tests
+        uses: actions-rs/cargo@v1
+        with:
+          command: test
+      - name: Build Wheels with maturin
+        uses: messense/maturin-action@v1
+        with:
+          target: x86_64
+          command: build
+          args: --release --strip --interpreter python --manifest-path py-forust/Cargo.toml --out dist
+      - name: Install wheel
+        run: pip install forust --no-index --find-links dist --no-deps --force-reinstall
+      - name: Run Package Tests
+        run: |
+          pip install pytest
+          cd py-forust
+          pytest tests
+          cd ..
+      - name: Save Artifacts
+        uses: actions/upload-artifact@v2
+        with:
+          name: wheels
+          path: dist
+      - if: "startsWith(github.ref, 'refs/tags/')"
+        name: Publish Wheels
+        uses: messense/maturin-action@v1
+        with:
+          command: publish
+          target: x86_64
+          args: --username ${{ secrets.PYPI_USERNAME }} --password ${{ secrets.PYPI_PASSWORD }} --interpreter python --skip-existing --manifest-path py-forust/Cargo.toml
+
+  linux-build-test:
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        pyversion: ["3.8", "3.9", "3.10", "3.11"]
+        # target: [x86_64, i686]
+    steps:
+      - uses: actions/checkout@v2
+      - name: Install latests stable Rust
+        uses: actions-rs/toolchain@v1
+        with:
+          toolchain: stable
+          override: true
+      - uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.pyversion }}
+          architecture: x64
+      - name: Install deps
+        run: pip install numpy pandas seaborn xgboost=='1.6.1' scikit-learn
+      - run: |
+          cp README.md py-forust/README.md
+          cp LICENSE py-forust/LICENSE
+      - name: Build test data
+        run: python scripts/make_resources.py
+      - name: Run Cargo tests
+        uses: actions-rs/cargo@v1
+        with:
+          command: test
+      - name: Build Wheels with maturin
+        uses: messense/maturin-action@v1
+        with:
+          target: x86_64
+          manylinux: auto
+          command: build
+          args: --release --strip --interpreter python${{ matrix.pyversion }} --manifest-path py-forust/Cargo.toml --out dist
+      - name: Install wheel
+        run: pip install forust --no-index --find-links dist --no-deps --force-reinstall
+      - name: Run Package Tests
+        run: |
+          pip install pytest
+          cd py-forust
+          pytest tests
+          cd ..
+      - name: Save Artifacts
+        uses: actions/upload-artifact@v2
+        with:
+          name: wheels
+          path: dist
+      - if: "startsWith(github.ref, 'refs/tags/')"
+        name: Publish Wheels
+        uses: messense/maturin-action@v1
+        with:
+          command: publish
+          target: x86_64
+          manylinux: auto
+          args: --username ${{ secrets.PYPI_USERNAME }} --password ${{ secrets.PYPI_PASSWORD }} --interpreter python${{ matrix.pyversion }} --skip-existing --manifest-path py-forust/Cargo.toml
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/LICENSE` & `forust-0.2.7/local_dependencies/forust-ml/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2022 James Inlow
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2022 James Inlow
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/README.md` & `forust-0.2.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,187 +1,229 @@
-<p align="center">
-  <img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/tree-image-crop.png">
-</p>
-
-
-<div align="center">
-
-  <a href="https://pypi.org/project/forust/">![PyPI](https://img.shields.io/pypi/v/forust?color=gr&style=for-the-badge)</a>
-  <a href="https://crates.io/crates/forust-ml">![Crates.io](https://img.shields.io/crates/v/forust-ml?color=gr&style=for-the-badge)</a>
-
-</div>
-
-# Forust
-## _A lightweight gradient boosting package_
-Forust, is a lightweight package for building gradient boosted decision tree ensembles. All of the algorithm code is written in [Rust](https://www.rust-lang.org/), with a python wrapper. The rust package can be used directly, however, most examples shown here will be for the python wrapper. For a self contained rust example, [see here](rs-example.md). It implements the same algorithm as the [XGBoost](https://xgboost.readthedocs.io/en/stable/) package, and in many cases will give nearly identical results.
-
-I developed this package for a few reasons, mainly to better understand the XGBoost algorithm, additionally to have a fun project to work on in rust, and because I wanted to be able to experiment with adding new features to the algorithm in a smaller simpler codebase.
-
-All of the rust code for the package can be found in the [src](src/) directory, while all of the python wrapper code is in the [py-forust](py-forust/) directory.
-
-## Installation
-The package can be installed directly from [pypi](https://pypi.org/project/forust/).
-```shell
-pip install forust
-```
-
-To use in a rust project add the following to your Cargo.toml file.
-```toml
-forust-ml = "0.2.6"
-```
-
-## Usage
-The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
-
-It can be initialized with the following arguments.
-
- - `objective_type` ***(str, optional)***: The name of objective function used to optimize.
-    Valid options include "LogLoss" to use logistic loss as the objective function (binary classification),
-    or "SquaredLoss" to use Squared Error as the objective function (continuous regression).
-    Defaults to "LogLoss".
- - `iterations` ***(int, optional)***: Total number of trees to train in the ensemble.
-    Defaults to 100.
- - `learning_rate` ***(float, optional)***: Step size to use at each iteration. Each
-    leaf weight is multiplied by this number. The smaller the value, the more
-    conservative the weights will be. Defaults to 0.3.
- - `max_depth` ***(int, optional)***: Maximum depth of an individual tree. Valid values
-    are 0 to infinity. Defaults to 5.
- - `max_leaves` ***(int, optional)***: Maximum number of leaves allowed on a tree. Valid values
-    are 0 to infinity. This is the total number of final nodes. Defaults to sys.maxsize.
- - `l2` ***(float, optional)***: L2 regularization term applied to the weights of the tree. Valid values
-    are 0 to infinity. Defaults to 1.0.
- - `gamma` ***(float, optional)***: The minimum amount of loss required to further split a node.
-    Valid values are 0 to infinity. Defaults to 0.0.
- - `min_leaf_weight` ***(float, optional)***: Minimum sum of the hessian values of the loss function
-    required to be in a node. Defaults to 1.0.
- - `base_score` ***(float, optional)***: The initial prediction value of the model. Defaults to 0.5.
- - `nbins` ***(int, optional)***: Number of bins to calculate to partition the data. Setting this to
-    a smaller number, will result in faster training time, while potentially sacrificing
-    accuracy. If there are more bins, than unique values in a column, all unique values
-    will be used. Defaults to 256.
- - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
-    with this model? Defaults to `True`.
- - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. If `create_missing_branch` is set to `True` having this parameter be set to `True` will result in the missing branch further split, if this parameter is `False` then in that case the missing branch will always be a terminal node. Defaults to `True`.
- - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
- - `subsample` ***(float, optional)***: Percent of records to randomly sample at each iteration when
-      training a tree. Defaults to 1.0, meaning all data is used for training.
- - `seed` ***(integer, optional)***: Integer value used to seed any randomness used in the
-      algorithm. Defaults to 0.
- - `missing` ***(float, optional)***: Value to consider missing, when training and predicting with the booster. Defaults to `np.nan`.
- - `create_missing_branch` ***(bool, optional)***: An experimental parameter, that if `True`, will create a separate branch for missing, creating a ternary tree, the missing node will be given the same weight value as the parent node. If this parameter is `False`, missing will be sent down either the left or right branch, creating a binary tree. Defaults to `False`.
-
-### Training and Predicting
-
-Once, the booster has been initialized, it can be fit on a provided dataset, and performance field. After fitting, the model can be used to predict on a dataset.
-In the case of this example, the predictions are the log odds of a given record being 1.
-
-```python
-# Small example dataset
-from seaborn import load_dataset
-
-df = load_dataset("titanic")
-X = df.select_dtypes("number").drop(columns=["survived"])
-y = df["survived"]
-
-# Initialize a booster with defaults.
-from forust import GradientBooster
-model = GradientBooster(objective_type="LogLoss")
-model.fit(X, y)
-
-# Predict on data
-model.predict(X.head())
-# array([-1.94919663,  2.25863229,  0.32963671,  2.48732194, -3.00371813])
-
-# predict contributions
-model.predict_contributions(X.head())
-# array([[-0.63014213,  0.33880048, -0.16520798, -0.07798772, -0.85083578,
-#        -1.07720813],
-#       [ 1.05406709,  0.08825999,  0.21662544, -0.12083538,  0.35209258,
-#        -1.07720813],
-```
-
-The `fit` method accepts the following arguments.
- - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
- - `y` ***(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If "LogLoss" was
-   the objective type specified, then this should only contain 1 or 0 values, where 1 is the positive class being predicted. If "SquaredLoss" is the objective type, then any continuous variable can be provided.
- - `sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use when training the model. If None is passed, a weight of 1 will be used for every record. Defaults to None.
-
-The predict method accepts the following arguments.
- - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
- - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict function should run in parallel on multiple threads. If `None` is passed, the `parallel` attribute of the booster will be used. Defaults to `None`.
-
-The `predict_contributions` method will predict with the fitted booster on new data, returning the feature contribution matrix. The last column is the bias term.
- - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
- - `method` ***(str, optional)***: Method to calculate the contributions, if "average" is specified, the average internal node values are calculated, this is equivalent to the `approx_contribs` parameter in XGBoost. The other supported method is "weight", this will use the internal leaf weights, to calculate the contributions. This is the same as what is described by Saabas [here](https://blog.datadive.net/interpreting-random-forests/).
- - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict function should run in parallel on multiple threads. If `None` is passed, the `parallel` attribute of the booster will be used. Defaults to `None`.
-
-### Inspecting the Model
-
-Once the booster has been fit, each individual tree structure can be retrieved in text form, using the `text_dump` method. This method returns a list, the same length as the number of trees in the model.
-
-```python
-model.text_dump()[0]
-# 0:[0 < 3] yes=1,no=2,missing=2,gain=91.50833,cover=209.388307
-#       1:[4 < 13.7917] yes=3,no=4,missing=4,gain=28.185467,cover=94.00148
-#             3:[1 < 18] yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348
-#                   7:[1 < 17] yes=15,no=16,missing=16,gain=0.691266,cover=0.705011
-#                         15:leaf=-0.15120,cover=0.23500
-#                         16:leaf=0.154097,cover=0.470007
-```
-
-The `json_dump` method performs the same action, but returns the model as a json representation rather than a text string.
-
-To see an estimate for how a given feature is used in the model, the `partial_dependence` method is provided. This method calculates the partial dependence values of a feature. For each unique value of the feature, this gives the estimate of the predicted value for that feature, with the effects of all features averaged out. This information gives an estimate of how a given feature impacts the model.
-
-The `partial_dependence` method takes the following parameters...
-
- - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array. This should be the same data passed into the models fit, or predict, with the columns in the same order.
- - `feature` ***(Union[str, int])***: The feature for which to calculate the partial dependence values. This can be the name of a column, if the provided X is a pandas DataFrame, or the index of the feature.
- - `samples` ***(int | None, optional)***: Number of evenly spaced samples to select. If None is passed all unique values will be used. Defaults to 100.
- - `exclude_missing` ***(bool, optional)***: Should missing excluded from the features? Defaults to True.
- - `percentile_bounds` ***(tuple[float, float], optional)***: Upper and lower percentiles to start at  when calculating the samples. Defaults to (0.2, 0.98) to cap the samples selected  at the 5th and 95th percentiles respectively.
-This method returns a 2 dimensional numpy array, where the first column is the sorted unique values of the feature, and then the second column is the partial dependence values for each feature value.
-
-This information can be plotted to visualize how a feature is used in the model, like so.
-
-```python
-from seaborn import lineplot
-import matplotlib.pyplot as plt
-
-pd_values = model.partial_dependence(X=X, feature="age", samples=None)
-
-fig = lineplot(x=pd_values[:,0], y=pd_values[:,1],)
-plt.title("Partial Dependence Plot")
-plt.xlabel("Age")
-plt.ylabel("Log Odds")
-```
-<img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/pdp_plot_age.png">
-
-We can see how this is impacted if a model is created, where a specific constraint is applied to the feature using the `monotone_constraint` parameter.
-
-```python
-model = GradientBooster(
-    objective_type="LogLoss",
-    monotone_constraints={"age": -1},
-)
-model.fit(X, y)
-
-pd_values = model.partial_dependence(X=X, feature="age")
-fig = lineplot(
-    x=pd_values[:, 0],
-    y=pd_values[:, 1],
-)
-plt.title("Partial Dependence Plot with Monotonicity")
-plt.xlabel("Age")
-plt.ylabel("Log Odds")
-```
-<img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/pdp_plot_age_mono.png">
-
-### Saving the model
-To save and subsequently load a trained booster, the `save_booster` and `load_booster` methods can be used. Each accepts a path, which is used to write the model to. The model is saved and loaded as a json object.
-
-```python
-trained_model.save_booster("model_path.json")
-
-# To load a model from a json path.
-loaded_model = GradientBooster.load_model("model_path.json")
-```
+Metadata-Version: 2.1
+Name: forust
+Version: 0.2.7
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: numpy>=1.21
+Requires-Dist: pandas>=1.3
+Requires-Dist: maturin; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: seaborn; extra == 'dev'
+Requires-Dist: xgboost==1.6.1; extra == 'dev'
+Requires-Dist: scikit-learn; extra == 'dev'
+Provides-Extra: dev
+License-File: LICENSE
+Summary: A lightweight gradient boosting implementation in Rust.
+Keywords: rust,forust,machine learning,xgboost,tree model,decision tree
+Author: James Inlow
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+
+<p align="center">
+  <img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/tree-image-crop.png">
+</p>
+
+
+<div align="center">
+
+  <a href="https://pypi.org/project/forust/">![PyPI](https://img.shields.io/pypi/v/forust?color=gr&style=for-the-badge)</a>
+  <a href="https://crates.io/crates/forust-ml">![Crates.io](https://img.shields.io/crates/v/forust-ml?color=gr&style=for-the-badge)</a>
+
+</div>
+
+# Forust
+## _A lightweight gradient boosting package_
+Forust, is a lightweight package for building gradient boosted decision tree ensembles. All of the algorithm code is written in [Rust](https://www.rust-lang.org/), with a python wrapper. The rust package can be used directly, however, most examples shown here will be for the python wrapper. For a self contained rust example, [see here](rs-example.md). It implements the same algorithm as the [XGBoost](https://xgboost.readthedocs.io/en/stable/) package, and in many cases will give nearly identical results.
+
+I developed this package for a few reasons, mainly to better understand the XGBoost algorithm, additionally to have a fun project to work on in rust, and because I wanted to be able to experiment with adding new features to the algorithm in a smaller simpler codebase.
+
+All of the rust code for the package can be found in the [src](src/) directory, while all of the python wrapper code is in the [py-forust](py-forust/) directory.
+
+## Installation
+The package can be installed directly from [pypi](https://pypi.org/project/forust/).
+```shell
+pip install forust
+```
+
+To use in a rust project add the following to your Cargo.toml file.
+```toml
+forust-ml = "0.2.7"
+```
+
+## Usage
+The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
+
+It can be initialized with the following arguments.
+
+ - `objective_type` ***(str, optional)***: The name of objective function used to optimize.
+    Valid options include "LogLoss" to use logistic loss as the objective function (binary classification),
+    or "SquaredLoss" to use Squared Error as the objective function (continuous regression).
+    Defaults to "LogLoss".
+ - `iterations` ***(int, optional)***: Total number of trees to train in the ensemble.
+    Defaults to 100.
+ - `learning_rate` ***(float, optional)***: Step size to use at each iteration. Each
+    leaf weight is multiplied by this number. The smaller the value, the more
+    conservative the weights will be. Defaults to 0.3.
+ - `max_depth` ***(int, optional)***: Maximum depth of an individual tree. Valid values
+    are 0 to infinity. Defaults to 5.
+ - `max_leaves` ***(int, optional)***: Maximum number of leaves allowed on a tree. Valid values
+    are 0 to infinity. This is the total number of final nodes. Defaults to sys.maxsize.
+ - `l2` ***(float, optional)***: L2 regularization term applied to the weights of the tree. Valid values
+    are 0 to infinity. Defaults to 1.0.
+ - `gamma` ***(float, optional)***: The minimum amount of loss required to further split a node.
+    Valid values are 0 to infinity. Defaults to 0.0.
+ - `min_leaf_weight` ***(float, optional)***: Minimum sum of the hessian values of the loss function
+    required to be in a node. Defaults to 1.0.
+ - `base_score` ***(float, optional)***: The initial prediction value of the model. Defaults to 0.5.
+ - `nbins` ***(int, optional)***: Number of bins to calculate to partition the data. Setting this to
+    a smaller number, will result in faster training time, while potentially sacrificing
+    accuracy. If there are more bins, than unique values in a column, all unique values
+    will be used. Defaults to 256.
+ - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
+    with this model? Defaults to `True`.
+ - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. If `create_missing_branch` is set to `True` having this parameter be set to `True` will result in the missing branch further split, if this parameter is `False` then in that case the missing branch will always be a terminal node. Defaults to `True`.
+ - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
+ - `subsample` ***(float, optional)***: Percent of records to randomly sample at each iteration when
+      training a tree. Defaults to 1.0, meaning all data is used for training.
+ - `seed` ***(integer, optional)***: Integer value used to seed any randomness used in the
+      algorithm. Defaults to 0.
+ - `missing` ***(float, optional)***: Value to consider missing, when training and predicting with the booster. Defaults to `np.nan`.
+ - `create_missing_branch` ***(bool, optional)***: An experimental parameter, that if `True`, will create a separate branch for missing, creating a ternary tree, the missing node will be given the same weight value as the parent node. If this parameter is `False`, missing will be sent down either the left or right branch, creating a binary tree. Defaults to `False`.
+ - `sample_method` ***(str | None, optional)***: Optional string value to use to determine the method to use to sample the data while training. If this is None, no sample method will be used. If the `subsample` parameter is less than 1 and no sample_method is provided this `sample_method` will be automatically set to "random". Valid options are "goss" and "random". Defaults to `None`.
+ - `evaluation_metric` ***(str | None, optional)***: Optional string value used to define an evaluation metric that will be calculated at each iteration if a `evaluation_dataset` is provided at fit time. The metric can be one of "AUC", "LogLoss", "RootMeanSquaredLogError", or "RootMeanSquaredError". If no `evaluation_metric` is passed, but an `evaluation_dataset` is passed, then "LogLoss", will be used with the "LogLoss" objective function, and "RootMeanSquaredLogError" will be used with "SquaredLoss".
+ - `early_stopping_rounds` ***(int | None, optional)***: If this is specified, and an `evaluation_dataset` is passed during fit, then an improvement in the `evaluation_metric` must be seen after at least this many iterations of training, otherwise training will be cut short.
+
+### Training and Predicting
+
+Once, the booster has been initialized, it can be fit on a provided dataset, and performance field. After fitting, the model can be used to predict on a dataset.
+In the case of this example, the predictions are the log odds of a given record being 1.
+
+```python
+# Small example dataset
+from seaborn import load_dataset
+
+df = load_dataset("titanic")
+X = df.select_dtypes("number").drop(columns=["survived"])
+y = df["survived"]
+
+# Initialize a booster with defaults.
+from forust import GradientBooster
+model = GradientBooster(objective_type="LogLoss")
+model.fit(X, y)
+
+# Predict on data
+model.predict(X.head())
+# array([-1.94919663,  2.25863229,  0.32963671,  2.48732194, -3.00371813])
+
+# predict contributions
+model.predict_contributions(X.head())
+# array([[-0.63014213,  0.33880048, -0.16520798, -0.07798772, -0.85083578,
+#        -1.07720813],
+#       [ 1.05406709,  0.08825999,  0.21662544, -0.12083538,  0.35209258,
+#        -1.07720813],
+```
+
+The `fit` method accepts the following arguments.
+ - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
+ - `y` ***(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If "LogLoss" was
+   the objective type specified, then this should only contain 1 or 0 values, where 1 is the positive class being predicted. If "SquaredLoss" is the objective type, then any continuous variable can be provided.
+ - `sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use when training the model. If None is passed, a weight of 1 will be used for every record. Defaults to None.
+ - `evaluation_data` ***(tuple[FrameLike, ArrayLike, ArrayLike] | tuple[FrameLike, ArrayLike], optional)***: An optional list of tuples, where each tuple should contain a dataset, and equal length target array, and optional an equal length sample weight array. If this is provided metric values will be calculated at each iteration of training. If `early_stopping_rounds` is supplied, the first entry of this list will be used to determine if performance has improved over the last set of iterations, for which if no improvement is not seen in `early_stopping_rounds` training will be cut short.
+
+The predict method accepts the following arguments.
+ - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
+ - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict function should run in parallel on multiple threads. If `None` is passed, the `parallel` attribute of the booster will be used. Defaults to `None`.
+
+The `predict_contributions` method will predict with the fitted booster on new data, returning the feature contribution matrix. The last column is the bias term.
+ - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
+ - `method` ***(str, optional)***: Method to calculate the contributions, if "average" is specified, the average internal node values are calculated, this is equivalent to the `approx_contribs` parameter in XGBoost. The other supported method is "weight", this will use the internal leaf weights, to calculate the contributions. This is the same as what is described by Saabas [here](https://blog.datadive.net/interpreting-random-forests/).
+ - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict function should run in parallel on multiple threads. If `None` is passed, the `parallel` attribute of the booster will be used. Defaults to `None`.
+
+When predicting with the data, the maximum iteration that will be used when predicting can be set using the `set_prediction_iteration` method. If `early_stopping_rounds` has been set, this will default to the best iteration, otherwise all of the trees will be used. It accepts a single value.
+ - `iteration` (int): Iteration number to use, this will use all trees, up to and including this index.
+
+If early stopping was used, the evaluation history can be retrieved with the `get_evaluation_history` method.
+
+```python
+model = GradientBooster(objective_type="LogLoss")
+model.fit(X, y, evaluation_data=[(X, y)])
+
+model.get_evaluation_history()[0:3]
+
+# array([[588.9158873 ],
+#        [532.01055803],
+#        [496.76933646]])
+```
+
+### Inspecting the Model
+
+Once the booster has been fit, each individual tree structure can be retrieved in text form, using the `text_dump` method. This method returns a list, the same length as the number of trees in the model.
+
+```python
+model.text_dump()[0]
+# 0:[0 < 3] yes=1,no=2,missing=2,gain=91.50833,cover=209.388307
+#       1:[4 < 13.7917] yes=3,no=4,missing=4,gain=28.185467,cover=94.00148
+#             3:[1 < 18] yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348
+#                   7:[1 < 17] yes=15,no=16,missing=16,gain=0.691266,cover=0.705011
+#                         15:leaf=-0.15120,cover=0.23500
+#                         16:leaf=0.154097,cover=0.470007
+```
+
+The `json_dump` method performs the same action, but returns the model as a json representation rather than a text string.
+
+To see an estimate for how a given feature is used in the model, the `partial_dependence` method is provided. This method calculates the partial dependence values of a feature. For each unique value of the feature, this gives the estimate of the predicted value for that feature, with the effects of all features averaged out. This information gives an estimate of how a given feature impacts the model.
+
+The `partial_dependence` method takes the following parameters...
+
+ - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array. This should be the same data passed into the models fit, or predict, with the columns in the same order.
+ - `feature` ***(Union[str, int])***: The feature for which to calculate the partial dependence values. This can be the name of a column, if the provided X is a pandas DataFrame, or the index of the feature.
+ - `samples` ***(int | None, optional)***: Number of evenly spaced samples to select. If None is passed all unique values will be used. Defaults to 100.
+ - `exclude_missing` ***(bool, optional)***: Should missing excluded from the features? Defaults to True.
+ - `percentile_bounds` ***(tuple[float, float], optional)***: Upper and lower percentiles to start at  when calculating the samples. Defaults to (0.2, 0.98) to cap the samples selected  at the 5th and 95th percentiles respectively.
+This method returns a 2 dimensional numpy array, where the first column is the sorted unique values of the feature, and then the second column is the partial dependence values for each feature value.
+
+This information can be plotted to visualize how a feature is used in the model, like so.
+
+```python
+from seaborn import lineplot
+import matplotlib.pyplot as plt
+
+pd_values = model.partial_dependence(X=X, feature="age", samples=None)
+
+fig = lineplot(x=pd_values[:,0], y=pd_values[:,1],)
+plt.title("Partial Dependence Plot")
+plt.xlabel("Age")
+plt.ylabel("Log Odds")
+```
+<img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/pdp_plot_age.png">
+
+We can see how this is impacted if a model is created, where a specific constraint is applied to the feature using the `monotone_constraint` parameter.
+
+```python
+model = GradientBooster(
+    objective_type="LogLoss",
+    monotone_constraints={"age": -1},
+)
+model.fit(X, y)
+
+pd_values = model.partial_dependence(X=X, feature="age")
+fig = lineplot(
+    x=pd_values[:, 0],
+    y=pd_values[:, 1],
+)
+plt.title("Partial Dependence Plot with Monotonicity")
+plt.xlabel("Age")
+plt.ylabel("Log Odds")
+```
+<img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/pdp_plot_age_mono.png">
+
+### Saving the model
+To save and subsequently load a trained booster, the `save_booster` and `load_booster` methods can be used. Each accepts a path, which is used to write the model to. The model is saved and loaded as a json object.
+
+```python
+trained_model.save_booster("model_path.json")
+
+# To load a model from a json path.
+loaded_model = GradientBooster.load_model("model_path.json")
+```
+
```

#### html2text {}

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1 Name: forust Version: 0.2.7 Classifier: Programming
+Language :: Rust Classifier: Programming Language :: Python :: Implementation
+:: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: numpy>=1.21 Requires-Dist: pandas>=1.3 Requires-Dist: maturin;
+extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist: seaborn;
+extra == 'dev' Requires-Dist: xgboost==1.6.1; extra == 'dev' Requires-Dist:
+scikit-learn; extra == 'dev' Provides-Extra: dev License-File: LICENSE Summary:
+A lightweight gradient boosting implementation in Rust. Keywords:
+rust,forust,machine learning,xgboost,tree model,decision tree Author: James
+Inlow Requires-Python: >=3.8 Description-Content-Type: text/markdown;
+charset=UTF-8; variant=GFM
    [https://github.com/jinlow/forust/raw/main/resources/tree-image-crop.png]
  ![PyPI](https://img.shields.io/pypi/v/forust?color=gr&style=for-the-badge) !
  [Crates.io](https://img.shields.io/crates/v/forust-ml?color=gr&style=for-the-
                                     badge)
 # Forust ## _A lightweight gradient boosting package_ Forust, is a lightweight
 package for building gradient boosted decision tree ensembles. All of the
 algorithm code is written in [Rust](https://www.rust-lang.org/), with a python
@@ -13,15 +24,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.6" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.7" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -70,56 +81,89 @@
 used in the algorithm. Defaults to 0. - `missing` ***(float, optional)***:
 Value to consider missing, when training and predicting with the booster.
 Defaults to `np.nan`. - `create_missing_branch` ***(bool, optional)***: An
 experimental parameter, that if `True`, will create a separate branch for
 missing, creating a ternary tree, the missing node will be given the same
 weight value as the parent node. If this parameter is `False`, missing will be
 sent down either the left or right branch, creating a binary tree. Defaults to
-`False`. ### Training and Predicting Once, the booster has been initialized, it
-can be fit on a provided dataset, and performance field. After fitting, the
-model can be used to predict on a dataset. In the case of this example, the
-predictions are the log odds of a given record being 1. ```python # Small
-example dataset from seaborn import load_dataset df = load_dataset("titanic") X
-= df.select_dtypes("number").drop(columns=["survived"]) y = df["survived"] #
-Initialize a booster with defaults. from forust import GradientBooster model =
-GradientBooster(objective_type="LogLoss") model.fit(X, y) # Predict on data
-model.predict(X.head()) # array([-1.94919663, 2.25863229, 0.32963671,
-2.48732194, -3.00371813]) # predict contributions model.predict_contributions
-(X.head()) # array([[-0.63014213, 0.33880048, -0.16520798, -0.07798772, -
-0.85083578, # -1.07720813], # [ 1.05406709, 0.08825999, 0.21662544, -
-0.12083538, 0.35209258, # -1.07720813], ``` The `fit` method accepts the
-following arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2
-dimensional numpy array, with numeric data. - `y` ***(ArrayLike)***: Either a
-pandas Series, or a 1 dimensional numpy array. If "LogLoss" was the objective
-type specified, then this should only contain 1 or 0 values, where 1 is the
-positive class being predicted. If "SquaredLoss" is the objective type, then
-any continuous variable can be provided. - `sample_weight` ***(Optional
-[ArrayLike], optional)***: Instance weights to use when training the model. If
-None is passed, a weight of 1 will be used for every record. Defaults to None.
-The predict method accepts the following arguments. - `X` ***(FrameLike)***:
+`False`. - `sample_method` ***(str | None, optional)***: Optional string value
+to use to determine the method to use to sample the data while training. If
+this is None, no sample method will be used. If the `subsample` parameter is
+less than 1 and no sample_method is provided this `sample_method` will be
+automatically set to "random". Valid options are "goss" and "random". Defaults
+to `None`. - `evaluation_metric` ***(str | None, optional)***: Optional string
+value used to define an evaluation metric that will be calculated at each
+iteration if a `evaluation_dataset` is provided at fit time. The metric can be
+one of "AUC", "LogLoss", "RootMeanSquaredLogError", or "RootMeanSquaredError".
+If no `evaluation_metric` is passed, but an `evaluation_dataset` is passed,
+then "LogLoss", will be used with the "LogLoss" objective function, and
+"RootMeanSquaredLogError" will be used with "SquaredLoss". -
+`early_stopping_rounds` ***(int | None, optional)***: If this is specified, and
+an `evaluation_dataset` is passed during fit, then an improvement in the
+`evaluation_metric` must be seen after at least this many iterations of
+training, otherwise training will be cut short. ### Training and Predicting
+Once, the booster has been initialized, it can be fit on a provided dataset,
+and performance field. After fitting, the model can be used to predict on a
+dataset. In the case of this example, the predictions are the log odds of a
+given record being 1. ```python # Small example dataset from seaborn import
+load_dataset df = load_dataset("titanic") X = df.select_dtypes("number").drop
+(columns=["survived"]) y = df["survived"] # Initialize a booster with defaults.
+from forust import GradientBooster model = GradientBooster
+(objective_type="LogLoss") model.fit(X, y) # Predict on data model.predict
+(X.head()) # array([-1.94919663, 2.25863229, 0.32963671, 2.48732194, -
+3.00371813]) # predict contributions model.predict_contributions(X.head()) #
+array([[-0.63014213, 0.33880048, -0.16520798, -0.07798772, -0.85083578, # -
+1.07720813], # [ 1.05406709, 0.08825999, 0.21662544, -0.12083538, 0.35209258, #
+-1.07720813], ``` The `fit` method accepts the following arguments. - `X` ***
+(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with
+numeric data. - `y` ***(ArrayLike)***: Either a pandas Series, or a 1
+dimensional numpy array. If "LogLoss" was the objective type specified, then
+this should only contain 1 or 0 values, where 1 is the positive class being
+predicted. If "SquaredLoss" is the objective type, then any continuous variable
+can be provided. - `sample_weight` ***(Optional[ArrayLike], optional)***:
+Instance weights to use when training the model. If None is passed, a weight of
+1 will be used for every record. Defaults to None. - `evaluation_data` ***
+(tuple[FrameLike, ArrayLike, ArrayLike] | tuple[FrameLike, ArrayLike],
+optional)***: An optional list of tuples, where each tuple should contain a
+dataset, and equal length target array, and optional an equal length sample
+weight array. If this is provided metric values will be calculated at each
+iteration of training. If `early_stopping_rounds` is supplied, the first entry
+of this list will be used to determine if performance has improved over the
+last set of iterations, for which if no improvement is not seen in
+`early_stopping_rounds` training will be cut short. The predict method accepts
+the following arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or
+a 2 dimensional numpy array, with numeric data. - `parallel` ***(Optional
+[bool], optional)***: Optionally specify if the predict function should run in
+parallel on multiple threads. If `None` is passed, the `parallel` attribute of
+the booster will be used. Defaults to `None`. The `predict_contributions`
+method will predict with the fitted booster on new data, returning the feature
+contribution matrix. The last column is the bias term. - `X` ***(FrameLike)***:
 Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data. -
-`parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
-function should run in parallel on multiple threads. If `None` is passed, the
-`parallel` attribute of the booster will be used. Defaults to `None`. The
-`predict_contributions` method will predict with the fitted booster on new
-data, returning the feature contribution matrix. The last column is the bias
-term. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional
-numpy array, with numeric data. - `method` ***(str, optional)***: Method to
-calculate the contributions, if "average" is specified, the average internal
-node values are calculated, this is equivalent to the `approx_contribs`
-parameter in XGBoost. The other supported method is "weight", this will use the
-internal leaf weights, to calculate the contributions. This is the same as what
-is described by Saabas [here](https://blog.datadive.net/interpreting-random-
-forests/). - `parallel` ***(Optional[bool], optional)***: Optionally specify if
-the predict function should run in parallel on multiple threads. If `None` is
-passed, the `parallel` attribute of the booster will be used. Defaults to
-`None`. ### Inspecting the Model Once the booster has been fit, each individual
-tree structure can be retrieved in text form, using the `text_dump` method.
-This method returns a list, the same length as the number of trees in the
-model. ```python model.text_dump()[0] # 0:[0 < 3]
+`method` ***(str, optional)***: Method to calculate the contributions, if
+"average" is specified, the average internal node values are calculated, this
+is equivalent to the `approx_contribs` parameter in XGBoost. The other
+supported method is "weight", this will use the internal leaf weights, to
+calculate the contributions. This is the same as what is described by Saabas
+[here](https://blog.datadive.net/interpreting-random-forests/). - `parallel`
+***(Optional[bool], optional)***: Optionally specify if the predict function
+should run in parallel on multiple threads. If `None` is passed, the `parallel`
+attribute of the booster will be used. Defaults to `None`. When predicting with
+the data, the maximum iteration that will be used when predicting can be set
+using the `set_prediction_iteration` method. If `early_stopping_rounds` has
+been set, this will default to the best iteration, otherwise all of the trees
+will be used. It accepts a single value. - `iteration` (int): Iteration number
+to use, this will use all trees, up to and including this index. If early
+stopping was used, the evaluation history can be retrieved with the
+`get_evaluation_history` method. ```python model = GradientBooster
+(objective_type="LogLoss") model.fit(X, y, evaluation_data=[(X, y)])
+model.get_evaluation_history()[0:3] # array([[588.9158873 ], # [532.01055803],
+# [496.76933646]]) ``` ### Inspecting the Model Once the booster has been fit,
+each individual tree structure can be retrieved in text form, using the
+`text_dump` method. This method returns a list, the same length as the number
+of trees in the model. ```python model.text_dump()[0] # 0:[0 < 3]
 yes=1,no=2,missing=2,gain=91.50833,cover=209.388307 # 1:[4 < 13.7917]
 yes=3,no=4,missing=4,gain=28.185467,cover=94.00148 # 3:[1 < 18]
 yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348 # 7:[1 < 17]
 yes=15,no=16,missing=16,gain=0.691266,cover=0.705011 # 15:leaf=-
 0.15120,cover=0.23500 # 16:leaf=0.154097,cover=0.470007 ``` The `json_dump`
 method performs the same action, but returns the model as a json representation
 rather than a text string. To see an estimate for how a given feature is used
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/benches/forust_benchmarks.rs` & `forust-0.2.7/local_dependencies/forust-ml/benches/forust_benchmarks.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,116 @@
-use criterion::{black_box, criterion_group, criterion_main, Criterion};
-use forust_ml::binning::bin_matrix;
-use forust_ml::constraints::ConstraintMap;
-use forust_ml::data::Matrix;
-use forust_ml::gradientbooster::GradientBooster;
-use forust_ml::objective::{LogLoss, ObjectiveFunction};
-use forust_ml::splitter::MissingImputerSplitter;
-use forust_ml::tree::Tree;
-use forust_ml::utils::{fast_f64_sum, fast_sum, naive_sum};
-use rand::rngs::StdRng;
-use rand::SeedableRng;
-use std::fs;
-use std::time::Duration;
-
-pub fn tree_benchmarks(c: &mut Criterion) {
-    let file = fs::read_to_string("resources/contiguous_no_missing_100k_samp_seed0.csv")
-        .expect("Something went wrong reading the file");
-    let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
-    let file = fs::read_to_string("resources/performance_100k_samp_seed0.csv")
-        .expect("Something went wrong reading the file");
-    let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
-    let yhat = vec![0.5; y.len()];
-    let w = vec![1.; y.len()];
-    let g = LogLoss::calc_grad(&y, &yhat, &w);
-    let h = LogLoss::calc_hess(&y, &yhat, &w);
-
-    let v: Vec<f32> = vec![10.; 300000];
-    c.bench_function("Niave Sum", |b| b.iter(|| naive_sum(black_box(&v))));
-    c.bench_function("fast sum", |b| b.iter(|| fast_sum(black_box(&v))));
-    c.bench_function("fast f64 sum", |b| b.iter(|| fast_f64_sum(black_box(&v))));
-
-    c.bench_function("calc_grad", |b| {
-        b.iter(|| LogLoss::calc_grad(black_box(&y), black_box(&yhat), black_box(&w)))
-    });
-
-    c.bench_function("calc_hess", |b| {
-        b.iter(|| LogLoss::calc_hess(black_box(&y), black_box(&yhat), black_box(&w)))
-    });
-
-    let data = Matrix::new(&data_vec, y.len(), 5);
-    let splitter = MissingImputerSplitter {
-        l2: 1.0,
-        gamma: 3.0,
-        min_leaf_weight: 1.0,
-        learning_rate: 0.3,
-        allow_missing_splits: true,
-        constraints_map: ConstraintMap::new(),
-    };
-    let mut tree = Tree::new();
-
-    let bindata = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
-    let bdata = Matrix::new(&bindata.binned_data, data.rows, data.cols);
-    let mut rng = StdRng::seed_from_u64(0);
-    tree.fit(
-        &bdata,
-        &bindata.cuts,
-        &g,
-        &h,
-        &splitter,
-        usize::MAX,
-        5,
-        true,
-        1.,
-        &mut rng,
-    );
-    println!("{}", tree.nodes.len());
-    c.bench_function("Train Tree", |b| {
-        b.iter(|| {
-            let mut train_tree: Tree = Tree::new();
-            train_tree.fit(
-                black_box(&bdata),
-                black_box(&bindata.cuts),
-                black_box(&g),
-                black_box(&h),
-                black_box(&splitter),
-                black_box(usize::MAX),
-                black_box(10),
-                black_box(false),
-                black_box(1.0),
-                black_box(&mut rng),
-            );
-        })
-    });
-    c.bench_function("Tree Predict (Single Threaded)", |b| {
-        b.iter(|| tree.predict(black_box(&data), black_box(false), black_box(&f64::NAN)))
-    });
-    c.bench_function("Tree Predict (Multi Threaded)", |b| {
-        b.iter(|| tree.predict(black_box(&data), black_box(true), black_box(&f64::NAN)))
-    });
-
-    // Gradient Booster
-    // Bench building
-    let mut booster_train = c.benchmark_group("train-booster");
-    booster_train.warm_up_time(Duration::from_secs(10));
-    booster_train.sample_size(50);
-    // booster_train.sampling_mode(SamplingMode::Linear);
-    booster_train.bench_function("Train Booster", |b| {
-        b.iter(|| {
-            let mut booster = GradientBooster::default().set_parallel(false);
-            booster
-                .fit(black_box(&data), black_box(&y), black_box(&w))
-                .unwrap();
-        })
-    });
-    let mut booster = GradientBooster::default();
-    booster.fit(&data, &y, &w).unwrap();
-    booster_train.bench_function("Predict Booster", |b| {
-        b.iter(|| booster.predict(black_box(&data), false))
-    });
-}
-
-criterion_group!(benches, tree_benchmarks);
-criterion_main!(benches);
+use criterion::{black_box, criterion_group, criterion_main, Criterion};
+use forust_ml::binning::bin_matrix;
+use forust_ml::constraints::ConstraintMap;
+use forust_ml::data::Matrix;
+use forust_ml::gradientbooster::GradientBooster;
+use forust_ml::objective::{LogLoss, ObjectiveFunction};
+use forust_ml::sampler::SampleMethod;
+use forust_ml::splitter::MissingImputerSplitter;
+use forust_ml::tree::Tree;
+use forust_ml::utils::{fast_f64_sum, fast_sum, naive_sum};
+use std::fs;
+use std::time::Duration;
+
+pub fn tree_benchmarks(c: &mut Criterion) {
+    let file = fs::read_to_string("resources/contiguous_no_missing_100k_samp_seed0.csv")
+        .expect("Something went wrong reading the file");
+    let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+    let file = fs::read_to_string("resources/performance_100k_samp_seed0.csv")
+        .expect("Something went wrong reading the file");
+    let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+    let yhat = vec![0.5; y.len()];
+    let w = vec![1.; y.len()];
+    let g = LogLoss::calc_grad(&y, &yhat, &w);
+    let h = LogLoss::calc_hess(&y, &yhat, &w);
+
+    let v: Vec<f32> = vec![10.; 300000];
+    c.bench_function("Niave Sum", |b| b.iter(|| naive_sum(black_box(&v))));
+    c.bench_function("fast sum", |b| b.iter(|| fast_sum(black_box(&v))));
+    c.bench_function("fast f64 sum", |b| b.iter(|| fast_f64_sum(black_box(&v))));
+
+    c.bench_function("calc_grad", |b| {
+        b.iter(|| LogLoss::calc_grad(black_box(&y), black_box(&yhat), black_box(&w)))
+    });
+
+    c.bench_function("calc_hess", |b| {
+        b.iter(|| LogLoss::calc_hess(black_box(&y), black_box(&yhat), black_box(&w)))
+    });
+
+    let data = Matrix::new(&data_vec, y.len(), 5);
+    let splitter = MissingImputerSplitter {
+        l2: 1.0,
+        gamma: 3.0,
+        min_leaf_weight: 1.0,
+        learning_rate: 0.3,
+        allow_missing_splits: true,
+        constraints_map: ConstraintMap::new(),
+    };
+    let mut tree = Tree::new();
+
+    let bindata = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
+    let bdata = Matrix::new(&bindata.binned_data, data.rows, data.cols);
+    tree.fit(
+        &bdata,
+        data.index.to_owned(),
+        &bindata.cuts,
+        &g,
+        &h,
+        &splitter,
+        usize::MAX,
+        5,
+        true,
+        &SampleMethod::None,
+    );
+    println!("{}", tree.nodes.len());
+    c.bench_function("Train Tree", |b| {
+        b.iter(|| {
+            let mut train_tree: Tree = Tree::new();
+            train_tree.fit(
+                black_box(&bdata),
+                black_box(data.index.to_owned()),
+                black_box(&bindata.cuts),
+                black_box(&g),
+                black_box(&h),
+                black_box(&splitter),
+                black_box(usize::MAX),
+                black_box(10),
+                black_box(false),
+                black_box(&SampleMethod::None),
+            );
+        })
+    });
+    c.bench_function("Tree Predict (Single Threaded)", |b| {
+        b.iter(|| tree.predict(black_box(&data), black_box(false), black_box(&f64::NAN)))
+    });
+    c.bench_function("Tree Predict (Multi Threaded)", |b| {
+        b.iter(|| tree.predict(black_box(&data), black_box(true), black_box(&f64::NAN)))
+    });
+
+    // Gradient Booster
+    // Bench building
+    let mut booster_train = c.benchmark_group("train-booster");
+    booster_train.warm_up_time(Duration::from_secs(10));
+    booster_train.sample_size(50);
+    // booster_train.sampling_mode(SamplingMode::Linear);
+    booster_train.bench_function("Train Booster", |b| {
+        b.iter(|| {
+            let mut booster = GradientBooster::default().set_parallel(false);
+            booster
+                .fit(
+                    black_box(&data),
+                    black_box(&y),
+                    black_box(&w),
+                    black_box(None),
+                )
+                .unwrap();
+        })
+    });
+    let mut booster = GradientBooster::default();
+    booster.fit(&data, &y, &w, None).unwrap();
+    booster_train.bench_function("Predict Booster", |b| {
+        b.iter(|| booster.predict(black_box(&data), false))
+    });
+}
+
+criterion_group!(benches, tree_benchmarks);
+criterion_main!(benches);
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/resources/pdp_plot_age.png` & `forust-0.2.7/local_dependencies/forust-ml/resources/pdp_plot_age.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.6/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png` & `forust-0.2.7/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.6/local_dependencies/forust-ml/resources/titanic.csv` & `forust-0.2.7/local_dependencies/forust-ml/resources/titanic.csv`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,892 +1,892 @@
-survived,pclass,sex,age,sibsp,parch,fare,embarked,class,who,adult_male,deck,embark_town,alive,alone
-0,3,male,22.0,1,0,7.25,S,Third,man,True,,Southampton,no,False
-1,1,female,38.0,1,0,71.2833,C,First,woman,False,C,Cherbourg,yes,False
-1,3,female,26.0,0,0,7.925,S,Third,woman,False,,Southampton,yes,True
-1,1,female,35.0,1,0,53.1,S,First,woman,False,C,Southampton,yes,False
-0,3,male,35.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,8.4583,Q,Third,man,True,,Queenstown,no,True
-0,1,male,54.0,0,0,51.8625,S,First,man,True,E,Southampton,no,True
-0,3,male,2.0,3,1,21.075,S,Third,child,False,,Southampton,no,False
-1,3,female,27.0,0,2,11.1333,S,Third,woman,False,,Southampton,yes,False
-1,2,female,14.0,1,0,30.0708,C,Second,child,False,,Cherbourg,yes,False
-1,3,female,4.0,1,1,16.7,S,Third,child,False,G,Southampton,yes,False
-1,1,female,58.0,0,0,26.55,S,First,woman,False,C,Southampton,yes,True
-0,3,male,20.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,male,39.0,1,5,31.275,S,Third,man,True,,Southampton,no,False
-0,3,female,14.0,0,0,7.8542,S,Third,child,False,,Southampton,no,True
-1,2,female,55.0,0,0,16.0,S,Second,woman,False,,Southampton,yes,True
-0,3,male,2.0,4,1,29.125,Q,Third,child,False,,Queenstown,no,False
-1,2,male,,0,0,13.0,S,Second,man,True,,Southampton,yes,True
-0,3,female,31.0,1,0,18.0,S,Third,woman,False,,Southampton,no,False
-1,3,female,,0,0,7.225,C,Third,woman,False,,Cherbourg,yes,True
-0,2,male,35.0,0,0,26.0,S,Second,man,True,,Southampton,no,True
-1,2,male,34.0,0,0,13.0,S,Second,man,True,D,Southampton,yes,True
-1,3,female,15.0,0,0,8.0292,Q,Third,child,False,,Queenstown,yes,True
-1,1,male,28.0,0,0,35.5,S,First,man,True,A,Southampton,yes,True
-0,3,female,8.0,3,1,21.075,S,Third,child,False,,Southampton,no,False
-1,3,female,38.0,1,5,31.3875,S,Third,woman,False,,Southampton,yes,False
-0,3,male,,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
-0,1,male,19.0,3,2,263.0,S,First,man,True,C,Southampton,no,False
-1,3,female,,0,0,7.8792,Q,Third,woman,False,,Queenstown,yes,True
-0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,1,male,40.0,0,0,27.7208,C,First,man,True,,Cherbourg,no,True
-1,1,female,,1,0,146.5208,C,First,woman,False,B,Cherbourg,yes,False
-1,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
-0,2,male,66.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
-0,1,male,28.0,1,0,82.1708,C,First,man,True,,Cherbourg,no,False
-0,1,male,42.0,1,0,52.0,S,First,man,True,,Southampton,no,False
-1,3,male,,0,0,7.2292,C,Third,man,True,,Cherbourg,yes,True
-0,3,male,21.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,female,18.0,2,0,18.0,S,Third,woman,False,,Southampton,no,False
-1,3,female,14.0,1,0,11.2417,C,Third,child,False,,Cherbourg,yes,False
-0,3,female,40.0,1,0,9.475,S,Third,woman,False,,Southampton,no,False
-0,2,female,27.0,1,0,21.0,S,Second,woman,False,,Southampton,no,False
-0,3,male,,0,0,7.8958,C,Third,man,True,,Cherbourg,no,True
-1,2,female,3.0,1,2,41.5792,C,Second,child,False,,Cherbourg,yes,False
-1,3,female,19.0,0,0,7.8792,Q,Third,woman,False,,Queenstown,yes,True
-0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,male,,1,0,15.5,Q,Third,man,True,,Queenstown,no,False
-1,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
-0,3,male,,2,0,21.6792,C,Third,man,True,,Cherbourg,no,False
-0,3,female,18.0,1,0,17.8,S,Third,woman,False,,Southampton,no,False
-0,3,male,7.0,4,1,39.6875,S,Third,child,False,,Southampton,no,False
-0,3,male,21.0,0,0,7.8,S,Third,man,True,,Southampton,no,True
-1,1,female,49.0,1,0,76.7292,C,First,woman,False,D,Cherbourg,yes,False
-1,2,female,29.0,1,0,26.0,S,Second,woman,False,,Southampton,yes,False
-0,1,male,65.0,0,1,61.9792,C,First,man,True,B,Cherbourg,no,False
-1,1,male,,0,0,35.5,S,First,man,True,C,Southampton,yes,True
-1,2,female,21.0,0,0,10.5,S,Second,woman,False,,Southampton,yes,True
-0,3,male,28.5,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
-1,2,female,5.0,1,2,27.75,S,Second,child,False,,Southampton,yes,False
-0,3,male,11.0,5,2,46.9,S,Third,child,False,,Southampton,no,False
-0,3,male,22.0,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
-1,1,female,38.0,0,0,80.0,,First,woman,False,B,,yes,True
-0,1,male,45.0,1,0,83.475,S,First,man,True,C,Southampton,no,False
-0,3,male,4.0,3,2,27.9,S,Third,child,False,,Southampton,no,False
-0,1,male,,0,0,27.7208,C,First,man,True,,Cherbourg,no,True
-1,3,male,,1,1,15.2458,C,Third,man,True,,Cherbourg,yes,False
-1,2,female,29.0,0,0,10.5,S,Second,woman,False,F,Southampton,yes,True
-0,3,male,19.0,0,0,8.1583,S,Third,man,True,,Southampton,no,True
-1,3,female,17.0,4,2,7.925,S,Third,woman,False,,Southampton,yes,False
-0,3,male,26.0,2,0,8.6625,S,Third,man,True,,Southampton,no,False
-0,2,male,32.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
-0,3,female,16.0,5,2,46.9,S,Third,woman,False,,Southampton,no,False
-0,2,male,21.0,0,0,73.5,S,Second,man,True,,Southampton,no,True
-0,3,male,26.0,1,0,14.4542,C,Third,man,True,,Cherbourg,no,False
-1,3,male,32.0,0,0,56.4958,S,Third,man,True,,Southampton,yes,True
-0,3,male,25.0,0,0,7.65,S,Third,man,True,F,Southampton,no,True
-0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
-1,2,male,0.83,0,2,29.0,S,Second,child,False,,Southampton,yes,False
-1,3,female,30.0,0,0,12.475,S,Third,woman,False,,Southampton,yes,True
-0,3,male,22.0,0,0,9.0,S,Third,man,True,,Southampton,no,True
-1,3,male,29.0,0,0,9.5,S,Third,man,True,,Southampton,yes,True
-1,3,female,,0,0,7.7875,Q,Third,woman,False,,Queenstown,yes,True
-0,1,male,28.0,0,0,47.1,S,First,man,True,,Southampton,no,True
-1,2,female,17.0,0,0,10.5,S,Second,woman,False,,Southampton,yes,True
-1,3,female,33.0,3,0,15.85,S,Third,woman,False,,Southampton,yes,False
-0,3,male,16.0,1,3,34.375,S,Third,man,True,,Southampton,no,False
-0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
-1,1,female,23.0,3,2,263.0,S,First,woman,False,C,Southampton,yes,False
-0,3,male,24.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,male,29.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,male,20.0,0,0,7.8542,S,Third,man,True,,Southampton,no,True
-0,1,male,46.0,1,0,61.175,S,First,man,True,E,Southampton,no,False
-0,3,male,26.0,1,2,20.575,S,Third,man,True,,Southampton,no,False
-0,3,male,59.0,0,0,7.25,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,1,male,71.0,0,0,34.6542,C,First,man,True,A,Cherbourg,no,True
-1,1,male,23.0,0,1,63.3583,C,First,man,True,D,Cherbourg,yes,False
-1,2,female,34.0,0,1,23.0,S,Second,woman,False,,Southampton,yes,False
-0,2,male,34.0,1,0,26.0,S,Second,man,True,,Southampton,no,False
-0,3,female,28.0,0,0,7.8958,S,Third,woman,False,,Southampton,no,True
-0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,1,male,21.0,0,1,77.2875,S,First,man,True,D,Southampton,no,False
-0,3,male,33.0,0,0,8.6542,S,Third,man,True,,Southampton,no,True
-0,3,male,37.0,2,0,7.925,S,Third,man,True,,Southampton,no,False
-0,3,male,28.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-1,3,female,21.0,0,0,7.65,S,Third,woman,False,,Southampton,yes,True
-1,3,male,,0,0,7.775,S,Third,man,True,,Southampton,yes,True
-0,3,male,38.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-1,3,female,,1,0,24.15,Q,Third,woman,False,,Queenstown,yes,False
-0,1,male,47.0,0,0,52.0,S,First,man,True,C,Southampton,no,True
-0,3,female,14.5,1,0,14.4542,C,Third,child,False,,Cherbourg,no,False
-0,3,male,22.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,female,20.0,1,0,9.825,S,Third,woman,False,,Southampton,no,False
-0,3,female,17.0,0,0,14.4583,C,Third,woman,False,,Cherbourg,no,True
-0,3,male,21.0,0,0,7.925,S,Third,man,True,,Southampton,no,True
-0,3,male,70.5,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
-0,2,male,29.0,1,0,21.0,S,Second,man,True,,Southampton,no,False
-0,1,male,24.0,0,1,247.5208,C,First,man,True,B,Cherbourg,no,False
-0,3,female,2.0,4,2,31.275,S,Third,child,False,,Southampton,no,False
-0,2,male,21.0,2,0,73.5,S,Second,man,True,,Southampton,no,False
-0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,2,male,32.5,1,0,30.0708,C,Second,man,True,,Cherbourg,no,False
-1,2,female,32.5,0,0,13.0,S,Second,woman,False,E,Southampton,yes,True
-0,1,male,54.0,0,1,77.2875,S,First,man,True,D,Southampton,no,False
-1,3,male,12.0,1,0,11.2417,C,Third,child,False,,Cherbourg,yes,False
-0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
-1,3,male,24.0,0,0,7.1417,S,Third,man,True,,Southampton,yes,True
-1,3,female,,1,1,22.3583,C,Third,woman,False,F,Cherbourg,yes,False
-0,3,male,45.0,0,0,6.975,S,Third,man,True,,Southampton,no,True
-0,3,male,33.0,0,0,7.8958,C,Third,man,True,,Cherbourg,no,True
-0,3,male,20.0,0,0,7.05,S,Third,man,True,,Southampton,no,True
-0,3,female,47.0,1,0,14.5,S,Third,woman,False,,Southampton,no,False
-1,2,female,29.0,1,0,26.0,S,Second,woman,False,,Southampton,yes,False
-0,2,male,25.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,2,male,23.0,0,0,15.0458,C,Second,man,True,,Cherbourg,no,True
-1,1,female,19.0,0,2,26.2833,S,First,woman,False,D,Southampton,yes,False
-0,1,male,37.0,1,0,53.1,S,First,man,True,C,Southampton,no,False
-0,3,male,16.0,0,0,9.2167,S,Third,man,True,,Southampton,no,True
-0,1,male,24.0,0,0,79.2,C,First,man,True,B,Cherbourg,no,True
-0,3,female,,0,2,15.2458,C,Third,woman,False,,Cherbourg,no,False
-1,3,female,22.0,0,0,7.75,S,Third,woman,False,,Southampton,yes,True
-1,3,female,24.0,1,0,15.85,S,Third,woman,False,,Southampton,yes,False
-0,3,male,19.0,0,0,6.75,Q,Third,man,True,,Queenstown,no,True
-0,2,male,18.0,0,0,11.5,S,Second,man,True,,Southampton,no,True
-0,2,male,19.0,1,1,36.75,S,Second,man,True,,Southampton,no,False
-1,3,male,27.0,0,0,7.7958,S,Third,man,True,,Southampton,yes,True
-0,3,female,9.0,2,2,34.375,S,Third,child,False,,Southampton,no,False
-0,2,male,36.5,0,2,26.0,S,Second,man,True,F,Southampton,no,False
-0,2,male,42.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,2,male,51.0,0,0,12.525,S,Second,man,True,,Southampton,no,True
-1,1,female,22.0,1,0,66.6,S,First,woman,False,C,Southampton,yes,False
-0,3,male,55.5,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,male,40.5,0,2,14.5,S,Third,man,True,,Southampton,no,False
-0,3,male,,0,0,7.3125,S,Third,man,True,,Southampton,no,True
-0,1,male,51.0,0,1,61.3792,C,First,man,True,,Cherbourg,no,False
-1,3,female,16.0,0,0,7.7333,Q,Third,woman,False,,Queenstown,yes,True
-0,3,male,30.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,8.6625,S,Third,man,True,,Southampton,no,True
-0,3,male,,8,2,69.55,S,Third,man,True,,Southampton,no,False
-0,3,male,44.0,0,1,16.1,S,Third,man,True,,Southampton,no,False
-1,2,female,40.0,0,0,15.75,S,Second,woman,False,,Southampton,yes,True
-0,3,male,26.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
-0,3,male,17.0,0,0,8.6625,S,Third,man,True,,Southampton,no,True
-0,3,male,1.0,4,1,39.6875,S,Third,child,False,,Southampton,no,False
-1,3,male,9.0,0,2,20.525,S,Third,child,False,,Southampton,yes,False
-1,1,female,,0,1,55.0,S,First,woman,False,E,Southampton,yes,False
-0,3,female,45.0,1,4,27.9,S,Third,woman,False,,Southampton,no,False
-0,1,male,,0,0,25.925,S,First,man,True,,Southampton,no,True
-0,3,male,28.0,0,0,56.4958,S,Third,man,True,,Southampton,no,True
-0,1,male,61.0,0,0,33.5,S,First,man,True,B,Southampton,no,True
-0,3,male,4.0,4,1,29.125,Q,Third,child,False,,Queenstown,no,False
-1,3,female,1.0,1,1,11.1333,S,Third,child,False,,Southampton,yes,False
-0,3,male,21.0,0,0,7.925,S,Third,man,True,,Southampton,no,True
-0,1,male,56.0,0,0,30.6958,C,First,man,True,A,Cherbourg,no,True
-0,3,male,18.0,1,1,7.8542,S,Third,man,True,,Southampton,no,False
-0,3,male,,3,1,25.4667,S,Third,man,True,,Southampton,no,False
-0,1,female,50.0,0,0,28.7125,C,First,woman,False,C,Cherbourg,no,True
-0,2,male,30.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,3,male,36.0,0,0,0.0,S,Third,man,True,,Southampton,no,True
-0,3,female,,8,2,69.55,S,Third,woman,False,,Southampton,no,False
-0,2,male,,0,0,15.05,C,Second,man,True,,Cherbourg,no,True
-0,3,male,9.0,4,2,31.3875,S,Third,child,False,,Southampton,no,False
-1,2,male,1.0,2,1,39.0,S,Second,child,False,F,Southampton,yes,False
-1,3,female,4.0,0,2,22.025,S,Third,child,False,,Southampton,yes,False
-0,1,male,,0,0,50.0,S,First,man,True,A,Southampton,no,True
-1,3,female,,1,0,15.5,Q,Third,woman,False,,Queenstown,yes,False
-1,1,male,45.0,0,0,26.55,S,First,man,True,,Southampton,yes,True
-0,3,male,40.0,1,1,15.5,Q,Third,man,True,,Queenstown,no,False
-0,3,male,36.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-1,2,female,32.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
-0,2,male,19.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-1,3,female,19.0,1,0,7.8542,S,Third,woman,False,,Southampton,yes,False
-1,2,male,3.0,1,1,26.0,S,Second,child,False,F,Southampton,yes,False
-1,1,female,44.0,0,0,27.7208,C,First,woman,False,B,Cherbourg,yes,True
-1,1,female,58.0,0,0,146.5208,C,First,woman,False,B,Cherbourg,yes,True
-0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
-0,3,male,42.0,0,1,8.4042,S,Third,man,True,,Southampton,no,False
-1,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
-0,2,female,24.0,0,0,13.0,S,Second,woman,False,,Southampton,no,True
-0,3,male,28.0,0,0,9.5,S,Third,man,True,,Southampton,no,True
-0,3,male,,8,2,69.55,S,Third,man,True,,Southampton,no,False
-0,3,male,34.0,0,0,6.4958,S,Third,man,True,,Southampton,no,True
-0,3,male,45.5,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
-1,3,male,18.0,0,0,8.05,S,Third,man,True,,Southampton,yes,True
-0,3,female,2.0,0,1,10.4625,S,Third,child,False,G,Southampton,no,False
-0,3,male,32.0,1,0,15.85,S,Third,man,True,,Southampton,no,False
-1,3,male,26.0,0,0,18.7875,C,Third,man,True,,Cherbourg,yes,True
-1,3,female,16.0,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
-1,1,male,40.0,0,0,31.0,C,First,man,True,A,Cherbourg,yes,True
-0,3,male,24.0,0,0,7.05,S,Third,man,True,,Southampton,no,True
-1,2,female,35.0,0,0,21.0,S,Second,woman,False,,Southampton,yes,True
-0,3,male,22.0,0,0,7.25,S,Third,man,True,,Southampton,no,True
-0,2,male,30.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,3,male,,1,0,7.75,Q,Third,man,True,,Queenstown,no,False
-1,1,female,31.0,1,0,113.275,C,First,woman,False,D,Cherbourg,yes,False
-1,3,female,27.0,0,0,7.925,S,Third,woman,False,,Southampton,yes,True
-0,2,male,42.0,1,0,27.0,S,Second,man,True,,Southampton,no,False
-1,1,female,32.0,0,0,76.2917,C,First,woman,False,D,Cherbourg,yes,True
-0,2,male,30.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
-1,3,male,16.0,0,0,8.05,S,Third,man,True,,Southampton,yes,True
-0,2,male,27.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,3,male,51.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-1,1,male,38.0,1,0,90.0,S,First,man,True,C,Southampton,yes,False
-0,3,male,22.0,0,0,9.35,S,Third,man,True,,Southampton,no,True
-1,2,male,19.0,0,0,10.5,S,Second,man,True,,Southampton,yes,True
-0,3,male,20.5,0,0,7.25,S,Third,man,True,,Southampton,no,True
-0,2,male,18.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,3,female,,3,1,25.4667,S,Third,woman,False,,Southampton,no,False
-1,1,female,35.0,1,0,83.475,S,First,woman,False,C,Southampton,yes,False
-0,3,male,29.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
-0,2,male,59.0,0,0,13.5,S,Second,man,True,,Southampton,no,True
-1,3,female,5.0,4,2,31.3875,S,Third,child,False,,Southampton,yes,False
-0,2,male,24.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
-0,3,female,,0,0,7.55,S,Third,woman,False,,Southampton,no,True
-0,2,male,44.0,1,0,26.0,S,Second,man,True,,Southampton,no,False
-1,2,female,8.0,0,2,26.25,S,Second,child,False,,Southampton,yes,False
-0,2,male,19.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
-0,2,male,33.0,0,0,12.275,S,Second,man,True,,Southampton,no,True
-0,3,female,,1,0,14.4542,C,Third,woman,False,,Cherbourg,no,False
-1,3,female,,1,0,15.5,Q,Third,woman,False,,Queenstown,yes,False
-0,2,male,29.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
-0,3,male,22.0,0,0,7.125,S,Third,man,True,,Southampton,no,True
-0,3,male,30.0,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
-0,1,male,44.0,2,0,90.0,Q,First,man,True,C,Queenstown,no,False
-0,3,female,25.0,0,0,7.775,S,Third,woman,False,,Southampton,no,True
-1,2,female,24.0,0,2,14.5,S,Second,woman,False,,Southampton,yes,False
-1,1,male,37.0,1,1,52.5542,S,First,man,True,D,Southampton,yes,False
-0,2,male,54.0,1,0,26.0,S,Second,man,True,,Southampton,no,False
-0,3,male,,0,0,7.25,S,Third,man,True,,Southampton,no,True
-0,3,female,29.0,1,1,10.4625,S,Third,woman,False,G,Southampton,no,False
-0,1,male,62.0,0,0,26.55,S,First,man,True,C,Southampton,no,True
-0,3,male,30.0,1,0,16.1,S,Third,man,True,,Southampton,no,False
-0,3,female,41.0,0,2,20.2125,S,Third,woman,False,,Southampton,no,False
-1,3,female,29.0,0,2,15.2458,C,Third,woman,False,,Cherbourg,yes,False
-1,1,female,,0,0,79.2,C,First,woman,False,,Cherbourg,yes,True
-1,1,female,30.0,0,0,86.5,S,First,woman,False,B,Southampton,yes,True
-1,1,female,35.0,0,0,512.3292,C,First,woman,False,,Cherbourg,yes,True
-1,2,female,50.0,0,1,26.0,S,Second,woman,False,,Southampton,yes,False
-0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
-1,3,male,3.0,4,2,31.3875,S,Third,child,False,,Southampton,yes,False
-0,1,male,52.0,1,1,79.65,S,First,man,True,E,Southampton,no,False
-0,1,male,40.0,0,0,0.0,S,First,man,True,B,Southampton,no,True
-0,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,no,True
-0,2,male,36.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
-0,3,male,16.0,4,1,39.6875,S,Third,man,True,,Southampton,no,False
-1,3,male,25.0,1,0,7.775,S,Third,man,True,,Southampton,yes,False
-1,1,female,58.0,0,1,153.4625,S,First,woman,False,C,Southampton,yes,False
-1,1,female,35.0,0,0,135.6333,S,First,woman,False,C,Southampton,yes,True
-0,1,male,,0,0,31.0,S,First,man,True,,Southampton,no,True
-1,3,male,25.0,0,0,0.0,S,Third,man,True,,Southampton,yes,True
-1,2,female,41.0,0,1,19.5,S,Second,woman,False,,Southampton,yes,False
-0,1,male,37.0,0,1,29.7,C,First,man,True,C,Cherbourg,no,False
-1,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
-1,1,female,63.0,1,0,77.9583,S,First,woman,False,D,Southampton,yes,False
-0,3,female,45.0,0,0,7.75,S,Third,woman,False,,Southampton,no,True
-0,2,male,,0,0,0.0,S,Second,man,True,,Southampton,no,True
-0,3,male,7.0,4,1,29.125,Q,Third,child,False,,Queenstown,no,False
-1,3,female,35.0,1,1,20.25,S,Third,woman,False,,Southampton,yes,False
-0,3,male,65.0,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
-0,3,male,28.0,0,0,7.8542,S,Third,man,True,,Southampton,no,True
-0,3,male,16.0,0,0,9.5,S,Third,man,True,,Southampton,no,True
-1,3,male,19.0,0,0,8.05,S,Third,man,True,,Southampton,yes,True
-0,1,male,,0,0,26.0,S,First,man,True,A,Southampton,no,True
-0,3,male,33.0,0,0,8.6625,C,Third,man,True,,Cherbourg,no,True
-1,3,male,30.0,0,0,9.5,S,Third,man,True,,Southampton,yes,True
-0,3,male,22.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-1,2,male,42.0,0,0,13.0,S,Second,man,True,,Southampton,yes,True
-1,3,female,22.0,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
-1,1,female,26.0,0,0,78.85,S,First,woman,False,,Southampton,yes,True
-1,1,female,19.0,1,0,91.0792,C,First,woman,False,B,Cherbourg,yes,False
-0,2,male,36.0,0,0,12.875,C,Second,man,True,D,Cherbourg,no,True
-0,3,female,24.0,0,0,8.85,S,Third,woman,False,,Southampton,no,True
-0,3,male,24.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,1,male,,0,0,27.7208,C,First,man,True,,Cherbourg,no,True
-0,3,male,23.5,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
-0,1,female,2.0,1,2,151.55,S,First,child,False,C,Southampton,no,False
-1,1,male,,0,0,30.5,S,First,man,True,C,Southampton,yes,True
-1,1,female,50.0,0,1,247.5208,C,First,woman,False,B,Cherbourg,yes,False
-1,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
-1,3,male,,2,0,23.25,Q,Third,man,True,,Queenstown,yes,False
-0,3,male,19.0,0,0,0.0,S,Third,man,True,,Southampton,no,True
-1,2,female,,0,0,12.35,Q,Second,woman,False,E,Queenstown,yes,True
-0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
-1,1,male,0.92,1,2,151.55,S,First,child,False,C,Southampton,yes,False
-1,1,female,,0,0,110.8833,C,First,woman,False,,Cherbourg,yes,True
-1,1,female,17.0,1,0,108.9,C,First,woman,False,C,Cherbourg,yes,False
-0,2,male,30.0,1,0,24.0,C,Second,man,True,,Cherbourg,no,False
-1,1,female,30.0,0,0,56.9292,C,First,woman,False,E,Cherbourg,yes,True
-1,1,female,24.0,0,0,83.1583,C,First,woman,False,C,Cherbourg,yes,True
-1,1,female,18.0,2,2,262.375,C,First,woman,False,B,Cherbourg,yes,False
-0,2,female,26.0,1,1,26.0,S,Second,woman,False,,Southampton,no,False
-0,3,male,28.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,2,male,43.0,1,1,26.25,S,Second,man,True,,Southampton,no,False
-1,3,female,26.0,0,0,7.8542,S,Third,woman,False,,Southampton,yes,True
-1,2,female,24.0,1,0,26.0,S,Second,woman,False,,Southampton,yes,False
-0,2,male,54.0,0,0,14.0,S,Second,man,True,,Southampton,no,True
-1,1,female,31.0,0,2,164.8667,S,First,woman,False,C,Southampton,yes,False
-1,1,female,40.0,1,1,134.5,C,First,woman,False,E,Cherbourg,yes,False
-0,3,male,22.0,0,0,7.25,S,Third,man,True,,Southampton,no,True
-0,3,male,27.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-1,2,female,30.0,0,0,12.35,Q,Second,woman,False,,Queenstown,yes,True
-1,2,female,22.0,1,1,29.0,S,Second,woman,False,,Southampton,yes,False
-0,3,male,,8,2,69.55,S,Third,man,True,,Southampton,no,False
-1,1,female,36.0,0,0,135.6333,C,First,woman,False,C,Cherbourg,yes,True
-0,3,male,61.0,0,0,6.2375,S,Third,man,True,,Southampton,no,True
-1,2,female,36.0,0,0,13.0,S,Second,woman,False,D,Southampton,yes,True
-1,3,female,31.0,1,1,20.525,S,Third,woman,False,,Southampton,yes,False
-1,1,female,16.0,0,1,57.9792,C,First,woman,False,B,Cherbourg,yes,False
-1,3,female,,2,0,23.25,Q,Third,woman,False,,Queenstown,yes,False
-0,1,male,45.5,0,0,28.5,S,First,man,True,C,Southampton,no,True
-0,1,male,38.0,0,1,153.4625,S,First,man,True,C,Southampton,no,False
-0,3,male,16.0,2,0,18.0,S,Third,man,True,,Southampton,no,False
-1,1,female,,1,0,133.65,S,First,woman,False,,Southampton,yes,False
-0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,1,male,29.0,1,0,66.6,S,First,man,True,C,Southampton,no,False
-1,1,female,41.0,0,0,134.5,C,First,woman,False,E,Cherbourg,yes,True
-1,3,male,45.0,0,0,8.05,S,Third,man,True,,Southampton,yes,True
-0,1,male,45.0,0,0,35.5,S,First,man,True,,Southampton,no,True
-1,2,male,2.0,1,1,26.0,S,Second,child,False,F,Southampton,yes,False
-1,1,female,24.0,3,2,263.0,S,First,woman,False,C,Southampton,yes,False
-0,2,male,28.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,2,male,25.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,2,male,36.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-1,2,female,24.0,0,0,13.0,S,Second,woman,False,F,Southampton,yes,True
-1,2,female,40.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
-1,3,female,,1,0,16.1,S,Third,woman,False,,Southampton,yes,False
-1,3,male,3.0,1,1,15.9,S,Third,child,False,,Southampton,yes,False
-0,3,male,42.0,0,0,8.6625,S,Third,man,True,,Southampton,no,True
-0,3,male,23.0,0,0,9.225,S,Third,man,True,,Southampton,no,True
-0,1,male,,0,0,35.0,S,First,man,True,C,Southampton,no,True
-0,3,male,15.0,1,1,7.2292,C,Third,child,False,,Cherbourg,no,False
-0,3,male,25.0,1,0,17.8,S,Third,man,True,,Southampton,no,False
-0,3,male,,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
-0,3,male,28.0,0,0,9.5,S,Third,man,True,,Southampton,no,True
-1,1,female,22.0,0,1,55.0,S,First,woman,False,E,Southampton,yes,False
-0,2,female,38.0,0,0,13.0,S,Second,woman,False,,Southampton,no,True
-1,3,female,,0,0,7.8792,Q,Third,woman,False,,Queenstown,yes,True
-1,3,female,,0,0,7.8792,Q,Third,woman,False,,Queenstown,yes,True
-0,3,male,40.0,1,4,27.9,S,Third,man,True,,Southampton,no,False
-0,2,male,29.0,1,0,27.7208,C,Second,man,True,,Cherbourg,no,False
-0,3,female,45.0,0,1,14.4542,C,Third,woman,False,,Cherbourg,no,False
-0,3,male,35.0,0,0,7.05,S,Third,man,True,,Southampton,no,True
-0,3,male,,1,0,15.5,Q,Third,man,True,,Queenstown,no,False
-0,3,male,30.0,0,0,7.25,S,Third,man,True,,Southampton,no,True
-1,1,female,60.0,1,0,75.25,C,First,woman,False,D,Cherbourg,yes,False
-1,3,female,,0,0,7.2292,C,Third,woman,False,,Cherbourg,yes,True
-1,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
-1,1,female,24.0,0,0,69.3,C,First,woman,False,B,Cherbourg,yes,True
-1,1,male,25.0,1,0,55.4417,C,First,man,True,E,Cherbourg,yes,False
-0,3,male,18.0,1,0,6.4958,S,Third,man,True,,Southampton,no,False
-0,3,male,19.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,1,male,22.0,0,0,135.6333,C,First,man,True,,Cherbourg,no,True
-0,3,female,3.0,3,1,21.075,S,Third,child,False,,Southampton,no,False
-1,1,female,,1,0,82.1708,C,First,woman,False,,Cherbourg,yes,False
-1,3,female,22.0,0,0,7.25,S,Third,woman,False,,Southampton,yes,True
-0,1,male,27.0,0,2,211.5,C,First,man,True,C,Cherbourg,no,False
-0,3,male,20.0,0,0,4.0125,C,Third,man,True,,Cherbourg,no,True
-0,3,male,19.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
-1,1,female,42.0,0,0,227.525,C,First,woman,False,,Cherbourg,yes,True
-1,3,female,1.0,0,2,15.7417,C,Third,child,False,,Cherbourg,yes,False
-0,3,male,32.0,0,0,7.925,S,Third,man,True,,Southampton,no,True
-1,1,female,35.0,1,0,52.0,S,First,woman,False,,Southampton,yes,False
-0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,2,male,18.0,0,0,73.5,S,Second,man,True,,Southampton,no,True
-0,3,male,1.0,5,2,46.9,S,Third,child,False,,Southampton,no,False
-1,2,female,36.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
-0,3,male,,0,0,7.7292,Q,Third,man,True,,Queenstown,no,True
-1,2,female,17.0,0,0,12.0,C,Second,woman,False,,Cherbourg,yes,True
-1,1,male,36.0,1,2,120.0,S,First,man,True,B,Southampton,yes,False
-1,3,male,21.0,0,0,7.7958,S,Third,man,True,,Southampton,yes,True
-0,3,male,28.0,2,0,7.925,S,Third,man,True,,Southampton,no,False
-1,1,female,23.0,1,0,113.275,C,First,woman,False,D,Cherbourg,yes,False
-1,3,female,24.0,0,2,16.7,S,Third,woman,False,G,Southampton,yes,False
-0,3,male,22.0,0,0,7.7958,S,Third,man,True,,Southampton,no,True
-0,3,female,31.0,0,0,7.8542,S,Third,woman,False,,Southampton,no,True
-0,2,male,46.0,0,0,26.0,S,Second,man,True,,Southampton,no,True
-0,2,male,23.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
-1,2,female,28.0,0,0,12.65,S,Second,woman,False,,Southampton,yes,True
-1,3,male,39.0,0,0,7.925,S,Third,man,True,,Southampton,yes,True
-0,3,male,26.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,female,21.0,1,0,9.825,S,Third,woman,False,,Southampton,no,False
-0,3,male,28.0,1,0,15.85,S,Third,man,True,,Southampton,no,False
-0,3,female,20.0,0,0,8.6625,S,Third,woman,False,,Southampton,no,True
-0,2,male,34.0,1,0,21.0,S,Second,man,True,,Southampton,no,False
-0,3,male,51.0,0,0,7.75,S,Third,man,True,,Southampton,no,True
-1,2,male,3.0,1,1,18.75,S,Second,child,False,,Southampton,yes,False
-0,3,male,21.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
-0,3,female,,3,1,25.4667,S,Third,woman,False,,Southampton,no,False
-0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,6.8583,Q,Third,man,True,,Queenstown,no,True
-1,1,female,33.0,1,0,90.0,Q,First,woman,False,C,Queenstown,yes,False
-0,2,male,,0,0,0.0,S,Second,man,True,,Southampton,no,True
-1,3,male,44.0,0,0,7.925,S,Third,man,True,,Southampton,yes,True
-0,3,female,,0,0,8.05,S,Third,woman,False,,Southampton,no,True
-1,2,female,34.0,1,1,32.5,S,Second,woman,False,,Southampton,yes,False
-1,2,female,18.0,0,2,13.0,S,Second,woman,False,,Southampton,yes,False
-0,2,male,30.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,3,female,10.0,0,2,24.15,S,Third,child,False,,Southampton,no,False
-0,3,male,,0,0,7.8958,C,Third,man,True,,Cherbourg,no,True
-0,3,male,21.0,0,0,7.7333,Q,Third,man,True,,Queenstown,no,True
-0,3,male,29.0,0,0,7.875,S,Third,man,True,,Southampton,no,True
-0,3,female,28.0,1,1,14.4,S,Third,woman,False,,Southampton,no,False
-0,3,male,18.0,1,1,20.2125,S,Third,man,True,,Southampton,no,False
-0,3,male,,0,0,7.25,S,Third,man,True,,Southampton,no,True
-1,2,female,28.0,1,0,26.0,S,Second,woman,False,,Southampton,yes,False
-1,2,female,19.0,0,0,26.0,S,Second,woman,False,,Southampton,yes,True
-0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
-1,3,male,32.0,0,0,8.05,S,Third,man,True,E,Southampton,yes,True
-1,1,male,28.0,0,0,26.55,S,First,man,True,C,Southampton,yes,True
-1,3,female,,1,0,16.1,S,Third,woman,False,,Southampton,yes,False
-1,2,female,42.0,1,0,26.0,S,Second,woman,False,,Southampton,yes,False
-0,3,male,17.0,0,0,7.125,S,Third,man,True,,Southampton,no,True
-0,1,male,50.0,1,0,55.9,S,First,man,True,E,Southampton,no,False
-1,1,female,14.0,1,2,120.0,S,First,child,False,B,Southampton,yes,False
-0,3,female,21.0,2,2,34.375,S,Third,woman,False,,Southampton,no,False
-1,2,female,24.0,2,3,18.75,S,Second,woman,False,,Southampton,yes,False
-0,1,male,64.0,1,4,263.0,S,First,man,True,C,Southampton,no,False
-0,2,male,31.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
-1,2,female,45.0,1,1,26.25,S,Second,woman,False,,Southampton,yes,False
-0,3,male,20.0,0,0,9.5,S,Third,man,True,,Southampton,no,True
-0,3,male,25.0,1,0,7.775,S,Third,man,True,,Southampton,no,False
-1,2,female,28.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
-1,3,male,,0,0,8.1125,S,Third,man,True,,Southampton,yes,True
-1,1,male,4.0,0,2,81.8583,S,First,child,False,A,Southampton,yes,False
-1,2,female,13.0,0,1,19.5,S,Second,child,False,,Southampton,yes,False
-1,1,male,34.0,0,0,26.55,S,First,man,True,,Southampton,yes,True
-1,3,female,5.0,2,1,19.2583,C,Third,child,False,,Cherbourg,yes,False
-1,1,male,52.0,0,0,30.5,S,First,man,True,C,Southampton,yes,True
-0,2,male,36.0,1,2,27.75,S,Second,man,True,,Southampton,no,False
-0,3,male,,1,0,19.9667,S,Third,man,True,,Southampton,no,False
-0,1,male,30.0,0,0,27.75,C,First,man,True,C,Cherbourg,no,True
-1,1,male,49.0,1,0,89.1042,C,First,man,True,C,Cherbourg,yes,False
-0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
-1,3,male,29.0,0,0,7.8958,C,Third,man,True,,Cherbourg,yes,True
-0,1,male,65.0,0,0,26.55,S,First,man,True,E,Southampton,no,True
-1,1,female,,1,0,51.8625,S,First,woman,False,D,Southampton,yes,False
-1,2,female,50.0,0,0,10.5,S,Second,woman,False,,Southampton,yes,True
-0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
-1,1,male,48.0,0,0,26.55,S,First,man,True,E,Southampton,yes,True
-0,3,male,34.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,1,male,47.0,0,0,38.5,S,First,man,True,E,Southampton,no,True
-0,2,male,48.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,male,38.0,0,0,7.05,S,Third,man,True,,Southampton,no,True
-0,2,male,,0,0,0.0,S,Second,man,True,,Southampton,no,True
-0,1,male,56.0,0,0,26.55,S,First,man,True,,Southampton,no,True
-0,3,male,,0,0,7.725,Q,Third,man,True,,Queenstown,no,True
-1,3,female,0.75,2,1,19.2583,C,Third,child,False,,Cherbourg,yes,False
-0,3,male,,0,0,7.25,S,Third,man,True,,Southampton,no,True
-0,3,male,38.0,0,0,8.6625,S,Third,man,True,,Southampton,no,True
-1,2,female,33.0,1,2,27.75,S,Second,woman,False,,Southampton,yes,False
-1,2,female,23.0,0,0,13.7917,C,Second,woman,False,D,Cherbourg,yes,True
-0,3,female,22.0,0,0,9.8375,S,Third,woman,False,,Southampton,no,True
-0,1,male,,0,0,52.0,S,First,man,True,A,Southampton,no,True
-0,2,male,34.0,1,0,21.0,S,Second,man,True,,Southampton,no,False
-0,3,male,29.0,1,0,7.0458,S,Third,man,True,,Southampton,no,False
-0,3,male,22.0,0,0,7.5208,S,Third,man,True,,Southampton,no,True
-1,3,female,2.0,0,1,12.2875,S,Third,child,False,,Southampton,yes,False
-0,3,male,9.0,5,2,46.9,S,Third,child,False,,Southampton,no,False
-0,2,male,,0,0,0.0,S,Second,man,True,,Southampton,no,True
-0,3,male,50.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-1,3,female,63.0,0,0,9.5875,S,Third,woman,False,,Southampton,yes,True
-1,1,male,25.0,1,0,91.0792,C,First,man,True,B,Cherbourg,yes,False
-0,3,female,,3,1,25.4667,S,Third,woman,False,,Southampton,no,False
-1,1,female,35.0,1,0,90.0,S,First,woman,False,C,Southampton,yes,False
-0,1,male,58.0,0,0,29.7,C,First,man,True,B,Cherbourg,no,True
-0,3,male,30.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-1,3,male,9.0,1,1,15.9,S,Third,child,False,,Southampton,yes,False
-0,3,male,,1,0,19.9667,S,Third,man,True,,Southampton,no,False
-0,3,male,21.0,0,0,7.25,S,Third,man,True,,Southampton,no,True
-0,1,male,55.0,0,0,30.5,S,First,man,True,C,Southampton,no,True
-0,1,male,71.0,0,0,49.5042,C,First,man,True,,Cherbourg,no,True
-0,3,male,21.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,14.4583,C,Third,man,True,,Cherbourg,no,True
-1,1,female,54.0,1,0,78.2667,C,First,woman,False,D,Cherbourg,yes,False
-0,3,male,,0,0,15.1,S,Third,man,True,,Southampton,no,True
-0,1,female,25.0,1,2,151.55,S,First,woman,False,C,Southampton,no,False
-0,3,male,24.0,0,0,7.7958,S,Third,man,True,,Southampton,no,True
-0,3,male,17.0,0,0,8.6625,S,Third,man,True,,Southampton,no,True
-0,3,female,21.0,0,0,7.75,Q,Third,woman,False,,Queenstown,no,True
-0,3,female,,0,0,7.6292,Q,Third,woman,False,,Queenstown,no,True
-0,3,female,37.0,0,0,9.5875,S,Third,woman,False,,Southampton,no,True
-1,1,female,16.0,0,0,86.5,S,First,woman,False,B,Southampton,yes,True
-0,1,male,18.0,1,0,108.9,C,First,man,True,C,Cherbourg,no,False
-1,2,female,33.0,0,2,26.0,S,Second,woman,False,,Southampton,yes,False
-1,1,male,,0,0,26.55,S,First,man,True,,Southampton,yes,True
-0,3,male,28.0,0,0,22.525,S,Third,man,True,,Southampton,no,True
-1,3,male,26.0,0,0,56.4958,S,Third,man,True,,Southampton,yes,True
-1,3,male,29.0,0,0,7.75,Q,Third,man,True,,Queenstown,yes,True
-0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
-1,1,male,36.0,0,0,26.2875,S,First,man,True,E,Southampton,yes,True
-1,1,female,54.0,1,0,59.4,C,First,woman,False,,Cherbourg,yes,False
-0,3,male,24.0,0,0,7.4958,S,Third,man,True,,Southampton,no,True
-0,1,male,47.0,0,0,34.0208,S,First,man,True,D,Southampton,no,True
-1,2,female,34.0,0,0,10.5,S,Second,woman,False,F,Southampton,yes,True
-0,3,male,,0,0,24.15,Q,Third,man,True,,Queenstown,no,True
-1,2,female,36.0,1,0,26.0,S,Second,woman,False,,Southampton,yes,False
-0,3,male,32.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-1,1,female,30.0,0,0,93.5,S,First,woman,False,B,Southampton,yes,True
-0,3,male,22.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
-1,1,female,44.0,0,1,57.9792,C,First,woman,False,B,Cherbourg,yes,False
-0,3,male,,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
-0,3,male,40.5,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
-1,2,female,50.0,0,0,10.5,S,Second,woman,False,,Southampton,yes,True
-0,1,male,,0,0,221.7792,S,First,man,True,C,Southampton,no,True
-0,3,male,39.0,0,0,7.925,S,Third,man,True,,Southampton,no,True
-0,2,male,23.0,2,1,11.5,S,Second,man,True,,Southampton,no,False
-1,2,female,2.0,1,1,26.0,S,Second,child,False,,Southampton,yes,False
-0,3,male,,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
-0,3,male,17.0,1,1,7.2292,C,Third,man,True,,Cherbourg,no,False
-1,3,female,,0,2,22.3583,C,Third,woman,False,,Cherbourg,yes,False
-0,3,female,30.0,0,0,8.6625,S,Third,woman,False,,Southampton,no,True
-1,2,female,7.0,0,2,26.25,S,Second,child,False,,Southampton,yes,False
-0,1,male,45.0,0,0,26.55,S,First,man,True,B,Southampton,no,True
-1,1,female,30.0,0,0,106.425,C,First,woman,False,,Cherbourg,yes,True
-0,3,male,,0,0,14.5,S,Third,man,True,,Southampton,no,True
-1,1,female,22.0,0,2,49.5,C,First,woman,False,B,Cherbourg,yes,False
-1,1,female,36.0,0,2,71.0,S,First,woman,False,B,Southampton,yes,False
-0,3,female,9.0,4,2,31.275,S,Third,child,False,,Southampton,no,False
-0,3,female,11.0,4,2,31.275,S,Third,child,False,,Southampton,no,False
-1,2,male,32.0,1,0,26.0,S,Second,man,True,,Southampton,yes,False
-0,1,male,50.0,1,0,106.425,C,First,man,True,C,Cherbourg,no,False
-0,1,male,64.0,0,0,26.0,S,First,man,True,,Southampton,no,True
-1,2,female,19.0,1,0,26.0,S,Second,woman,False,,Southampton,yes,False
-1,2,male,,0,0,13.8625,C,Second,man,True,,Cherbourg,yes,True
-0,3,male,33.0,1,1,20.525,S,Third,man,True,,Southampton,no,False
-1,2,male,8.0,1,1,36.75,S,Second,child,False,,Southampton,yes,False
-1,1,male,17.0,0,2,110.8833,C,First,man,True,C,Cherbourg,yes,False
-0,2,male,27.0,0,0,26.0,S,Second,man,True,,Southampton,no,True
-0,3,male,,0,0,7.8292,Q,Third,man,True,,Queenstown,no,True
-1,3,male,22.0,0,0,7.225,C,Third,man,True,,Cherbourg,yes,True
-1,3,female,22.0,0,0,7.775,S,Third,woman,False,,Southampton,yes,True
-0,1,male,62.0,0,0,26.55,S,First,man,True,,Southampton,no,True
-1,1,female,48.0,1,0,39.6,C,First,woman,False,A,Cherbourg,yes,False
-0,1,male,,0,0,227.525,C,First,man,True,,Cherbourg,no,True
-1,1,female,39.0,1,1,79.65,S,First,woman,False,E,Southampton,yes,False
-1,3,female,36.0,1,0,17.4,S,Third,woman,False,,Southampton,yes,False
-0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
-0,3,male,40.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,2,male,28.0,0,0,13.5,S,Second,man,True,,Southampton,no,True
-0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,female,,0,0,8.05,S,Third,woman,False,,Southampton,no,True
-0,3,male,24.0,2,0,24.15,S,Third,man,True,,Southampton,no,False
-0,3,male,19.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,3,female,29.0,0,4,21.075,S,Third,woman,False,,Southampton,no,False
-0,3,male,,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
-1,3,male,32.0,0,0,7.8542,S,Third,man,True,,Southampton,yes,True
-1,2,male,62.0,0,0,10.5,S,Second,man,True,,Southampton,yes,True
-1,1,female,53.0,2,0,51.4792,S,First,woman,False,C,Southampton,yes,False
-1,1,male,36.0,0,0,26.3875,S,First,man,True,E,Southampton,yes,True
-1,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
-0,3,male,16.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,male,19.0,0,0,14.5,S,Third,man,True,,Southampton,no,True
-1,2,female,34.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
-1,1,female,39.0,1,0,55.9,S,First,woman,False,E,Southampton,yes,False
-0,3,female,,1,0,14.4583,C,Third,woman,False,,Cherbourg,no,False
-1,3,male,32.0,0,0,7.925,S,Third,man,True,,Southampton,yes,True
-1,2,female,25.0,1,1,30.0,S,Second,woman,False,,Southampton,yes,False
-1,1,female,39.0,1,1,110.8833,C,First,woman,False,C,Cherbourg,yes,False
-0,2,male,54.0,0,0,26.0,S,Second,man,True,,Southampton,no,True
-0,1,male,36.0,0,0,40.125,C,First,man,True,A,Cherbourg,no,True
-0,3,male,,0,0,8.7125,C,Third,man,True,,Cherbourg,no,True
-1,1,female,18.0,0,2,79.65,S,First,woman,False,E,Southampton,yes,False
-0,2,male,47.0,0,0,15.0,S,Second,man,True,,Southampton,no,True
-1,1,male,60.0,1,1,79.2,C,First,man,True,B,Cherbourg,yes,False
-0,3,male,22.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,3,male,35.0,0,0,7.125,S,Third,man,True,,Southampton,no,True
-1,1,female,52.0,1,0,78.2667,C,First,woman,False,D,Cherbourg,yes,False
-0,3,male,47.0,0,0,7.25,S,Third,man,True,,Southampton,no,True
-0,3,female,,0,2,7.75,Q,Third,woman,False,,Queenstown,no,False
-0,2,male,37.0,1,0,26.0,S,Second,man,True,,Southampton,no,False
-0,3,male,36.0,1,1,24.15,S,Third,man,True,,Southampton,no,False
-1,2,female,,0,0,33.0,S,Second,woman,False,,Southampton,yes,True
-0,3,male,49.0,0,0,0.0,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
-1,1,male,49.0,1,0,56.9292,C,First,man,True,A,Cherbourg,yes,False
-1,2,female,24.0,2,1,27.0,S,Second,woman,False,,Southampton,yes,False
-0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,1,male,,0,0,42.4,S,First,man,True,,Southampton,no,True
-0,3,male,44.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-1,1,male,35.0,0,0,26.55,C,First,man,True,,Cherbourg,yes,True
-0,3,male,36.0,1,0,15.55,S,Third,man,True,,Southampton,no,False
-0,3,male,30.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-1,1,male,27.0,0,0,30.5,S,First,man,True,,Southampton,yes,True
-1,2,female,22.0,1,2,41.5792,C,Second,woman,False,,Cherbourg,yes,False
-1,1,female,40.0,0,0,153.4625,S,First,woman,False,C,Southampton,yes,True
-0,3,female,39.0,1,5,31.275,S,Third,woman,False,,Southampton,no,False
-0,3,male,,0,0,7.05,S,Third,man,True,,Southampton,no,True
-1,3,female,,1,0,15.5,Q,Third,woman,False,,Queenstown,yes,False
-0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
-0,3,male,35.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-1,2,female,24.0,1,2,65.0,S,Second,woman,False,,Southampton,yes,False
-0,3,male,34.0,1,1,14.4,S,Third,man,True,,Southampton,no,False
-0,3,female,26.0,1,0,16.1,S,Third,woman,False,,Southampton,no,False
-1,2,female,4.0,2,1,39.0,S,Second,child,False,F,Southampton,yes,False
-0,2,male,26.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
-0,3,male,27.0,1,0,14.4542,C,Third,man,True,,Cherbourg,no,False
-1,1,male,42.0,1,0,52.5542,S,First,man,True,D,Southampton,yes,False
-1,3,male,20.0,1,1,15.7417,C,Third,man,True,,Cherbourg,yes,False
-0,3,male,21.0,0,0,7.8542,S,Third,man,True,,Southampton,no,True
-0,3,male,21.0,0,0,16.1,S,Third,man,True,,Southampton,no,True
-0,1,male,61.0,0,0,32.3208,S,First,man,True,D,Southampton,no,True
-0,2,male,57.0,0,0,12.35,Q,Second,man,True,,Queenstown,no,True
-1,1,female,21.0,0,0,77.9583,S,First,woman,False,D,Southampton,yes,True
-0,3,male,26.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,7.7333,Q,Third,man,True,,Queenstown,no,True
-1,1,male,80.0,0,0,30.0,S,First,man,True,A,Southampton,yes,True
-0,3,male,51.0,0,0,7.0542,S,Third,man,True,,Southampton,no,True
-1,1,male,32.0,0,0,30.5,C,First,man,True,B,Cherbourg,yes,True
-0,1,male,,0,0,0.0,S,First,man,True,,Southampton,no,True
-0,3,female,9.0,3,2,27.9,S,Third,child,False,,Southampton,no,False
-1,2,female,28.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
-0,3,male,32.0,0,0,7.925,S,Third,man,True,,Southampton,no,True
-0,2,male,31.0,1,1,26.25,S,Second,man,True,,Southampton,no,False
-0,3,female,41.0,0,5,39.6875,S,Third,woman,False,,Southampton,no,False
-0,3,male,,1,0,16.1,S,Third,man,True,,Southampton,no,False
-0,3,male,20.0,0,0,7.8542,S,Third,man,True,,Southampton,no,True
-1,1,female,24.0,0,0,69.3,C,First,woman,False,B,Cherbourg,yes,True
-0,3,female,2.0,3,2,27.9,S,Third,child,False,,Southampton,no,False
-1,3,male,,0,0,56.4958,S,Third,man,True,,Southampton,yes,True
-1,3,female,0.75,2,1,19.2583,C,Third,child,False,,Cherbourg,yes,False
-1,1,male,48.0,1,0,76.7292,C,First,man,True,D,Cherbourg,yes,False
-0,3,male,19.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-1,1,male,56.0,0,0,35.5,C,First,man,True,A,Cherbourg,yes,True
-0,3,male,,0,0,7.55,S,Third,man,True,,Southampton,no,True
-1,3,female,23.0,0,0,7.55,S,Third,woman,False,,Southampton,yes,True
-0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-1,2,female,18.0,0,1,23.0,S,Second,woman,False,,Southampton,yes,False
-0,3,male,21.0,0,0,8.4333,S,Third,man,True,,Southampton,no,True
-1,3,female,,0,0,7.8292,Q,Third,woman,False,,Queenstown,yes,True
-0,3,female,18.0,0,0,6.75,Q,Third,woman,False,,Queenstown,no,True
-0,2,male,24.0,2,0,73.5,S,Second,man,True,,Southampton,no,False
-0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,3,female,32.0,1,1,15.5,Q,Third,woman,False,,Queenstown,no,False
-0,2,male,23.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,1,male,58.0,0,2,113.275,C,First,man,True,D,Cherbourg,no,False
-1,1,male,50.0,2,0,133.65,S,First,man,True,,Southampton,yes,False
-0,3,male,40.0,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
-0,1,male,47.0,0,0,25.5875,S,First,man,True,E,Southampton,no,True
-0,3,male,36.0,0,0,7.4958,S,Third,man,True,,Southampton,no,True
-1,3,male,20.0,1,0,7.925,S,Third,man,True,,Southampton,yes,False
-0,2,male,32.0,2,0,73.5,S,Second,man,True,,Southampton,no,False
-0,2,male,25.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,3,male,,0,0,7.775,S,Third,man,True,,Southampton,no,True
-0,3,male,43.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-1,1,female,,1,0,52.0,S,First,woman,False,C,Southampton,yes,False
-1,2,female,40.0,1,1,39.0,S,Second,woman,False,,Southampton,yes,False
-0,1,male,31.0,1,0,52.0,S,First,man,True,B,Southampton,no,False
-0,2,male,70.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
-1,2,male,31.0,0,0,13.0,S,Second,man,True,,Southampton,yes,True
-0,2,male,,0,0,0.0,S,Second,man,True,,Southampton,no,True
-0,3,male,18.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
-0,3,male,24.5,0,0,8.05,S,Third,man,True,,Southampton,no,True
-1,3,female,18.0,0,0,9.8417,S,Third,woman,False,,Southampton,yes,True
-0,3,female,43.0,1,6,46.9,S,Third,woman,False,,Southampton,no,False
-1,1,male,36.0,0,1,512.3292,C,First,man,True,B,Cherbourg,yes,False
-0,3,female,,0,0,8.1375,Q,Third,woman,False,,Queenstown,no,True
-1,1,male,27.0,0,0,76.7292,C,First,man,True,D,Cherbourg,yes,True
-0,3,male,20.0,0,0,9.225,S,Third,man,True,,Southampton,no,True
-0,3,male,14.0,5,2,46.9,S,Third,child,False,,Southampton,no,False
-0,2,male,60.0,1,1,39.0,S,Second,man,True,,Southampton,no,False
-0,2,male,25.0,1,2,41.5792,C,Second,man,True,,Cherbourg,no,False
-0,3,male,14.0,4,1,39.6875,S,Third,child,False,,Southampton,no,False
-0,3,male,19.0,0,0,10.1708,S,Third,man,True,,Southampton,no,True
-0,3,male,18.0,0,0,7.7958,S,Third,man,True,,Southampton,no,True
-1,1,female,15.0,0,1,211.3375,S,First,child,False,B,Southampton,yes,False
-1,1,male,31.0,1,0,57.0,S,First,man,True,B,Southampton,yes,False
-1,3,female,4.0,0,1,13.4167,C,Third,child,False,,Cherbourg,yes,False
-1,3,male,,0,0,56.4958,S,Third,man,True,,Southampton,yes,True
-0,3,male,25.0,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
-0,1,male,60.0,0,0,26.55,S,First,man,True,,Southampton,no,True
-0,2,male,52.0,0,0,13.5,S,Second,man,True,,Southampton,no,True
-0,3,male,44.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-1,3,female,,0,0,7.7333,Q,Third,woman,False,,Queenstown,yes,True
-0,1,male,49.0,1,1,110.8833,C,First,man,True,C,Cherbourg,no,False
-0,3,male,42.0,0,0,7.65,S,Third,man,True,F,Southampton,no,True
-1,1,female,18.0,1,0,227.525,C,First,woman,False,C,Cherbourg,yes,False
-1,1,male,35.0,0,0,26.2875,S,First,man,True,E,Southampton,yes,True
-0,3,female,18.0,0,1,14.4542,C,Third,woman,False,,Cherbourg,no,False
-0,3,male,25.0,0,0,7.7417,Q,Third,man,True,,Queenstown,no,True
-0,3,male,26.0,1,0,7.8542,S,Third,man,True,,Southampton,no,False
-0,2,male,39.0,0,0,26.0,S,Second,man,True,,Southampton,no,True
-1,2,female,45.0,0,0,13.5,S,Second,woman,False,,Southampton,yes,True
-1,1,male,42.0,0,0,26.2875,S,First,man,True,E,Southampton,yes,True
-1,1,female,22.0,0,0,151.55,S,First,woman,False,,Southampton,yes,True
-1,3,male,,1,1,15.2458,C,Third,man,True,,Cherbourg,yes,False
-1,1,female,24.0,0,0,49.5042,C,First,woman,False,C,Cherbourg,yes,True
-0,1,male,,0,0,26.55,S,First,man,True,C,Southampton,no,True
-1,1,male,48.0,1,0,52.0,S,First,man,True,C,Southampton,yes,False
-0,3,male,29.0,0,0,9.4833,S,Third,man,True,,Southampton,no,True
-0,2,male,52.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,3,male,19.0,0,0,7.65,S,Third,man,True,F,Southampton,no,True
-1,1,female,38.0,0,0,227.525,C,First,woman,False,C,Cherbourg,yes,True
-1,2,female,27.0,0,0,10.5,S,Second,woman,False,E,Southampton,yes,True
-0,3,male,,0,0,15.5,Q,Third,man,True,,Queenstown,no,True
-0,3,male,33.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
-1,2,female,6.0,0,1,33.0,S,Second,child,False,,Southampton,yes,False
-0,3,male,17.0,1,0,7.0542,S,Third,man,True,,Southampton,no,False
-0,2,male,34.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,2,male,50.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-1,1,male,27.0,1,0,53.1,S,First,man,True,E,Southampton,yes,False
-0,3,male,20.0,0,0,8.6625,S,Third,man,True,,Southampton,no,True
-1,2,female,30.0,3,0,21.0,S,Second,woman,False,,Southampton,yes,False
-1,3,female,,0,0,7.7375,Q,Third,woman,False,,Queenstown,yes,True
-0,2,male,25.0,1,0,26.0,S,Second,man,True,,Southampton,no,False
-0,3,female,25.0,1,0,7.925,S,Third,woman,False,,Southampton,no,False
-1,1,female,29.0,0,0,211.3375,S,First,woman,False,B,Southampton,yes,True
-0,3,male,11.0,0,0,18.7875,C,Third,child,False,,Cherbourg,no,True
-0,2,male,,0,0,0.0,S,Second,man,True,,Southampton,no,True
-0,2,male,23.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,2,male,23.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-0,3,male,28.5,0,0,16.1,S,Third,man,True,,Southampton,no,True
-0,3,female,48.0,1,3,34.375,S,Third,woman,False,,Southampton,no,False
-1,1,male,35.0,0,0,512.3292,C,First,man,True,B,Cherbourg,yes,True
-0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-1,1,male,,0,0,30.0,S,First,man,True,D,Southampton,yes,True
-0,1,male,36.0,1,0,78.85,S,First,man,True,C,Southampton,no,False
-1,1,female,21.0,2,2,262.375,C,First,woman,False,B,Cherbourg,yes,False
-0,3,male,24.0,1,0,16.1,S,Third,man,True,,Southampton,no,False
-1,3,male,31.0,0,0,7.925,S,Third,man,True,,Southampton,yes,True
-0,1,male,70.0,1,1,71.0,S,First,man,True,B,Southampton,no,False
-0,3,male,16.0,1,1,20.25,S,Third,man,True,,Southampton,no,False
-1,2,female,30.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
-0,1,male,19.0,1,0,53.1,S,First,man,True,D,Southampton,no,False
-0,3,male,31.0,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
-1,2,female,4.0,1,1,23.0,S,Second,child,False,,Southampton,yes,False
-1,3,male,6.0,0,1,12.475,S,Third,child,False,E,Southampton,yes,False
-0,3,male,33.0,0,0,9.5,S,Third,man,True,,Southampton,no,True
-0,3,male,23.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-1,2,female,48.0,1,2,65.0,S,Second,woman,False,,Southampton,yes,False
-1,2,male,0.67,1,1,14.5,S,Second,child,False,,Southampton,yes,False
-0,3,male,28.0,0,0,7.7958,S,Third,man,True,,Southampton,no,True
-0,2,male,18.0,0,0,11.5,S,Second,man,True,,Southampton,no,True
-0,3,male,34.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
-1,1,female,33.0,0,0,86.5,S,First,woman,False,B,Southampton,yes,True
-0,3,male,,0,0,14.5,S,Third,man,True,,Southampton,no,True
-0,3,male,41.0,0,0,7.125,S,Third,man,True,,Southampton,no,True
-1,3,male,20.0,0,0,7.2292,C,Third,man,True,,Cherbourg,yes,True
-1,1,female,36.0,1,2,120.0,S,First,woman,False,B,Southampton,yes,False
-0,3,male,16.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
-1,1,female,51.0,1,0,77.9583,S,First,woman,False,D,Southampton,yes,False
-0,1,male,,0,0,39.6,C,First,man,True,,Cherbourg,no,True
-0,3,female,30.5,0,0,7.75,Q,Third,woman,False,,Queenstown,no,True
-0,3,male,,1,0,24.15,Q,Third,man,True,,Queenstown,no,False
-0,3,male,32.0,0,0,8.3625,S,Third,man,True,,Southampton,no,True
-0,3,male,24.0,0,0,9.5,S,Third,man,True,,Southampton,no,True
-0,3,male,48.0,0,0,7.8542,S,Third,man,True,,Southampton,no,True
-0,2,female,57.0,0,0,10.5,S,Second,woman,False,E,Southampton,no,True
-0,3,male,,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
-1,2,female,54.0,1,3,23.0,S,Second,woman,False,,Southampton,yes,False
-0,3,male,18.0,0,0,7.75,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,7.75,Q,Third,man,True,F,Queenstown,no,True
-1,3,female,5.0,0,0,12.475,S,Third,child,False,,Southampton,yes,True
-0,3,male,,0,0,7.7375,Q,Third,man,True,,Queenstown,no,True
-1,1,female,43.0,0,1,211.3375,S,First,woman,False,B,Southampton,yes,False
-1,3,female,13.0,0,0,7.2292,C,Third,child,False,,Cherbourg,yes,True
-1,1,female,17.0,1,0,57.0,S,First,woman,False,B,Southampton,yes,False
-0,1,male,29.0,0,0,30.0,S,First,man,True,D,Southampton,no,True
-0,3,male,,1,2,23.45,S,Third,man,True,,Southampton,no,False
-0,3,male,25.0,0,0,7.05,S,Third,man,True,,Southampton,no,True
-0,3,male,25.0,0,0,7.25,S,Third,man,True,,Southampton,no,True
-1,3,female,18.0,0,0,7.4958,S,Third,woman,False,,Southampton,yes,True
-0,3,male,8.0,4,1,29.125,Q,Third,child,False,,Queenstown,no,False
-1,3,male,1.0,1,2,20.575,S,Third,child,False,,Southampton,yes,False
-0,1,male,46.0,0,0,79.2,C,First,man,True,B,Cherbourg,no,True
-0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
-0,2,male,16.0,0,0,26.0,S,Second,man,True,,Southampton,no,True
-0,3,female,,8,2,69.55,S,Third,woman,False,,Southampton,no,False
-0,1,male,,0,0,30.6958,C,First,man,True,,Cherbourg,no,True
-0,3,male,25.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,2,male,39.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-1,1,female,49.0,0,0,25.9292,S,First,woman,False,D,Southampton,yes,True
-1,3,female,31.0,0,0,8.6833,S,Third,woman,False,,Southampton,yes,True
-0,3,male,30.0,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
-0,3,female,30.0,1,1,24.15,S,Third,woman,False,,Southampton,no,False
-0,2,male,34.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-1,2,female,31.0,1,1,26.25,S,Second,woman,False,,Southampton,yes,False
-1,1,male,11.0,1,2,120.0,S,First,child,False,B,Southampton,yes,False
-1,3,male,0.42,0,1,8.5167,C,Third,child,False,,Cherbourg,yes,False
-1,3,male,27.0,0,0,6.975,S,Third,man,True,,Southampton,yes,True
-0,3,male,31.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
-0,1,male,39.0,0,0,0.0,S,First,man,True,A,Southampton,no,True
-0,3,female,18.0,0,0,7.775,S,Third,woman,False,,Southampton,no,True
-0,2,male,39.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-1,1,female,33.0,1,0,53.1,S,First,woman,False,E,Southampton,yes,False
-0,3,male,26.0,0,0,7.8875,S,Third,man,True,,Southampton,no,True
-0,3,male,39.0,0,0,24.15,S,Third,man,True,,Southampton,no,True
-0,2,male,35.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
-0,3,female,6.0,4,2,31.275,S,Third,child,False,,Southampton,no,False
-0,3,male,30.5,0,0,8.05,S,Third,man,True,,Southampton,no,True
-0,1,male,,0,0,0.0,S,First,man,True,B,Southampton,no,True
-0,3,female,23.0,0,0,7.925,S,Third,woman,False,,Southampton,no,True
-0,2,male,31.0,1,1,37.0042,C,Second,man,True,,Cherbourg,no,False
-0,3,male,43.0,0,0,6.45,S,Third,man,True,,Southampton,no,True
-0,3,male,10.0,3,2,27.9,S,Third,child,False,,Southampton,no,False
-1,1,female,52.0,1,1,93.5,S,First,woman,False,B,Southampton,yes,False
-1,3,male,27.0,0,0,8.6625,S,Third,man,True,,Southampton,yes,True
-0,1,male,38.0,0,0,0.0,S,First,man,True,,Southampton,no,True
-1,3,female,27.0,0,1,12.475,S,Third,woman,False,E,Southampton,yes,False
-0,3,male,2.0,4,1,39.6875,S,Third,child,False,,Southampton,no,False
-0,3,male,,0,0,6.95,Q,Third,man,True,,Queenstown,no,True
-0,3,male,,0,0,56.4958,S,Third,man,True,,Southampton,no,True
-1,2,male,1.0,0,2,37.0042,C,Second,child,False,,Cherbourg,yes,False
-1,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,yes,True
-1,1,female,62.0,0,0,80.0,,First,woman,False,B,,yes,True
-1,3,female,15.0,1,0,14.4542,C,Third,child,False,,Cherbourg,yes,False
-1,2,male,0.83,1,1,18.75,S,Second,child,False,,Southampton,yes,False
-0,3,male,,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
-0,3,male,23.0,0,0,7.8542,S,Third,man,True,,Southampton,no,True
-0,3,male,18.0,0,0,8.3,S,Third,man,True,,Southampton,no,True
-1,1,female,39.0,1,1,83.1583,C,First,woman,False,E,Cherbourg,yes,False
-0,3,male,21.0,0,0,8.6625,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
-1,3,male,32.0,0,0,56.4958,S,Third,man,True,,Southampton,yes,True
-1,1,male,,0,0,29.7,C,First,man,True,C,Cherbourg,yes,True
-0,3,male,20.0,0,0,7.925,S,Third,man,True,,Southampton,no,True
-0,2,male,16.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
-1,1,female,30.0,0,0,31.0,C,First,woman,False,,Cherbourg,yes,True
-0,3,male,34.5,0,0,6.4375,C,Third,man,True,,Cherbourg,no,True
-0,3,male,17.0,0,0,8.6625,S,Third,man,True,,Southampton,no,True
-0,3,male,42.0,0,0,7.55,S,Third,man,True,,Southampton,no,True
-0,3,male,,8,2,69.55,S,Third,man,True,,Southampton,no,False
-0,3,male,35.0,0,0,7.8958,C,Third,man,True,,Cherbourg,no,True
-0,2,male,28.0,0,1,33.0,S,Second,man,True,,Southampton,no,False
-1,1,female,,1,0,89.1042,C,First,woman,False,C,Cherbourg,yes,False
-0,3,male,4.0,4,2,31.275,S,Third,child,False,,Southampton,no,False
-0,3,male,74.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
-0,3,female,9.0,1,1,15.2458,C,Third,child,False,,Cherbourg,no,False
-1,1,female,16.0,0,1,39.4,S,First,woman,False,D,Southampton,yes,False
-0,2,female,44.0,1,0,26.0,S,Second,woman,False,,Southampton,no,False
-1,3,female,18.0,0,1,9.35,S,Third,woman,False,,Southampton,yes,False
-1,1,female,45.0,1,1,164.8667,S,First,woman,False,,Southampton,yes,False
-1,1,male,51.0,0,0,26.55,S,First,man,True,E,Southampton,yes,True
-1,3,female,24.0,0,3,19.2583,C,Third,woman,False,,Cherbourg,yes,False
-0,3,male,,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
-0,3,male,41.0,2,0,14.1083,S,Third,man,True,,Southampton,no,False
-0,2,male,21.0,1,0,11.5,S,Second,man,True,,Southampton,no,False
-1,1,female,48.0,0,0,25.9292,S,First,woman,False,D,Southampton,yes,True
-0,3,female,,8,2,69.55,S,Third,woman,False,,Southampton,no,False
-0,2,male,24.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-1,2,female,42.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
-1,2,female,27.0,1,0,13.8583,C,Second,woman,False,,Cherbourg,yes,False
-0,1,male,31.0,0,0,50.4958,S,First,man,True,A,Southampton,no,True
-0,3,male,,0,0,9.5,S,Third,man,True,,Southampton,no,True
-1,3,male,4.0,1,1,11.1333,S,Third,child,False,,Southampton,yes,False
-0,3,male,26.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-1,1,female,47.0,1,1,52.5542,S,First,woman,False,D,Southampton,yes,False
-0,1,male,33.0,0,0,5.0,S,First,man,True,B,Southampton,no,True
-0,3,male,47.0,0,0,9.0,S,Third,man,True,,Southampton,no,True
-1,2,female,28.0,1,0,24.0,C,Second,woman,False,,Cherbourg,yes,False
-1,3,female,15.0,0,0,7.225,C,Third,child,False,,Cherbourg,yes,True
-0,3,male,20.0,0,0,9.8458,S,Third,man,True,,Southampton,no,True
-0,3,male,19.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-1,1,female,56.0,0,1,83.1583,C,First,woman,False,C,Cherbourg,yes,False
-1,2,female,25.0,0,1,26.0,S,Second,woman,False,,Southampton,yes,False
-0,3,male,33.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
-0,3,female,22.0,0,0,10.5167,S,Third,woman,False,,Southampton,no,True
-0,2,male,28.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
-0,3,male,25.0,0,0,7.05,S,Third,man,True,,Southampton,no,True
-0,3,female,39.0,0,5,29.125,Q,Third,woman,False,,Queenstown,no,False
-0,2,male,27.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
-1,1,female,19.0,0,0,30.0,S,First,woman,False,B,Southampton,yes,True
-0,3,female,,1,2,23.45,S,Third,woman,False,,Southampton,no,False
-1,1,male,26.0,0,0,30.0,C,First,man,True,C,Cherbourg,yes,True
-0,3,male,32.0,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
+survived,pclass,sex,age,sibsp,parch,fare,embarked,class,who,adult_male,deck,embark_town,alive,alone
+0,3,male,22.0,1,0,7.25,S,Third,man,True,,Southampton,no,False
+1,1,female,38.0,1,0,71.2833,C,First,woman,False,C,Cherbourg,yes,False
+1,3,female,26.0,0,0,7.925,S,Third,woman,False,,Southampton,yes,True
+1,1,female,35.0,1,0,53.1,S,First,woman,False,C,Southampton,yes,False
+0,3,male,35.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,8.4583,Q,Third,man,True,,Queenstown,no,True
+0,1,male,54.0,0,0,51.8625,S,First,man,True,E,Southampton,no,True
+0,3,male,2.0,3,1,21.075,S,Third,child,False,,Southampton,no,False
+1,3,female,27.0,0,2,11.1333,S,Third,woman,False,,Southampton,yes,False
+1,2,female,14.0,1,0,30.0708,C,Second,child,False,,Cherbourg,yes,False
+1,3,female,4.0,1,1,16.7,S,Third,child,False,G,Southampton,yes,False
+1,1,female,58.0,0,0,26.55,S,First,woman,False,C,Southampton,yes,True
+0,3,male,20.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,male,39.0,1,5,31.275,S,Third,man,True,,Southampton,no,False
+0,3,female,14.0,0,0,7.8542,S,Third,child,False,,Southampton,no,True
+1,2,female,55.0,0,0,16.0,S,Second,woman,False,,Southampton,yes,True
+0,3,male,2.0,4,1,29.125,Q,Third,child,False,,Queenstown,no,False
+1,2,male,,0,0,13.0,S,Second,man,True,,Southampton,yes,True
+0,3,female,31.0,1,0,18.0,S,Third,woman,False,,Southampton,no,False
+1,3,female,,0,0,7.225,C,Third,woman,False,,Cherbourg,yes,True
+0,2,male,35.0,0,0,26.0,S,Second,man,True,,Southampton,no,True
+1,2,male,34.0,0,0,13.0,S,Second,man,True,D,Southampton,yes,True
+1,3,female,15.0,0,0,8.0292,Q,Third,child,False,,Queenstown,yes,True
+1,1,male,28.0,0,0,35.5,S,First,man,True,A,Southampton,yes,True
+0,3,female,8.0,3,1,21.075,S,Third,child,False,,Southampton,no,False
+1,3,female,38.0,1,5,31.3875,S,Third,woman,False,,Southampton,yes,False
+0,3,male,,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
+0,1,male,19.0,3,2,263.0,S,First,man,True,C,Southampton,no,False
+1,3,female,,0,0,7.8792,Q,Third,woman,False,,Queenstown,yes,True
+0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,1,male,40.0,0,0,27.7208,C,First,man,True,,Cherbourg,no,True
+1,1,female,,1,0,146.5208,C,First,woman,False,B,Cherbourg,yes,False
+1,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
+0,2,male,66.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
+0,1,male,28.0,1,0,82.1708,C,First,man,True,,Cherbourg,no,False
+0,1,male,42.0,1,0,52.0,S,First,man,True,,Southampton,no,False
+1,3,male,,0,0,7.2292,C,Third,man,True,,Cherbourg,yes,True
+0,3,male,21.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,female,18.0,2,0,18.0,S,Third,woman,False,,Southampton,no,False
+1,3,female,14.0,1,0,11.2417,C,Third,child,False,,Cherbourg,yes,False
+0,3,female,40.0,1,0,9.475,S,Third,woman,False,,Southampton,no,False
+0,2,female,27.0,1,0,21.0,S,Second,woman,False,,Southampton,no,False
+0,3,male,,0,0,7.8958,C,Third,man,True,,Cherbourg,no,True
+1,2,female,3.0,1,2,41.5792,C,Second,child,False,,Cherbourg,yes,False
+1,3,female,19.0,0,0,7.8792,Q,Third,woman,False,,Queenstown,yes,True
+0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,male,,1,0,15.5,Q,Third,man,True,,Queenstown,no,False
+1,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
+0,3,male,,2,0,21.6792,C,Third,man,True,,Cherbourg,no,False
+0,3,female,18.0,1,0,17.8,S,Third,woman,False,,Southampton,no,False
+0,3,male,7.0,4,1,39.6875,S,Third,child,False,,Southampton,no,False
+0,3,male,21.0,0,0,7.8,S,Third,man,True,,Southampton,no,True
+1,1,female,49.0,1,0,76.7292,C,First,woman,False,D,Cherbourg,yes,False
+1,2,female,29.0,1,0,26.0,S,Second,woman,False,,Southampton,yes,False
+0,1,male,65.0,0,1,61.9792,C,First,man,True,B,Cherbourg,no,False
+1,1,male,,0,0,35.5,S,First,man,True,C,Southampton,yes,True
+1,2,female,21.0,0,0,10.5,S,Second,woman,False,,Southampton,yes,True
+0,3,male,28.5,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
+1,2,female,5.0,1,2,27.75,S,Second,child,False,,Southampton,yes,False
+0,3,male,11.0,5,2,46.9,S,Third,child,False,,Southampton,no,False
+0,3,male,22.0,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
+1,1,female,38.0,0,0,80.0,,First,woman,False,B,,yes,True
+0,1,male,45.0,1,0,83.475,S,First,man,True,C,Southampton,no,False
+0,3,male,4.0,3,2,27.9,S,Third,child,False,,Southampton,no,False
+0,1,male,,0,0,27.7208,C,First,man,True,,Cherbourg,no,True
+1,3,male,,1,1,15.2458,C,Third,man,True,,Cherbourg,yes,False
+1,2,female,29.0,0,0,10.5,S,Second,woman,False,F,Southampton,yes,True
+0,3,male,19.0,0,0,8.1583,S,Third,man,True,,Southampton,no,True
+1,3,female,17.0,4,2,7.925,S,Third,woman,False,,Southampton,yes,False
+0,3,male,26.0,2,0,8.6625,S,Third,man,True,,Southampton,no,False
+0,2,male,32.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
+0,3,female,16.0,5,2,46.9,S,Third,woman,False,,Southampton,no,False
+0,2,male,21.0,0,0,73.5,S,Second,man,True,,Southampton,no,True
+0,3,male,26.0,1,0,14.4542,C,Third,man,True,,Cherbourg,no,False
+1,3,male,32.0,0,0,56.4958,S,Third,man,True,,Southampton,yes,True
+0,3,male,25.0,0,0,7.65,S,Third,man,True,F,Southampton,no,True
+0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
+1,2,male,0.83,0,2,29.0,S,Second,child,False,,Southampton,yes,False
+1,3,female,30.0,0,0,12.475,S,Third,woman,False,,Southampton,yes,True
+0,3,male,22.0,0,0,9.0,S,Third,man,True,,Southampton,no,True
+1,3,male,29.0,0,0,9.5,S,Third,man,True,,Southampton,yes,True
+1,3,female,,0,0,7.7875,Q,Third,woman,False,,Queenstown,yes,True
+0,1,male,28.0,0,0,47.1,S,First,man,True,,Southampton,no,True
+1,2,female,17.0,0,0,10.5,S,Second,woman,False,,Southampton,yes,True
+1,3,female,33.0,3,0,15.85,S,Third,woman,False,,Southampton,yes,False
+0,3,male,16.0,1,3,34.375,S,Third,man,True,,Southampton,no,False
+0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
+1,1,female,23.0,3,2,263.0,S,First,woman,False,C,Southampton,yes,False
+0,3,male,24.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,male,29.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,male,20.0,0,0,7.8542,S,Third,man,True,,Southampton,no,True
+0,1,male,46.0,1,0,61.175,S,First,man,True,E,Southampton,no,False
+0,3,male,26.0,1,2,20.575,S,Third,man,True,,Southampton,no,False
+0,3,male,59.0,0,0,7.25,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,1,male,71.0,0,0,34.6542,C,First,man,True,A,Cherbourg,no,True
+1,1,male,23.0,0,1,63.3583,C,First,man,True,D,Cherbourg,yes,False
+1,2,female,34.0,0,1,23.0,S,Second,woman,False,,Southampton,yes,False
+0,2,male,34.0,1,0,26.0,S,Second,man,True,,Southampton,no,False
+0,3,female,28.0,0,0,7.8958,S,Third,woman,False,,Southampton,no,True
+0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,1,male,21.0,0,1,77.2875,S,First,man,True,D,Southampton,no,False
+0,3,male,33.0,0,0,8.6542,S,Third,man,True,,Southampton,no,True
+0,3,male,37.0,2,0,7.925,S,Third,man,True,,Southampton,no,False
+0,3,male,28.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+1,3,female,21.0,0,0,7.65,S,Third,woman,False,,Southampton,yes,True
+1,3,male,,0,0,7.775,S,Third,man,True,,Southampton,yes,True
+0,3,male,38.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+1,3,female,,1,0,24.15,Q,Third,woman,False,,Queenstown,yes,False
+0,1,male,47.0,0,0,52.0,S,First,man,True,C,Southampton,no,True
+0,3,female,14.5,1,0,14.4542,C,Third,child,False,,Cherbourg,no,False
+0,3,male,22.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,female,20.0,1,0,9.825,S,Third,woman,False,,Southampton,no,False
+0,3,female,17.0,0,0,14.4583,C,Third,woman,False,,Cherbourg,no,True
+0,3,male,21.0,0,0,7.925,S,Third,man,True,,Southampton,no,True
+0,3,male,70.5,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
+0,2,male,29.0,1,0,21.0,S,Second,man,True,,Southampton,no,False
+0,1,male,24.0,0,1,247.5208,C,First,man,True,B,Cherbourg,no,False
+0,3,female,2.0,4,2,31.275,S,Third,child,False,,Southampton,no,False
+0,2,male,21.0,2,0,73.5,S,Second,man,True,,Southampton,no,False
+0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,2,male,32.5,1,0,30.0708,C,Second,man,True,,Cherbourg,no,False
+1,2,female,32.5,0,0,13.0,S,Second,woman,False,E,Southampton,yes,True
+0,1,male,54.0,0,1,77.2875,S,First,man,True,D,Southampton,no,False
+1,3,male,12.0,1,0,11.2417,C,Third,child,False,,Cherbourg,yes,False
+0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
+1,3,male,24.0,0,0,7.1417,S,Third,man,True,,Southampton,yes,True
+1,3,female,,1,1,22.3583,C,Third,woman,False,F,Cherbourg,yes,False
+0,3,male,45.0,0,0,6.975,S,Third,man,True,,Southampton,no,True
+0,3,male,33.0,0,0,7.8958,C,Third,man,True,,Cherbourg,no,True
+0,3,male,20.0,0,0,7.05,S,Third,man,True,,Southampton,no,True
+0,3,female,47.0,1,0,14.5,S,Third,woman,False,,Southampton,no,False
+1,2,female,29.0,1,0,26.0,S,Second,woman,False,,Southampton,yes,False
+0,2,male,25.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,2,male,23.0,0,0,15.0458,C,Second,man,True,,Cherbourg,no,True
+1,1,female,19.0,0,2,26.2833,S,First,woman,False,D,Southampton,yes,False
+0,1,male,37.0,1,0,53.1,S,First,man,True,C,Southampton,no,False
+0,3,male,16.0,0,0,9.2167,S,Third,man,True,,Southampton,no,True
+0,1,male,24.0,0,0,79.2,C,First,man,True,B,Cherbourg,no,True
+0,3,female,,0,2,15.2458,C,Third,woman,False,,Cherbourg,no,False
+1,3,female,22.0,0,0,7.75,S,Third,woman,False,,Southampton,yes,True
+1,3,female,24.0,1,0,15.85,S,Third,woman,False,,Southampton,yes,False
+0,3,male,19.0,0,0,6.75,Q,Third,man,True,,Queenstown,no,True
+0,2,male,18.0,0,0,11.5,S,Second,man,True,,Southampton,no,True
+0,2,male,19.0,1,1,36.75,S,Second,man,True,,Southampton,no,False
+1,3,male,27.0,0,0,7.7958,S,Third,man,True,,Southampton,yes,True
+0,3,female,9.0,2,2,34.375,S,Third,child,False,,Southampton,no,False
+0,2,male,36.5,0,2,26.0,S,Second,man,True,F,Southampton,no,False
+0,2,male,42.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,2,male,51.0,0,0,12.525,S,Second,man,True,,Southampton,no,True
+1,1,female,22.0,1,0,66.6,S,First,woman,False,C,Southampton,yes,False
+0,3,male,55.5,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,male,40.5,0,2,14.5,S,Third,man,True,,Southampton,no,False
+0,3,male,,0,0,7.3125,S,Third,man,True,,Southampton,no,True
+0,1,male,51.0,0,1,61.3792,C,First,man,True,,Cherbourg,no,False
+1,3,female,16.0,0,0,7.7333,Q,Third,woman,False,,Queenstown,yes,True
+0,3,male,30.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,8.6625,S,Third,man,True,,Southampton,no,True
+0,3,male,,8,2,69.55,S,Third,man,True,,Southampton,no,False
+0,3,male,44.0,0,1,16.1,S,Third,man,True,,Southampton,no,False
+1,2,female,40.0,0,0,15.75,S,Second,woman,False,,Southampton,yes,True
+0,3,male,26.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
+0,3,male,17.0,0,0,8.6625,S,Third,man,True,,Southampton,no,True
+0,3,male,1.0,4,1,39.6875,S,Third,child,False,,Southampton,no,False
+1,3,male,9.0,0,2,20.525,S,Third,child,False,,Southampton,yes,False
+1,1,female,,0,1,55.0,S,First,woman,False,E,Southampton,yes,False
+0,3,female,45.0,1,4,27.9,S,Third,woman,False,,Southampton,no,False
+0,1,male,,0,0,25.925,S,First,man,True,,Southampton,no,True
+0,3,male,28.0,0,0,56.4958,S,Third,man,True,,Southampton,no,True
+0,1,male,61.0,0,0,33.5,S,First,man,True,B,Southampton,no,True
+0,3,male,4.0,4,1,29.125,Q,Third,child,False,,Queenstown,no,False
+1,3,female,1.0,1,1,11.1333,S,Third,child,False,,Southampton,yes,False
+0,3,male,21.0,0,0,7.925,S,Third,man,True,,Southampton,no,True
+0,1,male,56.0,0,0,30.6958,C,First,man,True,A,Cherbourg,no,True
+0,3,male,18.0,1,1,7.8542,S,Third,man,True,,Southampton,no,False
+0,3,male,,3,1,25.4667,S,Third,man,True,,Southampton,no,False
+0,1,female,50.0,0,0,28.7125,C,First,woman,False,C,Cherbourg,no,True
+0,2,male,30.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,3,male,36.0,0,0,0.0,S,Third,man,True,,Southampton,no,True
+0,3,female,,8,2,69.55,S,Third,woman,False,,Southampton,no,False
+0,2,male,,0,0,15.05,C,Second,man,True,,Cherbourg,no,True
+0,3,male,9.0,4,2,31.3875,S,Third,child,False,,Southampton,no,False
+1,2,male,1.0,2,1,39.0,S,Second,child,False,F,Southampton,yes,False
+1,3,female,4.0,0,2,22.025,S,Third,child,False,,Southampton,yes,False
+0,1,male,,0,0,50.0,S,First,man,True,A,Southampton,no,True
+1,3,female,,1,0,15.5,Q,Third,woman,False,,Queenstown,yes,False
+1,1,male,45.0,0,0,26.55,S,First,man,True,,Southampton,yes,True
+0,3,male,40.0,1,1,15.5,Q,Third,man,True,,Queenstown,no,False
+0,3,male,36.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+1,2,female,32.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
+0,2,male,19.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+1,3,female,19.0,1,0,7.8542,S,Third,woman,False,,Southampton,yes,False
+1,2,male,3.0,1,1,26.0,S,Second,child,False,F,Southampton,yes,False
+1,1,female,44.0,0,0,27.7208,C,First,woman,False,B,Cherbourg,yes,True
+1,1,female,58.0,0,0,146.5208,C,First,woman,False,B,Cherbourg,yes,True
+0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
+0,3,male,42.0,0,1,8.4042,S,Third,man,True,,Southampton,no,False
+1,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
+0,2,female,24.0,0,0,13.0,S,Second,woman,False,,Southampton,no,True
+0,3,male,28.0,0,0,9.5,S,Third,man,True,,Southampton,no,True
+0,3,male,,8,2,69.55,S,Third,man,True,,Southampton,no,False
+0,3,male,34.0,0,0,6.4958,S,Third,man,True,,Southampton,no,True
+0,3,male,45.5,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
+1,3,male,18.0,0,0,8.05,S,Third,man,True,,Southampton,yes,True
+0,3,female,2.0,0,1,10.4625,S,Third,child,False,G,Southampton,no,False
+0,3,male,32.0,1,0,15.85,S,Third,man,True,,Southampton,no,False
+1,3,male,26.0,0,0,18.7875,C,Third,man,True,,Cherbourg,yes,True
+1,3,female,16.0,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
+1,1,male,40.0,0,0,31.0,C,First,man,True,A,Cherbourg,yes,True
+0,3,male,24.0,0,0,7.05,S,Third,man,True,,Southampton,no,True
+1,2,female,35.0,0,0,21.0,S,Second,woman,False,,Southampton,yes,True
+0,3,male,22.0,0,0,7.25,S,Third,man,True,,Southampton,no,True
+0,2,male,30.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,3,male,,1,0,7.75,Q,Third,man,True,,Queenstown,no,False
+1,1,female,31.0,1,0,113.275,C,First,woman,False,D,Cherbourg,yes,False
+1,3,female,27.0,0,0,7.925,S,Third,woman,False,,Southampton,yes,True
+0,2,male,42.0,1,0,27.0,S,Second,man,True,,Southampton,no,False
+1,1,female,32.0,0,0,76.2917,C,First,woman,False,D,Cherbourg,yes,True
+0,2,male,30.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
+1,3,male,16.0,0,0,8.05,S,Third,man,True,,Southampton,yes,True
+0,2,male,27.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,3,male,51.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+1,1,male,38.0,1,0,90.0,S,First,man,True,C,Southampton,yes,False
+0,3,male,22.0,0,0,9.35,S,Third,man,True,,Southampton,no,True
+1,2,male,19.0,0,0,10.5,S,Second,man,True,,Southampton,yes,True
+0,3,male,20.5,0,0,7.25,S,Third,man,True,,Southampton,no,True
+0,2,male,18.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,3,female,,3,1,25.4667,S,Third,woman,False,,Southampton,no,False
+1,1,female,35.0,1,0,83.475,S,First,woman,False,C,Southampton,yes,False
+0,3,male,29.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
+0,2,male,59.0,0,0,13.5,S,Second,man,True,,Southampton,no,True
+1,3,female,5.0,4,2,31.3875,S,Third,child,False,,Southampton,yes,False
+0,2,male,24.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
+0,3,female,,0,0,7.55,S,Third,woman,False,,Southampton,no,True
+0,2,male,44.0,1,0,26.0,S,Second,man,True,,Southampton,no,False
+1,2,female,8.0,0,2,26.25,S,Second,child,False,,Southampton,yes,False
+0,2,male,19.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
+0,2,male,33.0,0,0,12.275,S,Second,man,True,,Southampton,no,True
+0,3,female,,1,0,14.4542,C,Third,woman,False,,Cherbourg,no,False
+1,3,female,,1,0,15.5,Q,Third,woman,False,,Queenstown,yes,False
+0,2,male,29.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
+0,3,male,22.0,0,0,7.125,S,Third,man,True,,Southampton,no,True
+0,3,male,30.0,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
+0,1,male,44.0,2,0,90.0,Q,First,man,True,C,Queenstown,no,False
+0,3,female,25.0,0,0,7.775,S,Third,woman,False,,Southampton,no,True
+1,2,female,24.0,0,2,14.5,S,Second,woman,False,,Southampton,yes,False
+1,1,male,37.0,1,1,52.5542,S,First,man,True,D,Southampton,yes,False
+0,2,male,54.0,1,0,26.0,S,Second,man,True,,Southampton,no,False
+0,3,male,,0,0,7.25,S,Third,man,True,,Southampton,no,True
+0,3,female,29.0,1,1,10.4625,S,Third,woman,False,G,Southampton,no,False
+0,1,male,62.0,0,0,26.55,S,First,man,True,C,Southampton,no,True
+0,3,male,30.0,1,0,16.1,S,Third,man,True,,Southampton,no,False
+0,3,female,41.0,0,2,20.2125,S,Third,woman,False,,Southampton,no,False
+1,3,female,29.0,0,2,15.2458,C,Third,woman,False,,Cherbourg,yes,False
+1,1,female,,0,0,79.2,C,First,woman,False,,Cherbourg,yes,True
+1,1,female,30.0,0,0,86.5,S,First,woman,False,B,Southampton,yes,True
+1,1,female,35.0,0,0,512.3292,C,First,woman,False,,Cherbourg,yes,True
+1,2,female,50.0,0,1,26.0,S,Second,woman,False,,Southampton,yes,False
+0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
+1,3,male,3.0,4,2,31.3875,S,Third,child,False,,Southampton,yes,False
+0,1,male,52.0,1,1,79.65,S,First,man,True,E,Southampton,no,False
+0,1,male,40.0,0,0,0.0,S,First,man,True,B,Southampton,no,True
+0,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,no,True
+0,2,male,36.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
+0,3,male,16.0,4,1,39.6875,S,Third,man,True,,Southampton,no,False
+1,3,male,25.0,1,0,7.775,S,Third,man,True,,Southampton,yes,False
+1,1,female,58.0,0,1,153.4625,S,First,woman,False,C,Southampton,yes,False
+1,1,female,35.0,0,0,135.6333,S,First,woman,False,C,Southampton,yes,True
+0,1,male,,0,0,31.0,S,First,man,True,,Southampton,no,True
+1,3,male,25.0,0,0,0.0,S,Third,man,True,,Southampton,yes,True
+1,2,female,41.0,0,1,19.5,S,Second,woman,False,,Southampton,yes,False
+0,1,male,37.0,0,1,29.7,C,First,man,True,C,Cherbourg,no,False
+1,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
+1,1,female,63.0,1,0,77.9583,S,First,woman,False,D,Southampton,yes,False
+0,3,female,45.0,0,0,7.75,S,Third,woman,False,,Southampton,no,True
+0,2,male,,0,0,0.0,S,Second,man,True,,Southampton,no,True
+0,3,male,7.0,4,1,29.125,Q,Third,child,False,,Queenstown,no,False
+1,3,female,35.0,1,1,20.25,S,Third,woman,False,,Southampton,yes,False
+0,3,male,65.0,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
+0,3,male,28.0,0,0,7.8542,S,Third,man,True,,Southampton,no,True
+0,3,male,16.0,0,0,9.5,S,Third,man,True,,Southampton,no,True
+1,3,male,19.0,0,0,8.05,S,Third,man,True,,Southampton,yes,True
+0,1,male,,0,0,26.0,S,First,man,True,A,Southampton,no,True
+0,3,male,33.0,0,0,8.6625,C,Third,man,True,,Cherbourg,no,True
+1,3,male,30.0,0,0,9.5,S,Third,man,True,,Southampton,yes,True
+0,3,male,22.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+1,2,male,42.0,0,0,13.0,S,Second,man,True,,Southampton,yes,True
+1,3,female,22.0,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
+1,1,female,26.0,0,0,78.85,S,First,woman,False,,Southampton,yes,True
+1,1,female,19.0,1,0,91.0792,C,First,woman,False,B,Cherbourg,yes,False
+0,2,male,36.0,0,0,12.875,C,Second,man,True,D,Cherbourg,no,True
+0,3,female,24.0,0,0,8.85,S,Third,woman,False,,Southampton,no,True
+0,3,male,24.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,1,male,,0,0,27.7208,C,First,man,True,,Cherbourg,no,True
+0,3,male,23.5,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
+0,1,female,2.0,1,2,151.55,S,First,child,False,C,Southampton,no,False
+1,1,male,,0,0,30.5,S,First,man,True,C,Southampton,yes,True
+1,1,female,50.0,0,1,247.5208,C,First,woman,False,B,Cherbourg,yes,False
+1,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
+1,3,male,,2,0,23.25,Q,Third,man,True,,Queenstown,yes,False
+0,3,male,19.0,0,0,0.0,S,Third,man,True,,Southampton,no,True
+1,2,female,,0,0,12.35,Q,Second,woman,False,E,Queenstown,yes,True
+0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
+1,1,male,0.92,1,2,151.55,S,First,child,False,C,Southampton,yes,False
+1,1,female,,0,0,110.8833,C,First,woman,False,,Cherbourg,yes,True
+1,1,female,17.0,1,0,108.9,C,First,woman,False,C,Cherbourg,yes,False
+0,2,male,30.0,1,0,24.0,C,Second,man,True,,Cherbourg,no,False
+1,1,female,30.0,0,0,56.9292,C,First,woman,False,E,Cherbourg,yes,True
+1,1,female,24.0,0,0,83.1583,C,First,woman,False,C,Cherbourg,yes,True
+1,1,female,18.0,2,2,262.375,C,First,woman,False,B,Cherbourg,yes,False
+0,2,female,26.0,1,1,26.0,S,Second,woman,False,,Southampton,no,False
+0,3,male,28.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,2,male,43.0,1,1,26.25,S,Second,man,True,,Southampton,no,False
+1,3,female,26.0,0,0,7.8542,S,Third,woman,False,,Southampton,yes,True
+1,2,female,24.0,1,0,26.0,S,Second,woman,False,,Southampton,yes,False
+0,2,male,54.0,0,0,14.0,S,Second,man,True,,Southampton,no,True
+1,1,female,31.0,0,2,164.8667,S,First,woman,False,C,Southampton,yes,False
+1,1,female,40.0,1,1,134.5,C,First,woman,False,E,Cherbourg,yes,False
+0,3,male,22.0,0,0,7.25,S,Third,man,True,,Southampton,no,True
+0,3,male,27.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+1,2,female,30.0,0,0,12.35,Q,Second,woman,False,,Queenstown,yes,True
+1,2,female,22.0,1,1,29.0,S,Second,woman,False,,Southampton,yes,False
+0,3,male,,8,2,69.55,S,Third,man,True,,Southampton,no,False
+1,1,female,36.0,0,0,135.6333,C,First,woman,False,C,Cherbourg,yes,True
+0,3,male,61.0,0,0,6.2375,S,Third,man,True,,Southampton,no,True
+1,2,female,36.0,0,0,13.0,S,Second,woman,False,D,Southampton,yes,True
+1,3,female,31.0,1,1,20.525,S,Third,woman,False,,Southampton,yes,False
+1,1,female,16.0,0,1,57.9792,C,First,woman,False,B,Cherbourg,yes,False
+1,3,female,,2,0,23.25,Q,Third,woman,False,,Queenstown,yes,False
+0,1,male,45.5,0,0,28.5,S,First,man,True,C,Southampton,no,True
+0,1,male,38.0,0,1,153.4625,S,First,man,True,C,Southampton,no,False
+0,3,male,16.0,2,0,18.0,S,Third,man,True,,Southampton,no,False
+1,1,female,,1,0,133.65,S,First,woman,False,,Southampton,yes,False
+0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,1,male,29.0,1,0,66.6,S,First,man,True,C,Southampton,no,False
+1,1,female,41.0,0,0,134.5,C,First,woman,False,E,Cherbourg,yes,True
+1,3,male,45.0,0,0,8.05,S,Third,man,True,,Southampton,yes,True
+0,1,male,45.0,0,0,35.5,S,First,man,True,,Southampton,no,True
+1,2,male,2.0,1,1,26.0,S,Second,child,False,F,Southampton,yes,False
+1,1,female,24.0,3,2,263.0,S,First,woman,False,C,Southampton,yes,False
+0,2,male,28.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,2,male,25.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,2,male,36.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+1,2,female,24.0,0,0,13.0,S,Second,woman,False,F,Southampton,yes,True
+1,2,female,40.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
+1,3,female,,1,0,16.1,S,Third,woman,False,,Southampton,yes,False
+1,3,male,3.0,1,1,15.9,S,Third,child,False,,Southampton,yes,False
+0,3,male,42.0,0,0,8.6625,S,Third,man,True,,Southampton,no,True
+0,3,male,23.0,0,0,9.225,S,Third,man,True,,Southampton,no,True
+0,1,male,,0,0,35.0,S,First,man,True,C,Southampton,no,True
+0,3,male,15.0,1,1,7.2292,C,Third,child,False,,Cherbourg,no,False
+0,3,male,25.0,1,0,17.8,S,Third,man,True,,Southampton,no,False
+0,3,male,,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
+0,3,male,28.0,0,0,9.5,S,Third,man,True,,Southampton,no,True
+1,1,female,22.0,0,1,55.0,S,First,woman,False,E,Southampton,yes,False
+0,2,female,38.0,0,0,13.0,S,Second,woman,False,,Southampton,no,True
+1,3,female,,0,0,7.8792,Q,Third,woman,False,,Queenstown,yes,True
+1,3,female,,0,0,7.8792,Q,Third,woman,False,,Queenstown,yes,True
+0,3,male,40.0,1,4,27.9,S,Third,man,True,,Southampton,no,False
+0,2,male,29.0,1,0,27.7208,C,Second,man,True,,Cherbourg,no,False
+0,3,female,45.0,0,1,14.4542,C,Third,woman,False,,Cherbourg,no,False
+0,3,male,35.0,0,0,7.05,S,Third,man,True,,Southampton,no,True
+0,3,male,,1,0,15.5,Q,Third,man,True,,Queenstown,no,False
+0,3,male,30.0,0,0,7.25,S,Third,man,True,,Southampton,no,True
+1,1,female,60.0,1,0,75.25,C,First,woman,False,D,Cherbourg,yes,False
+1,3,female,,0,0,7.2292,C,Third,woman,False,,Cherbourg,yes,True
+1,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
+1,1,female,24.0,0,0,69.3,C,First,woman,False,B,Cherbourg,yes,True
+1,1,male,25.0,1,0,55.4417,C,First,man,True,E,Cherbourg,yes,False
+0,3,male,18.0,1,0,6.4958,S,Third,man,True,,Southampton,no,False
+0,3,male,19.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,1,male,22.0,0,0,135.6333,C,First,man,True,,Cherbourg,no,True
+0,3,female,3.0,3,1,21.075,S,Third,child,False,,Southampton,no,False
+1,1,female,,1,0,82.1708,C,First,woman,False,,Cherbourg,yes,False
+1,3,female,22.0,0,0,7.25,S,Third,woman,False,,Southampton,yes,True
+0,1,male,27.0,0,2,211.5,C,First,man,True,C,Cherbourg,no,False
+0,3,male,20.0,0,0,4.0125,C,Third,man,True,,Cherbourg,no,True
+0,3,male,19.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
+1,1,female,42.0,0,0,227.525,C,First,woman,False,,Cherbourg,yes,True
+1,3,female,1.0,0,2,15.7417,C,Third,child,False,,Cherbourg,yes,False
+0,3,male,32.0,0,0,7.925,S,Third,man,True,,Southampton,no,True
+1,1,female,35.0,1,0,52.0,S,First,woman,False,,Southampton,yes,False
+0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,2,male,18.0,0,0,73.5,S,Second,man,True,,Southampton,no,True
+0,3,male,1.0,5,2,46.9,S,Third,child,False,,Southampton,no,False
+1,2,female,36.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
+0,3,male,,0,0,7.7292,Q,Third,man,True,,Queenstown,no,True
+1,2,female,17.0,0,0,12.0,C,Second,woman,False,,Cherbourg,yes,True
+1,1,male,36.0,1,2,120.0,S,First,man,True,B,Southampton,yes,False
+1,3,male,21.0,0,0,7.7958,S,Third,man,True,,Southampton,yes,True
+0,3,male,28.0,2,0,7.925,S,Third,man,True,,Southampton,no,False
+1,1,female,23.0,1,0,113.275,C,First,woman,False,D,Cherbourg,yes,False
+1,3,female,24.0,0,2,16.7,S,Third,woman,False,G,Southampton,yes,False
+0,3,male,22.0,0,0,7.7958,S,Third,man,True,,Southampton,no,True
+0,3,female,31.0,0,0,7.8542,S,Third,woman,False,,Southampton,no,True
+0,2,male,46.0,0,0,26.0,S,Second,man,True,,Southampton,no,True
+0,2,male,23.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
+1,2,female,28.0,0,0,12.65,S,Second,woman,False,,Southampton,yes,True
+1,3,male,39.0,0,0,7.925,S,Third,man,True,,Southampton,yes,True
+0,3,male,26.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,female,21.0,1,0,9.825,S,Third,woman,False,,Southampton,no,False
+0,3,male,28.0,1,0,15.85,S,Third,man,True,,Southampton,no,False
+0,3,female,20.0,0,0,8.6625,S,Third,woman,False,,Southampton,no,True
+0,2,male,34.0,1,0,21.0,S,Second,man,True,,Southampton,no,False
+0,3,male,51.0,0,0,7.75,S,Third,man,True,,Southampton,no,True
+1,2,male,3.0,1,1,18.75,S,Second,child,False,,Southampton,yes,False
+0,3,male,21.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
+0,3,female,,3,1,25.4667,S,Third,woman,False,,Southampton,no,False
+0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,6.8583,Q,Third,man,True,,Queenstown,no,True
+1,1,female,33.0,1,0,90.0,Q,First,woman,False,C,Queenstown,yes,False
+0,2,male,,0,0,0.0,S,Second,man,True,,Southampton,no,True
+1,3,male,44.0,0,0,7.925,S,Third,man,True,,Southampton,yes,True
+0,3,female,,0,0,8.05,S,Third,woman,False,,Southampton,no,True
+1,2,female,34.0,1,1,32.5,S,Second,woman,False,,Southampton,yes,False
+1,2,female,18.0,0,2,13.0,S,Second,woman,False,,Southampton,yes,False
+0,2,male,30.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,3,female,10.0,0,2,24.15,S,Third,child,False,,Southampton,no,False
+0,3,male,,0,0,7.8958,C,Third,man,True,,Cherbourg,no,True
+0,3,male,21.0,0,0,7.7333,Q,Third,man,True,,Queenstown,no,True
+0,3,male,29.0,0,0,7.875,S,Third,man,True,,Southampton,no,True
+0,3,female,28.0,1,1,14.4,S,Third,woman,False,,Southampton,no,False
+0,3,male,18.0,1,1,20.2125,S,Third,man,True,,Southampton,no,False
+0,3,male,,0,0,7.25,S,Third,man,True,,Southampton,no,True
+1,2,female,28.0,1,0,26.0,S,Second,woman,False,,Southampton,yes,False
+1,2,female,19.0,0,0,26.0,S,Second,woman,False,,Southampton,yes,True
+0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
+1,3,male,32.0,0,0,8.05,S,Third,man,True,E,Southampton,yes,True
+1,1,male,28.0,0,0,26.55,S,First,man,True,C,Southampton,yes,True
+1,3,female,,1,0,16.1,S,Third,woman,False,,Southampton,yes,False
+1,2,female,42.0,1,0,26.0,S,Second,woman,False,,Southampton,yes,False
+0,3,male,17.0,0,0,7.125,S,Third,man,True,,Southampton,no,True
+0,1,male,50.0,1,0,55.9,S,First,man,True,E,Southampton,no,False
+1,1,female,14.0,1,2,120.0,S,First,child,False,B,Southampton,yes,False
+0,3,female,21.0,2,2,34.375,S,Third,woman,False,,Southampton,no,False
+1,2,female,24.0,2,3,18.75,S,Second,woman,False,,Southampton,yes,False
+0,1,male,64.0,1,4,263.0,S,First,man,True,C,Southampton,no,False
+0,2,male,31.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
+1,2,female,45.0,1,1,26.25,S,Second,woman,False,,Southampton,yes,False
+0,3,male,20.0,0,0,9.5,S,Third,man,True,,Southampton,no,True
+0,3,male,25.0,1,0,7.775,S,Third,man,True,,Southampton,no,False
+1,2,female,28.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
+1,3,male,,0,0,8.1125,S,Third,man,True,,Southampton,yes,True
+1,1,male,4.0,0,2,81.8583,S,First,child,False,A,Southampton,yes,False
+1,2,female,13.0,0,1,19.5,S,Second,child,False,,Southampton,yes,False
+1,1,male,34.0,0,0,26.55,S,First,man,True,,Southampton,yes,True
+1,3,female,5.0,2,1,19.2583,C,Third,child,False,,Cherbourg,yes,False
+1,1,male,52.0,0,0,30.5,S,First,man,True,C,Southampton,yes,True
+0,2,male,36.0,1,2,27.75,S,Second,man,True,,Southampton,no,False
+0,3,male,,1,0,19.9667,S,Third,man,True,,Southampton,no,False
+0,1,male,30.0,0,0,27.75,C,First,man,True,C,Cherbourg,no,True
+1,1,male,49.0,1,0,89.1042,C,First,man,True,C,Cherbourg,yes,False
+0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
+1,3,male,29.0,0,0,7.8958,C,Third,man,True,,Cherbourg,yes,True
+0,1,male,65.0,0,0,26.55,S,First,man,True,E,Southampton,no,True
+1,1,female,,1,0,51.8625,S,First,woman,False,D,Southampton,yes,False
+1,2,female,50.0,0,0,10.5,S,Second,woman,False,,Southampton,yes,True
+0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
+1,1,male,48.0,0,0,26.55,S,First,man,True,E,Southampton,yes,True
+0,3,male,34.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,1,male,47.0,0,0,38.5,S,First,man,True,E,Southampton,no,True
+0,2,male,48.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,male,38.0,0,0,7.05,S,Third,man,True,,Southampton,no,True
+0,2,male,,0,0,0.0,S,Second,man,True,,Southampton,no,True
+0,1,male,56.0,0,0,26.55,S,First,man,True,,Southampton,no,True
+0,3,male,,0,0,7.725,Q,Third,man,True,,Queenstown,no,True
+1,3,female,0.75,2,1,19.2583,C,Third,child,False,,Cherbourg,yes,False
+0,3,male,,0,0,7.25,S,Third,man,True,,Southampton,no,True
+0,3,male,38.0,0,0,8.6625,S,Third,man,True,,Southampton,no,True
+1,2,female,33.0,1,2,27.75,S,Second,woman,False,,Southampton,yes,False
+1,2,female,23.0,0,0,13.7917,C,Second,woman,False,D,Cherbourg,yes,True
+0,3,female,22.0,0,0,9.8375,S,Third,woman,False,,Southampton,no,True
+0,1,male,,0,0,52.0,S,First,man,True,A,Southampton,no,True
+0,2,male,34.0,1,0,21.0,S,Second,man,True,,Southampton,no,False
+0,3,male,29.0,1,0,7.0458,S,Third,man,True,,Southampton,no,False
+0,3,male,22.0,0,0,7.5208,S,Third,man,True,,Southampton,no,True
+1,3,female,2.0,0,1,12.2875,S,Third,child,False,,Southampton,yes,False
+0,3,male,9.0,5,2,46.9,S,Third,child,False,,Southampton,no,False
+0,2,male,,0,0,0.0,S,Second,man,True,,Southampton,no,True
+0,3,male,50.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+1,3,female,63.0,0,0,9.5875,S,Third,woman,False,,Southampton,yes,True
+1,1,male,25.0,1,0,91.0792,C,First,man,True,B,Cherbourg,yes,False
+0,3,female,,3,1,25.4667,S,Third,woman,False,,Southampton,no,False
+1,1,female,35.0,1,0,90.0,S,First,woman,False,C,Southampton,yes,False
+0,1,male,58.0,0,0,29.7,C,First,man,True,B,Cherbourg,no,True
+0,3,male,30.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+1,3,male,9.0,1,1,15.9,S,Third,child,False,,Southampton,yes,False
+0,3,male,,1,0,19.9667,S,Third,man,True,,Southampton,no,False
+0,3,male,21.0,0,0,7.25,S,Third,man,True,,Southampton,no,True
+0,1,male,55.0,0,0,30.5,S,First,man,True,C,Southampton,no,True
+0,1,male,71.0,0,0,49.5042,C,First,man,True,,Cherbourg,no,True
+0,3,male,21.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,14.4583,C,Third,man,True,,Cherbourg,no,True
+1,1,female,54.0,1,0,78.2667,C,First,woman,False,D,Cherbourg,yes,False
+0,3,male,,0,0,15.1,S,Third,man,True,,Southampton,no,True
+0,1,female,25.0,1,2,151.55,S,First,woman,False,C,Southampton,no,False
+0,3,male,24.0,0,0,7.7958,S,Third,man,True,,Southampton,no,True
+0,3,male,17.0,0,0,8.6625,S,Third,man,True,,Southampton,no,True
+0,3,female,21.0,0,0,7.75,Q,Third,woman,False,,Queenstown,no,True
+0,3,female,,0,0,7.6292,Q,Third,woman,False,,Queenstown,no,True
+0,3,female,37.0,0,0,9.5875,S,Third,woman,False,,Southampton,no,True
+1,1,female,16.0,0,0,86.5,S,First,woman,False,B,Southampton,yes,True
+0,1,male,18.0,1,0,108.9,C,First,man,True,C,Cherbourg,no,False
+1,2,female,33.0,0,2,26.0,S,Second,woman,False,,Southampton,yes,False
+1,1,male,,0,0,26.55,S,First,man,True,,Southampton,yes,True
+0,3,male,28.0,0,0,22.525,S,Third,man,True,,Southampton,no,True
+1,3,male,26.0,0,0,56.4958,S,Third,man,True,,Southampton,yes,True
+1,3,male,29.0,0,0,7.75,Q,Third,man,True,,Queenstown,yes,True
+0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
+1,1,male,36.0,0,0,26.2875,S,First,man,True,E,Southampton,yes,True
+1,1,female,54.0,1,0,59.4,C,First,woman,False,,Cherbourg,yes,False
+0,3,male,24.0,0,0,7.4958,S,Third,man,True,,Southampton,no,True
+0,1,male,47.0,0,0,34.0208,S,First,man,True,D,Southampton,no,True
+1,2,female,34.0,0,0,10.5,S,Second,woman,False,F,Southampton,yes,True
+0,3,male,,0,0,24.15,Q,Third,man,True,,Queenstown,no,True
+1,2,female,36.0,1,0,26.0,S,Second,woman,False,,Southampton,yes,False
+0,3,male,32.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+1,1,female,30.0,0,0,93.5,S,First,woman,False,B,Southampton,yes,True
+0,3,male,22.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
+1,1,female,44.0,0,1,57.9792,C,First,woman,False,B,Cherbourg,yes,False
+0,3,male,,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
+0,3,male,40.5,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
+1,2,female,50.0,0,0,10.5,S,Second,woman,False,,Southampton,yes,True
+0,1,male,,0,0,221.7792,S,First,man,True,C,Southampton,no,True
+0,3,male,39.0,0,0,7.925,S,Third,man,True,,Southampton,no,True
+0,2,male,23.0,2,1,11.5,S,Second,man,True,,Southampton,no,False
+1,2,female,2.0,1,1,26.0,S,Second,child,False,,Southampton,yes,False
+0,3,male,,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
+0,3,male,17.0,1,1,7.2292,C,Third,man,True,,Cherbourg,no,False
+1,3,female,,0,2,22.3583,C,Third,woman,False,,Cherbourg,yes,False
+0,3,female,30.0,0,0,8.6625,S,Third,woman,False,,Southampton,no,True
+1,2,female,7.0,0,2,26.25,S,Second,child,False,,Southampton,yes,False
+0,1,male,45.0,0,0,26.55,S,First,man,True,B,Southampton,no,True
+1,1,female,30.0,0,0,106.425,C,First,woman,False,,Cherbourg,yes,True
+0,3,male,,0,0,14.5,S,Third,man,True,,Southampton,no,True
+1,1,female,22.0,0,2,49.5,C,First,woman,False,B,Cherbourg,yes,False
+1,1,female,36.0,0,2,71.0,S,First,woman,False,B,Southampton,yes,False
+0,3,female,9.0,4,2,31.275,S,Third,child,False,,Southampton,no,False
+0,3,female,11.0,4,2,31.275,S,Third,child,False,,Southampton,no,False
+1,2,male,32.0,1,0,26.0,S,Second,man,True,,Southampton,yes,False
+0,1,male,50.0,1,0,106.425,C,First,man,True,C,Cherbourg,no,False
+0,1,male,64.0,0,0,26.0,S,First,man,True,,Southampton,no,True
+1,2,female,19.0,1,0,26.0,S,Second,woman,False,,Southampton,yes,False
+1,2,male,,0,0,13.8625,C,Second,man,True,,Cherbourg,yes,True
+0,3,male,33.0,1,1,20.525,S,Third,man,True,,Southampton,no,False
+1,2,male,8.0,1,1,36.75,S,Second,child,False,,Southampton,yes,False
+1,1,male,17.0,0,2,110.8833,C,First,man,True,C,Cherbourg,yes,False
+0,2,male,27.0,0,0,26.0,S,Second,man,True,,Southampton,no,True
+0,3,male,,0,0,7.8292,Q,Third,man,True,,Queenstown,no,True
+1,3,male,22.0,0,0,7.225,C,Third,man,True,,Cherbourg,yes,True
+1,3,female,22.0,0,0,7.775,S,Third,woman,False,,Southampton,yes,True
+0,1,male,62.0,0,0,26.55,S,First,man,True,,Southampton,no,True
+1,1,female,48.0,1,0,39.6,C,First,woman,False,A,Cherbourg,yes,False
+0,1,male,,0,0,227.525,C,First,man,True,,Cherbourg,no,True
+1,1,female,39.0,1,1,79.65,S,First,woman,False,E,Southampton,yes,False
+1,3,female,36.0,1,0,17.4,S,Third,woman,False,,Southampton,yes,False
+0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
+0,3,male,40.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,2,male,28.0,0,0,13.5,S,Second,man,True,,Southampton,no,True
+0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,female,,0,0,8.05,S,Third,woman,False,,Southampton,no,True
+0,3,male,24.0,2,0,24.15,S,Third,man,True,,Southampton,no,False
+0,3,male,19.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,3,female,29.0,0,4,21.075,S,Third,woman,False,,Southampton,no,False
+0,3,male,,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
+1,3,male,32.0,0,0,7.8542,S,Third,man,True,,Southampton,yes,True
+1,2,male,62.0,0,0,10.5,S,Second,man,True,,Southampton,yes,True
+1,1,female,53.0,2,0,51.4792,S,First,woman,False,C,Southampton,yes,False
+1,1,male,36.0,0,0,26.3875,S,First,man,True,E,Southampton,yes,True
+1,3,female,,0,0,7.75,Q,Third,woman,False,,Queenstown,yes,True
+0,3,male,16.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,male,19.0,0,0,14.5,S,Third,man,True,,Southampton,no,True
+1,2,female,34.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
+1,1,female,39.0,1,0,55.9,S,First,woman,False,E,Southampton,yes,False
+0,3,female,,1,0,14.4583,C,Third,woman,False,,Cherbourg,no,False
+1,3,male,32.0,0,0,7.925,S,Third,man,True,,Southampton,yes,True
+1,2,female,25.0,1,1,30.0,S,Second,woman,False,,Southampton,yes,False
+1,1,female,39.0,1,1,110.8833,C,First,woman,False,C,Cherbourg,yes,False
+0,2,male,54.0,0,0,26.0,S,Second,man,True,,Southampton,no,True
+0,1,male,36.0,0,0,40.125,C,First,man,True,A,Cherbourg,no,True
+0,3,male,,0,0,8.7125,C,Third,man,True,,Cherbourg,no,True
+1,1,female,18.0,0,2,79.65,S,First,woman,False,E,Southampton,yes,False
+0,2,male,47.0,0,0,15.0,S,Second,man,True,,Southampton,no,True
+1,1,male,60.0,1,1,79.2,C,First,man,True,B,Cherbourg,yes,False
+0,3,male,22.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,3,male,35.0,0,0,7.125,S,Third,man,True,,Southampton,no,True
+1,1,female,52.0,1,0,78.2667,C,First,woman,False,D,Cherbourg,yes,False
+0,3,male,47.0,0,0,7.25,S,Third,man,True,,Southampton,no,True
+0,3,female,,0,2,7.75,Q,Third,woman,False,,Queenstown,no,False
+0,2,male,37.0,1,0,26.0,S,Second,man,True,,Southampton,no,False
+0,3,male,36.0,1,1,24.15,S,Third,man,True,,Southampton,no,False
+1,2,female,,0,0,33.0,S,Second,woman,False,,Southampton,yes,True
+0,3,male,49.0,0,0,0.0,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
+1,1,male,49.0,1,0,56.9292,C,First,man,True,A,Cherbourg,yes,False
+1,2,female,24.0,2,1,27.0,S,Second,woman,False,,Southampton,yes,False
+0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,1,male,,0,0,42.4,S,First,man,True,,Southampton,no,True
+0,3,male,44.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+1,1,male,35.0,0,0,26.55,C,First,man,True,,Cherbourg,yes,True
+0,3,male,36.0,1,0,15.55,S,Third,man,True,,Southampton,no,False
+0,3,male,30.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+1,1,male,27.0,0,0,30.5,S,First,man,True,,Southampton,yes,True
+1,2,female,22.0,1,2,41.5792,C,Second,woman,False,,Cherbourg,yes,False
+1,1,female,40.0,0,0,153.4625,S,First,woman,False,C,Southampton,yes,True
+0,3,female,39.0,1,5,31.275,S,Third,woman,False,,Southampton,no,False
+0,3,male,,0,0,7.05,S,Third,man,True,,Southampton,no,True
+1,3,female,,1,0,15.5,Q,Third,woman,False,,Queenstown,yes,False
+0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
+0,3,male,35.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+1,2,female,24.0,1,2,65.0,S,Second,woman,False,,Southampton,yes,False
+0,3,male,34.0,1,1,14.4,S,Third,man,True,,Southampton,no,False
+0,3,female,26.0,1,0,16.1,S,Third,woman,False,,Southampton,no,False
+1,2,female,4.0,2,1,39.0,S,Second,child,False,F,Southampton,yes,False
+0,2,male,26.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
+0,3,male,27.0,1,0,14.4542,C,Third,man,True,,Cherbourg,no,False
+1,1,male,42.0,1,0,52.5542,S,First,man,True,D,Southampton,yes,False
+1,3,male,20.0,1,1,15.7417,C,Third,man,True,,Cherbourg,yes,False
+0,3,male,21.0,0,0,7.8542,S,Third,man,True,,Southampton,no,True
+0,3,male,21.0,0,0,16.1,S,Third,man,True,,Southampton,no,True
+0,1,male,61.0,0,0,32.3208,S,First,man,True,D,Southampton,no,True
+0,2,male,57.0,0,0,12.35,Q,Second,man,True,,Queenstown,no,True
+1,1,female,21.0,0,0,77.9583,S,First,woman,False,D,Southampton,yes,True
+0,3,male,26.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,7.7333,Q,Third,man,True,,Queenstown,no,True
+1,1,male,80.0,0,0,30.0,S,First,man,True,A,Southampton,yes,True
+0,3,male,51.0,0,0,7.0542,S,Third,man,True,,Southampton,no,True
+1,1,male,32.0,0,0,30.5,C,First,man,True,B,Cherbourg,yes,True
+0,1,male,,0,0,0.0,S,First,man,True,,Southampton,no,True
+0,3,female,9.0,3,2,27.9,S,Third,child,False,,Southampton,no,False
+1,2,female,28.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
+0,3,male,32.0,0,0,7.925,S,Third,man,True,,Southampton,no,True
+0,2,male,31.0,1,1,26.25,S,Second,man,True,,Southampton,no,False
+0,3,female,41.0,0,5,39.6875,S,Third,woman,False,,Southampton,no,False
+0,3,male,,1,0,16.1,S,Third,man,True,,Southampton,no,False
+0,3,male,20.0,0,0,7.8542,S,Third,man,True,,Southampton,no,True
+1,1,female,24.0,0,0,69.3,C,First,woman,False,B,Cherbourg,yes,True
+0,3,female,2.0,3,2,27.9,S,Third,child,False,,Southampton,no,False
+1,3,male,,0,0,56.4958,S,Third,man,True,,Southampton,yes,True
+1,3,female,0.75,2,1,19.2583,C,Third,child,False,,Cherbourg,yes,False
+1,1,male,48.0,1,0,76.7292,C,First,man,True,D,Cherbourg,yes,False
+0,3,male,19.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+1,1,male,56.0,0,0,35.5,C,First,man,True,A,Cherbourg,yes,True
+0,3,male,,0,0,7.55,S,Third,man,True,,Southampton,no,True
+1,3,female,23.0,0,0,7.55,S,Third,woman,False,,Southampton,yes,True
+0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+1,2,female,18.0,0,1,23.0,S,Second,woman,False,,Southampton,yes,False
+0,3,male,21.0,0,0,8.4333,S,Third,man,True,,Southampton,no,True
+1,3,female,,0,0,7.8292,Q,Third,woman,False,,Queenstown,yes,True
+0,3,female,18.0,0,0,6.75,Q,Third,woman,False,,Queenstown,no,True
+0,2,male,24.0,2,0,73.5,S,Second,man,True,,Southampton,no,False
+0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,3,female,32.0,1,1,15.5,Q,Third,woman,False,,Queenstown,no,False
+0,2,male,23.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,1,male,58.0,0,2,113.275,C,First,man,True,D,Cherbourg,no,False
+1,1,male,50.0,2,0,133.65,S,First,man,True,,Southampton,yes,False
+0,3,male,40.0,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
+0,1,male,47.0,0,0,25.5875,S,First,man,True,E,Southampton,no,True
+0,3,male,36.0,0,0,7.4958,S,Third,man,True,,Southampton,no,True
+1,3,male,20.0,1,0,7.925,S,Third,man,True,,Southampton,yes,False
+0,2,male,32.0,2,0,73.5,S,Second,man,True,,Southampton,no,False
+0,2,male,25.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,3,male,,0,0,7.775,S,Third,man,True,,Southampton,no,True
+0,3,male,43.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+1,1,female,,1,0,52.0,S,First,woman,False,C,Southampton,yes,False
+1,2,female,40.0,1,1,39.0,S,Second,woman,False,,Southampton,yes,False
+0,1,male,31.0,1,0,52.0,S,First,man,True,B,Southampton,no,False
+0,2,male,70.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
+1,2,male,31.0,0,0,13.0,S,Second,man,True,,Southampton,yes,True
+0,2,male,,0,0,0.0,S,Second,man,True,,Southampton,no,True
+0,3,male,18.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
+0,3,male,24.5,0,0,8.05,S,Third,man,True,,Southampton,no,True
+1,3,female,18.0,0,0,9.8417,S,Third,woman,False,,Southampton,yes,True
+0,3,female,43.0,1,6,46.9,S,Third,woman,False,,Southampton,no,False
+1,1,male,36.0,0,1,512.3292,C,First,man,True,B,Cherbourg,yes,False
+0,3,female,,0,0,8.1375,Q,Third,woman,False,,Queenstown,no,True
+1,1,male,27.0,0,0,76.7292,C,First,man,True,D,Cherbourg,yes,True
+0,3,male,20.0,0,0,9.225,S,Third,man,True,,Southampton,no,True
+0,3,male,14.0,5,2,46.9,S,Third,child,False,,Southampton,no,False
+0,2,male,60.0,1,1,39.0,S,Second,man,True,,Southampton,no,False
+0,2,male,25.0,1,2,41.5792,C,Second,man,True,,Cherbourg,no,False
+0,3,male,14.0,4,1,39.6875,S,Third,child,False,,Southampton,no,False
+0,3,male,19.0,0,0,10.1708,S,Third,man,True,,Southampton,no,True
+0,3,male,18.0,0,0,7.7958,S,Third,man,True,,Southampton,no,True
+1,1,female,15.0,0,1,211.3375,S,First,child,False,B,Southampton,yes,False
+1,1,male,31.0,1,0,57.0,S,First,man,True,B,Southampton,yes,False
+1,3,female,4.0,0,1,13.4167,C,Third,child,False,,Cherbourg,yes,False
+1,3,male,,0,0,56.4958,S,Third,man,True,,Southampton,yes,True
+0,3,male,25.0,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
+0,1,male,60.0,0,0,26.55,S,First,man,True,,Southampton,no,True
+0,2,male,52.0,0,0,13.5,S,Second,man,True,,Southampton,no,True
+0,3,male,44.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+1,3,female,,0,0,7.7333,Q,Third,woman,False,,Queenstown,yes,True
+0,1,male,49.0,1,1,110.8833,C,First,man,True,C,Cherbourg,no,False
+0,3,male,42.0,0,0,7.65,S,Third,man,True,F,Southampton,no,True
+1,1,female,18.0,1,0,227.525,C,First,woman,False,C,Cherbourg,yes,False
+1,1,male,35.0,0,0,26.2875,S,First,man,True,E,Southampton,yes,True
+0,3,female,18.0,0,1,14.4542,C,Third,woman,False,,Cherbourg,no,False
+0,3,male,25.0,0,0,7.7417,Q,Third,man,True,,Queenstown,no,True
+0,3,male,26.0,1,0,7.8542,S,Third,man,True,,Southampton,no,False
+0,2,male,39.0,0,0,26.0,S,Second,man,True,,Southampton,no,True
+1,2,female,45.0,0,0,13.5,S,Second,woman,False,,Southampton,yes,True
+1,1,male,42.0,0,0,26.2875,S,First,man,True,E,Southampton,yes,True
+1,1,female,22.0,0,0,151.55,S,First,woman,False,,Southampton,yes,True
+1,3,male,,1,1,15.2458,C,Third,man,True,,Cherbourg,yes,False
+1,1,female,24.0,0,0,49.5042,C,First,woman,False,C,Cherbourg,yes,True
+0,1,male,,0,0,26.55,S,First,man,True,C,Southampton,no,True
+1,1,male,48.0,1,0,52.0,S,First,man,True,C,Southampton,yes,False
+0,3,male,29.0,0,0,9.4833,S,Third,man,True,,Southampton,no,True
+0,2,male,52.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,3,male,19.0,0,0,7.65,S,Third,man,True,F,Southampton,no,True
+1,1,female,38.0,0,0,227.525,C,First,woman,False,C,Cherbourg,yes,True
+1,2,female,27.0,0,0,10.5,S,Second,woman,False,E,Southampton,yes,True
+0,3,male,,0,0,15.5,Q,Third,man,True,,Queenstown,no,True
+0,3,male,33.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
+1,2,female,6.0,0,1,33.0,S,Second,child,False,,Southampton,yes,False
+0,3,male,17.0,1,0,7.0542,S,Third,man,True,,Southampton,no,False
+0,2,male,34.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,2,male,50.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+1,1,male,27.0,1,0,53.1,S,First,man,True,E,Southampton,yes,False
+0,3,male,20.0,0,0,8.6625,S,Third,man,True,,Southampton,no,True
+1,2,female,30.0,3,0,21.0,S,Second,woman,False,,Southampton,yes,False
+1,3,female,,0,0,7.7375,Q,Third,woman,False,,Queenstown,yes,True
+0,2,male,25.0,1,0,26.0,S,Second,man,True,,Southampton,no,False
+0,3,female,25.0,1,0,7.925,S,Third,woman,False,,Southampton,no,False
+1,1,female,29.0,0,0,211.3375,S,First,woman,False,B,Southampton,yes,True
+0,3,male,11.0,0,0,18.7875,C,Third,child,False,,Cherbourg,no,True
+0,2,male,,0,0,0.0,S,Second,man,True,,Southampton,no,True
+0,2,male,23.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,2,male,23.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+0,3,male,28.5,0,0,16.1,S,Third,man,True,,Southampton,no,True
+0,3,female,48.0,1,3,34.375,S,Third,woman,False,,Southampton,no,False
+1,1,male,35.0,0,0,512.3292,C,First,man,True,B,Cherbourg,yes,True
+0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+1,1,male,,0,0,30.0,S,First,man,True,D,Southampton,yes,True
+0,1,male,36.0,1,0,78.85,S,First,man,True,C,Southampton,no,False
+1,1,female,21.0,2,2,262.375,C,First,woman,False,B,Cherbourg,yes,False
+0,3,male,24.0,1,0,16.1,S,Third,man,True,,Southampton,no,False
+1,3,male,31.0,0,0,7.925,S,Third,man,True,,Southampton,yes,True
+0,1,male,70.0,1,1,71.0,S,First,man,True,B,Southampton,no,False
+0,3,male,16.0,1,1,20.25,S,Third,man,True,,Southampton,no,False
+1,2,female,30.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
+0,1,male,19.0,1,0,53.1,S,First,man,True,D,Southampton,no,False
+0,3,male,31.0,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
+1,2,female,4.0,1,1,23.0,S,Second,child,False,,Southampton,yes,False
+1,3,male,6.0,0,1,12.475,S,Third,child,False,E,Southampton,yes,False
+0,3,male,33.0,0,0,9.5,S,Third,man,True,,Southampton,no,True
+0,3,male,23.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+1,2,female,48.0,1,2,65.0,S,Second,woman,False,,Southampton,yes,False
+1,2,male,0.67,1,1,14.5,S,Second,child,False,,Southampton,yes,False
+0,3,male,28.0,0,0,7.7958,S,Third,man,True,,Southampton,no,True
+0,2,male,18.0,0,0,11.5,S,Second,man,True,,Southampton,no,True
+0,3,male,34.0,0,0,8.05,S,Third,man,True,,Southampton,no,True
+1,1,female,33.0,0,0,86.5,S,First,woman,False,B,Southampton,yes,True
+0,3,male,,0,0,14.5,S,Third,man,True,,Southampton,no,True
+0,3,male,41.0,0,0,7.125,S,Third,man,True,,Southampton,no,True
+1,3,male,20.0,0,0,7.2292,C,Third,man,True,,Cherbourg,yes,True
+1,1,female,36.0,1,2,120.0,S,First,woman,False,B,Southampton,yes,False
+0,3,male,16.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
+1,1,female,51.0,1,0,77.9583,S,First,woman,False,D,Southampton,yes,False
+0,1,male,,0,0,39.6,C,First,man,True,,Cherbourg,no,True
+0,3,female,30.5,0,0,7.75,Q,Third,woman,False,,Queenstown,no,True
+0,3,male,,1,0,24.15,Q,Third,man,True,,Queenstown,no,False
+0,3,male,32.0,0,0,8.3625,S,Third,man,True,,Southampton,no,True
+0,3,male,24.0,0,0,9.5,S,Third,man,True,,Southampton,no,True
+0,3,male,48.0,0,0,7.8542,S,Third,man,True,,Southampton,no,True
+0,2,female,57.0,0,0,10.5,S,Second,woman,False,E,Southampton,no,True
+0,3,male,,0,0,7.225,C,Third,man,True,,Cherbourg,no,True
+1,2,female,54.0,1,3,23.0,S,Second,woman,False,,Southampton,yes,False
+0,3,male,18.0,0,0,7.75,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,7.75,Q,Third,man,True,F,Queenstown,no,True
+1,3,female,5.0,0,0,12.475,S,Third,child,False,,Southampton,yes,True
+0,3,male,,0,0,7.7375,Q,Third,man,True,,Queenstown,no,True
+1,1,female,43.0,0,1,211.3375,S,First,woman,False,B,Southampton,yes,False
+1,3,female,13.0,0,0,7.2292,C,Third,child,False,,Cherbourg,yes,True
+1,1,female,17.0,1,0,57.0,S,First,woman,False,B,Southampton,yes,False
+0,1,male,29.0,0,0,30.0,S,First,man,True,D,Southampton,no,True
+0,3,male,,1,2,23.45,S,Third,man,True,,Southampton,no,False
+0,3,male,25.0,0,0,7.05,S,Third,man,True,,Southampton,no,True
+0,3,male,25.0,0,0,7.25,S,Third,man,True,,Southampton,no,True
+1,3,female,18.0,0,0,7.4958,S,Third,woman,False,,Southampton,yes,True
+0,3,male,8.0,4,1,29.125,Q,Third,child,False,,Queenstown,no,False
+1,3,male,1.0,1,2,20.575,S,Third,child,False,,Southampton,yes,False
+0,1,male,46.0,0,0,79.2,C,First,man,True,B,Cherbourg,no,True
+0,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
+0,2,male,16.0,0,0,26.0,S,Second,man,True,,Southampton,no,True
+0,3,female,,8,2,69.55,S,Third,woman,False,,Southampton,no,False
+0,1,male,,0,0,30.6958,C,First,man,True,,Cherbourg,no,True
+0,3,male,25.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,2,male,39.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+1,1,female,49.0,0,0,25.9292,S,First,woman,False,D,Southampton,yes,True
+1,3,female,31.0,0,0,8.6833,S,Third,woman,False,,Southampton,yes,True
+0,3,male,30.0,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
+0,3,female,30.0,1,1,24.15,S,Third,woman,False,,Southampton,no,False
+0,2,male,34.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+1,2,female,31.0,1,1,26.25,S,Second,woman,False,,Southampton,yes,False
+1,1,male,11.0,1,2,120.0,S,First,child,False,B,Southampton,yes,False
+1,3,male,0.42,0,1,8.5167,C,Third,child,False,,Cherbourg,yes,False
+1,3,male,27.0,0,0,6.975,S,Third,man,True,,Southampton,yes,True
+0,3,male,31.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
+0,1,male,39.0,0,0,0.0,S,First,man,True,A,Southampton,no,True
+0,3,female,18.0,0,0,7.775,S,Third,woman,False,,Southampton,no,True
+0,2,male,39.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+1,1,female,33.0,1,0,53.1,S,First,woman,False,E,Southampton,yes,False
+0,3,male,26.0,0,0,7.8875,S,Third,man,True,,Southampton,no,True
+0,3,male,39.0,0,0,24.15,S,Third,man,True,,Southampton,no,True
+0,2,male,35.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
+0,3,female,6.0,4,2,31.275,S,Third,child,False,,Southampton,no,False
+0,3,male,30.5,0,0,8.05,S,Third,man,True,,Southampton,no,True
+0,1,male,,0,0,0.0,S,First,man,True,B,Southampton,no,True
+0,3,female,23.0,0,0,7.925,S,Third,woman,False,,Southampton,no,True
+0,2,male,31.0,1,1,37.0042,C,Second,man,True,,Cherbourg,no,False
+0,3,male,43.0,0,0,6.45,S,Third,man,True,,Southampton,no,True
+0,3,male,10.0,3,2,27.9,S,Third,child,False,,Southampton,no,False
+1,1,female,52.0,1,1,93.5,S,First,woman,False,B,Southampton,yes,False
+1,3,male,27.0,0,0,8.6625,S,Third,man,True,,Southampton,yes,True
+0,1,male,38.0,0,0,0.0,S,First,man,True,,Southampton,no,True
+1,3,female,27.0,0,1,12.475,S,Third,woman,False,E,Southampton,yes,False
+0,3,male,2.0,4,1,39.6875,S,Third,child,False,,Southampton,no,False
+0,3,male,,0,0,6.95,Q,Third,man,True,,Queenstown,no,True
+0,3,male,,0,0,56.4958,S,Third,man,True,,Southampton,no,True
+1,2,male,1.0,0,2,37.0042,C,Second,child,False,,Cherbourg,yes,False
+1,3,male,,0,0,7.75,Q,Third,man,True,,Queenstown,yes,True
+1,1,female,62.0,0,0,80.0,,First,woman,False,B,,yes,True
+1,3,female,15.0,1,0,14.4542,C,Third,child,False,,Cherbourg,yes,False
+1,2,male,0.83,1,1,18.75,S,Second,child,False,,Southampton,yes,False
+0,3,male,,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
+0,3,male,23.0,0,0,7.8542,S,Third,man,True,,Southampton,no,True
+0,3,male,18.0,0,0,8.3,S,Third,man,True,,Southampton,no,True
+1,1,female,39.0,1,1,83.1583,C,First,woman,False,E,Cherbourg,yes,False
+0,3,male,21.0,0,0,8.6625,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,8.05,S,Third,man,True,,Southampton,no,True
+1,3,male,32.0,0,0,56.4958,S,Third,man,True,,Southampton,yes,True
+1,1,male,,0,0,29.7,C,First,man,True,C,Cherbourg,yes,True
+0,3,male,20.0,0,0,7.925,S,Third,man,True,,Southampton,no,True
+0,2,male,16.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
+1,1,female,30.0,0,0,31.0,C,First,woman,False,,Cherbourg,yes,True
+0,3,male,34.5,0,0,6.4375,C,Third,man,True,,Cherbourg,no,True
+0,3,male,17.0,0,0,8.6625,S,Third,man,True,,Southampton,no,True
+0,3,male,42.0,0,0,7.55,S,Third,man,True,,Southampton,no,True
+0,3,male,,8,2,69.55,S,Third,man,True,,Southampton,no,False
+0,3,male,35.0,0,0,7.8958,C,Third,man,True,,Cherbourg,no,True
+0,2,male,28.0,0,1,33.0,S,Second,man,True,,Southampton,no,False
+1,1,female,,1,0,89.1042,C,First,woman,False,C,Cherbourg,yes,False
+0,3,male,4.0,4,2,31.275,S,Third,child,False,,Southampton,no,False
+0,3,male,74.0,0,0,7.775,S,Third,man,True,,Southampton,no,True
+0,3,female,9.0,1,1,15.2458,C,Third,child,False,,Cherbourg,no,False
+1,1,female,16.0,0,1,39.4,S,First,woman,False,D,Southampton,yes,False
+0,2,female,44.0,1,0,26.0,S,Second,woman,False,,Southampton,no,False
+1,3,female,18.0,0,1,9.35,S,Third,woman,False,,Southampton,yes,False
+1,1,female,45.0,1,1,164.8667,S,First,woman,False,,Southampton,yes,False
+1,1,male,51.0,0,0,26.55,S,First,man,True,E,Southampton,yes,True
+1,3,female,24.0,0,3,19.2583,C,Third,woman,False,,Cherbourg,yes,False
+0,3,male,,0,0,7.2292,C,Third,man,True,,Cherbourg,no,True
+0,3,male,41.0,2,0,14.1083,S,Third,man,True,,Southampton,no,False
+0,2,male,21.0,1,0,11.5,S,Second,man,True,,Southampton,no,False
+1,1,female,48.0,0,0,25.9292,S,First,woman,False,D,Southampton,yes,True
+0,3,female,,8,2,69.55,S,Third,woman,False,,Southampton,no,False
+0,2,male,24.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+1,2,female,42.0,0,0,13.0,S,Second,woman,False,,Southampton,yes,True
+1,2,female,27.0,1,0,13.8583,C,Second,woman,False,,Cherbourg,yes,False
+0,1,male,31.0,0,0,50.4958,S,First,man,True,A,Southampton,no,True
+0,3,male,,0,0,9.5,S,Third,man,True,,Southampton,no,True
+1,3,male,4.0,1,1,11.1333,S,Third,child,False,,Southampton,yes,False
+0,3,male,26.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+1,1,female,47.0,1,1,52.5542,S,First,woman,False,D,Southampton,yes,False
+0,1,male,33.0,0,0,5.0,S,First,man,True,B,Southampton,no,True
+0,3,male,47.0,0,0,9.0,S,Third,man,True,,Southampton,no,True
+1,2,female,28.0,1,0,24.0,C,Second,woman,False,,Cherbourg,yes,False
+1,3,female,15.0,0,0,7.225,C,Third,child,False,,Cherbourg,yes,True
+0,3,male,20.0,0,0,9.8458,S,Third,man,True,,Southampton,no,True
+0,3,male,19.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,3,male,,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+1,1,female,56.0,0,1,83.1583,C,First,woman,False,C,Cherbourg,yes,False
+1,2,female,25.0,0,1,26.0,S,Second,woman,False,,Southampton,yes,False
+0,3,male,33.0,0,0,7.8958,S,Third,man,True,,Southampton,no,True
+0,3,female,22.0,0,0,10.5167,S,Third,woman,False,,Southampton,no,True
+0,2,male,28.0,0,0,10.5,S,Second,man,True,,Southampton,no,True
+0,3,male,25.0,0,0,7.05,S,Third,man,True,,Southampton,no,True
+0,3,female,39.0,0,5,29.125,Q,Third,woman,False,,Queenstown,no,False
+0,2,male,27.0,0,0,13.0,S,Second,man,True,,Southampton,no,True
+1,1,female,19.0,0,0,30.0,S,First,woman,False,B,Southampton,yes,True
+0,3,female,,1,2,23.45,S,Third,woman,False,,Southampton,no,False
+1,1,male,26.0,0,0,30.0,C,First,man,True,C,Cherbourg,yes,True
+0,3,male,32.0,0,0,7.75,Q,Third,man,True,,Queenstown,no,True
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/resources/tree-image-crop.png` & `forust-0.2.7/local_dependencies/forust-ml/resources/tree-image-crop.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.6/local_dependencies/forust-ml/rs-example.md` & `forust-0.2.7/local_dependencies/forust-ml/rs-example.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-## A Complete Rust Example
-
-To run this example, add the following code to your `Cargo.toml` file.
-```toml
-[dependencies]
-forust-ml = "0.2.6"
-polars = "0.24"
-reqwest = { version = "0.11", features = ["blocking"] }
-```
-
-The following is a runable example using `polars` for data processing. The actual data manipulation can be performed with any tool, the only vital part, is the data be in column major format.
-```rust
-use forust_ml::{GradientBooster, Matrix};
-use polars::prelude::*;
-use reqwest::blocking::Client;
-use std::error::Error;
-use std::io::Cursor;
-
-fn main() -> Result<(), Box<dyn Error>> {
-    let data: Vec<u8> = Client::new()
-        .get("https://raw.githubusercontent.com/mwaskom/seaborn-data/master/titanic.csv")
-        .send()?
-        .text()?
-        .bytes()
-        .collect();
-
-    let df = CsvReader::new(Cursor::new(data))
-        .has_header(true)
-        .finish()?
-        .select(["survived", "pclass", "age", "sibsp", "parch", "fare"])?;
-
-    // Get data in column major format...
-    let id_vars: Vec<&str> = Vec::new();
-    let mdf = df.melt(id_vars, ["pclass", "age", "sibsp", "parch", "fare"])?;
-
-    let data: Vec<f64> = mdf
-        .select_at_idx(1)
-        .expect("Invalid column")
-        .f64()?
-        .into_iter()
-        .map(|v| v.unwrap_or(f64::NAN))
-        .collect();
-    let y: Vec<f64> = df
-        .column("survived")?
-        .cast(&DataType::Float64)?
-        .f64()?
-        .into_iter()
-        .map(|v| v.unwrap_or(f64::NAN))
-        .collect();
-
-    // Create Matrix from ndarray.
-    let matrix = Matrix::new(&data, y.len(), 5);
-
-    // Create booster
-    // To provide parameters generate a default booster, and then use
-    // the relevant "set_" methods for any parameters you would like to
-    // adjust.
-    let mut model = GradientBooster::default().set_learning_rate(0.3);
-    model.fit_unweighted(&matrix, &y)?;
-
-    // Predict output.
-    println!("{:?} ...", &model.predict(&matrix, true)[0..10]);
-    Ok(())
-}
-```
-```
-[-1.275806741323322, 0.9178487278986722, -1.4758225567638874, 1.0830510996747762, -1.7252372093498707, -1.4195771454833448, -0.27499967138282955, -0.9451315118931234, -0.08839774504303932, 1.374593096319586] ...
-```
-
-We first read in the data, and then, generate a contiguous matrix, that is used for training the booster. At this point, we can then instantiate out gradient booster, using the default parameters. These can be adjusted using the relevant `set_` methods, for any parameters of interest ([see here](src/gradientbooster.rs#L278) for all such methods).
+## A Complete Rust Example
+
+To run this example, add the following code to your `Cargo.toml` file.
+```toml
+[dependencies]
+forust-ml = "0.2.7"
+polars = "0.24"
+reqwest = { version = "0.11", features = ["blocking"] }
+```
+
+The following is a runable example using `polars` for data processing. The actual data manipulation can be performed with any tool, the only vital part, is the data be in column major format.
+```rust
+use forust_ml::{GradientBooster, Matrix};
+use polars::prelude::*;
+use reqwest::blocking::Client;
+use std::error::Error;
+use std::io::Cursor;
+
+fn main() -> Result<(), Box<dyn Error>> {
+    let data: Vec<u8> = Client::new()
+        .get("https://raw.githubusercontent.com/mwaskom/seaborn-data/master/titanic.csv")
+        .send()?
+        .text()?
+        .bytes()
+        .collect();
+
+    let df = CsvReader::new(Cursor::new(data))
+        .has_header(true)
+        .finish()?
+        .select(["survived", "pclass", "age", "sibsp", "parch", "fare"])?;
+
+    // Get data in column major format...
+    let id_vars: Vec<&str> = Vec::new();
+    let mdf = df.melt(id_vars, ["pclass", "age", "sibsp", "parch", "fare"])?;
+
+    let data: Vec<f64> = mdf
+        .select_at_idx(1)
+        .expect("Invalid column")
+        .f64()?
+        .into_iter()
+        .map(|v| v.unwrap_or(f64::NAN))
+        .collect();
+    let y: Vec<f64> = df
+        .column("survived")?
+        .cast(&DataType::Float64)?
+        .f64()?
+        .into_iter()
+        .map(|v| v.unwrap_or(f64::NAN))
+        .collect();
+
+    // Create Matrix from ndarray.
+    let matrix = Matrix::new(&data, y.len(), 5);
+
+    // Create booster
+    // To provide parameters generate a default booster, and then use
+    // the relevant "set_" methods for any parameters you would like to
+    // adjust.
+    let mut model = GradientBooster::default().set_learning_rate(0.3);
+    model.fit_unweighted(&matrix, &y)?;
+
+    // Predict output.
+    println!("{:?} ...", &model.predict(&matrix, true)[0..10]);
+    Ok(())
+}
+```
+```
+[-1.275806741323322, 0.9178487278986722, -1.4758225567638874, 1.0830510996747762, -1.7252372093498707, -1.4195771454833448, -0.27499967138282955, -0.9451315118931234, -0.08839774504303932, 1.374593096319586] ...
+```
+
+We first read in the data, and then, generate a contiguous matrix, that is used for training the booster. At this point, we can then instantiate out gradient booster, using the default parameters. These can be adjusted using the relevant `set_` methods, for any parameters of interest ([see here](src/gradientbooster.rs#L278) for all such methods).
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/scripts/make_resources.py` & `forust-0.2.7/local_dependencies/forust-ml/scripts/make_resources.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import pandas as pd
-import numpy as np
-import seaborn as sns
-
-if __name__ == "__main__":
-    df = sns.load_dataset("titanic")
-    X = df.select_dtypes("number").drop(columns=["survived"]).astype(float)
-    y = df["survived"].astype(float)
-
-    pd.Series(X.fillna(0).to_numpy().ravel(order="F")).to_csv(
-        "resources/contiguous_no_missing.csv",
-        index=False,
-        header=False,
-    )
-
-    pd.Series(X.to_numpy().ravel(order="F")).to_csv(
-        "resources/contiguous_with_missing.csv",
-        index=False,
-        header=False,
-    )
-
-    y.to_csv(
-        "resources/performance.csv",
-        index=False,
-        header=False,
-    )
-
-    dfb = df.sample(
-        100_000,
-        random_state=0,
-        replace=True,
-    ).reset_index(drop=True)
-
-    Xb = dfb.select_dtypes("number").drop(columns=["survived"]).astype(float)
-    yb = dfb["survived"].astype(float)
-
-    pd.Series(Xb.fillna(0).to_numpy().ravel(order="F")).to_csv(
-        "resources/contiguous_no_missing_100k_samp_seed0.csv",
-        index=False,
-        header=False,
-    )
-
-    yb.to_csv(
-        "resources/performance_100k_samp_seed0.csv",
-        index=False,
-        header=False,
-    )
+import pandas as pd
+import numpy as np
+import seaborn as sns
+
+if __name__ == "__main__":
+    df = sns.load_dataset("titanic")
+    X = df.select_dtypes("number").drop(columns=["survived"]).astype(float)
+    y = df["survived"].astype(float)
+
+    pd.Series(X.fillna(0).to_numpy().ravel(order="F")).to_csv(
+        "resources/contiguous_no_missing.csv",
+        index=False,
+        header=False,
+    )
+
+    pd.Series(X.to_numpy().ravel(order="F")).to_csv(
+        "resources/contiguous_with_missing.csv",
+        index=False,
+        header=False,
+    )
+
+    y.to_csv(
+        "resources/performance.csv",
+        index=False,
+        header=False,
+    )
+
+    dfb = df.sample(
+        100_000,
+        random_state=0,
+        replace=True,
+    ).reset_index(drop=True)
+
+    Xb = dfb.select_dtypes("number").drop(columns=["survived"]).astype(float)
+    yb = dfb["survived"].astype(float)
+
+    pd.Series(Xb.fillna(0).to_numpy().ravel(order="F")).to_csv(
+        "resources/contiguous_no_missing_100k_samp_seed0.csv",
+        index=False,
+        header=False,
+    )
+
+    yb.to_csv(
+        "resources/performance_100k_samp_seed0.csv",
+        index=False,
+        header=False,
+    )
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/src/data.rs` & `forust-0.2.7/local_dependencies/forust-ml/src/data.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,322 +1,379 @@
-use serde::{Deserialize, Serialize};
-use std::fmt::{self, Debug, Display};
-use std::iter::Sum;
-use std::ops::{Add, AddAssign, Div, Mul, Neg, Sub, SubAssign};
-use std::str::FromStr;
-
-/// Data trait used throughout the package
-/// to control for floating point numbers.
-pub trait FloatData<T>:
-    Mul<Output = T>
-    + Display
-    + Add<Output = T>
-    + Div<Output = T>
-    + Neg<Output = T>
-    + Copy
-    + Debug
-    + PartialEq
-    + PartialOrd
-    + AddAssign
-    + Sub<Output = T>
-    + SubAssign
-    + Sum
-    + std::marker::Send
-    + std::marker::Sync
-{
-    const ZERO: T;
-    const ONE: T;
-    const MIN: T;
-    const MAX: T;
-    const NAN: T;
-    fn from_usize(v: usize) -> T;
-    fn from_u16(v: u16) -> T;
-    fn is_nan(self) -> bool;
-    fn ln(self) -> T;
-    fn exp(self) -> T;
-}
-impl FloatData<f64> for f64 {
-    const ZERO: f64 = 0.0;
-    const ONE: f64 = 1.0;
-    const MIN: f64 = f64::MIN;
-    const MAX: f64 = f64::MAX;
-    const NAN: f64 = f64::NAN;
-    fn from_usize(v: usize) -> f64 {
-        v as f64
-    }
-    fn from_u16(v: u16) -> f64 {
-        f64::from(v)
-    }
-    fn is_nan(self) -> bool {
-        self.is_nan()
-    }
-    fn ln(self) -> f64 {
-        self.ln()
-    }
-    fn exp(self) -> f64 {
-        self.exp()
-    }
-}
-
-impl FloatData<f32> for f32 {
-    const ZERO: f32 = 0.0;
-    const ONE: f32 = 1.0;
-    const MIN: f32 = f32::MIN;
-    const MAX: f32 = f32::MAX;
-    const NAN: f32 = f32::NAN;
-    fn from_usize(v: usize) -> f32 {
-        v as f32
-    }
-    fn from_u16(v: u16) -> f32 {
-        f32::from(v)
-    }
-    fn is_nan(self) -> bool {
-        self.is_nan()
-    }
-    fn ln(self) -> f32 {
-        self.ln()
-    }
-    fn exp(self) -> f32 {
-        self.exp()
-    }
-}
-
-/// Contigious Column major matrix data container. This is
-/// used throughout the crate, to house both the user provided data
-/// as well as the binned data.
-pub struct Matrix<'a, T> {
-    pub data: &'a [T],
-    pub index: Vec<usize>,
-    pub rows: usize,
-    pub cols: usize,
-    stride1: usize,
-    stride2: usize,
-}
-
-impl<'a, T> Matrix<'a, T> {
-    // Defaults to column major
-    pub fn new(data: &'a [T], rows: usize, cols: usize) -> Self {
-        Matrix {
-            data,
-            index: (0..rows).collect(),
-            rows,
-            cols,
-            stride1: rows,
-            stride2: 1,
-        }
-    }
-
-    /// Get a single reference to an item in the matrix.
-    ///
-    /// * `i` - The ith row of the data to get.
-    /// * `j` - the jth column of the data to get.
-    pub fn get(&self, i: usize, j: usize) -> &T {
-        &self.data[self.item_index(i, j)]
-    }
-
-    fn item_index(&self, i: usize, j: usize) -> usize {
-        let mut idx = self.stride2 * i;
-        idx += j * self.stride1;
-        idx
-    }
-
-    /// Get access to a row of the data, as an iterator.
-    pub fn get_row_iter(
-        &self,
-        row: usize,
-    ) -> std::iter::StepBy<std::iter::Skip<std::slice::Iter<T>>> {
-        self.data.iter().skip(row).step_by(self.rows)
-    }
-
-    /// Get a slice of a column in the matrix.
-    ///
-    /// * `col` - The index of the column to select.
-    /// * `start_row` - The index of the start of the slice.
-    /// * `end_row` - The index of the end of the slice of the column to select.
-    pub fn get_col_slice(&self, col: usize, start_row: usize, end_row: usize) -> &[T] {
-        let i = self.item_index(start_row, col);
-        let j = self.item_index(end_row, col);
-        &self.data[i..j]
-    }
-
-    /// Get an entire column in the matrix.
-    ///
-    /// * `col` - The index of the column to get.
-    pub fn get_col(&self, col: usize) -> &[T] {
-        self.get_col_slice(col, 0, self.rows)
-    }
-}
-
-impl<'a, T> Matrix<'a, T>
-where
-    T: Copy,
-{
-    /// Get a row of the data as a vector.
-    pub fn get_row(&self, row: usize) -> Vec<T> {
-        self.get_row_iter(row).copied().collect()
-    }
-}
-
-/// A lightweight row major matrix, this is primarily
-/// for returning data to the user, it is especially
-/// suited for appending rows to, such as when building
-/// up a matrix of contributions to return to the
-/// user, the added benefit is it will be even
-/// faster to return to numpy.
-// pub struct RowMajorMatrix<T> {
-//     pub data: Vec<T>,
-//     pub rows: usize,
-//     pub cols: usize,
-//     stride1: usize,
-//     stride2: usize,
-// }
-
-impl<'a, T> fmt::Display for Matrix<'a, T>
-where
-    T: FromStr + std::fmt::Display,
-    <T as FromStr>::Err: 'static + std::error::Error,
-{
-    // This trait requires `fmt` with this exact signature.
-    /// Format a Matrix.
-    fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
-        let mut val = String::new();
-        for i in 0..self.rows {
-            for j in 0..self.cols {
-                val.push_str(self.get(i, j).to_string().as_str());
-                if j == (self.cols - 1) {
-                    val.push('\n');
-                } else {
-                    val.push(' ');
-                }
-            }
-        }
-        write!(f, "{}", val)
-    }
-}
-
-/// A jagged column aligned matrix, that owns it's data contents.
-#[derive(Debug, Deserialize, Serialize)]
-pub struct JaggedMatrix<T> {
-    /// The contents of the matrix.
-    pub data: Vec<T>,
-    /// The end index's of the matrix.
-    pub ends: Vec<usize>,
-    /// Number of columns in the matrix
-    pub cols: usize,
-    /// The number of elements in the matrix.
-    pub n_records: usize,
-}
-
-impl<T> JaggedMatrix<T>
-where
-    T: Copy,
-{
-    /// Generate a jagged array from a vector of vectors
-    pub fn from_vecs(vecs: &[Vec<T>]) -> Self {
-        let mut data = Vec::new();
-        let mut ends = Vec::new();
-        let mut e = 0;
-        let mut n_records = 0;
-        for vec in vecs {
-            for v in vec {
-                data.push(*v);
-            }
-            e += vec.len();
-            ends.push(e);
-            n_records += e;
-        }
-        let cols = vecs.len();
-
-        JaggedMatrix {
-            data,
-            ends,
-            cols,
-            n_records,
-        }
-    }
-}
-
-impl<T> JaggedMatrix<T> {
-    /// Create a new jagged matrix.
-    pub fn new() -> Self {
-        JaggedMatrix {
-            data: Vec::new(),
-            ends: Vec::new(),
-            cols: 0,
-            n_records: 0,
-        }
-    }
-    /// Get the column of a jagged array.
-    pub fn get_col(&self, col: usize) -> &[T] {
-        assert!(col < self.ends.len());
-        let (i, j) = if col == 0 {
-            (0, self.ends[col])
-        } else {
-            (self.ends[col - 1], self.ends[col])
-        };
-        &self.data[i..j]
-    }
-
-    /// Get a mutable reference to a column of the array.
-    pub fn get_col_mut(&mut self, col: usize) -> &mut [T] {
-        assert!(col < self.ends.len());
-        let (i, j) = if col == 0 {
-            (0, self.ends[col])
-        } else {
-            (self.ends[col - 1], self.ends[col])
-        };
-        &mut self.data[i..j]
-    }
-}
-
-impl<T> Default for JaggedMatrix<T> {
-    fn default() -> Self {
-        Self::new()
-    }
-}
-
-#[cfg(test)]
-mod tests {
-    use super::*;
-    #[test]
-    fn test_matrix_get() {
-        let v = vec![1, 2, 3, 5, 6, 7];
-        let m = Matrix::new(&v, 2, 3);
-        println!("{}", m);
-        assert_eq!(m.get(0, 0), &1);
-        assert_eq!(m.get(1, 0), &2);
-    }
-    #[test]
-    fn test_matrix_get_col_slice() {
-        let v = vec![1, 2, 3, 5, 6, 7];
-        let m = Matrix::new(&v, 3, 2);
-        assert_eq!(m.get_col_slice(0, 0, 3), &vec![1, 2, 3]);
-        assert_eq!(m.get_col_slice(1, 0, 2), &vec![5, 6]);
-        assert_eq!(m.get_col_slice(1, 1, 3), &vec![6, 7]);
-        assert_eq!(m.get_col_slice(0, 1, 2), &vec![2]);
-    }
-
-    #[test]
-    fn test_matrix_get_col() {
-        let v = vec![1, 2, 3, 5, 6, 7];
-        let m = Matrix::new(&v, 3, 2);
-        assert_eq!(m.get_col(1), &vec![5, 6, 7]);
-    }
-
-    #[test]
-    fn test_matrix_row() {
-        let v = vec![1, 2, 3, 5, 6, 7];
-        let m = Matrix::new(&v, 3, 2);
-        assert_eq!(m.get_row(2), vec![3, 7]);
-        assert_eq!(m.get_row(0), vec![1, 5]);
-        assert_eq!(m.get_row(1), vec![2, 6]);
-    }
-
-    #[test]
-    fn test_jaggedmatrix_get_col() {
-        let vecs = vec![vec![0], vec![5, 4, 3, 2], vec![4, 5]];
-        let jmatrix = JaggedMatrix::from_vecs(&vecs);
-        assert_eq!(jmatrix.get_col(1), vec![5, 4, 3, 2]);
-        assert_eq!(jmatrix.get_col(0), vec![0]);
-        assert_eq!(jmatrix.get_col(2), vec![4, 5]);
-    }
-}
+use serde::{Deserialize, Serialize};
+use std::fmt::{self, Debug, Display};
+use std::iter::Sum;
+use std::ops::{Add, AddAssign, Div, Mul, Neg, Sub, SubAssign};
+use std::str::FromStr;
+
+/// Data trait used throughout the package
+/// to control for floating point numbers.
+pub trait FloatData<T>:
+    Mul<Output = T>
+    + Display
+    + Add<Output = T>
+    + Div<Output = T>
+    + Neg<Output = T>
+    + Copy
+    + Debug
+    + PartialEq
+    + PartialOrd
+    + AddAssign
+    + Sub<Output = T>
+    + SubAssign
+    + Sum
+    + std::marker::Send
+    + std::marker::Sync
+{
+    const ZERO: T;
+    const ONE: T;
+    const MIN: T;
+    const MAX: T;
+    const NAN: T;
+    fn from_usize(v: usize) -> T;
+    fn from_u16(v: u16) -> T;
+    fn is_nan(self) -> bool;
+    fn ln(self) -> T;
+    fn exp(self) -> T;
+}
+impl FloatData<f64> for f64 {
+    const ZERO: f64 = 0.0;
+    const ONE: f64 = 1.0;
+    const MIN: f64 = f64::MIN;
+    const MAX: f64 = f64::MAX;
+    const NAN: f64 = f64::NAN;
+    fn from_usize(v: usize) -> f64 {
+        v as f64
+    }
+    fn from_u16(v: u16) -> f64 {
+        f64::from(v)
+    }
+    fn is_nan(self) -> bool {
+        self.is_nan()
+    }
+    fn ln(self) -> f64 {
+        self.ln()
+    }
+    fn exp(self) -> f64 {
+        self.exp()
+    }
+}
+
+impl FloatData<f32> for f32 {
+    const ZERO: f32 = 0.0;
+    const ONE: f32 = 1.0;
+    const MIN: f32 = f32::MIN;
+    const MAX: f32 = f32::MAX;
+    const NAN: f32 = f32::NAN;
+    fn from_usize(v: usize) -> f32 {
+        v as f32
+    }
+    fn from_u16(v: u16) -> f32 {
+        f32::from(v)
+    }
+    fn is_nan(self) -> bool {
+        self.is_nan()
+    }
+    fn ln(self) -> f32 {
+        self.ln()
+    }
+    fn exp(self) -> f32 {
+        self.exp()
+    }
+}
+
+/// Contigious Column major matrix data container. This is
+/// used throughout the crate, to house both the user provided data
+/// as well as the binned data.
+pub struct Matrix<'a, T> {
+    pub data: &'a [T],
+    pub index: Vec<usize>,
+    pub rows: usize,
+    pub cols: usize,
+    stride1: usize,
+    stride2: usize,
+}
+
+impl<'a, T> Matrix<'a, T> {
+    // Defaults to column major
+    pub fn new(data: &'a [T], rows: usize, cols: usize) -> Self {
+        Matrix {
+            data,
+            index: (0..rows).collect(),
+            rows,
+            cols,
+            stride1: rows,
+            stride2: 1,
+        }
+    }
+
+    /// Get a single reference to an item in the matrix.
+    ///
+    /// * `i` - The ith row of the data to get.
+    /// * `j` - the jth column of the data to get.
+    pub fn get(&self, i: usize, j: usize) -> &T {
+        &self.data[self.item_index(i, j)]
+    }
+
+    fn item_index(&self, i: usize, j: usize) -> usize {
+        let mut idx = self.stride2 * i;
+        idx += j * self.stride1;
+        idx
+    }
+
+    /// Get access to a row of the data, as an iterator.
+    pub fn get_row_iter(
+        &self,
+        row: usize,
+    ) -> std::iter::StepBy<std::iter::Skip<std::slice::Iter<T>>> {
+        self.data.iter().skip(row).step_by(self.rows)
+    }
+
+    /// Get a slice of a column in the matrix.
+    ///
+    /// * `col` - The index of the column to select.
+    /// * `start_row` - The index of the start of the slice.
+    /// * `end_row` - The index of the end of the slice of the column to select.
+    pub fn get_col_slice(&self, col: usize, start_row: usize, end_row: usize) -> &[T] {
+        let i = self.item_index(start_row, col);
+        let j = self.item_index(end_row, col);
+        &self.data[i..j]
+    }
+
+    /// Get an entire column in the matrix.
+    ///
+    /// * `col` - The index of the column to get.
+    pub fn get_col(&self, col: usize) -> &[T] {
+        self.get_col_slice(col, 0, self.rows)
+    }
+}
+
+impl<'a, T> Matrix<'a, T>
+where
+    T: Copy,
+{
+    /// Get a row of the data as a vector.
+    pub fn get_row(&self, row: usize) -> Vec<T> {
+        self.get_row_iter(row).copied().collect()
+    }
+}
+
+/// A lightweight row major matrix, this is primarily
+/// for returning data to the user, it is especially
+/// suited for appending rows to, such as when building
+/// up a matrix of data to return to the
+/// user, the added benefit is it will be even
+/// faster to return to numpy.
+#[derive(Debug, Serialize, Deserialize)]
+pub struct RowMajorMatrix<T> {
+    pub data: Vec<T>,
+    pub rows: usize,
+    pub cols: usize,
+    stride1: usize,
+    stride2: usize,
+}
+
+impl<T> RowMajorMatrix<T> {
+    // Defaults to column major
+    pub fn new(data: Vec<T>, rows: usize, cols: usize) -> Self {
+        RowMajorMatrix {
+            data,
+            rows,
+            cols,
+            stride1: 1,
+            stride2: cols,
+        }
+    }
+
+    /// Get a single reference to an item in the matrix.
+    ///
+    /// * `i` - The ith row of the data to get.
+    /// * `j` - the jth column of the data to get.
+    pub fn get(&self, i: usize, j: usize) -> &T {
+        &self.data[self.item_index(i, j)]
+    }
+
+    fn item_index(&self, i: usize, j: usize) -> usize {
+        let mut idx = self.stride2 * i;
+        idx += j * self.stride1;
+        idx
+    }
+
+    /// Add a rows to the matrix, this can be multiple
+    /// rows, if they are in sequential order in the items.
+    pub fn append_row(&mut self, items: Vec<T>) {
+        assert!(items.len() % self.cols == 0);
+        let new_rows = items.len() / self.cols;
+        self.rows += new_rows;
+        self.data.extend(items);
+    }
+}
+
+impl<'a, T> fmt::Display for Matrix<'a, T>
+where
+    T: FromStr + std::fmt::Display,
+    <T as FromStr>::Err: 'static + std::error::Error,
+{
+    // This trait requires `fmt` with this exact signature.
+    /// Format a Matrix.
+    fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
+        let mut val = String::new();
+        for i in 0..self.rows {
+            for j in 0..self.cols {
+                val.push_str(self.get(i, j).to_string().as_str());
+                if j == (self.cols - 1) {
+                    val.push('\n');
+                } else {
+                    val.push(' ');
+                }
+            }
+        }
+        write!(f, "{}", val)
+    }
+}
+
+/// A jagged column aligned matrix, that owns it's data contents.
+#[derive(Debug, Deserialize, Serialize)]
+pub struct JaggedMatrix<T> {
+    /// The contents of the matrix.
+    pub data: Vec<T>,
+    /// The end index's of the matrix.
+    pub ends: Vec<usize>,
+    /// Number of columns in the matrix
+    pub cols: usize,
+    /// The number of elements in the matrix.
+    pub n_records: usize,
+}
+
+impl<T> JaggedMatrix<T>
+where
+    T: Copy,
+{
+    /// Generate a jagged array from a vector of vectors
+    pub fn from_vecs(vecs: &[Vec<T>]) -> Self {
+        let mut data = Vec::new();
+        let mut ends = Vec::new();
+        let mut e = 0;
+        let mut n_records = 0;
+        for vec in vecs {
+            for v in vec {
+                data.push(*v);
+            }
+            e += vec.len();
+            ends.push(e);
+            n_records += e;
+        }
+        let cols = vecs.len();
+
+        JaggedMatrix {
+            data,
+            ends,
+            cols,
+            n_records,
+        }
+    }
+}
+
+impl<T> JaggedMatrix<T> {
+    /// Create a new jagged matrix.
+    pub fn new() -> Self {
+        JaggedMatrix {
+            data: Vec::new(),
+            ends: Vec::new(),
+            cols: 0,
+            n_records: 0,
+        }
+    }
+    /// Get the column of a jagged array.
+    pub fn get_col(&self, col: usize) -> &[T] {
+        assert!(col < self.ends.len());
+        let (i, j) = if col == 0 {
+            (0, self.ends[col])
+        } else {
+            (self.ends[col - 1], self.ends[col])
+        };
+        &self.data[i..j]
+    }
+
+    /// Get a mutable reference to a column of the array.
+    pub fn get_col_mut(&mut self, col: usize) -> &mut [T] {
+        assert!(col < self.ends.len());
+        let (i, j) = if col == 0 {
+            (0, self.ends[col])
+        } else {
+            (self.ends[col - 1], self.ends[col])
+        };
+        &mut self.data[i..j]
+    }
+}
+
+impl<T> Default for JaggedMatrix<T> {
+    fn default() -> Self {
+        Self::new()
+    }
+}
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+
+    #[test]
+    fn test_rowmatrix_get() {
+        let v = vec![1, 2, 3, 5, 6, 7];
+        let m = RowMajorMatrix::new(v, 2, 3);
+        println!("{:?}", m);
+        assert_eq!(m.get(0, 0), &1);
+        assert_eq!(m.get(1, 0), &5);
+        assert_eq!(m.get(0, 2), &3);
+        assert_eq!(m.get(1, 1), &6);
+    }
+
+    #[test]
+    fn test_rowmatrix_append() {
+        let v = vec![1, 2, 3, 5, 6, 7];
+        let mut m = RowMajorMatrix::new(v, 2, 3);
+        m.append_row(vec![-1, -2, -3]);
+        assert_eq!(m.get(2, 1), &-2);
+    }
+
+    #[test]
+    fn test_matrix_get() {
+        let v = vec![1, 2, 3, 5, 6, 7];
+        let m = Matrix::new(&v, 2, 3);
+        println!("{}", m);
+        assert_eq!(m.get(0, 0), &1);
+        assert_eq!(m.get(1, 0), &2);
+    }
+    #[test]
+    fn test_matrix_get_col_slice() {
+        let v = vec![1, 2, 3, 5, 6, 7];
+        let m = Matrix::new(&v, 3, 2);
+        assert_eq!(m.get_col_slice(0, 0, 3), &vec![1, 2, 3]);
+        assert_eq!(m.get_col_slice(1, 0, 2), &vec![5, 6]);
+        assert_eq!(m.get_col_slice(1, 1, 3), &vec![6, 7]);
+        assert_eq!(m.get_col_slice(0, 1, 2), &vec![2]);
+    }
+
+    #[test]
+    fn test_matrix_get_col() {
+        let v = vec![1, 2, 3, 5, 6, 7];
+        let m = Matrix::new(&v, 3, 2);
+        assert_eq!(m.get_col(1), &vec![5, 6, 7]);
+    }
+
+    #[test]
+    fn test_matrix_row() {
+        let v = vec![1, 2, 3, 5, 6, 7];
+        let m = Matrix::new(&v, 3, 2);
+        assert_eq!(m.get_row(2), vec![3, 7]);
+        assert_eq!(m.get_row(0), vec![1, 5]);
+        assert_eq!(m.get_row(1), vec![2, 6]);
+    }
+
+    #[test]
+    fn test_jaggedmatrix_get_col() {
+        let vecs = vec![vec![0], vec![5, 4, 3, 2], vec![4, 5]];
+        let jmatrix = JaggedMatrix::from_vecs(&vecs);
+        assert_eq!(jmatrix.get_col(1), vec![5, 4, 3, 2]);
+        assert_eq!(jmatrix.get_col(0), vec![0]);
+        assert_eq!(jmatrix.get_col(2), vec![4, 5]);
+    }
+}
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/src/errors.rs` & `forust-0.2.7/local_dependencies/forust-ml/src/errors.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-use thiserror::Error;
-
-#[derive(Debug, Error)]
-pub enum ForustError {
-    #[error("Feature number {0} has no variance, when missing values are excluded.")]
-    NoVariance(usize),
-    #[error("Unable to write model to file: {0}")]
-    UnableToWrite(String),
-    #[error("Unable to read model from a file {0}")]
-    UnableToRead(String),
-    #[error("The value {0} is set to missing, but a NaN value was found in the data.")]
-    NANVAlueFound(f64),
-    // #[error("NaN found in {0}.")]
-    // ContainsNaN(String),
-    // #[error("Unable to calculate prediction.")]
-    // Prediction,
-}
+use thiserror::Error;
+
+#[derive(Debug, Error)]
+pub enum ForustError {
+    #[error("Feature number {0} has no variance, when missing values are excluded.")]
+    NoVariance(usize),
+    #[error("Unable to write model to file: {0}")]
+    UnableToWrite(String),
+    #[error("Unable to read model from a file {0}")]
+    UnableToRead(String),
+    #[error("The value {0} is set to missing, but a NaN value was found in the data.")]
+    NANVAlueFound(f64),
+    #[error("Invalid value {0} passed for {1}, expected one of {2}.")]
+    ParseString(String, String, String),
+}
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/src/histogram.rs` & `forust-0.2.7/local_dependencies/forust-ml/src/histogram.rs`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,264 +1,264 @@
-use crate::data::{FloatData, JaggedMatrix, Matrix};
-use rayon::prelude::*;
-use serde::{Deserialize, Serialize};
-
-/// Struct to hold the information of a given bin.
-#[derive(Debug, Deserialize, Serialize, Clone)]
-pub struct Bin<T> {
-    /// The sum of the gradient for this bin.
-    pub gradient_sum: T,
-    /// The sum of the hession values for this bin.
-    pub hessian_sum: T,
-    /// The value used to split at, this is for deciding
-    /// the split value for non-binned values.
-    /// This value will be missing for the missing bin.
-    pub cut_value: f64,
-}
-
-impl Bin<f32> {
-    pub fn new_f32(cut_value: f64) -> Self {
-        Bin {
-            gradient_sum: f32::ZERO,
-            hessian_sum: f32::ZERO,
-            cut_value,
-        }
-    }
-
-    /// Calculate a new bin, using the subtraction trick on the parent bin,
-    /// and the child bin.
-    pub fn from_parent_child(root_bin: &Bin<f32>, child_bin: &Bin<f32>) -> Self {
-        Bin {
-            gradient_sum: root_bin.gradient_sum - child_bin.gradient_sum,
-            hessian_sum: root_bin.hessian_sum - child_bin.hessian_sum,
-            cut_value: root_bin.cut_value,
-        }
-    }
-
-    /// Calculate a new bin, using the subtraction trick when the parent node
-    /// has three directions, left, right, and missing.
-    pub fn from_parent_two_children(
-        root_bin: &Bin<f32>,
-        first_child_bin: &Bin<f32>,
-        second_child_bin: &Bin<f32>,
-    ) -> Self {
-        Bin {
-            gradient_sum: root_bin.gradient_sum
-                - (first_child_bin.gradient_sum + second_child_bin.gradient_sum),
-            hessian_sum: root_bin.hessian_sum
-                - (first_child_bin.hessian_sum + second_child_bin.hessian_sum),
-            cut_value: root_bin.cut_value,
-        }
-    }
-}
-
-impl Bin<f64> {
-    pub fn new_f64(cut_value: f64) -> Self {
-        Bin {
-            gradient_sum: f64::ZERO,
-            hessian_sum: f64::ZERO,
-            cut_value,
-        }
-    }
-
-    pub fn as_f32_bin(&self) -> Bin<f32> {
-        Bin {
-            gradient_sum: self.gradient_sum as f32,
-            hessian_sum: self.hessian_sum as f32,
-            cut_value: self.cut_value,
-        }
-    }
-}
-
-/// Histograms implemented as as jagged matrix.
-#[derive(Debug, Deserialize, Serialize)]
-pub struct HistogramMatrix(pub JaggedMatrix<Bin<f32>>);
-
-/// Create a histogram for a given feature, we use f64
-/// values to accumulate, so that we don't lose precision,
-/// but then still return f32 values for memory efficiency
-/// and speed.
-pub fn create_feature_histogram(
-    feature: &[u16],
-    cuts: &[f64],
-    sorted_grad: &[f32],
-    sorted_hess: &[f32],
-    index: &[usize],
-) -> Vec<Bin<f32>> {
-    let mut histogram: Vec<Bin<f64>> = Vec::with_capacity(cuts.len());
-    // The first value is missing, it seems to not matter that we are using
-    // Missing here, rather than the booster "missing" definition, because
-    // we just always assume the first bin of the histogram is missing.
-    histogram.push(Bin::new_f64(f64::NAN));
-    // The last cut value is simply the maximum possible value, so we don't need it.
-    // This value is needed initially for binning, but we don't need to count it as
-    // a histogram bin.
-    histogram.extend(cuts[..(cuts.len() - 1)].iter().map(|c| Bin::new_f64(*c)));
-    index
-        .iter()
-        .zip(sorted_grad)
-        .zip(sorted_hess)
-        .for_each(|((i, g), h)| {
-            if let Some(v) = histogram.get_mut(feature[*i] as usize) {
-                v.gradient_sum += f64::from(*g);
-                v.hessian_sum += f64::from(*h);
-            }
-        });
-    histogram.iter().map(|b| b.as_f32_bin()).collect()
-}
-
-impl HistogramMatrix {
-    /// Create an empty histogram matrix.
-    pub fn empty() -> Self {
-        HistogramMatrix(JaggedMatrix {
-            data: Vec::new(),
-            ends: Vec::new(),
-            cols: 0,
-            n_records: 0,
-        })
-    }
-    pub fn new(
-        data: &Matrix<u16>,
-        cuts: &JaggedMatrix<f64>,
-        grad: &[f32],
-        hess: &[f32],
-        index: &[usize],
-        parallel: bool,
-        sort: bool,
-    ) -> Self {
-        let col_index: Vec<usize> = (0..data.cols).collect();
-        // Sort gradients and hessians to reduce cache hits.
-        // This made a really sizeable difference on larger datasets
-        // Bringing training time down from nearly 6 minutes, to 2 minutes.
-        // Sort gradients and hessians to reduce cache hits.
-        // This made a really sizeable difference on larger datasets
-        // Bringing training time down from nearly 6 minutes, to 2 minutes.
-        let (sorted_grad, sorted_hess) = if !sort {
-            (grad.to_vec(), hess.to_vec())
-        } else {
-            let mut n_grad = Vec::new();
-            let mut n_hess = Vec::new();
-            for i in index {
-                let i_ = *i;
-                n_grad.push(grad[i_]);
-                n_hess.push(hess[i_]);
-            }
-            (n_grad, n_hess)
-        };
-
-        let histograms = if parallel {
-            col_index
-                .par_iter()
-                .flat_map(|col| {
-                    create_feature_histogram(
-                        data.get_col(*col),
-                        cuts.get_col(*col),
-                        &sorted_grad,
-                        &sorted_hess,
-                        index,
-                    )
-                })
-                .collect::<Vec<Bin<f32>>>()
-        } else {
-            col_index
-                .iter()
-                .flat_map(|col| {
-                    create_feature_histogram(
-                        data.get_col(*col),
-                        cuts.get_col(*col),
-                        &sorted_grad,
-                        &sorted_hess,
-                        index,
-                    )
-                })
-                .collect::<Vec<Bin<f32>>>()
-        };
-        HistogramMatrix(JaggedMatrix {
-            data: histograms,
-            ends: cuts.ends.to_owned(),
-            cols: cuts.cols,
-            n_records: cuts.n_records,
-        })
-    }
-
-    /// Calculate the histogram matrix, for a child, given the parent histogram
-    /// matrix, and the other child histogram matrix. This should be used
-    /// when the node has only two possible splits, left and right.
-    pub fn from_parent_child(
-        root_histogram: &HistogramMatrix,
-        child_histogram: &HistogramMatrix,
-    ) -> Self {
-        let HistogramMatrix(root) = root_histogram;
-        let HistogramMatrix(child) = child_histogram;
-        let histograms = root
-            .data
-            .iter()
-            .zip(child.data.iter())
-            .map(|(root_bin, child_bin)| Bin::from_parent_child(root_bin, child_bin))
-            .collect();
-        HistogramMatrix(JaggedMatrix {
-            data: histograms,
-            ends: child.ends.to_owned(),
-            cols: child.cols,
-            n_records: child.n_records,
-        })
-    }
-
-    /// Calculate the histogram matrix for a child, given the parent histogram
-    /// and two other child histograms. This should be used with the node has
-    /// three possible split paths, right, left, and missing.
-    pub fn from_parent_two_children(
-        root_histogram: &HistogramMatrix,
-        first_child_histogram: &HistogramMatrix,
-        second_child_histogram: &HistogramMatrix,
-    ) -> Self {
-        let HistogramMatrix(root) = root_histogram;
-        let HistogramMatrix(first_child) = first_child_histogram;
-        let HistogramMatrix(second_child) = second_child_histogram;
-        let histograms = root
-            .data
-            .iter()
-            .zip(first_child.data.iter())
-            .zip(second_child.data.iter())
-            .map(|((root_bin, first_child_bin), second_child_bin)| {
-                Bin::from_parent_two_children(root_bin, first_child_bin, second_child_bin)
-            })
-            .collect();
-        HistogramMatrix(JaggedMatrix {
-            data: histograms,
-            ends: first_child.ends.to_owned(),
-            cols: first_child.cols,
-            n_records: first_child.n_records,
-        })
-    }
-}
-
-#[cfg(test)]
-mod tests {
-    use super::*;
-    use crate::binning::bin_matrix;
-    use crate::objective::{LogLoss, ObjectiveFunction};
-    use std::fs;
-    #[test]
-    fn test_single_histogram() {
-        let file = fs::read_to_string("resources/contiguous_no_missing.csv")
-            .expect("Something went wrong reading the file");
-        let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
-        let data = Matrix::new(&data_vec, 891, 5);
-        let sample_weight = vec![1.; data.rows];
-        let b = bin_matrix(&data, &sample_weight, 10, f64::NAN).unwrap();
-        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
-        let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
-        let yhat = vec![0.5; y.len()];
-        let w = vec![1.; y.len()];
-        let g = LogLoss::calc_grad(&y, &yhat, &w);
-        let h = LogLoss::calc_hess(&y, &yhat, &w);
-        let hist =
-            create_feature_histogram(&bdata.get_col(1), &b.cuts.get_col(1), &g, &h, &bdata.index);
-        // println!("{:?}", hist);
-        let mut f = bdata.get_col(1).to_owned();
-        println!("{:?}", hist);
-        f.sort();
-        f.dedup();
-        assert_eq!(f.len() + 1, hist.len());
-    }
-}
+use crate::data::{FloatData, JaggedMatrix, Matrix};
+use rayon::prelude::*;
+use serde::{Deserialize, Serialize};
+
+/// Struct to hold the information of a given bin.
+#[derive(Debug, Deserialize, Serialize, Clone)]
+pub struct Bin<T> {
+    /// The sum of the gradient for this bin.
+    pub gradient_sum: T,
+    /// The sum of the hession values for this bin.
+    pub hessian_sum: T,
+    /// The value used to split at, this is for deciding
+    /// the split value for non-binned values.
+    /// This value will be missing for the missing bin.
+    pub cut_value: f64,
+}
+
+impl Bin<f32> {
+    pub fn new_f32(cut_value: f64) -> Self {
+        Bin {
+            gradient_sum: f32::ZERO,
+            hessian_sum: f32::ZERO,
+            cut_value,
+        }
+    }
+
+    /// Calculate a new bin, using the subtraction trick on the parent bin,
+    /// and the child bin.
+    pub fn from_parent_child(root_bin: &Bin<f32>, child_bin: &Bin<f32>) -> Self {
+        Bin {
+            gradient_sum: root_bin.gradient_sum - child_bin.gradient_sum,
+            hessian_sum: root_bin.hessian_sum - child_bin.hessian_sum,
+            cut_value: root_bin.cut_value,
+        }
+    }
+
+    /// Calculate a new bin, using the subtraction trick when the parent node
+    /// has three directions, left, right, and missing.
+    pub fn from_parent_two_children(
+        root_bin: &Bin<f32>,
+        first_child_bin: &Bin<f32>,
+        second_child_bin: &Bin<f32>,
+    ) -> Self {
+        Bin {
+            gradient_sum: root_bin.gradient_sum
+                - (first_child_bin.gradient_sum + second_child_bin.gradient_sum),
+            hessian_sum: root_bin.hessian_sum
+                - (first_child_bin.hessian_sum + second_child_bin.hessian_sum),
+            cut_value: root_bin.cut_value,
+        }
+    }
+}
+
+impl Bin<f64> {
+    pub fn new_f64(cut_value: f64) -> Self {
+        Bin {
+            gradient_sum: f64::ZERO,
+            hessian_sum: f64::ZERO,
+            cut_value,
+        }
+    }
+
+    pub fn as_f32_bin(&self) -> Bin<f32> {
+        Bin {
+            gradient_sum: self.gradient_sum as f32,
+            hessian_sum: self.hessian_sum as f32,
+            cut_value: self.cut_value,
+        }
+    }
+}
+
+/// Histograms implemented as as jagged matrix.
+#[derive(Debug, Deserialize, Serialize)]
+pub struct HistogramMatrix(pub JaggedMatrix<Bin<f32>>);
+
+/// Create a histogram for a given feature, we use f64
+/// values to accumulate, so that we don't lose precision,
+/// but then still return f32 values for memory efficiency
+/// and speed.
+pub fn create_feature_histogram(
+    feature: &[u16],
+    cuts: &[f64],
+    sorted_grad: &[f32],
+    sorted_hess: &[f32],
+    index: &[usize],
+) -> Vec<Bin<f32>> {
+    let mut histogram: Vec<Bin<f64>> = Vec::with_capacity(cuts.len());
+    // The first value is missing, it seems to not matter that we are using
+    // Missing here, rather than the booster "missing" definition, because
+    // we just always assume the first bin of the histogram is missing.
+    histogram.push(Bin::new_f64(f64::NAN));
+    // The last cut value is simply the maximum possible value, so we don't need it.
+    // This value is needed initially for binning, but we don't need to count it as
+    // a histogram bin.
+    histogram.extend(cuts[..(cuts.len() - 1)].iter().map(|c| Bin::new_f64(*c)));
+    index
+        .iter()
+        .zip(sorted_grad)
+        .zip(sorted_hess)
+        .for_each(|((i, g), h)| {
+            if let Some(v) = histogram.get_mut(feature[*i] as usize) {
+                v.gradient_sum += f64::from(*g);
+                v.hessian_sum += f64::from(*h);
+            }
+        });
+    histogram.iter().map(|b| b.as_f32_bin()).collect()
+}
+
+impl HistogramMatrix {
+    /// Create an empty histogram matrix.
+    pub fn empty() -> Self {
+        HistogramMatrix(JaggedMatrix {
+            data: Vec::new(),
+            ends: Vec::new(),
+            cols: 0,
+            n_records: 0,
+        })
+    }
+    pub fn new(
+        data: &Matrix<u16>,
+        cuts: &JaggedMatrix<f64>,
+        grad: &[f32],
+        hess: &[f32],
+        index: &[usize],
+        parallel: bool,
+        sort: bool,
+    ) -> Self {
+        let col_index: Vec<usize> = (0..data.cols).collect();
+        // Sort gradients and hessians to reduce cache hits.
+        // This made a really sizeable difference on larger datasets
+        // Bringing training time down from nearly 6 minutes, to 2 minutes.
+        // Sort gradients and hessians to reduce cache hits.
+        // This made a really sizeable difference on larger datasets
+        // Bringing training time down from nearly 6 minutes, to 2 minutes.
+        let (sorted_grad, sorted_hess) = if !sort {
+            (grad.to_vec(), hess.to_vec())
+        } else {
+            let mut n_grad = Vec::new();
+            let mut n_hess = Vec::new();
+            for i in index {
+                let i_ = *i;
+                n_grad.push(grad[i_]);
+                n_hess.push(hess[i_]);
+            }
+            (n_grad, n_hess)
+        };
+
+        let histograms = if parallel {
+            col_index
+                .par_iter()
+                .flat_map(|col| {
+                    create_feature_histogram(
+                        data.get_col(*col),
+                        cuts.get_col(*col),
+                        &sorted_grad,
+                        &sorted_hess,
+                        index,
+                    )
+                })
+                .collect::<Vec<Bin<f32>>>()
+        } else {
+            col_index
+                .iter()
+                .flat_map(|col| {
+                    create_feature_histogram(
+                        data.get_col(*col),
+                        cuts.get_col(*col),
+                        &sorted_grad,
+                        &sorted_hess,
+                        index,
+                    )
+                })
+                .collect::<Vec<Bin<f32>>>()
+        };
+        HistogramMatrix(JaggedMatrix {
+            data: histograms,
+            ends: cuts.ends.to_owned(),
+            cols: cuts.cols,
+            n_records: cuts.n_records,
+        })
+    }
+
+    /// Calculate the histogram matrix, for a child, given the parent histogram
+    /// matrix, and the other child histogram matrix. This should be used
+    /// when the node has only two possible splits, left and right.
+    pub fn from_parent_child(
+        root_histogram: &HistogramMatrix,
+        child_histogram: &HistogramMatrix,
+    ) -> Self {
+        let HistogramMatrix(root) = root_histogram;
+        let HistogramMatrix(child) = child_histogram;
+        let histograms = root
+            .data
+            .iter()
+            .zip(child.data.iter())
+            .map(|(root_bin, child_bin)| Bin::from_parent_child(root_bin, child_bin))
+            .collect();
+        HistogramMatrix(JaggedMatrix {
+            data: histograms,
+            ends: child.ends.to_owned(),
+            cols: child.cols,
+            n_records: child.n_records,
+        })
+    }
+
+    /// Calculate the histogram matrix for a child, given the parent histogram
+    /// and two other child histograms. This should be used with the node has
+    /// three possible split paths, right, left, and missing.
+    pub fn from_parent_two_children(
+        root_histogram: &HistogramMatrix,
+        first_child_histogram: &HistogramMatrix,
+        second_child_histogram: &HistogramMatrix,
+    ) -> Self {
+        let HistogramMatrix(root) = root_histogram;
+        let HistogramMatrix(first_child) = first_child_histogram;
+        let HistogramMatrix(second_child) = second_child_histogram;
+        let histograms = root
+            .data
+            .iter()
+            .zip(first_child.data.iter())
+            .zip(second_child.data.iter())
+            .map(|((root_bin, first_child_bin), second_child_bin)| {
+                Bin::from_parent_two_children(root_bin, first_child_bin, second_child_bin)
+            })
+            .collect();
+        HistogramMatrix(JaggedMatrix {
+            data: histograms,
+            ends: first_child.ends.to_owned(),
+            cols: first_child.cols,
+            n_records: first_child.n_records,
+        })
+    }
+}
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+    use crate::binning::bin_matrix;
+    use crate::objective::{LogLoss, ObjectiveFunction};
+    use std::fs;
+    #[test]
+    fn test_single_histogram() {
+        let file = fs::read_to_string("resources/contiguous_no_missing.csv")
+            .expect("Something went wrong reading the file");
+        let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+        let data = Matrix::new(&data_vec, 891, 5);
+        let sample_weight = vec![1.; data.rows];
+        let b = bin_matrix(&data, &sample_weight, 10, f64::NAN).unwrap();
+        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
+        let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+        let yhat = vec![0.5; y.len()];
+        let w = vec![1.; y.len()];
+        let g = LogLoss::calc_grad(&y, &yhat, &w);
+        let h = LogLoss::calc_hess(&y, &yhat, &w);
+        let hist =
+            create_feature_histogram(&bdata.get_col(1), &b.cuts.get_col(1), &g, &h, &bdata.index);
+        // println!("{:?}", hist);
+        let mut f = bdata.get_col(1).to_owned();
+        println!("{:?}", hist);
+        f.sort();
+        f.dedup();
+        assert_eq!(f.len() + 1, hist.len());
+    }
+}
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/src/node.rs` & `forust-0.2.7/local_dependencies/forust-ml/src/node.rs`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-use crate::data::FloatData;
-use crate::histogram::HistogramMatrix;
-use crate::splitter::{MissingInfo, NodeInfo, SplitInfo};
-use crate::utils::is_missing;
-use serde::{Deserialize, Serialize};
-use std::fmt::{self, Debug};
-
-#[derive(Debug, Deserialize, Serialize)]
-pub struct SplittableNode {
-    pub num: usize,
-    pub histograms: HistogramMatrix,
-    pub weight_value: f32,
-    pub gain_value: f32,
-    pub gradient_sum: f32,
-    pub hessian_sum: f32,
-    pub depth: usize,
-    pub split_value: f64,
-    pub split_feature: usize,
-    pub split_gain: f32,
-    pub missing_node: usize,
-    pub left_child: usize,
-    pub right_child: usize,
-    pub start_idx: usize,
-    pub stop_idx: usize,
-    pub lower_bound: f32,
-    pub upper_bound: f32,
-    pub is_leaf: bool,
-    pub is_missing_leaf: bool,
-}
-
-#[derive(Deserialize, Serialize)]
-pub struct Node {
-    pub num: usize,
-    pub weight_value: f32,
-    pub hessian_sum: f32,
-    pub depth: usize,
-    pub split_value: f64,
-    pub split_feature: usize,
-    pub split_gain: f32,
-    pub missing_node: usize,
-    pub left_child: usize,
-    pub right_child: usize,
-    pub is_leaf: bool,
-}
-
-impl Node {
-    /// Update all the info that is needed if this node is a
-    /// parent node, this consumes the SplitableNode.
-    pub fn make_parent_node(&mut self, split_node: SplittableNode) {
-        self.is_leaf = false;
-        self.missing_node = split_node.missing_node;
-        self.split_value = split_node.split_value;
-        self.split_feature = split_node.split_feature;
-        self.split_gain = split_node.split_gain;
-        self.left_child = split_node.left_child;
-        self.right_child = split_node.right_child;
-    }
-    /// Get the path that should be traveled down, given a value.
-    pub fn get_child_idx(&self, v: &f64, missing: &f64) -> usize {
-        if is_missing(v, missing) {
-            self.missing_node
-        } else if v < &self.split_value {
-            self.left_child
-        } else {
-            //  if v >= &self.split_value
-            self.right_child
-        }
-    }
-
-    pub fn has_missing_branch(&self) -> bool {
-        (self.missing_node != self.right_child) && (self.missing_node != self.left_child)
-    }
-}
-
-impl SplittableNode {
-    pub fn from_node_info(
-        num: usize,
-        histograms: HistogramMatrix,
-        depth: usize,
-        start_idx: usize,
-        stop_idx: usize,
-        node_info: NodeInfo,
-    ) -> Self {
-        SplittableNode {
-            num,
-            histograms,
-            weight_value: node_info.weight,
-            gain_value: node_info.gain,
-            gradient_sum: node_info.grad,
-            hessian_sum: node_info.cover,
-            depth,
-            split_value: f64::ZERO,
-            split_feature: 0,
-            split_gain: f32::ZERO,
-            missing_node: 0,
-            left_child: 0,
-            right_child: 0,
-            start_idx,
-            stop_idx,
-            lower_bound: node_info.bounds.0,
-            upper_bound: node_info.bounds.1,
-            is_leaf: true,
-            is_missing_leaf: false,
-        }
-    }
-
-    /// Create a default splitable node,
-    /// we default to the node being a leaf.
-    #[allow(clippy::too_many_arguments)]
-    pub fn new(
-        num: usize,
-        histograms: HistogramMatrix,
-        weight_value: f32,
-        gain_value: f32,
-        gradient_sum: f32,
-        hessian_sum: f32,
-        depth: usize,
-        start_idx: usize,
-        stop_idx: usize,
-        lower_bound: f32,
-        upper_bound: f32,
-    ) -> Self {
-        SplittableNode {
-            num,
-            histograms,
-            weight_value,
-            gain_value,
-            gradient_sum,
-            hessian_sum,
-            depth,
-            split_value: f64::ZERO,
-            split_feature: 0,
-            split_gain: f32::ZERO,
-            missing_node: 0,
-            left_child: 0,
-            right_child: 0,
-            start_idx,
-            stop_idx,
-            lower_bound,
-            upper_bound,
-            is_leaf: true,
-            is_missing_leaf: false,
-        }
-    }
-
-    pub fn update_children(
-        &mut self,
-        missing_child: usize,
-        left_child: usize,
-        right_child: usize,
-        split_info: &SplitInfo,
-    ) {
-        self.left_child = left_child;
-        self.right_child = right_child;
-        self.split_feature = split_info.split_feature;
-        let missing_split_gain = match &split_info.missing_node {
-            MissingInfo::Branch(ni) => ni.gain,
-            _ => 0.,
-        };
-        self.split_gain =
-            split_info.left_node.gain + split_info.right_node.gain + missing_split_gain
-                - self.gain_value;
-        self.split_value = split_info.split_value;
-        self.missing_node = missing_child;
-        self.is_leaf = false;
-    }
-    pub fn as_node(&self) -> Node {
-        Node {
-            num: self.num,
-            weight_value: self.weight_value,
-            hessian_sum: self.hessian_sum,
-            depth: self.depth,
-            missing_node: self.missing_node,
-            split_value: self.split_value,
-            split_feature: self.split_feature,
-            split_gain: self.split_gain,
-            left_child: self.left_child,
-            right_child: self.right_child,
-            is_leaf: self.is_leaf,
-        }
-    }
-}
-
-impl fmt::Display for Node {
-    // This trait requires `fmt` with this exact signature.
-    fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
-        if self.is_leaf {
-            write!(
-                f,
-                "{}:leaf={},cover={}",
-                self.num, self.weight_value, self.hessian_sum
-            )
-        } else {
-            write!(
-                f,
-                "{}:[{} < {}] yes={},no={},missing={},gain={},cover={}",
-                self.num,
-                self.split_feature,
-                self.split_value,
-                self.left_child,
-                self.right_child,
-                self.missing_node,
-                self.split_gain,
-                self.hessian_sum
-            )
-        }
-    }
-}
+use crate::data::FloatData;
+use crate::histogram::HistogramMatrix;
+use crate::splitter::{MissingInfo, NodeInfo, SplitInfo};
+use crate::utils::is_missing;
+use serde::{Deserialize, Serialize};
+use std::fmt::{self, Debug};
+
+#[derive(Debug, Deserialize, Serialize)]
+pub struct SplittableNode {
+    pub num: usize,
+    pub histograms: HistogramMatrix,
+    pub weight_value: f32,
+    pub gain_value: f32,
+    pub gradient_sum: f32,
+    pub hessian_sum: f32,
+    pub depth: usize,
+    pub split_value: f64,
+    pub split_feature: usize,
+    pub split_gain: f32,
+    pub missing_node: usize,
+    pub left_child: usize,
+    pub right_child: usize,
+    pub start_idx: usize,
+    pub stop_idx: usize,
+    pub lower_bound: f32,
+    pub upper_bound: f32,
+    pub is_leaf: bool,
+    pub is_missing_leaf: bool,
+}
+
+#[derive(Deserialize, Serialize)]
+pub struct Node {
+    pub num: usize,
+    pub weight_value: f32,
+    pub hessian_sum: f32,
+    pub depth: usize,
+    pub split_value: f64,
+    pub split_feature: usize,
+    pub split_gain: f32,
+    pub missing_node: usize,
+    pub left_child: usize,
+    pub right_child: usize,
+    pub is_leaf: bool,
+}
+
+impl Node {
+    /// Update all the info that is needed if this node is a
+    /// parent node, this consumes the SplitableNode.
+    pub fn make_parent_node(&mut self, split_node: SplittableNode) {
+        self.is_leaf = false;
+        self.missing_node = split_node.missing_node;
+        self.split_value = split_node.split_value;
+        self.split_feature = split_node.split_feature;
+        self.split_gain = split_node.split_gain;
+        self.left_child = split_node.left_child;
+        self.right_child = split_node.right_child;
+    }
+    /// Get the path that should be traveled down, given a value.
+    pub fn get_child_idx(&self, v: &f64, missing: &f64) -> usize {
+        if is_missing(v, missing) {
+            self.missing_node
+        } else if v < &self.split_value {
+            self.left_child
+        } else {
+            //  if v >= &self.split_value
+            self.right_child
+        }
+    }
+
+    pub fn has_missing_branch(&self) -> bool {
+        (self.missing_node != self.right_child) && (self.missing_node != self.left_child)
+    }
+}
+
+impl SplittableNode {
+    pub fn from_node_info(
+        num: usize,
+        histograms: HistogramMatrix,
+        depth: usize,
+        start_idx: usize,
+        stop_idx: usize,
+        node_info: NodeInfo,
+    ) -> Self {
+        SplittableNode {
+            num,
+            histograms,
+            weight_value: node_info.weight,
+            gain_value: node_info.gain,
+            gradient_sum: node_info.grad,
+            hessian_sum: node_info.cover,
+            depth,
+            split_value: f64::ZERO,
+            split_feature: 0,
+            split_gain: f32::ZERO,
+            missing_node: 0,
+            left_child: 0,
+            right_child: 0,
+            start_idx,
+            stop_idx,
+            lower_bound: node_info.bounds.0,
+            upper_bound: node_info.bounds.1,
+            is_leaf: true,
+            is_missing_leaf: false,
+        }
+    }
+
+    /// Create a default splitable node,
+    /// we default to the node being a leaf.
+    #[allow(clippy::too_many_arguments)]
+    pub fn new(
+        num: usize,
+        histograms: HistogramMatrix,
+        weight_value: f32,
+        gain_value: f32,
+        gradient_sum: f32,
+        hessian_sum: f32,
+        depth: usize,
+        start_idx: usize,
+        stop_idx: usize,
+        lower_bound: f32,
+        upper_bound: f32,
+    ) -> Self {
+        SplittableNode {
+            num,
+            histograms,
+            weight_value,
+            gain_value,
+            gradient_sum,
+            hessian_sum,
+            depth,
+            split_value: f64::ZERO,
+            split_feature: 0,
+            split_gain: f32::ZERO,
+            missing_node: 0,
+            left_child: 0,
+            right_child: 0,
+            start_idx,
+            stop_idx,
+            lower_bound,
+            upper_bound,
+            is_leaf: true,
+            is_missing_leaf: false,
+        }
+    }
+
+    pub fn update_children(
+        &mut self,
+        missing_child: usize,
+        left_child: usize,
+        right_child: usize,
+        split_info: &SplitInfo,
+    ) {
+        self.left_child = left_child;
+        self.right_child = right_child;
+        self.split_feature = split_info.split_feature;
+        let missing_split_gain = match &split_info.missing_node {
+            MissingInfo::Branch(ni) => ni.gain,
+            _ => 0.,
+        };
+        self.split_gain =
+            split_info.left_node.gain + split_info.right_node.gain + missing_split_gain
+                - self.gain_value;
+        self.split_value = split_info.split_value;
+        self.missing_node = missing_child;
+        self.is_leaf = false;
+    }
+    pub fn as_node(&self) -> Node {
+        Node {
+            num: self.num,
+            weight_value: self.weight_value,
+            hessian_sum: self.hessian_sum,
+            depth: self.depth,
+            missing_node: self.missing_node,
+            split_value: self.split_value,
+            split_feature: self.split_feature,
+            split_gain: self.split_gain,
+            left_child: self.left_child,
+            right_child: self.right_child,
+            is_leaf: self.is_leaf,
+        }
+    }
+}
+
+impl fmt::Display for Node {
+    // This trait requires `fmt` with this exact signature.
+    fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
+        if self.is_leaf {
+            write!(
+                f,
+                "{}:leaf={},cover={}",
+                self.num, self.weight_value, self.hessian_sum
+            )
+        } else {
+            write!(
+                f,
+                "{}:[{} < {}] yes={},no={},missing={},gain={},cover={}",
+                self.num,
+                self.split_feature,
+                self.split_value,
+                self.left_child,
+                self.right_child,
+                self.missing_node,
+                self.split_gain,
+                self.hessian_sum
+            )
+        }
+    }
+}
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/src/objective.rs` & `forust-0.2.7/local_dependencies/forust-ml/src/objective.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,155 @@
-use crate::data::FloatData;
-use serde::{Deserialize, Serialize};
-
-type ObjFn = fn(&[f64], &[f64], &[f64]) -> Vec<f32>;
-
-#[derive(Debug, Deserialize, Serialize)]
-pub enum ObjectiveType {
-    LogLoss,
-    SquaredLoss,
-}
-
-pub fn gradient_hessian_callables(objective_type: &ObjectiveType) -> (ObjFn, ObjFn) {
-    match objective_type {
-        ObjectiveType::LogLoss => (LogLoss::calc_grad, LogLoss::calc_hess),
-        ObjectiveType::SquaredLoss => (SquaredLoss::calc_grad, SquaredLoss::calc_hess),
-    }
-}
-
-pub trait ObjectiveFunction {
-    fn calc_loss(y: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32>;
-    fn calc_grad(y: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32>;
-    fn calc_hess(y: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32>;
-}
-
-#[derive(Default)]
-pub struct LogLoss {}
-
-impl ObjectiveFunction for LogLoss {
-    #[inline]
-    fn calc_loss(y: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32> {
-        y.iter()
-            .zip(yhat)
-            .zip(sample_weight)
-            .map(|((y_, yhat_), w_)| {
-                let yhat_ = f64::ONE / (f64::ONE + (-*yhat_).exp());
-                (-(*y_ * yhat_.ln() + (f64::ONE - *y_) * ((f64::ONE - yhat_).ln())) * *w_) as f32
-            })
-            .collect()
-    }
-
-    #[inline]
-    fn calc_grad(y: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32> {
-        y.iter()
-            .zip(yhat)
-            .zip(sample_weight)
-            .map(|((y_, yhat_), w_)| {
-                let yhat_ = f64::ONE / (f64::ONE + (-*yhat_).exp());
-                ((yhat_ - *y_) * *w_) as f32
-            })
-            .collect()
-    }
-    #[inline]
-    fn calc_hess(_: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32> {
-        yhat.iter()
-            .zip(sample_weight)
-            .map(|(yhat_, w_)| {
-                let yhat_ = f64::ONE / (f64::ONE + (-*yhat_).exp());
-                (yhat_ * (f64::ONE - yhat_) * *w_) as f32
-            })
-            .collect()
-    }
-}
-
-#[derive(Default)]
-pub struct SquaredLoss {}
-
-impl ObjectiveFunction for SquaredLoss {
-    #[inline]
-    fn calc_loss(y: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32> {
-        y.iter()
-            .zip(yhat)
-            .zip(sample_weight)
-            .map(|((y_, yhat_), w_)| {
-                let s = *y_ - *yhat_;
-                (s * s * *w_) as f32
-            })
-            .collect()
-    }
-
-    #[inline]
-    fn calc_grad(y: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32> {
-        y.iter()
-            .zip(yhat)
-            .zip(sample_weight)
-            .map(|((y_, yhat_), w_)| ((*yhat_ - *y_) * *w_) as f32)
-            .collect()
-    }
-
-    #[inline]
-    fn calc_hess(_: &[f64], _: &[f64], sample_weight: &[f64]) -> Vec<f32> {
-        sample_weight.iter().map(|v| *v as f32).collect()
-    }
-}
-
-#[cfg(test)]
-mod tests {
-    use super::*;
-    #[test]
-    fn test_logloss_loss() {
-        let y = vec![0.0, 0.0, 0.0, 1.0, 1.0, 1.0];
-        let yhat1 = vec![-1.0, -1.0, -1.0, 1.0, 1.0, 1.0];
-        let w = vec![1.; y.len()];
-        let l1 = LogLoss::calc_loss(&y, &yhat1, &w);
-        let yhat2 = vec![0.0, 0.0, -1.0, 1.0, 0.0, 1.0];
-        let l2 = LogLoss::calc_loss(&y, &yhat2, &w);
-        assert!(l1.iter().sum::<f32>() < l2.iter().sum::<f32>());
-    }
-
-    #[test]
-    fn test_logloss_grad() {
-        let y = vec![0.0, 0.0, 0.0, 1.0, 1.0, 1.0];
-        let yhat1 = vec![-1.0, -1.0, -1.0, 1.0, 1.0, 1.0];
-        let w = vec![1.; y.len()];
-        let g1 = LogLoss::calc_grad(&y, &yhat1, &w);
-        let yhat2 = vec![0.0, 0.0, -1.0, 1.0, 0.0, 1.0];
-        let g2 = LogLoss::calc_grad(&y, &yhat2, &w);
-        assert!(g1.iter().sum::<f32>() < g2.iter().sum::<f32>());
-    }
-
-    #[test]
-    fn test_logloss_hess() {
-        let y = vec![0.0, 0.0, 0.0, 1.0, 1.0, 1.0];
-        let yhat1 = vec![-1.0, -1.0, -1.0, 1.0, 1.0, 1.0];
-        let w = vec![1.; y.len()];
-        let h1 = LogLoss::calc_hess(&y, &yhat1, &w);
-        let yhat2 = vec![0.0, 0.0, -1.0, 1.0, 0.0, 1.0];
-        let h2 = LogLoss::calc_hess(&y, &yhat2, &w);
-        assert!(h1.iter().sum::<f32>() < h2.iter().sum::<f32>());
-    }
-}
+use std::str::FromStr;
+
+use crate::{data::FloatData, errors::ForustError, metric::Metric, utils::items_to_strings};
+use serde::{Deserialize, Serialize};
+
+type ObjFn = fn(&[f64], &[f64], &[f64]) -> Vec<f32>;
+
+#[derive(Debug, Deserialize, Serialize)]
+pub enum ObjectiveType {
+    LogLoss,
+    SquaredLoss,
+}
+
+impl FromStr for ObjectiveType {
+    type Err = ForustError;
+
+    fn from_str(s: &str) -> Result<Self, Self::Err> {
+        match s {
+            "LogLoss" => Ok(ObjectiveType::LogLoss),
+            "SquaredLoss" => Ok(ObjectiveType::SquaredLoss),
+            _ => Err(ForustError::ParseString(
+                s.to_string(),
+                "ObjectiveType".to_string(),
+                items_to_strings(vec!["LogLoss", "SquaredLoss"]),
+            )),
+        }
+    }
+}
+
+pub fn gradient_hessian_callables(objective_type: &ObjectiveType) -> (ObjFn, ObjFn) {
+    match objective_type {
+        ObjectiveType::LogLoss => (LogLoss::calc_grad, LogLoss::calc_hess),
+        ObjectiveType::SquaredLoss => (SquaredLoss::calc_grad, SquaredLoss::calc_hess),
+    }
+}
+
+pub trait ObjectiveFunction {
+    fn calc_loss(y: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32>;
+    fn calc_grad(y: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32>;
+    fn calc_hess(y: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32>;
+    fn default_metric() -> Metric;
+}
+
+#[derive(Default)]
+pub struct LogLoss {}
+
+impl ObjectiveFunction for LogLoss {
+    #[inline]
+    fn calc_loss(y: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32> {
+        y.iter()
+            .zip(yhat)
+            .zip(sample_weight)
+            .map(|((y_, yhat_), w_)| {
+                let yhat_ = f64::ONE / (f64::ONE + (-*yhat_).exp());
+                (-(*y_ * yhat_.ln() + (f64::ONE - *y_) * ((f64::ONE - yhat_).ln())) * *w_) as f32
+            })
+            .collect()
+    }
+
+    #[inline]
+    fn calc_grad(y: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32> {
+        y.iter()
+            .zip(yhat)
+            .zip(sample_weight)
+            .map(|((y_, yhat_), w_)| {
+                let yhat_ = f64::ONE / (f64::ONE + (-*yhat_).exp());
+                ((yhat_ - *y_) * *w_) as f32
+            })
+            .collect()
+    }
+    #[inline]
+    fn calc_hess(_: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32> {
+        yhat.iter()
+            .zip(sample_weight)
+            .map(|(yhat_, w_)| {
+                let yhat_ = f64::ONE / (f64::ONE + (-*yhat_).exp());
+                (yhat_ * (f64::ONE - yhat_) * *w_) as f32
+            })
+            .collect()
+    }
+    fn default_metric() -> Metric {
+        Metric::LogLoss
+    }
+}
+
+#[derive(Default)]
+pub struct SquaredLoss {}
+
+impl ObjectiveFunction for SquaredLoss {
+    #[inline]
+    fn calc_loss(y: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32> {
+        y.iter()
+            .zip(yhat)
+            .zip(sample_weight)
+            .map(|((y_, yhat_), w_)| {
+                let s = *y_ - *yhat_;
+                (s * s * *w_) as f32
+            })
+            .collect()
+    }
+
+    #[inline]
+    fn calc_grad(y: &[f64], yhat: &[f64], sample_weight: &[f64]) -> Vec<f32> {
+        y.iter()
+            .zip(yhat)
+            .zip(sample_weight)
+            .map(|((y_, yhat_), w_)| ((*yhat_ - *y_) * *w_) as f32)
+            .collect()
+    }
+
+    #[inline]
+    fn calc_hess(_: &[f64], _: &[f64], sample_weight: &[f64]) -> Vec<f32> {
+        sample_weight.iter().map(|v| *v as f32).collect()
+    }
+    fn default_metric() -> Metric {
+        Metric::RootMeanSquaredLogError
+    }
+}
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+    #[test]
+    fn test_logloss_loss() {
+        let y = vec![0.0, 0.0, 0.0, 1.0, 1.0, 1.0];
+        let yhat1 = vec![-1.0, -1.0, -1.0, 1.0, 1.0, 1.0];
+        let w = vec![1.; y.len()];
+        let l1 = LogLoss::calc_loss(&y, &yhat1, &w);
+        let yhat2 = vec![0.0, 0.0, -1.0, 1.0, 0.0, 1.0];
+        let l2 = LogLoss::calc_loss(&y, &yhat2, &w);
+        assert!(l1.iter().sum::<f32>() < l2.iter().sum::<f32>());
+    }
+
+    #[test]
+    fn test_logloss_grad() {
+        let y = vec![0.0, 0.0, 0.0, 1.0, 1.0, 1.0];
+        let yhat1 = vec![-1.0, -1.0, -1.0, 1.0, 1.0, 1.0];
+        let w = vec![1.; y.len()];
+        let g1 = LogLoss::calc_grad(&y, &yhat1, &w);
+        let yhat2 = vec![0.0, 0.0, -1.0, 1.0, 0.0, 1.0];
+        let g2 = LogLoss::calc_grad(&y, &yhat2, &w);
+        assert!(g1.iter().sum::<f32>() < g2.iter().sum::<f32>());
+    }
+
+    #[test]
+    fn test_logloss_hess() {
+        let y = vec![0.0, 0.0, 0.0, 1.0, 1.0, 1.0];
+        let yhat1 = vec![-1.0, -1.0, -1.0, 1.0, 1.0, 1.0];
+        let w = vec![1.; y.len()];
+        let h1 = LogLoss::calc_hess(&y, &yhat1, &w);
+        let yhat2 = vec![0.0, 0.0, -1.0, 1.0, 0.0, 1.0];
+        let h2 = LogLoss::calc_hess(&y, &yhat2, &w);
+        assert!(h1.iter().sum::<f32>() < h2.iter().sum::<f32>());
+    }
+}
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/src/partial_dependence.rs` & `forust-0.2.7/local_dependencies/forust-ml/src/partial_dependence.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,132 +1,129 @@
-use crate::{tree::Tree, utils::is_missing};
-
-/// Partial Dependence Calculator
-// struct PDCalculator {
-//     partial_dependence: f32,
-//     base_score: f64,
-//     tree_prediction: f64,
-
-// }
-
-fn get_node_cover(tree: &Tree, node_idx: usize) -> f32 {
-    tree.nodes[node_idx].hessian_sum
-}
-
-pub fn tree_partial_dependence(
-    tree: &Tree,
-    node_idx: usize,
-    feature: usize,
-    value: f64,
-    proportion: f32,
-    missing: &f64,
-) -> f64 {
-    let n = &tree.nodes[node_idx];
-    if n.is_leaf {
-        f64::from(proportion * n.weight_value)
-    } else if n.split_feature == feature {
-        let child = if is_missing(&value, missing) {
-            n.missing_node
-        } else if value < n.split_value {
-            n.left_child
-        } else {
-            n.right_child
-        };
-        tree_partial_dependence(tree, child, feature, value, proportion, missing)
-    } else {
-        let left_cover = get_node_cover(tree, n.left_child);
-        let right_cover = get_node_cover(tree, n.right_child);
-        let missing_cover = if n.has_missing_branch() {
-            get_node_cover(tree, n.missing_node)
-        } else {
-            0.0
-        };
-        let total_cover = left_cover + right_cover + missing_cover;
-        let missing_pd = if n.has_missing_branch() {
-            tree_partial_dependence(
-                tree,
-                n.missing_node,
-                feature,
-                value,
-                proportion * (missing_cover / total_cover),
-                missing,
-            )
-        } else {
-            0.
-        };
-        tree_partial_dependence(
-            tree,
-            n.left_child,
-            feature,
-            value,
-            proportion * (left_cover / total_cover),
-            missing,
-        ) + tree_partial_dependence(
-            tree,
-            n.right_child,
-            feature,
-            value,
-            proportion * (right_cover / total_cover),
-            missing,
-        ) + missing_pd
-    }
-}
-
-#[cfg(test)]
-mod tests {
-    use rand::rngs::StdRng;
-    use rand::SeedableRng;
-
-    use super::*;
-    use crate::binning::bin_matrix;
-    use crate::constraints::ConstraintMap;
-    use crate::data::Matrix;
-    use crate::objective::{LogLoss, ObjectiveFunction};
-    use crate::splitter::MissingImputerSplitter;
-    use crate::tree::Tree;
-    use std::fs;
-    #[test]
-    fn test_partial_dependence() {
-        let file = fs::read_to_string("resources/contiguous_no_missing.csv")
-            .expect("Something went wrong reading the file");
-        let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
-        let file = fs::read_to_string("resources/performance.csv")
-            .expect("Something went wrong reading the file");
-        let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
-        let yhat = vec![0.5; y.len()];
-        let w = vec![1.; y.len()];
-        let g = LogLoss::calc_grad(&y, &yhat, &w);
-        let h = LogLoss::calc_hess(&y, &yhat, &w);
-
-        let data = Matrix::new(&data_vec, 891, 5);
-        let splitter = MissingImputerSplitter {
-            l2: 1.0,
-            gamma: 3.0,
-            min_leaf_weight: 1.0,
-            learning_rate: 0.3,
-            allow_missing_splits: true,
-            constraints_map: ConstraintMap::new(),
-        };
-        let mut tree = Tree::new();
-
-        let b = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
-        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
-
-        let mut rng = StdRng::seed_from_u64(0);
-        tree.fit(
-            &bdata,
-            &b.cuts,
-            &g,
-            &h,
-            &splitter,
-            usize::MAX,
-            5,
-            true,
-            1.,
-            &mut rng,
-        );
-        let pdp1 = tree_partial_dependence(&tree, 0, 0, 1.0, 1.0, &f64::NAN);
-        let pdp2 = tree_partial_dependence(&tree, 0, 0, 2.0, 1.0, &f64::NAN);
-        let pdp3 = tree_partial_dependence(&tree, 0, 0, 3.0, 1.0, &f64::NAN);
-        println!("{}, {}, {}", pdp1, pdp2, pdp3);
-    }
-}
+use crate::{tree::Tree, utils::is_missing};
+
+/// Partial Dependence Calculator
+// struct PDCalculator {
+//     partial_dependence: f32,
+//     base_score: f64,
+//     tree_prediction: f64,
+
+// }
+
+fn get_node_cover(tree: &Tree, node_idx: usize) -> f32 {
+    tree.nodes[node_idx].hessian_sum
+}
+
+pub fn tree_partial_dependence(
+    tree: &Tree,
+    node_idx: usize,
+    feature: usize,
+    value: f64,
+    proportion: f32,
+    missing: &f64,
+) -> f64 {
+    let n = &tree.nodes[node_idx];
+    if n.is_leaf {
+        f64::from(proportion * n.weight_value)
+    } else if n.split_feature == feature {
+        let child = if is_missing(&value, missing) {
+            n.missing_node
+        } else if value < n.split_value {
+            n.left_child
+        } else {
+            n.right_child
+        };
+        tree_partial_dependence(tree, child, feature, value, proportion, missing)
+    } else {
+        let left_cover = get_node_cover(tree, n.left_child);
+        let right_cover = get_node_cover(tree, n.right_child);
+        let missing_cover = if n.has_missing_branch() {
+            get_node_cover(tree, n.missing_node)
+        } else {
+            0.0
+        };
+        let total_cover = left_cover + right_cover + missing_cover;
+        let missing_pd = if n.has_missing_branch() {
+            tree_partial_dependence(
+                tree,
+                n.missing_node,
+                feature,
+                value,
+                proportion * (missing_cover / total_cover),
+                missing,
+            )
+        } else {
+            0.
+        };
+        tree_partial_dependence(
+            tree,
+            n.left_child,
+            feature,
+            value,
+            proportion * (left_cover / total_cover),
+            missing,
+        ) + tree_partial_dependence(
+            tree,
+            n.right_child,
+            feature,
+            value,
+            proportion * (right_cover / total_cover),
+            missing,
+        ) + missing_pd
+    }
+}
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+    use crate::binning::bin_matrix;
+    use crate::constraints::ConstraintMap;
+    use crate::data::Matrix;
+    use crate::objective::{LogLoss, ObjectiveFunction};
+    use crate::sampler::SampleMethod;
+    use crate::splitter::MissingImputerSplitter;
+    use crate::tree::Tree;
+    use std::fs;
+    #[test]
+    fn test_partial_dependence() {
+        let file = fs::read_to_string("resources/contiguous_no_missing.csv")
+            .expect("Something went wrong reading the file");
+        let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+        let file = fs::read_to_string("resources/performance.csv")
+            .expect("Something went wrong reading the file");
+        let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+        let yhat = vec![0.5; y.len()];
+        let w = vec![1.; y.len()];
+        let g = LogLoss::calc_grad(&y, &yhat, &w);
+        let h = LogLoss::calc_hess(&y, &yhat, &w);
+
+        let data = Matrix::new(&data_vec, 891, 5);
+        let splitter = MissingImputerSplitter {
+            l2: 1.0,
+            gamma: 3.0,
+            min_leaf_weight: 1.0,
+            learning_rate: 0.3,
+            allow_missing_splits: true,
+            constraints_map: ConstraintMap::new(),
+        };
+        let mut tree = Tree::new();
+
+        let b = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
+        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
+
+        tree.fit(
+            &bdata,
+            data.index.to_owned(),
+            &b.cuts,
+            &g,
+            &h,
+            &splitter,
+            usize::MAX,
+            5,
+            true,
+            &SampleMethod::None,
+        );
+        let pdp1 = tree_partial_dependence(&tree, 0, 0, 1.0, 1.0, &f64::NAN);
+        let pdp2 = tree_partial_dependence(&tree, 0, 0, 2.0, 1.0, &f64::NAN);
+        let pdp3 = tree_partial_dependence(&tree, 0, 0, 3.0, 1.0, &f64::NAN);
+        println!("{}, {}, {}", pdp1, pdp2, pdp3);
+    }
+}
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/src/splitter.rs` & `forust-0.2.7/local_dependencies/forust-ml/src/splitter.rs`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,1016 +1,1016 @@
-use crate::constraints::{Constraint, ConstraintMap};
-use crate::data::{JaggedMatrix, Matrix};
-use crate::histogram::HistogramMatrix;
-use crate::node::SplittableNode;
-use crate::utils::{
-    constrained_weight, cull_gain, gain_given_weight, pivot_on_split,
-    pivot_on_split_exclude_missing, weight,
-};
-
-#[derive(Debug)]
-pub struct SplitInfo {
-    pub split_gain: f32,
-    pub split_feature: usize,
-    pub split_value: f64,
-    pub split_bin: u16,
-    pub left_node: NodeInfo,
-    pub right_node: NodeInfo,
-    pub missing_node: MissingInfo,
-}
-
-#[derive(Debug)]
-pub struct NodeInfo {
-    pub grad: f32,
-    pub gain: f32,
-    pub cover: f32,
-    pub weight: f32,
-    pub bounds: (f32, f32),
-}
-
-#[derive(Debug)]
-pub enum MissingInfo {
-    Left,
-    Right,
-    Leaf(NodeInfo),
-    Branch(NodeInfo),
-}
-
-pub trait Splitter {
-    fn get_constraint(&self, feature: &usize) -> Option<&Constraint>;
-    // fn get_allow_missing_splits(&self) -> bool;
-    fn get_gamma(&self) -> f32;
-    fn get_l2(&self) -> f32;
-
-    /// Find the best possible split, considering all feature histograms.
-    /// If we wanted to add Column sampling, this is probably where
-    /// we would need to do it, otherwise, it would be at the tree level.
-    fn best_split(&self, node: &SplittableNode) -> Option<SplitInfo> {
-        let mut best_split_info = None;
-        let mut best_gain = 0.0;
-        let HistogramMatrix(histograms) = &node.histograms;
-        for i in 0..histograms.cols {
-            let split_info = self.best_feature_split(node, i);
-            match split_info {
-                Some(info) => {
-                    if info.split_gain > best_gain {
-                        best_gain = info.split_gain;
-                        best_split_info = Some(info);
-                    }
-                }
-                None => continue,
-            }
-        }
-        best_split_info
-    }
-
-    /// Evaluate a split, returning the node info for the left, and right splits,
-    /// as well as the node info the missing data of a feature.
-    #[allow(clippy::too_many_arguments)]
-    fn evaluate_split(
-        &self,
-        left_gradient: f32,
-        left_hessian: f32,
-        right_gradient: f32,
-        right_hessian: f32,
-        missing_gradient: f32,
-        missing_hessian: f32,
-        lower_bound: f32,
-        upper_bound: f32,
-        constraint: Option<&Constraint>,
-    ) -> Option<(NodeInfo, NodeInfo, MissingInfo)>;
-
-    fn best_feature_split(&self, node: &SplittableNode, feature: usize) -> Option<SplitInfo> {
-        let mut split_info: Option<SplitInfo> = None;
-        let mut max_gain: Option<f32> = None;
-
-        let HistogramMatrix(histograms) = &node.histograms;
-        let histogram = histograms.get_col(feature);
-
-        // We also know we will have a missing bin.
-        let missing = &histogram[0];
-        let mut cuml_grad = 0.0; // first_bin.gradient_sum;
-        let mut cuml_hess = 0.0; // first_bin.hessian_sum;
-        let constraint = self.get_constraint(&feature);
-
-        let elements = histogram.len();
-        assert!(elements == histogram.len());
-
-        for (i, bin) in histogram[1..].iter().enumerate() {
-            let left_gradient = cuml_grad;
-            let left_hessian = cuml_hess;
-            let right_gradient = node.gradient_sum - cuml_grad - missing.gradient_sum;
-            let right_hessian = node.hessian_sum - cuml_hess - missing.hessian_sum;
-
-            let (mut left_node_info, mut right_node_info, missing_info) = match self.evaluate_split(
-                left_gradient,
-                left_hessian,
-                right_gradient,
-                right_hessian,
-                missing.gradient_sum,
-                missing.hessian_sum,
-                node.lower_bound,
-                node.upper_bound,
-                constraint,
-            ) {
-                None => {
-                    cuml_grad += bin.gradient_sum;
-                    cuml_hess += bin.hessian_sum;
-                    continue;
-                }
-                Some(v) => v,
-            };
-
-            // TODO!
-            // Should we be doing this?
-            // or should missing gain not factor in at
-            // all to the split gain?
-            let missing_gain = match &missing_info {
-                MissingInfo::Branch(v) | MissingInfo::Leaf(v) => v.gain,
-                _ => 0.0,
-            };
-            let split_gain = (left_node_info.gain + right_node_info.gain + missing_gain
-                - node.gain_value)
-                - self.get_gamma();
-
-            // Check monotonicity holds
-            let split_gain = cull_gain(
-                split_gain,
-                left_node_info.weight,
-                right_node_info.weight,
-                constraint,
-            );
-
-            if split_gain <= 0.0 {
-                // Update for new value
-                cuml_grad += bin.gradient_sum;
-                cuml_hess += bin.hessian_sum;
-                continue;
-            }
-
-            let mid = (left_node_info.weight + right_node_info.weight) / 2.0;
-            let (left_bounds, right_bounds) = match constraint {
-                None | Some(Constraint::Unconstrained) => (
-                    (node.lower_bound, node.upper_bound),
-                    (node.lower_bound, node.upper_bound),
-                ),
-                Some(Constraint::Negative) => ((mid, node.upper_bound), (node.lower_bound, mid)),
-                Some(Constraint::Positive) => ((node.lower_bound, mid), (mid, node.upper_bound)),
-            };
-            left_node_info.bounds = left_bounds;
-            right_node_info.bounds = right_bounds;
-
-            // If split gain is NaN, one of the sides is empty, do not allow
-            // this split.
-            let split_gain = if split_gain.is_nan() { 0.0 } else { split_gain };
-            if max_gain.is_none() || split_gain > max_gain.unwrap() {
-                max_gain = Some(split_gain);
-                split_info = Some(SplitInfo {
-                    split_gain,
-                    split_feature: feature,
-                    split_value: bin.cut_value,
-                    split_bin: (i + 1) as u16,
-                    left_node: left_node_info,
-                    right_node: right_node_info,
-                    missing_node: missing_info,
-                });
-            }
-            // Update for new value
-            cuml_grad += bin.gradient_sum;
-            cuml_hess += bin.hessian_sum;
-        }
-        split_info
-    }
-
-    /// Handle the split info, creating the children nodes, this function
-    /// will return a vector of new splitable nodes, that can be added to the
-    /// growable stack, and further split, or converted to leaf nodes.
-    #[allow(clippy::too_many_arguments)]
-    fn handle_split_info(
-        &self,
-        split_info: SplitInfo,
-        n_nodes: &usize,
-        node: &mut SplittableNode,
-        index: &mut [usize],
-        data: &Matrix<u16>,
-        cuts: &JaggedMatrix<f64>,
-        grad: &[f32],
-        hess: &[f32],
-        parallel: bool,
-    ) -> Vec<SplittableNode>;
-
-    /// Split the node, if we cant find a best split, we will need to
-    /// return an empty vector, this node is a leaf.
-    #[allow(clippy::too_many_arguments)]
-    fn split_node(
-        &self,
-        n_nodes: &usize,
-        node: &mut SplittableNode,
-        index: &mut [usize],
-        data: &Matrix<u16>,
-        cuts: &JaggedMatrix<f64>,
-        grad: &[f32],
-        hess: &[f32],
-        parallel: bool,
-    ) -> Vec<SplittableNode> {
-        match self.best_split(node) {
-            Some(split_info) => self.handle_split_info(
-                split_info, n_nodes, node, index, data, cuts, grad, hess, parallel,
-            ),
-            None => Vec::new(),
-        }
-    }
-}
-
-/// Missing branch splitter
-/// Always creates a separate branch for the missing values of a feature.
-/// This results, in every node having a specific "missing", direction.
-/// If this node is able, it will be split further, otherwise it will
-/// a leaf node will be generated.
-pub struct MissingBranchSplitter {
-    pub l2: f32,
-    pub gamma: f32,
-    pub min_leaf_weight: f32,
-    pub learning_rate: f32,
-    pub allow_missing_splits: bool,
-    pub constraints_map: ConstraintMap,
-}
-
-impl Splitter for MissingBranchSplitter {
-    fn get_constraint(&self, feature: &usize) -> Option<&Constraint> {
-        self.constraints_map.get(feature)
-    }
-
-    fn get_gamma(&self) -> f32 {
-        self.gamma
-    }
-
-    fn get_l2(&self) -> f32 {
-        self.l2
-    }
-
-    fn evaluate_split(
-        &self,
-        left_gradient: f32,
-        left_hessian: f32,
-        right_gradient: f32,
-        right_hessian: f32,
-        missing_gradient: f32,
-        missing_hessian: f32,
-        lower_bound: f32,
-        upper_bound: f32,
-        constraint: Option<&Constraint>,
-    ) -> Option<(NodeInfo, NodeInfo, MissingInfo)> {
-        // If there is no info right, or there is no
-        // info left, there is nothing to split on,
-        // and so we should continue.
-        if (left_gradient == 0.0) && (left_hessian == 0.0)
-            || (right_gradient == 0.0) && (right_hessian == 0.0)
-        {
-            return None;
-        }
-
-        let left_gradient = left_gradient;
-        let left_hessian = left_hessian;
-
-        let right_gradient = right_gradient;
-        let right_hessian = right_hessian;
-
-        let left_weight = constrained_weight(
-            &self.l2,
-            left_gradient,
-            left_hessian,
-            lower_bound,
-            upper_bound,
-            constraint,
-        );
-        let right_weight = constrained_weight(
-            &self.l2,
-            right_gradient,
-            right_hessian,
-            lower_bound,
-            upper_bound,
-            constraint,
-        );
-
-        let left_gain = gain_given_weight(&self.l2, left_gradient, left_hessian, left_weight);
-        let right_gain = gain_given_weight(&self.l2, right_gradient, right_hessian, right_weight);
-
-        // Check the min_hessian constraint first
-        if (right_hessian < self.min_leaf_weight) || (left_hessian < self.min_leaf_weight) {
-            // Update for new value
-            return None;
-        }
-
-        // We have not considered missing at all up until this point, we could if we wanted
-        // to give more predictive power probably to missing.
-        // If we don't want to allow the missing branch to be split further,
-        // we will default to creating an empty branch.
-
-        // Set weight to the parent weight...
-        let missing_weight = weight(
-            &self.get_l2(),
-            missing_gradient + left_gradient + right_gradient,
-            missing_hessian + left_hessian + right_hessian,
-        ); // weight(&self.get_l2(), missing_gradient, missing_hessian);
-        let missing_gain = gain_given_weight(
-            &self.get_l2(),
-            missing_gradient,
-            missing_hessian,
-            missing_weight,
-        );
-        let missing_info = NodeInfo {
-            grad: missing_gradient,
-            gain: missing_gain,
-            cover: missing_hessian,
-            weight: missing_weight * self.learning_rate,
-            bounds: (f32::NEG_INFINITY, f32::INFINITY),
-        };
-        let missing_node = // Check Missing direction
-        if ((missing_gradient != 0.0) || (missing_hessian != 0.0)) && self.allow_missing_splits {
-            MissingInfo::Branch(
-                missing_info
-            )
-        } else {
-            MissingInfo::Leaf(
-                missing_info
-            )
-        };
-
-        if (right_hessian < self.min_leaf_weight) || (left_hessian < self.min_leaf_weight) {
-            // Update for new value
-            return None;
-        }
-        Some((
-            NodeInfo {
-                grad: left_gradient,
-                gain: left_gain,
-                cover: left_hessian,
-                weight: left_weight * self.learning_rate,
-                bounds: (f32::NEG_INFINITY, f32::INFINITY),
-            },
-            NodeInfo {
-                grad: right_gradient,
-                gain: right_gain,
-                cover: right_hessian,
-                weight: right_weight * self.learning_rate,
-                bounds: (f32::NEG_INFINITY, f32::INFINITY),
-            },
-            missing_node,
-        ))
-    }
-
-    fn handle_split_info(
-        &self,
-        split_info: SplitInfo,
-        n_nodes: &usize,
-        node: &mut SplittableNode,
-        index: &mut [usize],
-        data: &Matrix<u16>,
-        cuts: &JaggedMatrix<f64>,
-        grad: &[f32],
-        hess: &[f32],
-        parallel: bool,
-    ) -> Vec<SplittableNode> {
-        let missing_child = *n_nodes;
-        let left_child = missing_child + 1;
-        let right_child = missing_child + 2;
-        node.update_children(missing_child, left_child, right_child, &split_info);
-
-        let (missing_is_leaf, mut missing_info) = match split_info.missing_node {
-            MissingInfo::Branch(i) => (false, i),
-            MissingInfo::Leaf(i) => (true, i),
-            _ => unreachable!(),
-        };
-        // Set missing weight to parent weight value...
-        // This essentially neutralizes missing.
-        // Manually calculating it, was leading to some small numeric
-        // rounding differences...
-        missing_info.weight = node.weight_value;
-
-        // We need to move all of the index's above and below our
-        // split value.
-        // pivot the sub array that this node has on our split value
-        // Missing all falls to the bottom.
-        let (mut missing_split_idx, mut split_idx) = pivot_on_split_exclude_missing(
-            &mut index[node.start_idx..node.stop_idx],
-            data.get_col(split_info.split_feature),
-            split_info.split_bin,
-        );
-        // Calculate histograms
-        let total_recs = node.stop_idx - node.start_idx;
-        let n_right = total_recs - split_idx;
-        let n_left = total_recs - n_right - missing_split_idx;
-        let n_missing = total_recs - (n_right + n_left);
-        let max_ = match vec![n_missing, n_left, n_right]
-            .iter()
-            .enumerate()
-            .max_by(|(_, i), (_, j)| i.cmp(j))
-        {
-            Some((i, _)) => i,
-            // if we can't compare them, it doesn't
-            // really matter, build the histogram on
-            // any of them.
-            None => 0,
-        };
-
-        // Now that we have calculated the number of records
-        // add the start index, to make the split_index
-        // relative to the entire index array
-        split_idx += node.start_idx;
-        missing_split_idx += node.start_idx;
-
-        // Build the histograms for the smaller node.
-        let left_histograms: HistogramMatrix;
-        let right_histograms: HistogramMatrix;
-        let missing_histograms: HistogramMatrix;
-        if n_missing == 0 {
-            if max_ == 1 {
-                missing_histograms = HistogramMatrix::empty();
-                right_histograms = HistogramMatrix::new(
-                    data,
-                    cuts,
-                    grad,
-                    hess,
-                    &index[split_idx..node.stop_idx],
-                    parallel,
-                    true,
-                );
-                left_histograms =
-                    HistogramMatrix::from_parent_child(&node.histograms, &right_histograms);
-            } else {
-                missing_histograms = HistogramMatrix::empty();
-                left_histograms = HistogramMatrix::new(
-                    data,
-                    cuts,
-                    grad,
-                    hess,
-                    &index[missing_split_idx..split_idx],
-                    parallel,
-                    true,
-                );
-                right_histograms =
-                    HistogramMatrix::from_parent_child(&node.histograms, &left_histograms);
-            }
-        } else if max_ == 0 {
-            // Max is missing, calculate the other two
-            // levels histograms.
-            left_histograms = HistogramMatrix::new(
-                data,
-                cuts,
-                grad,
-                hess,
-                &index[missing_split_idx..split_idx],
-                parallel,
-                true,
-            );
-            right_histograms = HistogramMatrix::new(
-                data,
-                cuts,
-                grad,
-                hess,
-                &index[split_idx..node.stop_idx],
-                parallel,
-                true,
-            );
-            missing_histograms = HistogramMatrix::from_parent_two_children(
-                &node.histograms,
-                &left_histograms,
-                &right_histograms,
-            )
-        } else if max_ == 1 {
-            missing_histograms = HistogramMatrix::new(
-                data,
-                cuts,
-                grad,
-                hess,
-                &index[node.start_idx..missing_split_idx],
-                parallel,
-                true,
-            );
-            right_histograms = HistogramMatrix::new(
-                data,
-                cuts,
-                grad,
-                hess,
-                &index[split_idx..node.stop_idx],
-                parallel,
-                true,
-            );
-            left_histograms = HistogramMatrix::from_parent_two_children(
-                &node.histograms,
-                &missing_histograms,
-                &right_histograms,
-            )
-        } else {
-            // right is the largest
-
-            missing_histograms = HistogramMatrix::new(
-                data,
-                cuts,
-                grad,
-                hess,
-                &index[node.start_idx..missing_split_idx],
-                parallel,
-                true,
-            );
-            left_histograms = HistogramMatrix::new(
-                data,
-                cuts,
-                grad,
-                hess,
-                &index[missing_split_idx..split_idx],
-                parallel,
-                true,
-            );
-            right_histograms = HistogramMatrix::from_parent_two_children(
-                &node.histograms,
-                &missing_histograms,
-                &left_histograms,
-            )
-        }
-
-        let mut missing_node = SplittableNode::from_node_info(
-            missing_child,
-            missing_histograms,
-            node.depth + 1,
-            node.start_idx,
-            missing_split_idx,
-            missing_info,
-        );
-        missing_node.is_missing_leaf = missing_is_leaf;
-        let left_node = SplittableNode::from_node_info(
-            left_child,
-            left_histograms,
-            node.depth + 1,
-            missing_split_idx,
-            split_idx,
-            split_info.left_node,
-        );
-        let right_node = SplittableNode::from_node_info(
-            right_child,
-            right_histograms,
-            node.depth + 1,
-            split_idx,
-            node.stop_idx,
-            split_info.right_node,
-        );
-        vec![missing_node, left_node, right_node]
-    }
-}
-
-/// Missing imputer splitter
-/// Splitter that imputes missing values, by sending
-/// them down either the right or left branch, depending
-/// on which results in a higher increase in gain.
-pub struct MissingImputerSplitter {
-    pub l2: f32,
-    pub gamma: f32,
-    pub min_leaf_weight: f32,
-    pub learning_rate: f32,
-    pub allow_missing_splits: bool,
-    pub constraints_map: ConstraintMap,
-}
-
-impl MissingImputerSplitter {
-    /// Generate a new missing imputer splitter object.
-    pub fn new(
-        l2: f32,
-        gamma: f32,
-        min_leaf_weight: f32,
-        learning_rate: f32,
-        allow_missing_splits: bool,
-        constraints_map: ConstraintMap,
-    ) -> Self {
-        MissingImputerSplitter {
-            l2,
-            gamma,
-            min_leaf_weight,
-            learning_rate,
-            allow_missing_splits,
-            constraints_map,
-        }
-    }
-}
-
-impl Splitter for MissingImputerSplitter {
-    #[allow(clippy::too_many_arguments)]
-    fn evaluate_split(
-        &self,
-        left_gradient: f32,
-        left_hessian: f32,
-        right_gradient: f32,
-        right_hessian: f32,
-        missing_gradient: f32,
-        missing_hessian: f32,
-        lower_bound: f32,
-        upper_bound: f32,
-        constraint: Option<&Constraint>,
-    ) -> Option<(NodeInfo, NodeInfo, MissingInfo)> {
-        // If there is no info right, or there is no
-        // info left, we will possibly lead to a missing only
-        // split, if we don't want this, bomb.
-        if ((left_gradient == 0.0) && (left_hessian == 0.0)
-            || (right_gradient == 0.0) && (right_hessian == 0.0))
-            && !self.allow_missing_splits
-        {
-            return None;
-        }
-
-        // By default missing values will go into the right node.
-        let mut missing_info = MissingInfo::Right;
-
-        let mut left_gradient = left_gradient;
-        let mut left_hessian = left_hessian;
-
-        let mut right_gradient = right_gradient;
-        let mut right_hessian = right_hessian;
-
-        let mut left_weight = constrained_weight(
-            &self.l2,
-            left_gradient,
-            left_hessian,
-            lower_bound,
-            upper_bound,
-            constraint,
-        );
-        let mut right_weight = constrained_weight(
-            &self.l2,
-            right_gradient,
-            right_hessian,
-            lower_bound,
-            upper_bound,
-            constraint,
-        );
-
-        let mut left_gain = gain_given_weight(&self.l2, left_gradient, left_hessian, left_weight);
-        let mut right_gain =
-            gain_given_weight(&self.l2, right_gradient, right_hessian, right_weight);
-
-        if !self.allow_missing_splits {
-            // Check the min_hessian constraint first, if we do not
-            // want to allow missing only splits.
-            if (right_hessian < self.min_leaf_weight) || (left_hessian < self.min_leaf_weight) {
-                // Update for new value
-                return None;
-            }
-        }
-
-        // Check Missing direction
-        // Don't even worry about it, if there are no missing values
-        // in this bin.
-        if (missing_gradient != 0.0) || (missing_hessian != 0.0) {
-            // TODO: Consider making this safer, by casting to f64, summing, and then
-            // back to f32...
-
-            // The weight if missing went left
-            let missing_left_weight = constrained_weight(
-                &self.l2,
-                left_gradient + missing_gradient,
-                left_hessian + missing_hessian,
-                lower_bound,
-                upper_bound,
-                constraint,
-            );
-            // The gain if missing went left
-            let missing_left_gain = gain_given_weight(
-                &self.l2,
-                left_gradient + missing_gradient,
-                left_hessian + missing_hessian,
-                missing_left_weight,
-            );
-            // Confirm this wouldn't break monotonicity.
-            let missing_left_gain = cull_gain(
-                missing_left_gain,
-                missing_left_weight,
-                right_weight,
-                constraint,
-            );
-
-            // The gain if missing went right
-            let missing_right_weight = weight(
-                &self.l2,
-                right_gradient + missing_gradient,
-                right_hessian + missing_hessian,
-            );
-            // The gain is missing went right
-            let missing_right_gain = gain_given_weight(
-                &self.l2,
-                right_gradient + missing_gradient,
-                right_hessian + missing_hessian,
-                missing_right_weight,
-            );
-            // Confirm this wouldn't break monotonicity.
-            let missing_left_gain = cull_gain(
-                missing_left_gain,
-                missing_left_weight,
-                right_weight,
-                constraint,
-            );
-
-            if (missing_right_gain - right_gain) < (missing_left_gain - left_gain) {
-                // Missing goes left
-                left_gradient += missing_gradient;
-                left_hessian += missing_hessian;
-                left_gain = missing_left_gain;
-                left_weight = missing_left_weight;
-                missing_info = MissingInfo::Left;
-            } else {
-                // Missing goes right
-                right_gradient += missing_gradient;
-                right_hessian += missing_hessian;
-                right_gain = missing_right_gain;
-                right_weight = missing_right_weight;
-                missing_info = MissingInfo::Right;
-            }
-        }
-
-        if (right_hessian < self.min_leaf_weight) || (left_hessian < self.min_leaf_weight) {
-            // Update for new value
-            return None;
-        }
-        Some((
-            NodeInfo {
-                grad: left_gradient,
-                gain: left_gain,
-                cover: left_hessian,
-                weight: left_weight * self.learning_rate,
-                bounds: (f32::NEG_INFINITY, f32::INFINITY),
-            },
-            NodeInfo {
-                grad: right_gradient,
-                gain: right_gain,
-                cover: right_hessian,
-                weight: right_weight * self.learning_rate,
-                bounds: (f32::NEG_INFINITY, f32::INFINITY),
-            },
-            missing_info,
-        ))
-    }
-
-    fn handle_split_info(
-        &self,
-        split_info: SplitInfo,
-        n_nodes: &usize,
-        node: &mut SplittableNode,
-        index: &mut [usize],
-        data: &Matrix<u16>,
-        cuts: &JaggedMatrix<f64>,
-        grad: &[f32],
-        hess: &[f32],
-        parallel: bool,
-    ) -> Vec<SplittableNode> {
-        let left_child = *n_nodes;
-        let right_child = left_child + 1;
-
-        let missing_right = match split_info.missing_node {
-            MissingInfo::Left => false,
-            MissingInfo::Right => true,
-            _ => unreachable!(),
-        };
-
-        // We need to move all of the index's above and below our
-        // split value.
-        // pivot the sub array that this node has on our split value
-        // Here we assign missing to a specific direction.
-        // This will need to be refactored once we add a
-        // separate missing branch.
-        let mut split_idx = pivot_on_split(
-            &mut index[node.start_idx..node.stop_idx],
-            data.get_col(split_info.split_feature),
-            split_info.split_bin,
-            missing_right,
-        );
-        // Calculate histograms
-        let total_recs = node.stop_idx - node.start_idx;
-        let n_right = total_recs - split_idx;
-        let n_left = total_recs - n_right;
-
-        // Now that we have calculated the number of records
-        // add the start index, to make the split_index
-        // relative to the entire index array
-        split_idx += node.start_idx;
-
-        // Build the histograms for the smaller node.
-        let left_histograms: HistogramMatrix;
-        let right_histograms: HistogramMatrix;
-        if n_left < n_right {
-            left_histograms = HistogramMatrix::new(
-                data,
-                cuts,
-                grad,
-                hess,
-                &index[node.start_idx..split_idx],
-                parallel,
-                true,
-            );
-            right_histograms =
-                HistogramMatrix::from_parent_child(&node.histograms, &left_histograms);
-        } else {
-            right_histograms = HistogramMatrix::new(
-                data,
-                cuts,
-                grad,
-                hess,
-                &index[split_idx..node.stop_idx],
-                parallel,
-                true,
-            );
-            left_histograms =
-                HistogramMatrix::from_parent_child(&node.histograms, &right_histograms);
-        }
-        let missing_child = if missing_right {
-            right_child
-        } else {
-            left_child
-        };
-        node.update_children(missing_child, left_child, right_child, &split_info);
-
-        let left_node = SplittableNode::from_node_info(
-            left_child,
-            left_histograms,
-            node.depth + 1,
-            node.start_idx,
-            split_idx,
-            split_info.left_node,
-        );
-        let right_node = SplittableNode::from_node_info(
-            right_child,
-            right_histograms,
-            node.depth + 1,
-            split_idx,
-            node.stop_idx,
-            split_info.right_node,
-        );
-        vec![left_node, right_node]
-    }
-
-    fn get_constraint(&self, feature: &usize) -> Option<&Constraint> {
-        self.constraints_map.get(feature)
-    }
-
-    fn get_gamma(&self) -> f32 {
-        self.gamma
-    }
-
-    fn get_l2(&self) -> f32 {
-        self.l2
-    }
-}
-
-#[cfg(test)]
-mod tests {
-    use super::*;
-    use crate::binning::bin_matrix;
-    use crate::data::Matrix;
-    use crate::node::SplittableNode;
-    use crate::objective::{LogLoss, ObjectiveFunction};
-    use crate::utils::gain;
-    use std::fs;
-    #[test]
-    fn test_best_feature_split() {
-        let d = vec![4., 2., 3., 4., 5., 1., 4.];
-        let data = Matrix::new(&d, 7, 1);
-        let y = vec![0., 0., 0., 1., 1., 0., 1.];
-        let yhat = vec![0.; 7];
-        let w = vec![1.; y.len()];
-        let grad = LogLoss::calc_grad(&y, &yhat, &w);
-        let hess = LogLoss::calc_hess(&y, &yhat, &w);
-        let b = bin_matrix(&data, &w, 10, f64::NAN).unwrap();
-        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
-        let index = data.index.to_owned();
-        let hists = HistogramMatrix::new(&bdata, &b.cuts, &grad, &hess, &index, true, true);
-        let splitter = MissingImputerSplitter {
-            l2: 0.0,
-            gamma: 0.0,
-            min_leaf_weight: 0.0,
-            learning_rate: 1.0,
-            allow_missing_splits: true,
-            constraints_map: ConstraintMap::new(),
-        };
-        // println!("{:?}", hists);
-        let mut n = SplittableNode::new(
-            0,
-            // vec![0, 1, 2, 3, 4, 5, 6],
-            hists,
-            0.0,
-            0.14,
-            grad.iter().sum::<f32>(),
-            hess.iter().sum::<f32>(),
-            0,
-            0,
-            grad.len(),
-            f32::NEG_INFINITY,
-            f32::INFINITY,
-        );
-        let s = splitter.best_feature_split(&mut n, 0).unwrap();
-        println!("{:?}", s);
-        assert_eq!(s.split_value, 4.0);
-        assert_eq!(s.left_node.cover, 0.75);
-        assert_eq!(s.right_node.cover, 1.0);
-        assert_eq!(s.left_node.gain, 3.0);
-        assert_eq!(s.right_node.gain, 1.0);
-        assert_eq!(s.split_gain, 3.86);
-    }
-
-    #[test]
-    fn test_best_split() {
-        let d: Vec<f64> = vec![0., 0., 0., 1., 0., 0., 0., 4., 2., 3., 4., 5., 1., 4.];
-        let data = Matrix::new(&d, 7, 2);
-        let y = vec![0., 0., 0., 1., 1., 0., 1.];
-        let yhat = vec![0.; 7];
-        let w = vec![1.; y.len()];
-        let grad = LogLoss::calc_grad(&y, &yhat, &w);
-        let hess = LogLoss::calc_hess(&y, &yhat, &w);
-
-        let b = bin_matrix(&data, &w, 10, f64::NAN).unwrap();
-        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
-        let index = data.index.to_owned();
-        let hists = HistogramMatrix::new(&bdata, &b.cuts, &grad, &hess, &index, true, true);
-        println!("{:?}", hists);
-        let splitter = MissingImputerSplitter {
-            l2: 0.0,
-            gamma: 0.0,
-            min_leaf_weight: 0.0,
-            learning_rate: 1.0,
-            allow_missing_splits: true,
-            constraints_map: ConstraintMap::new(),
-        };
-        let mut n = SplittableNode::new(
-            0,
-            // vec![0, 1, 2, 3, 4, 5, 6],
-            hists,
-            0.0,
-            0.14,
-            grad.iter().sum::<f32>(),
-            hess.iter().sum::<f32>(),
-            0,
-            0,
-            grad.len(),
-            f32::NEG_INFINITY,
-            f32::INFINITY,
-        );
-        let s = splitter.best_split(&mut n).unwrap();
-        println!("{:?}", s);
-        assert_eq!(s.split_feature, 1);
-        assert_eq!(s.split_value, 4.);
-        assert_eq!(s.left_node.cover, 0.75);
-        assert_eq!(s.right_node.cover, 1.);
-        assert_eq!(s.left_node.gain, 3.);
-        assert_eq!(s.right_node.gain, 1.);
-        assert_eq!(s.split_gain, 3.86);
-    }
-
-    #[test]
-    fn test_data_split() {
-        let file = fs::read_to_string("resources/contiguous_no_missing.csv")
-            .expect("Something went wrong reading the file");
-        let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
-        let file = fs::read_to_string("resources/performance.csv")
-            .expect("Something went wrong reading the file");
-        let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
-        let yhat = vec![0.5; y.len()];
-        let w = vec![1.; y.len()];
-        let grad = LogLoss::calc_grad(&y, &yhat, &w);
-        let hess = LogLoss::calc_hess(&y, &yhat, &w);
-
-        let splitter = MissingImputerSplitter {
-            l2: 1.0,
-            gamma: 3.0,
-            min_leaf_weight: 1.0,
-            learning_rate: 0.3,
-            allow_missing_splits: true,
-            constraints_map: ConstraintMap::new(),
-        };
-        let gradient_sum = grad.iter().copied().sum();
-        let hessian_sum = hess.iter().copied().sum();
-        let root_gain = gain(&splitter.l2, gradient_sum, hessian_sum);
-        let root_weight = weight(&splitter.l2, gradient_sum, hessian_sum);
-        // let gain_given_weight = splitter.gain_given_weight(gradient_sum, hessian_sum, root_weight);
-        // println!("gain: {}, weight: {}, gain from weight: {}", root_gain, root_weight, gain_given_weight);
-        let data = Matrix::new(&data_vec, 891, 5);
-
-        let b = bin_matrix(&data, &w, 10, f64::NAN).unwrap();
-        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
-        let index = data.index.to_owned();
-        let hists = HistogramMatrix::new(&bdata, &b.cuts, &grad, &hess, &index, true, false);
-
-        let mut n = SplittableNode::new(
-            0,
-            // (0..(data.rows - 1)).collect(),
-            hists,
-            root_weight,
-            root_gain,
-            grad.iter().copied().sum::<f32>(),
-            hess.iter().copied().sum::<f32>(),
-            0,
-            0,
-            grad.len(),
-            f32::NEG_INFINITY,
-            f32::INFINITY,
-        );
-        let s = splitter.best_split(&mut n).unwrap();
-        println!("{:?}", s);
-        n.update_children(2, 1, 2, &s);
-        assert_eq!(0, s.split_feature);
-    }
-}
+use crate::constraints::{Constraint, ConstraintMap};
+use crate::data::{JaggedMatrix, Matrix};
+use crate::histogram::HistogramMatrix;
+use crate::node::SplittableNode;
+use crate::utils::{
+    constrained_weight, cull_gain, gain_given_weight, pivot_on_split,
+    pivot_on_split_exclude_missing, weight,
+};
+
+#[derive(Debug)]
+pub struct SplitInfo {
+    pub split_gain: f32,
+    pub split_feature: usize,
+    pub split_value: f64,
+    pub split_bin: u16,
+    pub left_node: NodeInfo,
+    pub right_node: NodeInfo,
+    pub missing_node: MissingInfo,
+}
+
+#[derive(Debug)]
+pub struct NodeInfo {
+    pub grad: f32,
+    pub gain: f32,
+    pub cover: f32,
+    pub weight: f32,
+    pub bounds: (f32, f32),
+}
+
+#[derive(Debug)]
+pub enum MissingInfo {
+    Left,
+    Right,
+    Leaf(NodeInfo),
+    Branch(NodeInfo),
+}
+
+pub trait Splitter {
+    fn get_constraint(&self, feature: &usize) -> Option<&Constraint>;
+    // fn get_allow_missing_splits(&self) -> bool;
+    fn get_gamma(&self) -> f32;
+    fn get_l2(&self) -> f32;
+
+    /// Find the best possible split, considering all feature histograms.
+    /// If we wanted to add Column sampling, this is probably where
+    /// we would need to do it, otherwise, it would be at the tree level.
+    fn best_split(&self, node: &SplittableNode) -> Option<SplitInfo> {
+        let mut best_split_info = None;
+        let mut best_gain = 0.0;
+        let HistogramMatrix(histograms) = &node.histograms;
+        for i in 0..histograms.cols {
+            let split_info = self.best_feature_split(node, i);
+            match split_info {
+                Some(info) => {
+                    if info.split_gain > best_gain {
+                        best_gain = info.split_gain;
+                        best_split_info = Some(info);
+                    }
+                }
+                None => continue,
+            }
+        }
+        best_split_info
+    }
+
+    /// Evaluate a split, returning the node info for the left, and right splits,
+    /// as well as the node info the missing data of a feature.
+    #[allow(clippy::too_many_arguments)]
+    fn evaluate_split(
+        &self,
+        left_gradient: f32,
+        left_hessian: f32,
+        right_gradient: f32,
+        right_hessian: f32,
+        missing_gradient: f32,
+        missing_hessian: f32,
+        lower_bound: f32,
+        upper_bound: f32,
+        constraint: Option<&Constraint>,
+    ) -> Option<(NodeInfo, NodeInfo, MissingInfo)>;
+
+    fn best_feature_split(&self, node: &SplittableNode, feature: usize) -> Option<SplitInfo> {
+        let mut split_info: Option<SplitInfo> = None;
+        let mut max_gain: Option<f32> = None;
+
+        let HistogramMatrix(histograms) = &node.histograms;
+        let histogram = histograms.get_col(feature);
+
+        // We also know we will have a missing bin.
+        let missing = &histogram[0];
+        let mut cuml_grad = 0.0; // first_bin.gradient_sum;
+        let mut cuml_hess = 0.0; // first_bin.hessian_sum;
+        let constraint = self.get_constraint(&feature);
+
+        let elements = histogram.len();
+        assert!(elements == histogram.len());
+
+        for (i, bin) in histogram[1..].iter().enumerate() {
+            let left_gradient = cuml_grad;
+            let left_hessian = cuml_hess;
+            let right_gradient = node.gradient_sum - cuml_grad - missing.gradient_sum;
+            let right_hessian = node.hessian_sum - cuml_hess - missing.hessian_sum;
+
+            let (mut left_node_info, mut right_node_info, missing_info) = match self.evaluate_split(
+                left_gradient,
+                left_hessian,
+                right_gradient,
+                right_hessian,
+                missing.gradient_sum,
+                missing.hessian_sum,
+                node.lower_bound,
+                node.upper_bound,
+                constraint,
+            ) {
+                None => {
+                    cuml_grad += bin.gradient_sum;
+                    cuml_hess += bin.hessian_sum;
+                    continue;
+                }
+                Some(v) => v,
+            };
+
+            // TODO!
+            // Should we be doing this?
+            // or should missing gain not factor in at
+            // all to the split gain?
+            let missing_gain = match &missing_info {
+                MissingInfo::Branch(v) | MissingInfo::Leaf(v) => v.gain,
+                _ => 0.0,
+            };
+            let split_gain = (left_node_info.gain + right_node_info.gain + missing_gain
+                - node.gain_value)
+                - self.get_gamma();
+
+            // Check monotonicity holds
+            let split_gain = cull_gain(
+                split_gain,
+                left_node_info.weight,
+                right_node_info.weight,
+                constraint,
+            );
+
+            if split_gain <= 0.0 {
+                // Update for new value
+                cuml_grad += bin.gradient_sum;
+                cuml_hess += bin.hessian_sum;
+                continue;
+            }
+
+            let mid = (left_node_info.weight + right_node_info.weight) / 2.0;
+            let (left_bounds, right_bounds) = match constraint {
+                None | Some(Constraint::Unconstrained) => (
+                    (node.lower_bound, node.upper_bound),
+                    (node.lower_bound, node.upper_bound),
+                ),
+                Some(Constraint::Negative) => ((mid, node.upper_bound), (node.lower_bound, mid)),
+                Some(Constraint::Positive) => ((node.lower_bound, mid), (mid, node.upper_bound)),
+            };
+            left_node_info.bounds = left_bounds;
+            right_node_info.bounds = right_bounds;
+
+            // If split gain is NaN, one of the sides is empty, do not allow
+            // this split.
+            let split_gain = if split_gain.is_nan() { 0.0 } else { split_gain };
+            if max_gain.is_none() || split_gain > max_gain.unwrap() {
+                max_gain = Some(split_gain);
+                split_info = Some(SplitInfo {
+                    split_gain,
+                    split_feature: feature,
+                    split_value: bin.cut_value,
+                    split_bin: (i + 1) as u16,
+                    left_node: left_node_info,
+                    right_node: right_node_info,
+                    missing_node: missing_info,
+                });
+            }
+            // Update for new value
+            cuml_grad += bin.gradient_sum;
+            cuml_hess += bin.hessian_sum;
+        }
+        split_info
+    }
+
+    /// Handle the split info, creating the children nodes, this function
+    /// will return a vector of new splitable nodes, that can be added to the
+    /// growable stack, and further split, or converted to leaf nodes.
+    #[allow(clippy::too_many_arguments)]
+    fn handle_split_info(
+        &self,
+        split_info: SplitInfo,
+        n_nodes: &usize,
+        node: &mut SplittableNode,
+        index: &mut [usize],
+        data: &Matrix<u16>,
+        cuts: &JaggedMatrix<f64>,
+        grad: &[f32],
+        hess: &[f32],
+        parallel: bool,
+    ) -> Vec<SplittableNode>;
+
+    /// Split the node, if we cant find a best split, we will need to
+    /// return an empty vector, this node is a leaf.
+    #[allow(clippy::too_many_arguments)]
+    fn split_node(
+        &self,
+        n_nodes: &usize,
+        node: &mut SplittableNode,
+        index: &mut [usize],
+        data: &Matrix<u16>,
+        cuts: &JaggedMatrix<f64>,
+        grad: &[f32],
+        hess: &[f32],
+        parallel: bool,
+    ) -> Vec<SplittableNode> {
+        match self.best_split(node) {
+            Some(split_info) => self.handle_split_info(
+                split_info, n_nodes, node, index, data, cuts, grad, hess, parallel,
+            ),
+            None => Vec::new(),
+        }
+    }
+}
+
+/// Missing branch splitter
+/// Always creates a separate branch for the missing values of a feature.
+/// This results, in every node having a specific "missing", direction.
+/// If this node is able, it will be split further, otherwise it will
+/// a leaf node will be generated.
+pub struct MissingBranchSplitter {
+    pub l2: f32,
+    pub gamma: f32,
+    pub min_leaf_weight: f32,
+    pub learning_rate: f32,
+    pub allow_missing_splits: bool,
+    pub constraints_map: ConstraintMap,
+}
+
+impl Splitter for MissingBranchSplitter {
+    fn get_constraint(&self, feature: &usize) -> Option<&Constraint> {
+        self.constraints_map.get(feature)
+    }
+
+    fn get_gamma(&self) -> f32 {
+        self.gamma
+    }
+
+    fn get_l2(&self) -> f32 {
+        self.l2
+    }
+
+    fn evaluate_split(
+        &self,
+        left_gradient: f32,
+        left_hessian: f32,
+        right_gradient: f32,
+        right_hessian: f32,
+        missing_gradient: f32,
+        missing_hessian: f32,
+        lower_bound: f32,
+        upper_bound: f32,
+        constraint: Option<&Constraint>,
+    ) -> Option<(NodeInfo, NodeInfo, MissingInfo)> {
+        // If there is no info right, or there is no
+        // info left, there is nothing to split on,
+        // and so we should continue.
+        if (left_gradient == 0.0) && (left_hessian == 0.0)
+            || (right_gradient == 0.0) && (right_hessian == 0.0)
+        {
+            return None;
+        }
+
+        let left_gradient = left_gradient;
+        let left_hessian = left_hessian;
+
+        let right_gradient = right_gradient;
+        let right_hessian = right_hessian;
+
+        let left_weight = constrained_weight(
+            &self.l2,
+            left_gradient,
+            left_hessian,
+            lower_bound,
+            upper_bound,
+            constraint,
+        );
+        let right_weight = constrained_weight(
+            &self.l2,
+            right_gradient,
+            right_hessian,
+            lower_bound,
+            upper_bound,
+            constraint,
+        );
+
+        let left_gain = gain_given_weight(&self.l2, left_gradient, left_hessian, left_weight);
+        let right_gain = gain_given_weight(&self.l2, right_gradient, right_hessian, right_weight);
+
+        // Check the min_hessian constraint first
+        if (right_hessian < self.min_leaf_weight) || (left_hessian < self.min_leaf_weight) {
+            // Update for new value
+            return None;
+        }
+
+        // We have not considered missing at all up until this point, we could if we wanted
+        // to give more predictive power probably to missing.
+        // If we don't want to allow the missing branch to be split further,
+        // we will default to creating an empty branch.
+
+        // Set weight to the parent weight...
+        let missing_weight = weight(
+            &self.get_l2(),
+            missing_gradient + left_gradient + right_gradient,
+            missing_hessian + left_hessian + right_hessian,
+        ); // weight(&self.get_l2(), missing_gradient, missing_hessian);
+        let missing_gain = gain_given_weight(
+            &self.get_l2(),
+            missing_gradient,
+            missing_hessian,
+            missing_weight,
+        );
+        let missing_info = NodeInfo {
+            grad: missing_gradient,
+            gain: missing_gain,
+            cover: missing_hessian,
+            weight: missing_weight * self.learning_rate,
+            bounds: (f32::NEG_INFINITY, f32::INFINITY),
+        };
+        let missing_node = // Check Missing direction
+        if ((missing_gradient != 0.0) || (missing_hessian != 0.0)) && self.allow_missing_splits {
+            MissingInfo::Branch(
+                missing_info
+            )
+        } else {
+            MissingInfo::Leaf(
+                missing_info
+            )
+        };
+
+        if (right_hessian < self.min_leaf_weight) || (left_hessian < self.min_leaf_weight) {
+            // Update for new value
+            return None;
+        }
+        Some((
+            NodeInfo {
+                grad: left_gradient,
+                gain: left_gain,
+                cover: left_hessian,
+                weight: left_weight * self.learning_rate,
+                bounds: (f32::NEG_INFINITY, f32::INFINITY),
+            },
+            NodeInfo {
+                grad: right_gradient,
+                gain: right_gain,
+                cover: right_hessian,
+                weight: right_weight * self.learning_rate,
+                bounds: (f32::NEG_INFINITY, f32::INFINITY),
+            },
+            missing_node,
+        ))
+    }
+
+    fn handle_split_info(
+        &self,
+        split_info: SplitInfo,
+        n_nodes: &usize,
+        node: &mut SplittableNode,
+        index: &mut [usize],
+        data: &Matrix<u16>,
+        cuts: &JaggedMatrix<f64>,
+        grad: &[f32],
+        hess: &[f32],
+        parallel: bool,
+    ) -> Vec<SplittableNode> {
+        let missing_child = *n_nodes;
+        let left_child = missing_child + 1;
+        let right_child = missing_child + 2;
+        node.update_children(missing_child, left_child, right_child, &split_info);
+
+        let (missing_is_leaf, mut missing_info) = match split_info.missing_node {
+            MissingInfo::Branch(i) => (false, i),
+            MissingInfo::Leaf(i) => (true, i),
+            _ => unreachable!(),
+        };
+        // Set missing weight to parent weight value...
+        // This essentially neutralizes missing.
+        // Manually calculating it, was leading to some small numeric
+        // rounding differences...
+        missing_info.weight = node.weight_value;
+
+        // We need to move all of the index's above and below our
+        // split value.
+        // pivot the sub array that this node has on our split value
+        // Missing all falls to the bottom.
+        let (mut missing_split_idx, mut split_idx) = pivot_on_split_exclude_missing(
+            &mut index[node.start_idx..node.stop_idx],
+            data.get_col(split_info.split_feature),
+            split_info.split_bin,
+        );
+        // Calculate histograms
+        let total_recs = node.stop_idx - node.start_idx;
+        let n_right = total_recs - split_idx;
+        let n_left = total_recs - n_right - missing_split_idx;
+        let n_missing = total_recs - (n_right + n_left);
+        let max_ = match vec![n_missing, n_left, n_right]
+            .iter()
+            .enumerate()
+            .max_by(|(_, i), (_, j)| i.cmp(j))
+        {
+            Some((i, _)) => i,
+            // if we can't compare them, it doesn't
+            // really matter, build the histogram on
+            // any of them.
+            None => 0,
+        };
+
+        // Now that we have calculated the number of records
+        // add the start index, to make the split_index
+        // relative to the entire index array
+        split_idx += node.start_idx;
+        missing_split_idx += node.start_idx;
+
+        // Build the histograms for the smaller node.
+        let left_histograms: HistogramMatrix;
+        let right_histograms: HistogramMatrix;
+        let missing_histograms: HistogramMatrix;
+        if n_missing == 0 {
+            if max_ == 1 {
+                missing_histograms = HistogramMatrix::empty();
+                right_histograms = HistogramMatrix::new(
+                    data,
+                    cuts,
+                    grad,
+                    hess,
+                    &index[split_idx..node.stop_idx],
+                    parallel,
+                    true,
+                );
+                left_histograms =
+                    HistogramMatrix::from_parent_child(&node.histograms, &right_histograms);
+            } else {
+                missing_histograms = HistogramMatrix::empty();
+                left_histograms = HistogramMatrix::new(
+                    data,
+                    cuts,
+                    grad,
+                    hess,
+                    &index[missing_split_idx..split_idx],
+                    parallel,
+                    true,
+                );
+                right_histograms =
+                    HistogramMatrix::from_parent_child(&node.histograms, &left_histograms);
+            }
+        } else if max_ == 0 {
+            // Max is missing, calculate the other two
+            // levels histograms.
+            left_histograms = HistogramMatrix::new(
+                data,
+                cuts,
+                grad,
+                hess,
+                &index[missing_split_idx..split_idx],
+                parallel,
+                true,
+            );
+            right_histograms = HistogramMatrix::new(
+                data,
+                cuts,
+                grad,
+                hess,
+                &index[split_idx..node.stop_idx],
+                parallel,
+                true,
+            );
+            missing_histograms = HistogramMatrix::from_parent_two_children(
+                &node.histograms,
+                &left_histograms,
+                &right_histograms,
+            )
+        } else if max_ == 1 {
+            missing_histograms = HistogramMatrix::new(
+                data,
+                cuts,
+                grad,
+                hess,
+                &index[node.start_idx..missing_split_idx],
+                parallel,
+                true,
+            );
+            right_histograms = HistogramMatrix::new(
+                data,
+                cuts,
+                grad,
+                hess,
+                &index[split_idx..node.stop_idx],
+                parallel,
+                true,
+            );
+            left_histograms = HistogramMatrix::from_parent_two_children(
+                &node.histograms,
+                &missing_histograms,
+                &right_histograms,
+            )
+        } else {
+            // right is the largest
+
+            missing_histograms = HistogramMatrix::new(
+                data,
+                cuts,
+                grad,
+                hess,
+                &index[node.start_idx..missing_split_idx],
+                parallel,
+                true,
+            );
+            left_histograms = HistogramMatrix::new(
+                data,
+                cuts,
+                grad,
+                hess,
+                &index[missing_split_idx..split_idx],
+                parallel,
+                true,
+            );
+            right_histograms = HistogramMatrix::from_parent_two_children(
+                &node.histograms,
+                &missing_histograms,
+                &left_histograms,
+            )
+        }
+
+        let mut missing_node = SplittableNode::from_node_info(
+            missing_child,
+            missing_histograms,
+            node.depth + 1,
+            node.start_idx,
+            missing_split_idx,
+            missing_info,
+        );
+        missing_node.is_missing_leaf = missing_is_leaf;
+        let left_node = SplittableNode::from_node_info(
+            left_child,
+            left_histograms,
+            node.depth + 1,
+            missing_split_idx,
+            split_idx,
+            split_info.left_node,
+        );
+        let right_node = SplittableNode::from_node_info(
+            right_child,
+            right_histograms,
+            node.depth + 1,
+            split_idx,
+            node.stop_idx,
+            split_info.right_node,
+        );
+        vec![missing_node, left_node, right_node]
+    }
+}
+
+/// Missing imputer splitter
+/// Splitter that imputes missing values, by sending
+/// them down either the right or left branch, depending
+/// on which results in a higher increase in gain.
+pub struct MissingImputerSplitter {
+    pub l2: f32,
+    pub gamma: f32,
+    pub min_leaf_weight: f32,
+    pub learning_rate: f32,
+    pub allow_missing_splits: bool,
+    pub constraints_map: ConstraintMap,
+}
+
+impl MissingImputerSplitter {
+    /// Generate a new missing imputer splitter object.
+    pub fn new(
+        l2: f32,
+        gamma: f32,
+        min_leaf_weight: f32,
+        learning_rate: f32,
+        allow_missing_splits: bool,
+        constraints_map: ConstraintMap,
+    ) -> Self {
+        MissingImputerSplitter {
+            l2,
+            gamma,
+            min_leaf_weight,
+            learning_rate,
+            allow_missing_splits,
+            constraints_map,
+        }
+    }
+}
+
+impl Splitter for MissingImputerSplitter {
+    #[allow(clippy::too_many_arguments)]
+    fn evaluate_split(
+        &self,
+        left_gradient: f32,
+        left_hessian: f32,
+        right_gradient: f32,
+        right_hessian: f32,
+        missing_gradient: f32,
+        missing_hessian: f32,
+        lower_bound: f32,
+        upper_bound: f32,
+        constraint: Option<&Constraint>,
+    ) -> Option<(NodeInfo, NodeInfo, MissingInfo)> {
+        // If there is no info right, or there is no
+        // info left, we will possibly lead to a missing only
+        // split, if we don't want this, bomb.
+        if ((left_gradient == 0.0) && (left_hessian == 0.0)
+            || (right_gradient == 0.0) && (right_hessian == 0.0))
+            && !self.allow_missing_splits
+        {
+            return None;
+        }
+
+        // By default missing values will go into the right node.
+        let mut missing_info = MissingInfo::Right;
+
+        let mut left_gradient = left_gradient;
+        let mut left_hessian = left_hessian;
+
+        let mut right_gradient = right_gradient;
+        let mut right_hessian = right_hessian;
+
+        let mut left_weight = constrained_weight(
+            &self.l2,
+            left_gradient,
+            left_hessian,
+            lower_bound,
+            upper_bound,
+            constraint,
+        );
+        let mut right_weight = constrained_weight(
+            &self.l2,
+            right_gradient,
+            right_hessian,
+            lower_bound,
+            upper_bound,
+            constraint,
+        );
+
+        let mut left_gain = gain_given_weight(&self.l2, left_gradient, left_hessian, left_weight);
+        let mut right_gain =
+            gain_given_weight(&self.l2, right_gradient, right_hessian, right_weight);
+
+        if !self.allow_missing_splits {
+            // Check the min_hessian constraint first, if we do not
+            // want to allow missing only splits.
+            if (right_hessian < self.min_leaf_weight) || (left_hessian < self.min_leaf_weight) {
+                // Update for new value
+                return None;
+            }
+        }
+
+        // Check Missing direction
+        // Don't even worry about it, if there are no missing values
+        // in this bin.
+        if (missing_gradient != 0.0) || (missing_hessian != 0.0) {
+            // TODO: Consider making this safer, by casting to f64, summing, and then
+            // back to f32...
+
+            // The weight if missing went left
+            let missing_left_weight = constrained_weight(
+                &self.l2,
+                left_gradient + missing_gradient,
+                left_hessian + missing_hessian,
+                lower_bound,
+                upper_bound,
+                constraint,
+            );
+            // The gain if missing went left
+            let missing_left_gain = gain_given_weight(
+                &self.l2,
+                left_gradient + missing_gradient,
+                left_hessian + missing_hessian,
+                missing_left_weight,
+            );
+            // Confirm this wouldn't break monotonicity.
+            let missing_left_gain = cull_gain(
+                missing_left_gain,
+                missing_left_weight,
+                right_weight,
+                constraint,
+            );
+
+            // The gain if missing went right
+            let missing_right_weight = weight(
+                &self.l2,
+                right_gradient + missing_gradient,
+                right_hessian + missing_hessian,
+            );
+            // The gain is missing went right
+            let missing_right_gain = gain_given_weight(
+                &self.l2,
+                right_gradient + missing_gradient,
+                right_hessian + missing_hessian,
+                missing_right_weight,
+            );
+            // Confirm this wouldn't break monotonicity.
+            let missing_left_gain = cull_gain(
+                missing_left_gain,
+                missing_left_weight,
+                right_weight,
+                constraint,
+            );
+
+            if (missing_right_gain - right_gain) < (missing_left_gain - left_gain) {
+                // Missing goes left
+                left_gradient += missing_gradient;
+                left_hessian += missing_hessian;
+                left_gain = missing_left_gain;
+                left_weight = missing_left_weight;
+                missing_info = MissingInfo::Left;
+            } else {
+                // Missing goes right
+                right_gradient += missing_gradient;
+                right_hessian += missing_hessian;
+                right_gain = missing_right_gain;
+                right_weight = missing_right_weight;
+                missing_info = MissingInfo::Right;
+            }
+        }
+
+        if (right_hessian < self.min_leaf_weight) || (left_hessian < self.min_leaf_weight) {
+            // Update for new value
+            return None;
+        }
+        Some((
+            NodeInfo {
+                grad: left_gradient,
+                gain: left_gain,
+                cover: left_hessian,
+                weight: left_weight * self.learning_rate,
+                bounds: (f32::NEG_INFINITY, f32::INFINITY),
+            },
+            NodeInfo {
+                grad: right_gradient,
+                gain: right_gain,
+                cover: right_hessian,
+                weight: right_weight * self.learning_rate,
+                bounds: (f32::NEG_INFINITY, f32::INFINITY),
+            },
+            missing_info,
+        ))
+    }
+
+    fn handle_split_info(
+        &self,
+        split_info: SplitInfo,
+        n_nodes: &usize,
+        node: &mut SplittableNode,
+        index: &mut [usize],
+        data: &Matrix<u16>,
+        cuts: &JaggedMatrix<f64>,
+        grad: &[f32],
+        hess: &[f32],
+        parallel: bool,
+    ) -> Vec<SplittableNode> {
+        let left_child = *n_nodes;
+        let right_child = left_child + 1;
+
+        let missing_right = match split_info.missing_node {
+            MissingInfo::Left => false,
+            MissingInfo::Right => true,
+            _ => unreachable!(),
+        };
+
+        // We need to move all of the index's above and below our
+        // split value.
+        // pivot the sub array that this node has on our split value
+        // Here we assign missing to a specific direction.
+        // This will need to be refactored once we add a
+        // separate missing branch.
+        let mut split_idx = pivot_on_split(
+            &mut index[node.start_idx..node.stop_idx],
+            data.get_col(split_info.split_feature),
+            split_info.split_bin,
+            missing_right,
+        );
+        // Calculate histograms
+        let total_recs = node.stop_idx - node.start_idx;
+        let n_right = total_recs - split_idx;
+        let n_left = total_recs - n_right;
+
+        // Now that we have calculated the number of records
+        // add the start index, to make the split_index
+        // relative to the entire index array
+        split_idx += node.start_idx;
+
+        // Build the histograms for the smaller node.
+        let left_histograms: HistogramMatrix;
+        let right_histograms: HistogramMatrix;
+        if n_left < n_right {
+            left_histograms = HistogramMatrix::new(
+                data,
+                cuts,
+                grad,
+                hess,
+                &index[node.start_idx..split_idx],
+                parallel,
+                true,
+            );
+            right_histograms =
+                HistogramMatrix::from_parent_child(&node.histograms, &left_histograms);
+        } else {
+            right_histograms = HistogramMatrix::new(
+                data,
+                cuts,
+                grad,
+                hess,
+                &index[split_idx..node.stop_idx],
+                parallel,
+                true,
+            );
+            left_histograms =
+                HistogramMatrix::from_parent_child(&node.histograms, &right_histograms);
+        }
+        let missing_child = if missing_right {
+            right_child
+        } else {
+            left_child
+        };
+        node.update_children(missing_child, left_child, right_child, &split_info);
+
+        let left_node = SplittableNode::from_node_info(
+            left_child,
+            left_histograms,
+            node.depth + 1,
+            node.start_idx,
+            split_idx,
+            split_info.left_node,
+        );
+        let right_node = SplittableNode::from_node_info(
+            right_child,
+            right_histograms,
+            node.depth + 1,
+            split_idx,
+            node.stop_idx,
+            split_info.right_node,
+        );
+        vec![left_node, right_node]
+    }
+
+    fn get_constraint(&self, feature: &usize) -> Option<&Constraint> {
+        self.constraints_map.get(feature)
+    }
+
+    fn get_gamma(&self) -> f32 {
+        self.gamma
+    }
+
+    fn get_l2(&self) -> f32 {
+        self.l2
+    }
+}
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+    use crate::binning::bin_matrix;
+    use crate::data::Matrix;
+    use crate::node::SplittableNode;
+    use crate::objective::{LogLoss, ObjectiveFunction};
+    use crate::utils::gain;
+    use std::fs;
+    #[test]
+    fn test_best_feature_split() {
+        let d = vec![4., 2., 3., 4., 5., 1., 4.];
+        let data = Matrix::new(&d, 7, 1);
+        let y = vec![0., 0., 0., 1., 1., 0., 1.];
+        let yhat = vec![0.; 7];
+        let w = vec![1.; y.len()];
+        let grad = LogLoss::calc_grad(&y, &yhat, &w);
+        let hess = LogLoss::calc_hess(&y, &yhat, &w);
+        let b = bin_matrix(&data, &w, 10, f64::NAN).unwrap();
+        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
+        let index = data.index.to_owned();
+        let hists = HistogramMatrix::new(&bdata, &b.cuts, &grad, &hess, &index, true, true);
+        let splitter = MissingImputerSplitter {
+            l2: 0.0,
+            gamma: 0.0,
+            min_leaf_weight: 0.0,
+            learning_rate: 1.0,
+            allow_missing_splits: true,
+            constraints_map: ConstraintMap::new(),
+        };
+        // println!("{:?}", hists);
+        let mut n = SplittableNode::new(
+            0,
+            // vec![0, 1, 2, 3, 4, 5, 6],
+            hists,
+            0.0,
+            0.14,
+            grad.iter().sum::<f32>(),
+            hess.iter().sum::<f32>(),
+            0,
+            0,
+            grad.len(),
+            f32::NEG_INFINITY,
+            f32::INFINITY,
+        );
+        let s = splitter.best_feature_split(&mut n, 0).unwrap();
+        println!("{:?}", s);
+        assert_eq!(s.split_value, 4.0);
+        assert_eq!(s.left_node.cover, 0.75);
+        assert_eq!(s.right_node.cover, 1.0);
+        assert_eq!(s.left_node.gain, 3.0);
+        assert_eq!(s.right_node.gain, 1.0);
+        assert_eq!(s.split_gain, 3.86);
+    }
+
+    #[test]
+    fn test_best_split() {
+        let d: Vec<f64> = vec![0., 0., 0., 1., 0., 0., 0., 4., 2., 3., 4., 5., 1., 4.];
+        let data = Matrix::new(&d, 7, 2);
+        let y = vec![0., 0., 0., 1., 1., 0., 1.];
+        let yhat = vec![0.; 7];
+        let w = vec![1.; y.len()];
+        let grad = LogLoss::calc_grad(&y, &yhat, &w);
+        let hess = LogLoss::calc_hess(&y, &yhat, &w);
+
+        let b = bin_matrix(&data, &w, 10, f64::NAN).unwrap();
+        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
+        let index = data.index.to_owned();
+        let hists = HistogramMatrix::new(&bdata, &b.cuts, &grad, &hess, &index, true, true);
+        println!("{:?}", hists);
+        let splitter = MissingImputerSplitter {
+            l2: 0.0,
+            gamma: 0.0,
+            min_leaf_weight: 0.0,
+            learning_rate: 1.0,
+            allow_missing_splits: true,
+            constraints_map: ConstraintMap::new(),
+        };
+        let mut n = SplittableNode::new(
+            0,
+            // vec![0, 1, 2, 3, 4, 5, 6],
+            hists,
+            0.0,
+            0.14,
+            grad.iter().sum::<f32>(),
+            hess.iter().sum::<f32>(),
+            0,
+            0,
+            grad.len(),
+            f32::NEG_INFINITY,
+            f32::INFINITY,
+        );
+        let s = splitter.best_split(&mut n).unwrap();
+        println!("{:?}", s);
+        assert_eq!(s.split_feature, 1);
+        assert_eq!(s.split_value, 4.);
+        assert_eq!(s.left_node.cover, 0.75);
+        assert_eq!(s.right_node.cover, 1.);
+        assert_eq!(s.left_node.gain, 3.);
+        assert_eq!(s.right_node.gain, 1.);
+        assert_eq!(s.split_gain, 3.86);
+    }
+
+    #[test]
+    fn test_data_split() {
+        let file = fs::read_to_string("resources/contiguous_no_missing.csv")
+            .expect("Something went wrong reading the file");
+        let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+        let file = fs::read_to_string("resources/performance.csv")
+            .expect("Something went wrong reading the file");
+        let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+        let yhat = vec![0.5; y.len()];
+        let w = vec![1.; y.len()];
+        let grad = LogLoss::calc_grad(&y, &yhat, &w);
+        let hess = LogLoss::calc_hess(&y, &yhat, &w);
+
+        let splitter = MissingImputerSplitter {
+            l2: 1.0,
+            gamma: 3.0,
+            min_leaf_weight: 1.0,
+            learning_rate: 0.3,
+            allow_missing_splits: true,
+            constraints_map: ConstraintMap::new(),
+        };
+        let gradient_sum = grad.iter().copied().sum();
+        let hessian_sum = hess.iter().copied().sum();
+        let root_gain = gain(&splitter.l2, gradient_sum, hessian_sum);
+        let root_weight = weight(&splitter.l2, gradient_sum, hessian_sum);
+        // let gain_given_weight = splitter.gain_given_weight(gradient_sum, hessian_sum, root_weight);
+        // println!("gain: {}, weight: {}, gain from weight: {}", root_gain, root_weight, gain_given_weight);
+        let data = Matrix::new(&data_vec, 891, 5);
+
+        let b = bin_matrix(&data, &w, 10, f64::NAN).unwrap();
+        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
+        let index = data.index.to_owned();
+        let hists = HistogramMatrix::new(&bdata, &b.cuts, &grad, &hess, &index, true, false);
+
+        let mut n = SplittableNode::new(
+            0,
+            // (0..(data.rows - 1)).collect(),
+            hists,
+            root_weight,
+            root_gain,
+            grad.iter().copied().sum::<f32>(),
+            hess.iter().copied().sum::<f32>(),
+            0,
+            0,
+            grad.len(),
+            f32::NEG_INFINITY,
+            f32::INFINITY,
+        );
+        let s = splitter.best_split(&mut n).unwrap();
+        println!("{:?}", s);
+        n.update_children(2, 1, 2, &s);
+        assert_eq!(0, s.split_feature);
+    }
+}
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/src/tree.rs` & `forust-0.2.7/local_dependencies/forust-ml/src/tree.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,624 +1,613 @@
-use crate::data::{JaggedMatrix, Matrix};
-use crate::histogram::HistogramMatrix;
-use crate::node::{Node, SplittableNode};
-use crate::partial_dependence::tree_partial_dependence;
-use crate::splitter::Splitter;
-use crate::utils::fast_f64_sum;
-use crate::utils::{gain, weight};
-use rand::rngs::StdRng;
-use rand::Rng;
-use rayon::prelude::*;
-use serde::{Deserialize, Serialize};
-use std::collections::VecDeque;
-use std::fmt::{self, Display};
-
-#[derive(Deserialize, Serialize)]
-pub struct Tree {
-    pub nodes: Vec<Node>,
-}
-
-impl Default for Tree {
-    fn default() -> Self {
-        Self::new()
-    }
-}
-
-impl Tree {
-    pub fn new() -> Self {
-        Tree { nodes: Vec::new() }
-    }
-
-    #[allow(clippy::too_many_arguments)]
-    pub fn fit<T: Splitter>(
-        &mut self,
-        data: &Matrix<u16>,
-        cuts: &JaggedMatrix<f64>,
-        grad: &[f32],
-        hess: &[f32],
-        splitter: &T,
-        max_leaves: usize,
-        max_depth: usize,
-        parallel: bool,
-        subsample: f32,
-        rng: &mut StdRng,
-    ) {
-        // Recreating the index for each tree, ensures that the tree construction is faster
-        // for the root node. This also ensures that sorting the records is always fast,
-        // because we are starting from a nearly sorted array.
-        let (mut index, gradient_sum, hessian_sum, sort) = if subsample == 1. {
-            // We don't need to sort, if we are not sampling. This is because
-            // the data is already sorted.
-            (
-                data.index.to_owned(),
-                fast_f64_sum(grad),
-                fast_f64_sum(hess),
-                false,
-            )
-        } else {
-            // Accumulate using f64 for numeric fidelity.
-            let mut gs: f64 = 0.;
-            let mut hs: f64 = 0.;
-            let mut index = Vec::new();
-            for ((i, g), h) in data
-                .index
-                .iter()
-                .zip(grad)
-                .zip(hess)
-                .filter(|_| rng.gen_range(0.0..1.0) < subsample)
-            {
-                index.push(*i);
-                gs += *g as f64;
-                hs += *h as f64;
-            }
-            (index, gs as f32, hs as f32, true)
-        };
-
-        let mut n_nodes = 1;
-        let root_gain = gain(&splitter.get_l2(), gradient_sum, hessian_sum);
-        let root_weight = weight(&splitter.get_l2(), gradient_sum, hessian_sum);
-        // Calculate the histograms for the root node.
-        let root_hists = HistogramMatrix::new(data, cuts, grad, hess, &index, parallel, sort);
-        let root_node = SplittableNode::new(
-            0,
-            root_hists,
-            root_weight,
-            root_gain,
-            gradient_sum,
-            hessian_sum,
-            0,
-            0,
-            index.len(),
-            f32::NEG_INFINITY,
-            f32::INFINITY,
-        );
-        // Add the first node to the tree nodes.
-        self.nodes.push(root_node.as_node());
-        let mut n_leaves = 1;
-        let mut growable: VecDeque<SplittableNode> = VecDeque::new();
-        growable.push_front(root_node);
-        while !growable.is_empty() {
-            if n_leaves >= max_leaves {
-                break;
-            }
-
-            // We know there is a value here, because of how the
-            // while loop is setup.
-            // Grab a splitable node from the stack
-            // If we can split it, and update the corresponding
-            // tree nodes children.
-            let mut node = growable
-                .pop_back()
-                .expect("Growable buffer should not be empty.");
-            let n_idx = node.num;
-            // This will only be splittable nodes
-
-            let depth = node.depth + 1;
-
-            // If we have hit max depth, skip this node
-            // but keep going, because there may be other
-            // valid shallower nodes.
-            if depth > max_depth {
-                // self.nodes[n_idx] = node.as_leaf_node();
-                continue;
-            }
-
-            // For max_leaves, subtract 1 from the n_leaves
-            // every time we pop from the growable stack
-            // then, if we can add two children, add two to
-            // n_leaves. If we can't split the node any
-            // more, then just add 1 back to n_leaves
-            n_leaves -= 1;
-
-            let new_nodes = splitter.split_node(
-                &n_nodes, &mut node, &mut index, data, cuts, grad, hess, parallel,
-            );
-
-            let n_new_nodes = new_nodes.len();
-            if n_new_nodes == 0 {
-                n_leaves += 1;
-            } else {
-                self.nodes[n_idx].make_parent_node(node);
-                n_leaves += n_new_nodes;
-                n_nodes += n_new_nodes;
-                for n in new_nodes {
-                    self.nodes.push(n.as_node());
-                    if !n.is_missing_leaf {
-                        growable.push_front(n)
-                    }
-                }
-            }
-        }
-    }
-
-    pub fn predict_contributions_row_weight(
-        &self,
-        row: &[f64],
-        contribs: &mut [f64],
-        missing: &f64,
-    ) {
-        // Add the bias term first...
-        contribs[contribs.len() - 1] += self.nodes[0].weight_value as f64;
-        let mut node_idx = 0;
-        loop {
-            let node = &self.nodes[node_idx];
-            if node.is_leaf {
-                break;
-            }
-            // Get change of weight given child's weight.
-            let child_idx = node.get_child_idx(&row[node.split_feature], missing);
-            let node_weight = self.nodes[node_idx].weight_value as f64;
-            let child_weight = self.nodes[child_idx].weight_value as f64;
-            let delta = child_weight - node_weight;
-            contribs[node.split_feature] += delta;
-            node_idx = child_idx
-        }
-    }
-
-    fn predict_contributions_single_threaded_weight(
-        &self,
-        data: &Matrix<f64>,
-        contribs: &mut [f64],
-        missing: &f64,
-    ) {
-        // There needs to always be at least 2 trees
-        data.index
-            .iter()
-            .zip(contribs.chunks_mut(data.cols + 1))
-            .for_each(|(row, contribs)| {
-                self.predict_contributions_row_weight(&data.get_row(*row), contribs, missing)
-            })
-    }
-
-    fn predict_contributions_parallel_weight(
-        &self,
-        data: &Matrix<f64>,
-        contribs: &mut [f64],
-        missing: &f64,
-    ) {
-        // There needs to always be at least 2 trees
-        data.index
-            .par_iter()
-            .zip(contribs.par_chunks_mut(data.cols + 1))
-            .for_each(|(row, contribs)| {
-                self.predict_contributions_row_weight(&data.get_row(*row), contribs, missing)
-            })
-    }
-
-    pub fn predict_contributions_weight(
-        &self,
-        data: &Matrix<f64>,
-        contribs: &mut [f64],
-        parallel: bool,
-        missing: &f64,
-    ) {
-        if parallel {
-            self.predict_contributions_parallel_weight(data, contribs, missing)
-        } else {
-            self.predict_contributions_single_threaded_weight(data, contribs, missing)
-        }
-    }
-
-    /// This is the method that XGBoost uses.
-    pub fn predict_contributions_row_average(
-        &self,
-        row: &[f64],
-        contribs: &mut [f64],
-        weights: &[f64],
-        missing: &f64,
-    ) {
-        // Add the bias term first...
-        contribs[contribs.len() - 1] += weights[0];
-        let mut node_idx = 0;
-        loop {
-            let node = &self.nodes[node_idx];
-            if node.is_leaf {
-                break;
-            }
-            // Get change of weight given child's weight.
-            let child_idx = node.get_child_idx(&row[node.split_feature], missing);
-            let node_weight = weights[node_idx];
-            let child_weight = weights[child_idx];
-            let delta = child_weight - node_weight;
-            contribs[node.split_feature] += delta;
-            node_idx = child_idx
-        }
-    }
-
-    fn predict_contributions_single_threaded_average(
-        &self,
-        data: &Matrix<f64>,
-        contribs: &mut [f64],
-        weights: &[f64],
-        missing: &f64,
-    ) {
-        // There needs to always be at least 2 trees
-        data.index
-            .iter()
-            .zip(contribs.chunks_mut(data.cols + 1))
-            .for_each(|(row, contribs)| {
-                self.predict_contributions_row_average(
-                    &data.get_row(*row),
-                    contribs,
-                    weights,
-                    missing,
-                )
-            })
-    }
-
-    fn predict_contributions_parallel_average(
-        &self,
-        data: &Matrix<f64>,
-        contribs: &mut [f64],
-        weights: &[f64],
-        missing: &f64,
-    ) {
-        // There needs to always be at least 2 trees
-        data.index
-            .par_iter()
-            .zip(contribs.par_chunks_mut(data.cols + 1))
-            .for_each(|(row, contribs)| {
-                self.predict_contributions_row_average(
-                    &data.get_row(*row),
-                    contribs,
-                    weights,
-                    missing,
-                )
-            })
-    }
-
-    pub fn predict_contributions_average(
-        &self,
-        data: &Matrix<f64>,
-        contribs: &mut [f64],
-        weights: &[f64],
-        parallel: bool,
-        missing: &f64,
-    ) {
-        if parallel {
-            self.predict_contributions_parallel_average(data, contribs, weights, missing)
-        } else {
-            self.predict_contributions_single_threaded_average(data, contribs, weights, missing)
-        }
-    }
-
-    fn predict_row(&self, data: &Matrix<f64>, row: usize, missing: &f64) -> f64 {
-        let mut node_idx = 0;
-        loop {
-            let node = &self.nodes[node_idx];
-            if node.is_leaf {
-                return node.weight_value as f64;
-            } else {
-                node_idx = node.get_child_idx(data.get(row, node.split_feature), missing);
-            }
-        }
-    }
-
-    pub fn predict_row_from_row_slice(&self, row: &[f64], missing: &f64) -> f64 {
-        let mut node_idx = 0;
-        loop {
-            let node = &self.nodes[node_idx];
-            if node.is_leaf {
-                return node.weight_value as f64;
-            } else {
-                node_idx = node.get_child_idx(&row[node.split_feature], missing);
-            }
-        }
-    }
-
-    fn predict_single_threaded(&self, data: &Matrix<f64>, missing: &f64) -> Vec<f64> {
-        data.index
-            .iter()
-            .map(|i| self.predict_row(data, *i, missing))
-            .collect()
-    }
-
-    fn predict_parallel(&self, data: &Matrix<f64>, missing: &f64) -> Vec<f64> {
-        data.index
-            .par_iter()
-            .map(|i| self.predict_row(data, *i, missing))
-            .collect()
-    }
-
-    pub fn predict(&self, data: &Matrix<f64>, parallel: bool, missing: &f64) -> Vec<f64> {
-        if parallel {
-            self.predict_parallel(data, missing)
-        } else {
-            self.predict_single_threaded(data, missing)
-        }
-    }
-
-    pub fn value_partial_dependence(&self, feature: usize, value: f64, missing: &f64) -> f64 {
-        tree_partial_dependence(self, 0, feature, value, 1.0, missing)
-    }
-    fn distribute_node_leaf_weights(&self, i: usize, weights: &mut [f64]) -> f64 {
-        let node = &self.nodes[i];
-        let mut w = node.weight_value as f64;
-        if !node.is_leaf {
-            let left_node = &self.nodes[node.left_child];
-            let right_node = &self.nodes[node.right_child];
-            w = left_node.hessian_sum as f64
-                * self.distribute_node_leaf_weights(node.left_child, weights);
-            w += right_node.hessian_sum as f64
-                * self.distribute_node_leaf_weights(node.right_child, weights);
-            // If this a tree with a missing branch.
-            if node.has_missing_branch() {
-                let missing_node = &self.nodes[node.missing_node];
-                w += missing_node.hessian_sum as f64
-                    * self.distribute_node_leaf_weights(node.missing_node, weights);
-            }
-            w /= node.hessian_sum as f64;
-        }
-        weights[i] = w;
-        w
-    }
-    pub fn distribute_leaf_weights(&self) -> Vec<f64> {
-        let mut weights = vec![0.; self.nodes.len()];
-        self.distribute_node_leaf_weights(0, &mut weights);
-        weights
-    }
-}
-
-impl Display for Tree {
-    // This trait requires `fmt` with this exact signature.
-    fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
-        let mut print_buffer: Vec<usize> = vec![0];
-        let mut r = String::new();
-        while !print_buffer.is_empty() {
-            // This will always be populated, because we confirm
-            // that the buffer is not empty.
-            let idx = print_buffer.pop().unwrap();
-            let node = &self.nodes[idx];
-            if node.is_leaf {
-                r += format!("{}{}\n", "      ".repeat(node.depth).as_str(), node).as_str();
-            } else {
-                r += format!("{}{}\n", "      ".repeat(node.depth).as_str(), node).as_str();
-                print_buffer.push(node.right_child);
-                print_buffer.push(node.left_child);
-                if node.has_missing_branch() {
-                    print_buffer.push(node.missing_node);
-                }
-            }
-        }
-        write!(f, "{}", r)
-    }
-}
-
-#[cfg(test)]
-mod tests {
-    use super::*;
-    use crate::binning::bin_matrix;
-    use crate::constraints::{Constraint, ConstraintMap};
-    use crate::objective::{LogLoss, ObjectiveFunction};
-    use crate::splitter::MissingImputerSplitter;
-    use crate::utils::precision_round;
-    use rand::rngs::StdRng;
-    use rand::SeedableRng;
-    use std::fs;
-    #[test]
-    fn test_tree_fit_with_subsample() {
-        let file = fs::read_to_string("resources/contiguous_no_missing.csv")
-            .expect("Something went wrong reading the file");
-        let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
-        let file = fs::read_to_string("resources/performance.csv")
-            .expect("Something went wrong reading the file");
-        let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
-        let yhat = vec![0.5; y.len()];
-        let w = vec![1.; y.len()];
-        let g = LogLoss::calc_grad(&y, &yhat, &w);
-        let h = LogLoss::calc_hess(&y, &yhat, &w);
-
-        let data = Matrix::new(&data_vec, 891, 5);
-        let splitter = MissingImputerSplitter {
-            l2: 1.0,
-            gamma: 3.0,
-            min_leaf_weight: 1.0,
-            learning_rate: 0.3,
-            allow_missing_splits: true,
-            constraints_map: ConstraintMap::new(),
-        };
-        let mut tree = Tree::new();
-
-        let b = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
-        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
-        let mut rng = StdRng::seed_from_u64(0);
-        tree.fit(
-            &bdata,
-            &b.cuts,
-            &g,
-            &h,
-            &splitter,
-            usize::MAX,
-            5,
-            true,
-            0.5,
-            &mut rng,
-        );
-    }
-
-    #[test]
-    fn test_tree_fit() {
-        let file = fs::read_to_string("resources/contiguous_no_missing.csv")
-            .expect("Something went wrong reading the file");
-        let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
-        let file = fs::read_to_string("resources/performance.csv")
-            .expect("Something went wrong reading the file");
-        let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
-        let yhat = vec![0.5; y.len()];
-        let w = vec![1.; y.len()];
-        let g = LogLoss::calc_grad(&y, &yhat, &w);
-        let h = LogLoss::calc_hess(&y, &yhat, &w);
-
-        let data = Matrix::new(&data_vec, 891, 5);
-        let splitter = MissingImputerSplitter {
-            l2: 1.0,
-            gamma: 3.0,
-            min_leaf_weight: 1.0,
-            learning_rate: 0.3,
-            allow_missing_splits: true,
-            constraints_map: ConstraintMap::new(),
-        };
-        let mut tree = Tree::new();
-
-        let b = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
-        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
-        let mut rng = StdRng::seed_from_u64(0);
-        tree.fit(
-            &bdata,
-            &b.cuts,
-            &g,
-            &h,
-            &splitter,
-            usize::MAX,
-            5,
-            true,
-            1.,
-            &mut rng,
-        );
-
-        // println!("{}", tree);
-        // let preds = tree.predict(&data, false);
-        // println!("{:?}", &preds[0..10]);
-        assert_eq!(25, tree.nodes.len());
-        // Test contributions prediction...
-        let weights = tree.distribute_leaf_weights();
-        let mut contribs = vec![0.; (data.cols + 1) * data.rows];
-        tree.predict_contributions_average(&data, &mut contribs, &weights, false, &f64::NAN);
-        let full_preds = tree.predict(&data, true, &f64::NAN);
-        assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
-
-        let contribs_preds: Vec<f64> = contribs
-            .chunks(data.cols + 1)
-            .map(|i| i.iter().sum())
-            .collect();
-        println!("{:?}", &contribs[0..10]);
-        println!("{:?}", &contribs_preds[0..10]);
-
-        assert_eq!(contribs_preds.len(), full_preds.len());
-        for (i, j) in full_preds.iter().zip(contribs_preds) {
-            assert_eq!(precision_round(*i, 7), precision_round(j, 7));
-        }
-
-        // Weight contributions
-        let mut contribs = vec![0.; (data.cols + 1) * data.rows];
-        tree.predict_contributions_weight(&data, &mut contribs, false, &f64::NAN);
-        let full_preds = tree.predict(&data, true, &f64::NAN);
-        assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
-
-        let contribs_preds: Vec<f64> = contribs
-            .chunks(data.cols + 1)
-            .map(|i| i.iter().sum())
-            .collect();
-        println!("{:?}", &contribs[0..10]);
-        println!("{:?}", &contribs_preds[0..10]);
-
-        assert_eq!(contribs_preds.len(), full_preds.len());
-        for (i, j) in full_preds.iter().zip(contribs_preds) {
-            assert_eq!(precision_round(*i, 7), precision_round(j, 7));
-        }
-    }
-
-    #[test]
-    fn test_tree_fit_monotone() {
-        let file = fs::read_to_string("resources/contiguous_no_missing.csv")
-            .expect("Something went wrong reading the file");
-        let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
-        let file = fs::read_to_string("resources/performance.csv")
-            .expect("Something went wrong reading the file");
-        let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
-        let yhat = vec![0.5; y.len()];
-        let w = vec![1.; y.len()];
-        let g = LogLoss::calc_grad(&y, &yhat, &w);
-        let h = LogLoss::calc_hess(&y, &yhat, &w);
-        println!("GRADIENT -- {:?}", h);
-
-        let data_ = Matrix::new(&data_vec, 891, 5);
-        let data = Matrix::new(data_.get_col(1), 891, 1);
-        let map = ConstraintMap::from([(0, Constraint::Negative)]);
-        let splitter = MissingImputerSplitter {
-            l2: 1.0,
-            gamma: 0.0,
-            min_leaf_weight: 1.0,
-            learning_rate: 0.3,
-            allow_missing_splits: true,
-            constraints_map: map,
-        };
-        let mut tree = Tree::new();
-
-        let b = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
-        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
-
-        let mut rng = StdRng::seed_from_u64(0);
-        tree.fit(
-            &bdata,
-            &b.cuts,
-            &g,
-            &h,
-            &splitter,
-            usize::MAX,
-            5,
-            true,
-            1.,
-            &mut rng,
-        );
-
-        // println!("{}", tree);
-        let mut pred_data_vec = data.get_col(0).to_owned();
-        pred_data_vec.sort_by(|a, b| a.partial_cmp(b).unwrap());
-        pred_data_vec.dedup();
-        let pred_data = Matrix::new(&pred_data_vec, pred_data_vec.len(), 1);
-
-        let preds = tree.predict(&pred_data, false, &f64::NAN);
-        let increasing = preds.windows(2).all(|a| a[0] >= a[1]);
-        assert!(increasing);
-
-        let weights = tree.distribute_leaf_weights();
-
-        // Average contributions
-        let mut contribs = vec![0.; (data.cols + 1) * data.rows];
-        tree.predict_contributions_average(&data, &mut contribs, &weights, false, &f64::NAN);
-        let full_preds = tree.predict(&data, true, &f64::NAN);
-        assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
-        let contribs_preds: Vec<f64> = contribs
-            .chunks(data.cols + 1)
-            .map(|i| i.iter().sum())
-            .collect();
-        assert_eq!(contribs_preds.len(), full_preds.len());
-        for (i, j) in full_preds.iter().zip(contribs_preds) {
-            assert_eq!(precision_round(*i, 7), precision_round(j, 7));
-        }
-
-        // Weight contributions
-        let mut contribs = vec![0.; (data.cols + 1) * data.rows];
-        tree.predict_contributions_weight(&data, &mut contribs, false, &f64::NAN);
-        let full_preds = tree.predict(&data, true, &f64::NAN);
-        assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
-        let contribs_preds: Vec<f64> = contribs
-            .chunks(data.cols + 1)
-            .map(|i| i.iter().sum())
-            .collect();
-        assert_eq!(contribs_preds.len(), full_preds.len());
-        for (i, j) in full_preds.iter().zip(contribs_preds) {
-            assert_eq!(precision_round(*i, 7), precision_round(j, 7));
-        }
-    }
-}
+use crate::data::{JaggedMatrix, Matrix};
+use crate::histogram::HistogramMatrix;
+use crate::node::{Node, SplittableNode};
+use crate::partial_dependence::tree_partial_dependence;
+use crate::sampler::SampleMethod;
+use crate::splitter::Splitter;
+use crate::utils::fast_f64_sum;
+use crate::utils::{gain, weight};
+use rayon::prelude::*;
+use serde::{Deserialize, Serialize};
+use std::collections::VecDeque;
+use std::fmt::{self, Display};
+
+#[derive(Deserialize, Serialize)]
+pub struct Tree {
+    pub nodes: Vec<Node>,
+}
+
+impl Default for Tree {
+    fn default() -> Self {
+        Self::new()
+    }
+}
+
+impl Tree {
+    pub fn new() -> Self {
+        Tree { nodes: Vec::new() }
+    }
+
+    #[allow(clippy::too_many_arguments)]
+    pub fn fit<T: Splitter>(
+        &mut self,
+        data: &Matrix<u16>,
+        mut index: Vec<usize>,
+        cuts: &JaggedMatrix<f64>,
+        grad: &[f32],
+        hess: &[f32],
+        splitter: &T,
+        max_leaves: usize,
+        max_depth: usize,
+        parallel: bool,
+        sample_method: &SampleMethod,
+    ) {
+        // Recreating the index for each tree, ensures that the tree construction is faster
+        // for the root node. This also ensures that sorting the records is always fast,
+        // because we are starting from a nearly sorted array.
+        let (gradient_sum, hessian_sum, sort) = match sample_method {
+            // We don't need to sort, if we are not sampling. This is because
+            // the data is already sorted.
+            SampleMethod::None => (fast_f64_sum(grad), fast_f64_sum(hess), false),
+            _ => {
+                // Accumulate using f64 for numeric fidelity.
+                let mut gs: f64 = 0.;
+                let mut hs: f64 = 0.;
+                for i in index.iter() {
+                    let i_ = *i;
+                    gs += grad[i_] as f64;
+                    hs += hess[i_] as f64;
+                }
+                (gs as f32, hs as f32, true)
+            }
+        };
+
+        let mut n_nodes = 1;
+        let root_gain = gain(&splitter.get_l2(), gradient_sum, hessian_sum);
+        let root_weight = weight(&splitter.get_l2(), gradient_sum, hessian_sum);
+        // Calculate the histograms for the root node.
+        let root_hists = HistogramMatrix::new(data, cuts, grad, hess, &index, parallel, sort);
+        let root_node = SplittableNode::new(
+            0,
+            root_hists,
+            root_weight,
+            root_gain,
+            gradient_sum,
+            hessian_sum,
+            0,
+            0,
+            index.len(),
+            f32::NEG_INFINITY,
+            f32::INFINITY,
+        );
+        // Add the first node to the tree nodes.
+        self.nodes.push(root_node.as_node());
+        let mut n_leaves = 1;
+        let mut growable: VecDeque<SplittableNode> = VecDeque::new();
+        growable.push_front(root_node);
+        while !growable.is_empty() {
+            if n_leaves >= max_leaves {
+                break;
+            }
+
+            // We know there is a value here, because of how the
+            // while loop is setup.
+            // Grab a splitable node from the stack
+            // If we can split it, and update the corresponding
+            // tree nodes children.
+            let mut node = growable
+                .pop_back()
+                .expect("Growable buffer should not be empty.");
+            let n_idx = node.num;
+            // This will only be splittable nodes
+
+            let depth = node.depth + 1;
+
+            // If we have hit max depth, skip this node
+            // but keep going, because there may be other
+            // valid shallower nodes.
+            if depth > max_depth {
+                // self.nodes[n_idx] = node.as_leaf_node();
+                continue;
+            }
+
+            // For max_leaves, subtract 1 from the n_leaves
+            // every time we pop from the growable stack
+            // then, if we can add two children, add two to
+            // n_leaves. If we can't split the node any
+            // more, then just add 1 back to n_leaves
+            n_leaves -= 1;
+
+            let new_nodes = splitter.split_node(
+                &n_nodes, &mut node, &mut index, data, cuts, grad, hess, parallel,
+            );
+
+            let n_new_nodes = new_nodes.len();
+            if n_new_nodes == 0 {
+                n_leaves += 1;
+            } else {
+                self.nodes[n_idx].make_parent_node(node);
+                n_leaves += n_new_nodes;
+                n_nodes += n_new_nodes;
+                for n in new_nodes {
+                    self.nodes.push(n.as_node());
+                    if !n.is_missing_leaf {
+                        growable.push_front(n)
+                    }
+                }
+            }
+        }
+    }
+
+    pub fn predict_contributions_row_weight(
+        &self,
+        row: &[f64],
+        contribs: &mut [f64],
+        missing: &f64,
+    ) {
+        // Add the bias term first...
+        contribs[contribs.len() - 1] += self.nodes[0].weight_value as f64;
+        let mut node_idx = 0;
+        loop {
+            let node = &self.nodes[node_idx];
+            if node.is_leaf {
+                break;
+            }
+            // Get change of weight given child's weight.
+            let child_idx = node.get_child_idx(&row[node.split_feature], missing);
+            let node_weight = self.nodes[node_idx].weight_value as f64;
+            let child_weight = self.nodes[child_idx].weight_value as f64;
+            let delta = child_weight - node_weight;
+            contribs[node.split_feature] += delta;
+            node_idx = child_idx
+        }
+    }
+
+    fn predict_contributions_single_threaded_weight(
+        &self,
+        data: &Matrix<f64>,
+        contribs: &mut [f64],
+        missing: &f64,
+    ) {
+        // There needs to always be at least 2 trees
+        data.index
+            .iter()
+            .zip(contribs.chunks_mut(data.cols + 1))
+            .for_each(|(row, contribs)| {
+                self.predict_contributions_row_weight(&data.get_row(*row), contribs, missing)
+            })
+    }
+
+    fn predict_contributions_parallel_weight(
+        &self,
+        data: &Matrix<f64>,
+        contribs: &mut [f64],
+        missing: &f64,
+    ) {
+        // There needs to always be at least 2 trees
+        data.index
+            .par_iter()
+            .zip(contribs.par_chunks_mut(data.cols + 1))
+            .for_each(|(row, contribs)| {
+                self.predict_contributions_row_weight(&data.get_row(*row), contribs, missing)
+            })
+    }
+
+    pub fn predict_contributions_weight(
+        &self,
+        data: &Matrix<f64>,
+        contribs: &mut [f64],
+        parallel: bool,
+        missing: &f64,
+    ) {
+        if parallel {
+            self.predict_contributions_parallel_weight(data, contribs, missing)
+        } else {
+            self.predict_contributions_single_threaded_weight(data, contribs, missing)
+        }
+    }
+
+    /// This is the method that XGBoost uses.
+    pub fn predict_contributions_row_average(
+        &self,
+        row: &[f64],
+        contribs: &mut [f64],
+        weights: &[f64],
+        missing: &f64,
+    ) {
+        // Add the bias term first...
+        contribs[contribs.len() - 1] += weights[0];
+        let mut node_idx = 0;
+        loop {
+            let node = &self.nodes[node_idx];
+            if node.is_leaf {
+                break;
+            }
+            // Get change of weight given child's weight.
+            let child_idx = node.get_child_idx(&row[node.split_feature], missing);
+            let node_weight = weights[node_idx];
+            let child_weight = weights[child_idx];
+            let delta = child_weight - node_weight;
+            contribs[node.split_feature] += delta;
+            node_idx = child_idx
+        }
+    }
+
+    fn predict_contributions_single_threaded_average(
+        &self,
+        data: &Matrix<f64>,
+        contribs: &mut [f64],
+        weights: &[f64],
+        missing: &f64,
+    ) {
+        // There needs to always be at least 2 trees
+        data.index
+            .iter()
+            .zip(contribs.chunks_mut(data.cols + 1))
+            .for_each(|(row, contribs)| {
+                self.predict_contributions_row_average(
+                    &data.get_row(*row),
+                    contribs,
+                    weights,
+                    missing,
+                )
+            })
+    }
+
+    fn predict_contributions_parallel_average(
+        &self,
+        data: &Matrix<f64>,
+        contribs: &mut [f64],
+        weights: &[f64],
+        missing: &f64,
+    ) {
+        // There needs to always be at least 2 trees
+        data.index
+            .par_iter()
+            .zip(contribs.par_chunks_mut(data.cols + 1))
+            .for_each(|(row, contribs)| {
+                self.predict_contributions_row_average(
+                    &data.get_row(*row),
+                    contribs,
+                    weights,
+                    missing,
+                )
+            })
+    }
+
+    pub fn predict_contributions_average(
+        &self,
+        data: &Matrix<f64>,
+        contribs: &mut [f64],
+        weights: &[f64],
+        parallel: bool,
+        missing: &f64,
+    ) {
+        if parallel {
+            self.predict_contributions_parallel_average(data, contribs, weights, missing)
+        } else {
+            self.predict_contributions_single_threaded_average(data, contribs, weights, missing)
+        }
+    }
+
+    fn predict_row(&self, data: &Matrix<f64>, row: usize, missing: &f64) -> f64 {
+        let mut node_idx = 0;
+        loop {
+            let node = &self.nodes[node_idx];
+            if node.is_leaf {
+                return node.weight_value as f64;
+            } else {
+                node_idx = node.get_child_idx(data.get(row, node.split_feature), missing);
+            }
+        }
+    }
+
+    pub fn predict_row_from_row_slice(&self, row: &[f64], missing: &f64) -> f64 {
+        let mut node_idx = 0;
+        loop {
+            let node = &self.nodes[node_idx];
+            if node.is_leaf {
+                return node.weight_value as f64;
+            } else {
+                node_idx = node.get_child_idx(&row[node.split_feature], missing);
+            }
+        }
+    }
+
+    fn predict_single_threaded(&self, data: &Matrix<f64>, missing: &f64) -> Vec<f64> {
+        data.index
+            .iter()
+            .map(|i| self.predict_row(data, *i, missing))
+            .collect()
+    }
+
+    fn predict_parallel(&self, data: &Matrix<f64>, missing: &f64) -> Vec<f64> {
+        data.index
+            .par_iter()
+            .map(|i| self.predict_row(data, *i, missing))
+            .collect()
+    }
+
+    pub fn predict(&self, data: &Matrix<f64>, parallel: bool, missing: &f64) -> Vec<f64> {
+        if parallel {
+            self.predict_parallel(data, missing)
+        } else {
+            self.predict_single_threaded(data, missing)
+        }
+    }
+
+    pub fn value_partial_dependence(&self, feature: usize, value: f64, missing: &f64) -> f64 {
+        tree_partial_dependence(self, 0, feature, value, 1.0, missing)
+    }
+    fn distribute_node_leaf_weights(&self, i: usize, weights: &mut [f64]) -> f64 {
+        let node = &self.nodes[i];
+        let mut w = node.weight_value as f64;
+        if !node.is_leaf {
+            let left_node = &self.nodes[node.left_child];
+            let right_node = &self.nodes[node.right_child];
+            w = left_node.hessian_sum as f64
+                * self.distribute_node_leaf_weights(node.left_child, weights);
+            w += right_node.hessian_sum as f64
+                * self.distribute_node_leaf_weights(node.right_child, weights);
+            // If this a tree with a missing branch.
+            if node.has_missing_branch() {
+                let missing_node = &self.nodes[node.missing_node];
+                w += missing_node.hessian_sum as f64
+                    * self.distribute_node_leaf_weights(node.missing_node, weights);
+            }
+            w /= node.hessian_sum as f64;
+        }
+        weights[i] = w;
+        w
+    }
+    pub fn distribute_leaf_weights(&self) -> Vec<f64> {
+        let mut weights = vec![0.; self.nodes.len()];
+        self.distribute_node_leaf_weights(0, &mut weights);
+        weights
+    }
+}
+
+impl Display for Tree {
+    // This trait requires `fmt` with this exact signature.
+    fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
+        let mut print_buffer: Vec<usize> = vec![0];
+        let mut r = String::new();
+        while !print_buffer.is_empty() {
+            // This will always be populated, because we confirm
+            // that the buffer is not empty.
+            let idx = print_buffer.pop().unwrap();
+            let node = &self.nodes[idx];
+            if node.is_leaf {
+                r += format!("{}{}\n", "      ".repeat(node.depth).as_str(), node).as_str();
+            } else {
+                r += format!("{}{}\n", "      ".repeat(node.depth).as_str(), node).as_str();
+                print_buffer.push(node.right_child);
+                print_buffer.push(node.left_child);
+                if node.has_missing_branch() {
+                    print_buffer.push(node.missing_node);
+                }
+            }
+        }
+        write!(f, "{}", r)
+    }
+}
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+    use crate::binning::bin_matrix;
+    use crate::constraints::{Constraint, ConstraintMap};
+    use crate::objective::{LogLoss, ObjectiveFunction};
+    use crate::sampler::{RandomSampler, Sampler};
+    use crate::splitter::MissingImputerSplitter;
+    use crate::utils::precision_round;
+    use rand::rngs::StdRng;
+    use rand::SeedableRng;
+    use std::fs;
+    #[test]
+    fn test_tree_fit_with_subsample() {
+        let file = fs::read_to_string("resources/contiguous_no_missing.csv")
+            .expect("Something went wrong reading the file");
+        let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+        let file = fs::read_to_string("resources/performance.csv")
+            .expect("Something went wrong reading the file");
+        let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+        let yhat = vec![0.5; y.len()];
+        let w = vec![1.; y.len()];
+        let g = LogLoss::calc_grad(&y, &yhat, &w);
+        let h = LogLoss::calc_hess(&y, &yhat, &w);
+
+        let data = Matrix::new(&data_vec, 891, 5);
+        let splitter = MissingImputerSplitter {
+            l2: 1.0,
+            gamma: 3.0,
+            min_leaf_weight: 1.0,
+            learning_rate: 0.3,
+            allow_missing_splits: true,
+            constraints_map: ConstraintMap::new(),
+        };
+        let mut tree = Tree::new();
+
+        let b = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
+        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
+        let mut rng = StdRng::seed_from_u64(0);
+        let (index, excluded) = RandomSampler::new(0.5).sample(&mut rng, &data.index);
+        assert!(excluded.len() > 0);
+        tree.fit(
+            &bdata,
+            index,
+            &b.cuts,
+            &g,
+            &h,
+            &splitter,
+            usize::MAX,
+            5,
+            true,
+            &SampleMethod::Random,
+        );
+    }
+
+    #[test]
+    fn test_tree_fit() {
+        let file = fs::read_to_string("resources/contiguous_no_missing.csv")
+            .expect("Something went wrong reading the file");
+        let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+        let file = fs::read_to_string("resources/performance.csv")
+            .expect("Something went wrong reading the file");
+        let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+        let yhat = vec![0.5; y.len()];
+        let w = vec![1.; y.len()];
+        let g = LogLoss::calc_grad(&y, &yhat, &w);
+        let h = LogLoss::calc_hess(&y, &yhat, &w);
+
+        let data = Matrix::new(&data_vec, 891, 5);
+        let splitter = MissingImputerSplitter {
+            l2: 1.0,
+            gamma: 3.0,
+            min_leaf_weight: 1.0,
+            learning_rate: 0.3,
+            allow_missing_splits: true,
+            constraints_map: ConstraintMap::new(),
+        };
+        let mut tree = Tree::new();
+
+        let b = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
+        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
+        tree.fit(
+            &bdata,
+            data.index.to_owned(),
+            &b.cuts,
+            &g,
+            &h,
+            &splitter,
+            usize::MAX,
+            5,
+            true,
+            &SampleMethod::None,
+        );
+
+        // println!("{}", tree);
+        // let preds = tree.predict(&data, false);
+        // println!("{:?}", &preds[0..10]);
+        assert_eq!(25, tree.nodes.len());
+        // Test contributions prediction...
+        let weights = tree.distribute_leaf_weights();
+        let mut contribs = vec![0.; (data.cols + 1) * data.rows];
+        tree.predict_contributions_average(&data, &mut contribs, &weights, false, &f64::NAN);
+        let full_preds = tree.predict(&data, true, &f64::NAN);
+        assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
+
+        let contribs_preds: Vec<f64> = contribs
+            .chunks(data.cols + 1)
+            .map(|i| i.iter().sum())
+            .collect();
+        println!("{:?}", &contribs[0..10]);
+        println!("{:?}", &contribs_preds[0..10]);
+
+        assert_eq!(contribs_preds.len(), full_preds.len());
+        for (i, j) in full_preds.iter().zip(contribs_preds) {
+            assert_eq!(precision_round(*i, 7), precision_round(j, 7));
+        }
+
+        // Weight contributions
+        let mut contribs = vec![0.; (data.cols + 1) * data.rows];
+        tree.predict_contributions_weight(&data, &mut contribs, false, &f64::NAN);
+        let full_preds = tree.predict(&data, true, &f64::NAN);
+        assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
+
+        let contribs_preds: Vec<f64> = contribs
+            .chunks(data.cols + 1)
+            .map(|i| i.iter().sum())
+            .collect();
+        println!("{:?}", &contribs[0..10]);
+        println!("{:?}", &contribs_preds[0..10]);
+
+        assert_eq!(contribs_preds.len(), full_preds.len());
+        for (i, j) in full_preds.iter().zip(contribs_preds) {
+            assert_eq!(precision_round(*i, 7), precision_round(j, 7));
+        }
+    }
+
+    #[test]
+    fn test_tree_fit_monotone() {
+        let file = fs::read_to_string("resources/contiguous_no_missing.csv")
+            .expect("Something went wrong reading the file");
+        let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+        let file = fs::read_to_string("resources/performance.csv")
+            .expect("Something went wrong reading the file");
+        let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
+        let yhat = vec![0.5; y.len()];
+        let w = vec![1.; y.len()];
+        let g = LogLoss::calc_grad(&y, &yhat, &w);
+        let h = LogLoss::calc_hess(&y, &yhat, &w);
+        println!("GRADIENT -- {:?}", h);
+
+        let data_ = Matrix::new(&data_vec, 891, 5);
+        let data = Matrix::new(data_.get_col(1), 891, 1);
+        let map = ConstraintMap::from([(0, Constraint::Negative)]);
+        let splitter = MissingImputerSplitter {
+            l2: 1.0,
+            gamma: 0.0,
+            min_leaf_weight: 1.0,
+            learning_rate: 0.3,
+            allow_missing_splits: true,
+            constraints_map: map,
+        };
+        let mut tree = Tree::new();
+
+        let b = bin_matrix(&data, &w, 300, f64::NAN).unwrap();
+        let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
+
+        tree.fit(
+            &bdata,
+            data.index.to_owned(),
+            &b.cuts,
+            &g,
+            &h,
+            &splitter,
+            usize::MAX,
+            5,
+            true,
+            &SampleMethod::None,
+        );
+
+        // println!("{}", tree);
+        let mut pred_data_vec = data.get_col(0).to_owned();
+        pred_data_vec.sort_by(|a, b| a.partial_cmp(b).unwrap());
+        pred_data_vec.dedup();
+        let pred_data = Matrix::new(&pred_data_vec, pred_data_vec.len(), 1);
+
+        let preds = tree.predict(&pred_data, false, &f64::NAN);
+        let increasing = preds.windows(2).all(|a| a[0] >= a[1]);
+        assert!(increasing);
+
+        let weights = tree.distribute_leaf_weights();
+
+        // Average contributions
+        let mut contribs = vec![0.; (data.cols + 1) * data.rows];
+        tree.predict_contributions_average(&data, &mut contribs, &weights, false, &f64::NAN);
+        let full_preds = tree.predict(&data, true, &f64::NAN);
+        assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
+        let contribs_preds: Vec<f64> = contribs
+            .chunks(data.cols + 1)
+            .map(|i| i.iter().sum())
+            .collect();
+        assert_eq!(contribs_preds.len(), full_preds.len());
+        for (i, j) in full_preds.iter().zip(contribs_preds) {
+            assert_eq!(precision_round(*i, 7), precision_round(j, 7));
+        }
+
+        // Weight contributions
+        let mut contribs = vec![0.; (data.cols + 1) * data.rows];
+        tree.predict_contributions_weight(&data, &mut contribs, false, &f64::NAN);
+        let full_preds = tree.predict(&data, true, &f64::NAN);
+        assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
+        let contribs_preds: Vec<f64> = contribs
+            .chunks(data.cols + 1)
+            .map(|i| i.iter().sum())
+            .collect();
+        assert_eq!(contribs_preds.len(), full_preds.len());
+        for (i, j) in full_preds.iter().zip(contribs_preds) {
+            assert_eq!(precision_round(*i, 7), precision_round(j, 7));
+        }
+    }
+}
```

### Comparing `forust-0.2.6/local_dependencies/forust-ml/src/utils.rs` & `forust-0.2.7/local_dependencies/forust-ml/src/utils.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,820 +1,830 @@
-use crate::constraints::Constraint;
-use crate::data::FloatData;
-use std::cmp::Ordering;
-use std::collections::VecDeque;
-use std::convert::TryInto;
-
-/// Calculate if a value is missing.
-#[inline]
-pub fn is_missing(value: &f64, missing: &f64) -> bool {
-    if missing.is_nan() {
-        value.is_nan()
-    } else if value.is_nan() {
-        panic!(
-            "Missing value is {}, however NAN value found in data.",
-            missing
-        )
-    } else {
-        value == missing
-    }
-}
-
-/// Calculate the constraint weight given bounds
-/// and a constraint.
-#[inline]
-pub fn constrained_weight(
-    l2: &f32,
-    gradient_sum: f32,
-    hessian_sum: f32,
-    lower_bound: f32,
-    upper_bound: f32,
-    constraint: Option<&Constraint>,
-) -> f32 {
-    let weight = weight(l2, gradient_sum, hessian_sum);
-    match constraint {
-        None | Some(Constraint::Unconstrained) => weight,
-        _ => {
-            if weight > upper_bound {
-                upper_bound
-            } else if weight < lower_bound {
-                lower_bound
-            } else {
-                weight
-            }
-        }
-    }
-}
-
-/// Calculate the gain given the gradient and hessian of the node.
-#[inline]
-pub fn gain(l2: &f32, gradient_sum: f32, hessian_sum: f32) -> f32 {
-    (gradient_sum * gradient_sum) / (hessian_sum + l2)
-}
-
-/// Calculate the gain of a split given a specific weight value.
-/// This is for if the weight has to be constrained, for example for
-/// monotonicity constraints.
-#[inline]
-pub fn gain_given_weight(l2: &f32, gradient_sum: f32, hessian_sum: f32, weight: f32) -> f32 {
-    -(2.0 * gradient_sum * weight + (hessian_sum + l2) * (weight * weight))
-}
-
-/// Cull gain, if it does not conform to constraints.
-#[inline]
-pub fn cull_gain(
-    gain: f32,
-    left_weight: f32,
-    right_weight: f32,
-    constraint: Option<&Constraint>,
-) -> f32 {
-    match constraint {
-        None | Some(Constraint::Unconstrained) => gain,
-        Some(Constraint::Negative) => {
-            if left_weight < right_weight {
-                f32::NEG_INFINITY
-            } else {
-                gain
-            }
-        }
-        Some(Constraint::Positive) => {
-            if left_weight > right_weight {
-                f32::NEG_INFINITY
-            } else {
-                gain
-            }
-        }
-    }
-}
-
-/// Calculate the weight of a given node, given the sum
-/// of the gradients, and the hessians in a node.
-#[inline]
-pub fn weight(l2: &f32, gradient_sum: f32, hessian_sum: f32) -> f32 {
-    -(gradient_sum / (hessian_sum + l2))
-}
-
-const LANES: usize = 16;
-
-/// Fast summation, ends up being roughly 8 to 10 times faster
-/// than values.iter().copied().sum().
-/// Shamelessly stolen from https://stackoverflow.com/a/67191480
-#[inline]
-pub fn fast_sum<T: FloatData<T>>(values: &[T]) -> T {
-    let chunks = values.chunks_exact(LANES);
-    let remainder = chunks.remainder();
-
-    let sum = chunks.fold([T::ZERO; LANES], |mut acc, chunk| {
-        let chunk: [T; LANES] = chunk.try_into().unwrap();
-        for i in 0..LANES {
-            acc[i] += chunk[i];
-        }
-        acc
-    });
-
-    let remainder: T = remainder.iter().copied().sum();
-
-    let mut reduced = T::ZERO;
-    for s in sum.iter().take(LANES) {
-        reduced += *s;
-    }
-    reduced + remainder
-}
-
-/// Fast summation, but using f64 as the internal representation so that
-/// we don't have issues with the precision.
-/// This way, we can still work with f32 values, but get the correct sum
-/// value.
-#[inline]
-pub fn fast_f64_sum(values: &[f32]) -> f32 {
-    let chunks = values.chunks_exact(LANES);
-    let remainder = chunks.remainder();
-
-    let sum = chunks.fold([f64::ZERO; LANES], |mut acc, chunk| {
-        let chunk: [f32; LANES] = chunk.try_into().unwrap();
-        for i in 0..LANES {
-            acc[i] += f64::from(chunk[i]);
-        }
-        acc
-    });
-
-    let remainder: f64 = remainder
-        .iter()
-        .fold(f64::ZERO, |acc, b| acc + f64::from(*b));
-
-    let mut reduced: f64 = 0.;
-    for s in sum.iter().take(LANES) {
-        reduced += *s;
-    }
-    (reduced + remainder) as f32
-}
-
-pub fn naive_sum<T: FloatData<T>>(values: &[T]) -> T {
-    values.iter().copied().sum()
-}
-
-/// Naive weighted percentiles calculation.
-///
-/// Currently this function does not support missing values.
-///   
-/// * `v` - A Vector of which to find percentiles for.
-/// * `sample_weight` - Sample weights for the instances of the vector.
-/// * `percentiles` - Percentiles to look for in the data. This should be
-///     values from 0 to 1, and in sorted order.
-pub fn percentiles<T>(v: &[T], sample_weight: &[T], percentiles: &[T]) -> Vec<T>
-where
-    T: FloatData<T>,
-{
-    let mut idx: Vec<usize> = (0..v.len()).collect();
-    idx.sort_unstable_by(|a, b| v[*a].partial_cmp(&v[*b]).unwrap());
-
-    // Setup percentiles
-    let mut pcts = VecDeque::from_iter(percentiles.iter());
-    let mut current_pct = *pcts.pop_front().expect("No percentiles were provided");
-
-    // Prepare a vector to put the percentiles in...
-    let mut p = Vec::new();
-    let mut cuml_pct = T::ZERO;
-    let mut current_value = v[idx[0]];
-    let total_values = fast_sum(sample_weight);
-
-    for i in idx.iter() {
-        if current_value != v[*i] {
-            current_value = v[*i];
-        }
-        cuml_pct += sample_weight[*i] / total_values;
-        if (current_pct == T::ZERO) || (cuml_pct >= current_pct) {
-            // We loop here, because the same number might be a valid
-            // value to make the percentile several times.
-            while cuml_pct >= current_pct {
-                p.push(current_value);
-                match pcts.pop_front() {
-                    Some(p_) => current_pct = *p_,
-                    None => return p,
-                }
-            }
-        } else if current_pct == T::ONE {
-            if let Some(i_) = idx.last() {
-                p.push(v[*i_]);
-                break;
-            }
-        }
-    }
-    p
-}
-
-// Return the index of the first value in a slice that
-// is less another number. This will return the first index for
-// missing values.
-/// Return the index of the first value in a sorted
-/// vector that is greater than a provided value.
-///
-/// * `x` - The sorted slice of values.
-/// * `v` - The value used to calculate the first
-///   value larger than it.
-#[inline]
-pub fn map_bin<T: std::cmp::PartialOrd>(x: &[T], v: &T) -> Option<u16> {
-    let mut low = 0;
-    let mut high = x.len();
-    while low != high {
-        let mid = (low + high) / 2;
-        // This will always be false for NaNs.
-        // This it will force us to the bottom,
-        // and thus Zero.
-        if x[mid] <= *v {
-            low = mid + 1;
-        } else {
-            high = mid;
-        }
-    }
-    u16::try_from(low).ok()
-}
-
-/// Provided a list of index values, pivot those values
-/// around a specific split value so all of the values less
-/// than the split value are on one side, and then all of the
-/// values greater than or equal to the split value are above.
-///
-/// * `index` - The index values to sort.
-/// * `feature` - The feature vector to use to sort the index by.
-/// * `split_value` - the split value to use to pivot on.
-/// * `missing_right` - Should missing values go to the left, or
-///    to the right of the split value.
-#[inline]
-pub fn pivot_on_split(
-    index: &mut [usize],
-    feature: &[u16],
-    split_value: u16,
-    missing_right: bool,
-) -> usize {
-    // I think we can do this in O(n) time...
-    let mut low = 0;
-    let mut high = index.len() - 1;
-    let max_idx = high;
-    while low < high {
-        // Go until we find a low value that needs to
-        // be swapped, this will be the first value
-        // that our split value is less or equal to.
-        while low < max_idx {
-            let l = feature[index[low]];
-            match missing_compare(&split_value, l, missing_right) {
-                Ordering::Less | Ordering::Equal => break,
-                Ordering::Greater => low += 1,
-            }
-        }
-        while high > low {
-            let h = feature[index[high]];
-            // Go until we find a high value that needs to be
-            // swapped, this will be the first value that our
-            // split_value is greater than.
-            match missing_compare(&split_value, h, missing_right) {
-                Ordering::Less | Ordering::Equal => high -= 1,
-                Ordering::Greater => break,
-            }
-        }
-        if low < high {
-            index.swap(high, low);
-        }
-    }
-    low
-}
-
-/// Provided a list of index values, pivot those values
-/// around a specific split value so all of the values less
-/// than the split value are on one side, and then all of the
-/// values greater than or equal to the split value are above.
-/// Missing values, will be pushed to the bottom, a value of
-/// zero is missing in this case.
-/// Returns a tuple, the first is the first non-missing value
-/// index, the second is the first value that is greater than
-/// our provided split value.
-///
-/// WARNING!!! Currently, this function fails, if all the values are
-/// missing...
-///
-/// * `index` - The index values to sort.
-/// * `feature` - The feature vector to use to sort the index by.
-/// * `split_value` - the split value to use to pivot on.
-#[inline]
-pub fn pivot_on_split_exclude_missing(
-    index: &mut [usize],
-    feature: &[u16],
-    split_value: u16,
-) -> (usize, usize) {
-    // I think we can do this in O(n) time...
-    let mut low = 0;
-    let mut high = index.len() - 1;
-    // The index of the first value, that is not
-    // missing.
-    let mut missing = 0;
-    let max_idx = high;
-    while low < high {
-        // Go until we find a low value that needs to
-        // be swapped, this will be the first value
-        // that our split value is less or equal to.
-        while low < max_idx {
-            let l = feature[index[low]];
-            if l == 0 {
-                index.swap(missing, low);
-                missing += 1;
-            }
-            match &split_value.cmp(&l) {
-                Ordering::Less | Ordering::Equal => break,
-                Ordering::Greater => low += 1,
-            }
-        }
-        while high > low {
-            let h = feature[index[high]];
-            // If this is missing, we need to
-            // swap this value with missing, and
-            // then that value with low.
-            if h == 0 {
-                index.swap(missing, high);
-                missing += 1;
-                // Low must be at least equal to
-                // missing. Otherwise, we would get
-                // stuck, because low will be zero
-                // then...
-                if missing > low {
-                    low = missing;
-                }
-            }
-            // Go until we find a high value that needs to be
-            // swapped, this will be the first value that our
-            // split_value is greater than.
-            match &split_value.cmp(&h) {
-                Ordering::Less | Ordering::Equal => high -= 1,
-                Ordering::Greater => break,
-            }
-        }
-        if low < high {
-            index.swap(high, low);
-        }
-    }
-    (missing, low)
-}
-
-/// Function to compare a value to our split value.
-/// Our split value will _never_ be missing (0), thus we
-/// don't have to worry about that.
-#[inline]
-pub fn missing_compare(split_value: &u16, cmp_value: u16, missing_right: bool) -> Ordering {
-    if cmp_value == 0 {
-        if missing_right {
-            // If missing is right, then our split_value
-            // will always be considered less than missing.
-            Ordering::Less
-        } else {
-            // Otherwise less to send it left by considering
-            // our split value being always greater than missing
-            Ordering::Greater
-        }
-    } else {
-        split_value.cmp(&cmp_value)
-    }
-}
-
-#[inline]
-pub fn precision_round(n: f64, precision: i32) -> f64 {
-    let p = (10.0_f64).powi(precision);
-    (n * p).round() / p
-}
-
-#[cfg(test)]
-mod tests {
-    use super::*;
-    use rand::rngs::StdRng;
-    use rand::seq::SliceRandom;
-    use rand::Rng;
-    use rand::SeedableRng;
-    #[test]
-    fn test_round() {
-        assert_eq!(0.3, precision_round(0.3333, 1));
-        assert_eq!(0.2343, precision_round(0.2343123123123, 4));
-    }
-    #[test]
-    fn test_percentiles() {
-        let v = vec![4., 5., 6., 1., 2., 3., 7., 8., 9., 10.];
-        let w = vec![1.; v.len()];
-        let p = vec![0.3, 0.5, 0.75, 1.0];
-        let p = percentiles(&v, &w, &p);
-        assert_eq!(p, vec![3.0, 5.0, 8.0, 10.0]);
-    }
-
-    #[test]
-    fn test_percentiles_weighted() {
-        let v = vec![10., 8., 9., 1., 2., 3., 6., 7., 4., 5.];
-        let w = vec![1., 1., 1., 1., 1., 2., 1., 1., 5., 1.];
-        let p = vec![0.3, 0.5, 0.75, 1.0];
-        let p = percentiles(&v, &w, &p);
-        assert_eq!(p, vec![4.0, 4.0, 7.0, 10.0]);
-    }
-
-    #[test]
-    fn test_map_bin_or_equal() {
-        let v = vec![f64::MIN, 1., 4., 8., 9.];
-        assert_eq!(1, map_bin(&v, &0.).unwrap());
-        assert_eq!(2, map_bin(&v, &1.).unwrap());
-        // Less than the bin value of 2, means the value is less
-        // than 4...
-        assert_eq!(2, map_bin(&v, &2.).unwrap());
-        assert_eq!(3, map_bin(&v, &4.).unwrap());
-        assert_eq!(5, map_bin(&v, &9.).unwrap());
-        assert_eq!(5, map_bin(&v, &10.).unwrap());
-        assert_eq!(2, map_bin(&v, &1.).unwrap());
-        assert_eq!(0, map_bin(&v, &f64::NAN).unwrap());
-    }
-
-    #[test]
-    fn test_missing_compare() {
-        assert_eq!(missing_compare(&10, 0, true), Ordering::Less);
-        assert_eq!(missing_compare(&10, 0, false), Ordering::Greater);
-        assert_eq!(missing_compare(&10, 11, true), Ordering::Less);
-        assert_eq!(missing_compare(&10, 1, true), Ordering::Greater);
-    }
-
-    #[test]
-    fn test_pivot() {
-        fn pivot_assert(
-            f: &[u16],
-            idx: &[usize],
-            split_i: usize,
-            missing_right: bool,
-            split_val: u16,
-        ) {
-            if missing_right {
-                for i in 0..split_i {
-                    assert!((f[idx[i]] < split_val) && f[idx[i]] != 0);
-                }
-                for i in idx[split_i..].iter() {
-                    assert!((f[*i] >= split_val) || (f[*i] == 0));
-                }
-            } else {
-                for i in 0..split_i {
-                    assert!((f[idx[i]] < split_val) || (f[idx[i]] == 0));
-                }
-                for i in idx[split_i..].iter() {
-                    assert!((f[*i] >= split_val) || (f[*i] != 0));
-                }
-            }
-        }
-
-        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
-        let f = vec![15, 10, 10, 11, 3, 18, 0, 9, 3, 5, 2, 6, 13, 19, 14];
-        let split_i = pivot_on_split(&mut idx, &f, 10, true);
-        pivot_assert(&f, &idx, split_i, true, 10);
-
-        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
-        let f = vec![15, 10, 10, 11, 3, 18, 0, 9, 3, 5, 2, 6, 13, 19, 14];
-        let split_i = pivot_on_split(&mut idx, &f, 10, false);
-        pivot_assert(&f, &idx, split_i, false, 10);
-
-        // Test Minimum value...
-        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
-        let f = vec![15, 10, 10, 11, 3, 18, 0, 9, 3, 5, 2, 6, 13, 19, 14];
-        let split_i = pivot_on_split(&mut idx, &f, 1, true);
-        pivot_assert(&f, &idx, split_i, true, 1);
-
-        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
-        let f = vec![15, 10, 10, 11, 3, 18, 0, 9, 3, 5, 2, 6, 13, 19, 14];
-        let split_i = pivot_on_split(&mut idx, &f, 1, false);
-        pivot_assert(&f, &idx, split_i, false, 1);
-
-        // Test Maximum value...
-        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
-        let f = vec![15, 10, 10, 11, 3, 18, 0, 9, 3, 5, 2, 6, 13, 19, 14];
-        let split_i = pivot_on_split(&mut idx, &f, 19, true);
-        pivot_assert(&f, &idx, split_i, true, 19);
-
-        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
-        let f = vec![15, 10, 10, 11, 3, 18, 0, 9, 3, 5, 2, 6, 13, 19, 14];
-        let split_i = pivot_on_split(&mut idx, &f, 19, false);
-        pivot_assert(&f, &idx, split_i, false, 19);
-
-        // Random tests... right...
-        // With missing
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let split_i = pivot_on_split(&mut idx, &f, 7, true);
-        pivot_assert(&f, &idx, split_i, true, 7);
-
-        // Already sorted...
-        let split_i = pivot_on_split(&mut idx, &f, 7, true);
-        pivot_assert(&f, &idx, split_i, true, 7);
-
-        // Reversed
-        idx.reverse();
-        let split_i = pivot_on_split(&mut idx, &f, 7, true);
-        pivot_assert(&f, &idx, split_i, true, 7);
-
-        // Without missing...
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(1..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let split_i = pivot_on_split(&mut idx, &f, 5, true);
-        pivot_assert(&f, &idx, split_i, true, 5);
-
-        // Using max...
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let sv = idx.iter().map(|i| f[*i]).max().unwrap();
-        let split_i = pivot_on_split(&mut idx, &f, sv, true);
-        pivot_assert(&f, &idx, split_i, true, sv);
-
-        // Using non-0 minimum...
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let sv = idx
-            .iter()
-            .filter(|i| f[**i] > 0)
-            .map(|i| f[*i])
-            .min()
-            .unwrap();
-        let split_i = pivot_on_split(&mut idx, &f, sv, true);
-        pivot_assert(&f, &idx, split_i, true, sv);
-
-        // Using non-0 minimum with no missing...
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(1..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let sv = idx
-            .iter()
-            .filter(|i| f[**i] > 0)
-            .map(|i| f[*i])
-            .min()
-            .unwrap();
-        let split_i = pivot_on_split(&mut idx, &f, sv, true);
-        pivot_assert(&f, &idx, split_i, true, sv);
-
-        // Left
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let split_i = pivot_on_split(&mut idx, &f, 7, false);
-        pivot_assert(&f, &idx, split_i, false, 7);
-
-        // Already sorted...
-        let split_i = pivot_on_split(&mut idx, &f, 7, false);
-        pivot_assert(&f, &idx, split_i, false, 7);
-
-        // Reversed
-        idx.reverse();
-        let split_i = pivot_on_split(&mut idx, &f, 7, false);
-        pivot_assert(&f, &idx, split_i, false, 7);
-
-        // Without missing...
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(1..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let split_i = pivot_on_split(&mut idx, &f, 5, false);
-        pivot_assert(&f, &idx, split_i, false, 5);
-
-        // Using max...
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let sv = idx.iter().map(|i| f[*i]).max().unwrap();
-        let split_i = pivot_on_split(&mut idx, &f, sv, false);
-        pivot_assert(&f, &idx, split_i, false, sv);
-
-        // Using non-0 minimum...
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let sv = idx
-            .iter()
-            .filter(|i| f[**i] > 0)
-            .map(|i| f[*i])
-            .min()
-            .unwrap();
-        let split_i = pivot_on_split(&mut idx, &f, sv, false);
-        pivot_assert(&f, &idx, split_i, false, sv);
-
-        // Using non-0 minimum with no missing...
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(1..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let sv = idx
-            .iter()
-            .filter(|i| f[**i] > 0)
-            .map(|i| f[*i])
-            .min()
-            .unwrap();
-        let split_i = pivot_on_split(&mut idx, &f, sv, false);
-        pivot_assert(&f, &idx, split_i, false, sv);
-    }
-
-    #[test]
-    fn test_pivot_missing() {
-        fn pivot_missing_assert(
-            split_value: u16,
-            idx: &[usize],
-            f: &[u16],
-            split_i: &(usize, usize),
-        ) {
-            // Check they are lower than..
-            for i in 0..split_i.1 {
-                assert!(f[idx[i]] < split_value);
-            }
-            // Check missing got moved
-            for i in 0..split_i.0 {
-                assert!(f[idx[i]] == 0);
-            }
-            // Check none are less than...
-            for i in split_i.1..(idx.len()) {
-                assert!(!(f[idx[i]] < split_value));
-            }
-            // Check none other are missing...
-            for i in split_i.0..(idx.len()) {
-                assert!(f[idx[i]] != 0);
-            }
-        }
-        // TODO: Add more tests for this...
-        // Using minimum value...
-        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
-        let f = vec![15, 10, 10, 0, 3, 0, 0, 9, 3, 5, 2, 6, 13, 19, 14];
-        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 1);
-        // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
-        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
-        pivot_missing_assert(1, &idx, &f, &split_i);
-
-        // Higher value...
-        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
-        let f = vec![15, 10, 10, 0, 3, 0, 0, 9, 3, 5, 2, 6, 13, 19, 14];
-        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 10);
-        //let split_i = pivot_on_split(&mut idx, &f, 10, false);
-        // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
-        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
-        pivot_missing_assert(10, &idx, &f, &split_i);
-
-        // Run it again, and ensure it works on an already sorted list...
-        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 10);
-        //let split_i = pivot_on_split(&mut idx, &f, 10, false);
-        // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
-        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
-        pivot_missing_assert(10, &idx, &f, &split_i);
-
-        // Run it again, and ensure it works on reversed list...
-        idx.reverse();
-        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 10);
-        //let split_i = pivot_on_split(&mut idx, &f, 10, false);
-        // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
-        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
-        pivot_missing_assert(10, &idx, &f, &split_i);
-
-        // Small test done with python
-        let mut idx = vec![0, 1, 2, 3, 4, 5];
-        let f = vec![1, 0, 1, 3, 0, 4];
-        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 2);
-        // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
-        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
-        pivot_missing_assert(2, &idx, &f, &split_i);
-
-        // Ensure it works on all missing...
-        // let mut idx = vec![0, 1, 2, 3, 4, 5];
-        // let f: Vec<u16> = vec![3; idx.len()];
-        // let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 2);
-        // // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
-        // // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
-        // pivot_missing_assert(2, &idx, &f, &split_i);
-
-        // Check if none missing...
-        // TODO: Add more tests for this...
-        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
-        let f = vec![15, 10, 10, 2, 3, 5, 7, 9, 3, 5, 2, 6, 13, 19, 14];
-        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 10);
-        //let split_i = pivot_on_split(&mut idx, &f, 10, false);
-        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
-        // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
-        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
-        pivot_missing_assert(10, &idx, &f, &split_i);
-
-        // Random tests...
-        // With missing
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 10);
-        pivot_missing_assert(10, &idx, &f, &split_i);
-
-        // Already sorted...
-        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 10);
-        pivot_missing_assert(10, &idx, &f, &split_i);
-
-        // Without missing...
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(1..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 5);
-        // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
-        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
-        pivot_missing_assert(5, &idx, &f, &split_i);
-
-        // Using max...
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let sv = idx.iter().map(|i| f[*i]).max().unwrap();
-        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, sv);
-        pivot_missing_assert(sv, &idx, &f, &split_i);
-
-        // Using non-0 minimum...
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let sv = idx
-            .iter()
-            .filter(|i| f[**i] > 0)
-            .map(|i| f[*i])
-            .min()
-            .unwrap();
-        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, sv);
-        pivot_missing_assert(sv, &idx, &f, &split_i);
-
-        // Using non-0 minimum with no missing...
-        let index = (0..100).collect::<Vec<usize>>();
-        let mut rng = StdRng::seed_from_u64(0);
-        let f = (0..100).map(|_| rng.gen_range(1..15)).collect::<Vec<u16>>();
-        let mut idx = index
-            .choose_multiple(&mut rng, 73)
-            .copied()
-            .collect::<Vec<usize>>();
-        let sv = idx
-            .iter()
-            .filter(|i| f[**i] > 0)
-            .map(|i| f[*i])
-            .min()
-            .unwrap();
-        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, sv);
-        pivot_missing_assert(sv, &idx, &f, &split_i);
-    }
-
-    #[test]
-    fn test_fast_f64_sum() {
-        let records = 300000;
-        let vec = vec![0.23500371; records];
-        assert_ne!(vec.iter().sum::<f32>(), vec[0] * (records as f32));
-        assert_eq!(vec[0] * (records as f32), fast_f64_sum(&vec));
-        // println!("Sum Result: {}", vec.iter().sum::<f32>());
-        // println!("Multiplication Results {}", vec[0] * (records as f32));
-        // println!("f64_sum Results {}", f64_sum(&vec));
-    }
-}
+use crate::constraints::Constraint;
+use crate::data::FloatData;
+use std::cmp::Ordering;
+use std::collections::VecDeque;
+use std::convert::TryInto;
+
+/// Create a string of all available items.
+pub fn items_to_strings(items: Vec<&str>) -> String {
+    let mut s = String::new();
+    for i in items {
+        s.push_str(i);
+        s.push_str(&String::from(", "));
+    }
+    s
+}
+
+/// Calculate if a value is missing.
+#[inline]
+pub fn is_missing(value: &f64, missing: &f64) -> bool {
+    if missing.is_nan() {
+        value.is_nan()
+    } else if value.is_nan() {
+        panic!(
+            "Missing value is {}, however NAN value found in data.",
+            missing
+        )
+    } else {
+        value == missing
+    }
+}
+
+/// Calculate the constraint weight given bounds
+/// and a constraint.
+#[inline]
+pub fn constrained_weight(
+    l2: &f32,
+    gradient_sum: f32,
+    hessian_sum: f32,
+    lower_bound: f32,
+    upper_bound: f32,
+    constraint: Option<&Constraint>,
+) -> f32 {
+    let weight = weight(l2, gradient_sum, hessian_sum);
+    match constraint {
+        None | Some(Constraint::Unconstrained) => weight,
+        _ => {
+            if weight > upper_bound {
+                upper_bound
+            } else if weight < lower_bound {
+                lower_bound
+            } else {
+                weight
+            }
+        }
+    }
+}
+
+/// Calculate the gain given the gradient and hessian of the node.
+#[inline]
+pub fn gain(l2: &f32, gradient_sum: f32, hessian_sum: f32) -> f32 {
+    (gradient_sum * gradient_sum) / (hessian_sum + l2)
+}
+
+/// Calculate the gain of a split given a specific weight value.
+/// This is for if the weight has to be constrained, for example for
+/// monotonicity constraints.
+#[inline]
+pub fn gain_given_weight(l2: &f32, gradient_sum: f32, hessian_sum: f32, weight: f32) -> f32 {
+    -(2.0 * gradient_sum * weight + (hessian_sum + l2) * (weight * weight))
+}
+
+/// Cull gain, if it does not conform to constraints.
+#[inline]
+pub fn cull_gain(
+    gain: f32,
+    left_weight: f32,
+    right_weight: f32,
+    constraint: Option<&Constraint>,
+) -> f32 {
+    match constraint {
+        None | Some(Constraint::Unconstrained) => gain,
+        Some(Constraint::Negative) => {
+            if left_weight < right_weight {
+                f32::NEG_INFINITY
+            } else {
+                gain
+            }
+        }
+        Some(Constraint::Positive) => {
+            if left_weight > right_weight {
+                f32::NEG_INFINITY
+            } else {
+                gain
+            }
+        }
+    }
+}
+
+/// Calculate the weight of a given node, given the sum
+/// of the gradients, and the hessians in a node.
+#[inline]
+pub fn weight(l2: &f32, gradient_sum: f32, hessian_sum: f32) -> f32 {
+    -(gradient_sum / (hessian_sum + l2))
+}
+
+const LANES: usize = 16;
+
+/// Fast summation, ends up being roughly 8 to 10 times faster
+/// than values.iter().copied().sum().
+/// Shamelessly stolen from https://stackoverflow.com/a/67191480
+#[inline]
+pub fn fast_sum<T: FloatData<T>>(values: &[T]) -> T {
+    let chunks = values.chunks_exact(LANES);
+    let remainder = chunks.remainder();
+
+    let sum = chunks.fold([T::ZERO; LANES], |mut acc, chunk| {
+        let chunk: [T; LANES] = chunk.try_into().unwrap();
+        for i in 0..LANES {
+            acc[i] += chunk[i];
+        }
+        acc
+    });
+
+    let remainder: T = remainder.iter().copied().sum();
+
+    let mut reduced = T::ZERO;
+    for s in sum.iter().take(LANES) {
+        reduced += *s;
+    }
+    reduced + remainder
+}
+
+/// Fast summation, but using f64 as the internal representation so that
+/// we don't have issues with the precision.
+/// This way, we can still work with f32 values, but get the correct sum
+/// value.
+#[inline]
+pub fn fast_f64_sum(values: &[f32]) -> f32 {
+    let chunks = values.chunks_exact(LANES);
+    let remainder = chunks.remainder();
+
+    let sum = chunks.fold([f64::ZERO; LANES], |mut acc, chunk| {
+        let chunk: [f32; LANES] = chunk.try_into().unwrap();
+        for i in 0..LANES {
+            acc[i] += f64::from(chunk[i]);
+        }
+        acc
+    });
+
+    let remainder: f64 = remainder
+        .iter()
+        .fold(f64::ZERO, |acc, b| acc + f64::from(*b));
+
+    let mut reduced: f64 = 0.;
+    for s in sum.iter().take(LANES) {
+        reduced += *s;
+    }
+    (reduced + remainder) as f32
+}
+
+pub fn naive_sum<T: FloatData<T>>(values: &[T]) -> T {
+    values.iter().copied().sum()
+}
+
+/// Naive weighted percentiles calculation.
+///
+/// Currently this function does not support missing values.
+///   
+/// * `v` - A Vector of which to find percentiles for.
+/// * `sample_weight` - Sample weights for the instances of the vector.
+/// * `percentiles` - Percentiles to look for in the data. This should be
+///     values from 0 to 1, and in sorted order.
+pub fn percentiles<T>(v: &[T], sample_weight: &[T], percentiles: &[T]) -> Vec<T>
+where
+    T: FloatData<T>,
+{
+    let mut idx: Vec<usize> = (0..v.len()).collect();
+    idx.sort_unstable_by(|a, b| v[*a].partial_cmp(&v[*b]).unwrap());
+
+    // Setup percentiles
+    let mut pcts = VecDeque::from_iter(percentiles.iter());
+    let mut current_pct = *pcts.pop_front().expect("No percentiles were provided");
+
+    // Prepare a vector to put the percentiles in...
+    let mut p = Vec::new();
+    let mut cuml_pct = T::ZERO;
+    let mut current_value = v[idx[0]];
+    let total_values = fast_sum(sample_weight);
+
+    for i in idx.iter() {
+        if current_value != v[*i] {
+            current_value = v[*i];
+        }
+        cuml_pct += sample_weight[*i] / total_values;
+        if (current_pct == T::ZERO) || (cuml_pct >= current_pct) {
+            // We loop here, because the same number might be a valid
+            // value to make the percentile several times.
+            while cuml_pct >= current_pct {
+                p.push(current_value);
+                match pcts.pop_front() {
+                    Some(p_) => current_pct = *p_,
+                    None => return p,
+                }
+            }
+        } else if current_pct == T::ONE {
+            if let Some(i_) = idx.last() {
+                p.push(v[*i_]);
+                break;
+            }
+        }
+    }
+    p
+}
+
+// Return the index of the first value in a slice that
+// is less another number. This will return the first index for
+// missing values.
+/// Return the index of the first value in a sorted
+/// vector that is greater than a provided value.
+///
+/// * `x` - The sorted slice of values.
+/// * `v` - The value used to calculate the first
+///   value larger than it.
+#[inline]
+pub fn map_bin<T: std::cmp::PartialOrd>(x: &[T], v: &T) -> Option<u16> {
+    let mut low = 0;
+    let mut high = x.len();
+    while low != high {
+        let mid = (low + high) / 2;
+        // This will always be false for NaNs.
+        // This it will force us to the bottom,
+        // and thus Zero.
+        if x[mid] <= *v {
+            low = mid + 1;
+        } else {
+            high = mid;
+        }
+    }
+    u16::try_from(low).ok()
+}
+
+/// Provided a list of index values, pivot those values
+/// around a specific split value so all of the values less
+/// than the split value are on one side, and then all of the
+/// values greater than or equal to the split value are above.
+///
+/// * `index` - The index values to sort.
+/// * `feature` - The feature vector to use to sort the index by.
+/// * `split_value` - the split value to use to pivot on.
+/// * `missing_right` - Should missing values go to the left, or
+///    to the right of the split value.
+#[inline]
+pub fn pivot_on_split(
+    index: &mut [usize],
+    feature: &[u16],
+    split_value: u16,
+    missing_right: bool,
+) -> usize {
+    // I think we can do this in O(n) time...
+    let mut low = 0;
+    let mut high = index.len() - 1;
+    let max_idx = high;
+    while low < high {
+        // Go until we find a low value that needs to
+        // be swapped, this will be the first value
+        // that our split value is less or equal to.
+        while low < max_idx {
+            let l = feature[index[low]];
+            match missing_compare(&split_value, l, missing_right) {
+                Ordering::Less | Ordering::Equal => break,
+                Ordering::Greater => low += 1,
+            }
+        }
+        while high > low {
+            let h = feature[index[high]];
+            // Go until we find a high value that needs to be
+            // swapped, this will be the first value that our
+            // split_value is greater than.
+            match missing_compare(&split_value, h, missing_right) {
+                Ordering::Less | Ordering::Equal => high -= 1,
+                Ordering::Greater => break,
+            }
+        }
+        if low < high {
+            index.swap(high, low);
+        }
+    }
+    low
+}
+
+/// Provided a list of index values, pivot those values
+/// around a specific split value so all of the values less
+/// than the split value are on one side, and then all of the
+/// values greater than or equal to the split value are above.
+/// Missing values, will be pushed to the bottom, a value of
+/// zero is missing in this case.
+/// Returns a tuple, the first is the first non-missing value
+/// index, the second is the first value that is greater than
+/// our provided split value.
+///
+/// WARNING!!! Currently, this function fails, if all the values are
+/// missing...
+///
+/// * `index` - The index values to sort.
+/// * `feature` - The feature vector to use to sort the index by.
+/// * `split_value` - the split value to use to pivot on.
+#[inline]
+pub fn pivot_on_split_exclude_missing(
+    index: &mut [usize],
+    feature: &[u16],
+    split_value: u16,
+) -> (usize, usize) {
+    // I think we can do this in O(n) time...
+    let mut low = 0;
+    let mut high = index.len() - 1;
+    // The index of the first value, that is not
+    // missing.
+    let mut missing = 0;
+    let max_idx = high;
+    while low < high {
+        // Go until we find a low value that needs to
+        // be swapped, this will be the first value
+        // that our split value is less or equal to.
+        while low < max_idx {
+            let l = feature[index[low]];
+            if l == 0 {
+                index.swap(missing, low);
+                missing += 1;
+            }
+            match &split_value.cmp(&l) {
+                Ordering::Less | Ordering::Equal => break,
+                Ordering::Greater => low += 1,
+            }
+        }
+        while high > low {
+            let h = feature[index[high]];
+            // If this is missing, we need to
+            // swap this value with missing, and
+            // then that value with low.
+            if h == 0 {
+                index.swap(missing, high);
+                missing += 1;
+                // Low must be at least equal to
+                // missing. Otherwise, we would get
+                // stuck, because low will be zero
+                // then...
+                if missing > low {
+                    low = missing;
+                }
+            }
+            // Go until we find a high value that needs to be
+            // swapped, this will be the first value that our
+            // split_value is greater than.
+            match &split_value.cmp(&h) {
+                Ordering::Less | Ordering::Equal => high -= 1,
+                Ordering::Greater => break,
+            }
+        }
+        if low < high {
+            index.swap(high, low);
+        }
+    }
+    (missing, low)
+}
+
+/// Function to compare a value to our split value.
+/// Our split value will _never_ be missing (0), thus we
+/// don't have to worry about that.
+#[inline]
+pub fn missing_compare(split_value: &u16, cmp_value: u16, missing_right: bool) -> Ordering {
+    if cmp_value == 0 {
+        if missing_right {
+            // If missing is right, then our split_value
+            // will always be considered less than missing.
+            Ordering::Less
+        } else {
+            // Otherwise less to send it left by considering
+            // our split value being always greater than missing
+            Ordering::Greater
+        }
+    } else {
+        split_value.cmp(&cmp_value)
+    }
+}
+
+#[inline]
+pub fn precision_round(n: f64, precision: i32) -> f64 {
+    let p = (10.0_f64).powi(precision);
+    (n * p).round() / p
+}
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+    use rand::rngs::StdRng;
+    use rand::seq::SliceRandom;
+    use rand::Rng;
+    use rand::SeedableRng;
+    #[test]
+    fn test_round() {
+        assert_eq!(0.3, precision_round(0.3333, 1));
+        assert_eq!(0.2343, precision_round(0.2343123123123, 4));
+    }
+    #[test]
+    fn test_percentiles() {
+        let v = vec![4., 5., 6., 1., 2., 3., 7., 8., 9., 10.];
+        let w = vec![1.; v.len()];
+        let p = vec![0.3, 0.5, 0.75, 1.0];
+        let p = percentiles(&v, &w, &p);
+        assert_eq!(p, vec![3.0, 5.0, 8.0, 10.0]);
+    }
+
+    #[test]
+    fn test_percentiles_weighted() {
+        let v = vec![10., 8., 9., 1., 2., 3., 6., 7., 4., 5.];
+        let w = vec![1., 1., 1., 1., 1., 2., 1., 1., 5., 1.];
+        let p = vec![0.3, 0.5, 0.75, 1.0];
+        let p = percentiles(&v, &w, &p);
+        assert_eq!(p, vec![4.0, 4.0, 7.0, 10.0]);
+    }
+
+    #[test]
+    fn test_map_bin_or_equal() {
+        let v = vec![f64::MIN, 1., 4., 8., 9.];
+        assert_eq!(1, map_bin(&v, &0.).unwrap());
+        assert_eq!(2, map_bin(&v, &1.).unwrap());
+        // Less than the bin value of 2, means the value is less
+        // than 4...
+        assert_eq!(2, map_bin(&v, &2.).unwrap());
+        assert_eq!(3, map_bin(&v, &4.).unwrap());
+        assert_eq!(5, map_bin(&v, &9.).unwrap());
+        assert_eq!(5, map_bin(&v, &10.).unwrap());
+        assert_eq!(2, map_bin(&v, &1.).unwrap());
+        assert_eq!(0, map_bin(&v, &f64::NAN).unwrap());
+    }
+
+    #[test]
+    fn test_missing_compare() {
+        assert_eq!(missing_compare(&10, 0, true), Ordering::Less);
+        assert_eq!(missing_compare(&10, 0, false), Ordering::Greater);
+        assert_eq!(missing_compare(&10, 11, true), Ordering::Less);
+        assert_eq!(missing_compare(&10, 1, true), Ordering::Greater);
+    }
+
+    #[test]
+    fn test_pivot() {
+        fn pivot_assert(
+            f: &[u16],
+            idx: &[usize],
+            split_i: usize,
+            missing_right: bool,
+            split_val: u16,
+        ) {
+            if missing_right {
+                for i in 0..split_i {
+                    assert!((f[idx[i]] < split_val) && f[idx[i]] != 0);
+                }
+                for i in idx[split_i..].iter() {
+                    assert!((f[*i] >= split_val) || (f[*i] == 0));
+                }
+            } else {
+                for i in 0..split_i {
+                    assert!((f[idx[i]] < split_val) || (f[idx[i]] == 0));
+                }
+                for i in idx[split_i..].iter() {
+                    assert!((f[*i] >= split_val) || (f[*i] != 0));
+                }
+            }
+        }
+
+        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
+        let f = vec![15, 10, 10, 11, 3, 18, 0, 9, 3, 5, 2, 6, 13, 19, 14];
+        let split_i = pivot_on_split(&mut idx, &f, 10, true);
+        pivot_assert(&f, &idx, split_i, true, 10);
+
+        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
+        let f = vec![15, 10, 10, 11, 3, 18, 0, 9, 3, 5, 2, 6, 13, 19, 14];
+        let split_i = pivot_on_split(&mut idx, &f, 10, false);
+        pivot_assert(&f, &idx, split_i, false, 10);
+
+        // Test Minimum value...
+        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
+        let f = vec![15, 10, 10, 11, 3, 18, 0, 9, 3, 5, 2, 6, 13, 19, 14];
+        let split_i = pivot_on_split(&mut idx, &f, 1, true);
+        pivot_assert(&f, &idx, split_i, true, 1);
+
+        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
+        let f = vec![15, 10, 10, 11, 3, 18, 0, 9, 3, 5, 2, 6, 13, 19, 14];
+        let split_i = pivot_on_split(&mut idx, &f, 1, false);
+        pivot_assert(&f, &idx, split_i, false, 1);
+
+        // Test Maximum value...
+        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
+        let f = vec![15, 10, 10, 11, 3, 18, 0, 9, 3, 5, 2, 6, 13, 19, 14];
+        let split_i = pivot_on_split(&mut idx, &f, 19, true);
+        pivot_assert(&f, &idx, split_i, true, 19);
+
+        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
+        let f = vec![15, 10, 10, 11, 3, 18, 0, 9, 3, 5, 2, 6, 13, 19, 14];
+        let split_i = pivot_on_split(&mut idx, &f, 19, false);
+        pivot_assert(&f, &idx, split_i, false, 19);
+
+        // Random tests... right...
+        // With missing
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let split_i = pivot_on_split(&mut idx, &f, 7, true);
+        pivot_assert(&f, &idx, split_i, true, 7);
+
+        // Already sorted...
+        let split_i = pivot_on_split(&mut idx, &f, 7, true);
+        pivot_assert(&f, &idx, split_i, true, 7);
+
+        // Reversed
+        idx.reverse();
+        let split_i = pivot_on_split(&mut idx, &f, 7, true);
+        pivot_assert(&f, &idx, split_i, true, 7);
+
+        // Without missing...
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(1..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let split_i = pivot_on_split(&mut idx, &f, 5, true);
+        pivot_assert(&f, &idx, split_i, true, 5);
+
+        // Using max...
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let sv = idx.iter().map(|i| f[*i]).max().unwrap();
+        let split_i = pivot_on_split(&mut idx, &f, sv, true);
+        pivot_assert(&f, &idx, split_i, true, sv);
+
+        // Using non-0 minimum...
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let sv = idx
+            .iter()
+            .filter(|i| f[**i] > 0)
+            .map(|i| f[*i])
+            .min()
+            .unwrap();
+        let split_i = pivot_on_split(&mut idx, &f, sv, true);
+        pivot_assert(&f, &idx, split_i, true, sv);
+
+        // Using non-0 minimum with no missing...
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(1..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let sv = idx
+            .iter()
+            .filter(|i| f[**i] > 0)
+            .map(|i| f[*i])
+            .min()
+            .unwrap();
+        let split_i = pivot_on_split(&mut idx, &f, sv, true);
+        pivot_assert(&f, &idx, split_i, true, sv);
+
+        // Left
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let split_i = pivot_on_split(&mut idx, &f, 7, false);
+        pivot_assert(&f, &idx, split_i, false, 7);
+
+        // Already sorted...
+        let split_i = pivot_on_split(&mut idx, &f, 7, false);
+        pivot_assert(&f, &idx, split_i, false, 7);
+
+        // Reversed
+        idx.reverse();
+        let split_i = pivot_on_split(&mut idx, &f, 7, false);
+        pivot_assert(&f, &idx, split_i, false, 7);
+
+        // Without missing...
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(1..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let split_i = pivot_on_split(&mut idx, &f, 5, false);
+        pivot_assert(&f, &idx, split_i, false, 5);
+
+        // Using max...
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let sv = idx.iter().map(|i| f[*i]).max().unwrap();
+        let split_i = pivot_on_split(&mut idx, &f, sv, false);
+        pivot_assert(&f, &idx, split_i, false, sv);
+
+        // Using non-0 minimum...
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let sv = idx
+            .iter()
+            .filter(|i| f[**i] > 0)
+            .map(|i| f[*i])
+            .min()
+            .unwrap();
+        let split_i = pivot_on_split(&mut idx, &f, sv, false);
+        pivot_assert(&f, &idx, split_i, false, sv);
+
+        // Using non-0 minimum with no missing...
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(1..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let sv = idx
+            .iter()
+            .filter(|i| f[**i] > 0)
+            .map(|i| f[*i])
+            .min()
+            .unwrap();
+        let split_i = pivot_on_split(&mut idx, &f, sv, false);
+        pivot_assert(&f, &idx, split_i, false, sv);
+    }
+
+    #[test]
+    fn test_pivot_missing() {
+        fn pivot_missing_assert(
+            split_value: u16,
+            idx: &[usize],
+            f: &[u16],
+            split_i: &(usize, usize),
+        ) {
+            // Check they are lower than..
+            for i in 0..split_i.1 {
+                assert!(f[idx[i]] < split_value);
+            }
+            // Check missing got moved
+            for i in 0..split_i.0 {
+                assert!(f[idx[i]] == 0);
+            }
+            // Check none are less than...
+            for i in split_i.1..(idx.len()) {
+                assert!(!(f[idx[i]] < split_value));
+            }
+            // Check none other are missing...
+            for i in split_i.0..(idx.len()) {
+                assert!(f[idx[i]] != 0);
+            }
+        }
+        // TODO: Add more tests for this...
+        // Using minimum value...
+        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
+        let f = vec![15, 10, 10, 0, 3, 0, 0, 9, 3, 5, 2, 6, 13, 19, 14];
+        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 1);
+        // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
+        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
+        pivot_missing_assert(1, &idx, &f, &split_i);
+
+        // Higher value...
+        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
+        let f = vec![15, 10, 10, 0, 3, 0, 0, 9, 3, 5, 2, 6, 13, 19, 14];
+        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 10);
+        //let split_i = pivot_on_split(&mut idx, &f, 10, false);
+        // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
+        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
+        pivot_missing_assert(10, &idx, &f, &split_i);
+
+        // Run it again, and ensure it works on an already sorted list...
+        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 10);
+        //let split_i = pivot_on_split(&mut idx, &f, 10, false);
+        // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
+        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
+        pivot_missing_assert(10, &idx, &f, &split_i);
+
+        // Run it again, and ensure it works on reversed list...
+        idx.reverse();
+        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 10);
+        //let split_i = pivot_on_split(&mut idx, &f, 10, false);
+        // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
+        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
+        pivot_missing_assert(10, &idx, &f, &split_i);
+
+        // Small test done with python
+        let mut idx = vec![0, 1, 2, 3, 4, 5];
+        let f = vec![1, 0, 1, 3, 0, 4];
+        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 2);
+        // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
+        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
+        pivot_missing_assert(2, &idx, &f, &split_i);
+
+        // Ensure it works on all missing...
+        // let mut idx = vec![0, 1, 2, 3, 4, 5];
+        // let f: Vec<u16> = vec![3; idx.len()];
+        // let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 2);
+        // // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
+        // // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
+        // pivot_missing_assert(2, &idx, &f, &split_i);
+
+        // Check if none missing...
+        // TODO: Add more tests for this...
+        let mut idx = vec![2, 6, 9, 5, 8, 13, 11, 7];
+        let f = vec![15, 10, 10, 2, 3, 5, 7, 9, 3, 5, 2, 6, 13, 19, 14];
+        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 10);
+        //let split_i = pivot_on_split(&mut idx, &f, 10, false);
+        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
+        // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
+        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
+        pivot_missing_assert(10, &idx, &f, &split_i);
+
+        // Random tests...
+        // With missing
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 10);
+        pivot_missing_assert(10, &idx, &f, &split_i);
+
+        // Already sorted...
+        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 10);
+        pivot_missing_assert(10, &idx, &f, &split_i);
+
+        // Without missing...
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(1..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, 5);
+        // let map_ = idx.iter().map(|i| f[*i]).collect::<Vec<u16>>();
+        // println!("{:?}, {:?}, {:?}", split_i, idx, map_);
+        pivot_missing_assert(5, &idx, &f, &split_i);
+
+        // Using max...
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let sv = idx.iter().map(|i| f[*i]).max().unwrap();
+        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, sv);
+        pivot_missing_assert(sv, &idx, &f, &split_i);
+
+        // Using non-0 minimum...
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(0..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let sv = idx
+            .iter()
+            .filter(|i| f[**i] > 0)
+            .map(|i| f[*i])
+            .min()
+            .unwrap();
+        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, sv);
+        pivot_missing_assert(sv, &idx, &f, &split_i);
+
+        // Using non-0 minimum with no missing...
+        let index = (0..100).collect::<Vec<usize>>();
+        let mut rng = StdRng::seed_from_u64(0);
+        let f = (0..100).map(|_| rng.gen_range(1..15)).collect::<Vec<u16>>();
+        let mut idx = index
+            .choose_multiple(&mut rng, 73)
+            .copied()
+            .collect::<Vec<usize>>();
+        let sv = idx
+            .iter()
+            .filter(|i| f[**i] > 0)
+            .map(|i| f[*i])
+            .min()
+            .unwrap();
+        let split_i = pivot_on_split_exclude_missing(&mut idx, &f, sv);
+        pivot_missing_assert(sv, &idx, &f, &split_i);
+    }
+
+    #[test]
+    fn test_fast_f64_sum() {
+        let records = 300000;
+        let vec = vec![0.23500371; records];
+        assert_ne!(vec.iter().sum::<f32>(), vec[0] * (records as f32));
+        assert_eq!(vec[0] * (records as f32), fast_f64_sum(&vec));
+        // println!("Sum Result: {}", vec.iter().sum::<f32>());
+        // println!("Multiplication Results {}", vec[0] * (records as f32));
+        // println!("f64_sum Results {}", f64_sum(&vec));
+    }
+}
```

### Comparing `forust-0.2.6/pyproject.toml` & `forust-0.2.7/pyproject.toml`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-[build-system]
-requires = ["maturin>=0.12,<0.13"]
-build-backend = "maturin"
-
-[project]
-name = "forust"
-description = "A lightweight gradient boosting implementation in Rust."
-license = { file = "LICENSE" }
-keywords = [
-  "rust",
-  "forust",
-  "machine learning",
-  "xgboost",
-  "tree model",
-  "decision tree",
-]
-authors = [{ name = "James Inlow" }]
-readme = "README.md"
-dependencies = ["numpy>=1.21", "pandas>=1.3"]
-requires-python = ">=3.8"
-classifiers = [
-  "Programming Language :: Rust",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
-]
-
-[project.optional-dependencies]
-dev = ["maturin", "pytest", "seaborn", "xgboost==1.6.1", "scikit-learn"]
-
-[tool.maturin]
-sdist-include = ["LICENSE", "README.md"]
+[build-system]
+requires = ["maturin>=0.12,<0.13"]
+build-backend = "maturin"
+
+[project]
+name = "forust"
+description = "A lightweight gradient boosting implementation in Rust."
+license = { file = "LICENSE" }
+keywords = [
+  "rust",
+  "forust",
+  "machine learning",
+  "xgboost",
+  "tree model",
+  "decision tree",
+]
+authors = [{ name = "James Inlow" }]
+readme = "README.md"
+dependencies = ["numpy>=1.21", "pandas>=1.3"]
+requires-python = ">=3.8"
+classifiers = [
+  "Programming Language :: Rust",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
+]
+
+[project.optional-dependencies]
+dev = ["maturin", "pytest", "seaborn", "xgboost==1.6.1", "scikit-learn"]
+
+[tool.maturin]
+sdist-include = ["LICENSE", "README.md"]
```

### Comparing `forust-0.2.6/scratch.py` & `forust-0.2.7/scratch.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,271 +1,271 @@
-# # import pandas as pd
-# # import numpy as np
-# # from forust import rust_bin_matrix
-
-# # df = pd.read_csv(
-# #     "../resources/titanic.csv"
-# # )  # .sample(1_000_000, replace=True, random_state=0)
-
-# # X = (
-# #     df.select_dtypes("number").drop(columns="survived").reset_index(drop=True)
-# # )  # [["pclass"]].astype(float)
-# # X_vec = X.to_numpy().ravel(order="F")
-
-# # w = np.ones(X.shape[0])  # np.random.uniform(0.1, 100, X.shape[0]),
-# # # w[X["age"] > 56] = 100000
-
-# # b, c, n = rust_bin_matrix(X_vec, X.shape[0], X.shape[1], w, nbins=5)
-# # Xb = pd.DataFrame(b.reshape(X.shape, order="F"))
-# # c[-1]
-
-# # X_rs = X.copy()
-# # for i in range(X.shape[1]):
-# #     X_rs.iloc[:, i] = pd.cut(X.iloc[:, i], c[i], right=False).cat.add_categories(
-# #         0
-# #     )  # pd.Series(np.digitize(X.iloc[:,i], c[i], right=True))
-# #     X_rs.iloc[X.iloc[:, i].isna(), i] = 0
-
-# # for i in range(X.shape[1]):
-# #     X_rs.iloc[:, i].value_counts()
-# #     Xb.iloc[:, i].value_counts()
-
-# # print(X_rs.iloc[:, 0].value_counts().sort_index())
-# # print(Xb.iloc[:, 0].value_counts().sort_index())
-
-# # print(X_rs.iloc[:, -1].value_counts().sort_index())
-# # print(Xb.iloc[:, -1].value_counts().sort_index())
-
-# # (X_rs.rename(columns={k: i for i, k in enumerate(X_rs.columns)}) == Xb).all()
-
-# # pd.concat([Xb.iloc[:, -1].head(), X.iloc[:, -1].head()], axis=1)
-# # c[-1]
-# # ####
-# # import pandas as pd
-# # import numpy as np
-# # from forust import percentiles
-
-# # df = pd.read_csv("../resources/titanic.csv").sample(
-# #     2_000_000, replace=True, random_state=0
-# # )
-# # pcts = np.array([0.1, 0.2, 0.5, 0.78])
-# # pcts = np.linspace(0, 1, num=200, endpoint=True)
-# # p1 = percentiles(df["fare"].to_numpy(), np.ones(df.shape[0]), pcts)
-
-
-# # df["fare"].nunique()
-# # p2 = np.percentile(df["fare"], pcts * 100)
-# # np.allclose(p1, p2)
-
-# # ####
-# # import pandas as pd
-# # import numpy as np
-# # from forust import GradientBooster
-
-# # df = pd.read_csv(
-# #     "../resources/titanic.csv"
-# # )  # .sample(100_000, replace=True, random_state=0)
-# # # for i in range(0, 50):
-# # i = 1000
-# # X = df.select_dtypes("number").drop(columns="survived").reset_index(drop=True)
-# # X["age"] = X["age"]  # .mul(-1)
-# # y = df["survived"].to_numpy().astype("float64")
-# # mod = GradientBooster(
-# #     iterations=i,
-# #     learning_rate=0.3,
-# #     max_depth=5,
-# #     l2=1,
-# #     min_leaf_weight=1,
-# #     gamma=1,
-# #     objective_type="LogLoss",
-# #     nbins=500,
-# #     parallel=False,
-# # )
-# # mod.fit(X, y)
-# # # print(mod.predict(X_vec, y.shape[0], 5)[0:10])
-
-# # from sklearn.ensemble import HistGradientBoostingClassifier
-
-# # # hgb = HistGradientBoostingClassifier(max_iter=100)
-# # # hgb.fit(X, y)
-# # # hgb.predict_proba(X)[0:10]
-
-# # from xgboost import XGBClassifier, XGBRegressor
-
-# # xmod = XGBClassifier(
-# #     n_estimators=i,
-# #     learning_rate=0.3,
-# #     max_depth=5,
-# #     reg_lambda=1,
-# #     min_child_weight=1,
-# #     gamma=1,
-# #     objective="binary:logitraw",
-# #     eval_metric="auc",
-# #     tree_method="hist",
-# #     max_bin=10000,
-# # )
-# # xmod.fit(X, y)
-# # # print(xmod.predict(X, output_margin=True)[0:10])
-# # np.allclose(
-# #     xmod.predict(X, output_margin=True).astype(np.float64),
-# #     mod.predict(X).astype(np.float32),
-# #     rtol=0.0001,
-# # )
-# # # if not np.allclose(xmod.predict(X, output_margin=True).astype(np.float32), mod.predict(X_vec, y.shape[0], 5).astype(np.float32), rtol=0.1):
-# # #     print(i)
-# # #     break
-# # mp = mod.predict(X)
-# # xp = xmod.predict(X, output_margin=True)
-# # print(mp[0:5])
-# # print(xp[0:5])
-
-# # mp[~np.isclose(mp, xp, rtol=0.0001)]
-# # xp[~np.isclose(mp, xp, rtol=0.0001)]
-
-
-# # print(xmod.get_booster().get_dump(with_stats=True)[-1])
-# # print(mod.text_dump()[-1])
-
-# import numpy as np
-
-# ### Testing weights
-# import pandas as pd
-# from xgboost import XGBClassifier
-
-# from forust import GradientBooster
-
-# df = (
-#     pd.read_csv("../resources/titanic.csv")
-#     .sample(500_000, replace=True, random_state=0)
-#     .reset_index(drop=True)
-# )
-# X = df.select_dtypes("number").drop(columns="survived").reset_index(drop=True)
-# y = df["survived"]
-
-# # X = X.fillna(0)
-# # w = X["fare"].to_numpy() + 1
-# xmod = XGBClassifier(
-#     n_estimators=100,
-#     learning_rate=0.3,
-#     max_depth=5,
-#     reg_lambda=1,
-#     min_child_weight=1.0,
-#     gamma=0.0,
-#     objective="binary:logitraw",
-#     eval_metric="auc",
-#     tree_method="hist",
-#     # max_bin=1000,
-# )
-# xmod.fit(X, y)  # , sample_weight=w)
-# xmod_preds = xmod.predict(X, output_margin=True)
-
-# fmod = GradientBooster(
-#     iterations=100,
-#     learning_rate=0.3,
-#     max_depth=5,
-#     l2=1,
-#     min_leaf_weight=1.0,
-#     gamma=0.0,
-#     objective_type="LogLoss",
-# )
-# fmod.fit(X, y=y)  # , sample_weight=w)
-# fmod_preds = fmod.predict(X)
-
-# print(fmod_preds[0:10])
-# print(xmod_preds[0:10])
-# print(np.allclose(fmod_preds, xmod_preds, atol=0.0001))
-
-
-# fmod.save_booster("mod2.json")
-# fmod2 = GradientBooster.load_booster("mod2.json")
-# fmod2.predict(X)
-
-
-# # from sklearn.metrics import roc_auc_score
-# # print(roc_auc_score(y, fmod_preds))
-# # print(roc_auc_score(y, xmod_preds))
-
-# # from forust import GradientBoosterF32
-# # import sys
-# # flat_data = X.to_numpy().ravel(order="F")
-# # mod = GradientBoosterF32(
-# #     objective_type = "LogLoss",
-# #         iterations = 100,
-# #         learning_rate = 0.3,
-# #         max_depth = 5,
-# #         max_leaves = sys.maxsize,
-# #         l2 = 1.0,
-# #         gamma = 0.0,
-# #         min_leaf_weight = 0.0,
-# #         base_score = 0.5,
-# #         nbins = 256,
-# #         parallel = True
-# # )
-# # mod.fit(
-# #     flat_data, *X.shape, y.to_numpy(), np.ones(y.shape, "float32")
-# # )
-
-# # print(fmod.text_dump()[0])
-# # print(xmod.get_booster().get_dump(with_stats=True)[0])
-
-
-# fmod_preds[~np.isclose(fmod_preds, xmod_preds, rtol=0.001)]
-# xmod_preds[~np.isclose(fmod_preds, xmod_preds, atol=0.001)]
-# fmod_preds[~np.isclose(fmod_preds, xmod_preds, atol=0.001)]
-# assert np.allclose(fmod_preds, xmod_preds, rtol=0.001)
-
-
-# import numpy as np
-
-# # Trying regression
-# import pandas as pd
-# from xgboost import XGBClassifier
-
-# from forust import GradientBooster
-
-# df = (
-#     pd.read_csv("../resources/titanic.csv")
-#     .sample(100_000, replace=True, random_state=0)
-#     .reset_index(drop=True)
-# )
-# X = df.select_dtypes("number").drop(columns="fare").reset_index(drop=True)
-# y = df["fare"]
-
-# # X = X.fillna(0)
-# # w = X["fare"].to_numpy() + 1
-# from xgboost import XGBRegressor
-
-# xmod = XGBRegressor(
-#     n_estimators=100,
-#     learning_rate=0.3,
-#     max_depth=5,
-#     reg_lambda=1,
-#     min_child_weight=1.0,
-#     gamma=0.0,
-#     objective="reg:squarederror",
-#     eval_metric="auc",
-#     # tree_method="hist",
-#     # max_bin=1000,
-# )
-# xmod.fit(X, y)  # , sample_weight=w)
-# xmod_preds = xmod.predict(X, output_margin=True)
-
-# fmod = GradientBooster(
-#     iterations=100,
-#     learning_rate=0.3,
-#     max_depth=5,
-#     l2=1,
-#     min_leaf_weight=1.0,
-#     gamma=0.0,
-#     objective_type="SquaredLoss",
-# )
-# fmod.fit(X, y=y)  # , sample_weight=w)
-# fmod_preds = fmod.predict(X)
-
-# print(fmod_preds[0:10])
-# print(xmod_preds[0:10])
-
-# fmod.save_booster("mod2.json")
-# fmod2 = GradientBooster.load_booster("mod2.json")
-# fmod2.predict(X)
-
-# fmod.booster.json_dump()
+# # import pandas as pd
+# # import numpy as np
+# # from forust import rust_bin_matrix
+
+# # df = pd.read_csv(
+# #     "../resources/titanic.csv"
+# # )  # .sample(1_000_000, replace=True, random_state=0)
+
+# # X = (
+# #     df.select_dtypes("number").drop(columns="survived").reset_index(drop=True)
+# # )  # [["pclass"]].astype(float)
+# # X_vec = X.to_numpy().ravel(order="F")
+
+# # w = np.ones(X.shape[0])  # np.random.uniform(0.1, 100, X.shape[0]),
+# # # w[X["age"] > 56] = 100000
+
+# # b, c, n = rust_bin_matrix(X_vec, X.shape[0], X.shape[1], w, nbins=5)
+# # Xb = pd.DataFrame(b.reshape(X.shape, order="F"))
+# # c[-1]
+
+# # X_rs = X.copy()
+# # for i in range(X.shape[1]):
+# #     X_rs.iloc[:, i] = pd.cut(X.iloc[:, i], c[i], right=False).cat.add_categories(
+# #         0
+# #     )  # pd.Series(np.digitize(X.iloc[:,i], c[i], right=True))
+# #     X_rs.iloc[X.iloc[:, i].isna(), i] = 0
+
+# # for i in range(X.shape[1]):
+# #     X_rs.iloc[:, i].value_counts()
+# #     Xb.iloc[:, i].value_counts()
+
+# # print(X_rs.iloc[:, 0].value_counts().sort_index())
+# # print(Xb.iloc[:, 0].value_counts().sort_index())
+
+# # print(X_rs.iloc[:, -1].value_counts().sort_index())
+# # print(Xb.iloc[:, -1].value_counts().sort_index())
+
+# # (X_rs.rename(columns={k: i for i, k in enumerate(X_rs.columns)}) == Xb).all()
+
+# # pd.concat([Xb.iloc[:, -1].head(), X.iloc[:, -1].head()], axis=1)
+# # c[-1]
+# # ####
+# # import pandas as pd
+# # import numpy as np
+# # from forust import percentiles
+
+# # df = pd.read_csv("../resources/titanic.csv").sample(
+# #     2_000_000, replace=True, random_state=0
+# # )
+# # pcts = np.array([0.1, 0.2, 0.5, 0.78])
+# # pcts = np.linspace(0, 1, num=200, endpoint=True)
+# # p1 = percentiles(df["fare"].to_numpy(), np.ones(df.shape[0]), pcts)
+
+
+# # df["fare"].nunique()
+# # p2 = np.percentile(df["fare"], pcts * 100)
+# # np.allclose(p1, p2)
+
+# # ####
+# # import pandas as pd
+# # import numpy as np
+# # from forust import GradientBooster
+
+# # df = pd.read_csv(
+# #     "../resources/titanic.csv"
+# # )  # .sample(100_000, replace=True, random_state=0)
+# # # for i in range(0, 50):
+# # i = 1000
+# # X = df.select_dtypes("number").drop(columns="survived").reset_index(drop=True)
+# # X["age"] = X["age"]  # .mul(-1)
+# # y = df["survived"].to_numpy().astype("float64")
+# # mod = GradientBooster(
+# #     iterations=i,
+# #     learning_rate=0.3,
+# #     max_depth=5,
+# #     l2=1,
+# #     min_leaf_weight=1,
+# #     gamma=1,
+# #     objective_type="LogLoss",
+# #     nbins=500,
+# #     parallel=False,
+# # )
+# # mod.fit(X, y)
+# # # print(mod.predict(X_vec, y.shape[0], 5)[0:10])
+
+# # from sklearn.ensemble import HistGradientBoostingClassifier
+
+# # # hgb = HistGradientBoostingClassifier(max_iter=100)
+# # # hgb.fit(X, y)
+# # # hgb.predict_proba(X)[0:10]
+
+# # from xgboost import XGBClassifier, XGBRegressor
+
+# # xmod = XGBClassifier(
+# #     n_estimators=i,
+# #     learning_rate=0.3,
+# #     max_depth=5,
+# #     reg_lambda=1,
+# #     min_child_weight=1,
+# #     gamma=1,
+# #     objective="binary:logitraw",
+# #     eval_metric="auc",
+# #     tree_method="hist",
+# #     max_bin=10000,
+# # )
+# # xmod.fit(X, y)
+# # # print(xmod.predict(X, output_margin=True)[0:10])
+# # np.allclose(
+# #     xmod.predict(X, output_margin=True).astype(np.float64),
+# #     mod.predict(X).astype(np.float32),
+# #     rtol=0.0001,
+# # )
+# # # if not np.allclose(xmod.predict(X, output_margin=True).astype(np.float32), mod.predict(X_vec, y.shape[0], 5).astype(np.float32), rtol=0.1):
+# # #     print(i)
+# # #     break
+# # mp = mod.predict(X)
+# # xp = xmod.predict(X, output_margin=True)
+# # print(mp[0:5])
+# # print(xp[0:5])
+
+# # mp[~np.isclose(mp, xp, rtol=0.0001)]
+# # xp[~np.isclose(mp, xp, rtol=0.0001)]
+
+
+# # print(xmod.get_booster().get_dump(with_stats=True)[-1])
+# # print(mod.text_dump()[-1])
+
+# import numpy as np
+
+# ### Testing weights
+# import pandas as pd
+# from xgboost import XGBClassifier
+
+# from forust import GradientBooster
+
+# df = (
+#     pd.read_csv("../resources/titanic.csv")
+#     .sample(500_000, replace=True, random_state=0)
+#     .reset_index(drop=True)
+# )
+# X = df.select_dtypes("number").drop(columns="survived").reset_index(drop=True)
+# y = df["survived"]
+
+# # X = X.fillna(0)
+# # w = X["fare"].to_numpy() + 1
+# xmod = XGBClassifier(
+#     n_estimators=100,
+#     learning_rate=0.3,
+#     max_depth=5,
+#     reg_lambda=1,
+#     min_child_weight=1.0,
+#     gamma=0.0,
+#     objective="binary:logitraw",
+#     eval_metric="auc",
+#     tree_method="hist",
+#     # max_bin=1000,
+# )
+# xmod.fit(X, y)  # , sample_weight=w)
+# xmod_preds = xmod.predict(X, output_margin=True)
+
+# fmod = GradientBooster(
+#     iterations=100,
+#     learning_rate=0.3,
+#     max_depth=5,
+#     l2=1,
+#     min_leaf_weight=1.0,
+#     gamma=0.0,
+#     objective_type="LogLoss",
+# )
+# fmod.fit(X, y=y)  # , sample_weight=w)
+# fmod_preds = fmod.predict(X)
+
+# print(fmod_preds[0:10])
+# print(xmod_preds[0:10])
+# print(np.allclose(fmod_preds, xmod_preds, atol=0.0001))
+
+
+# fmod.save_booster("mod2.json")
+# fmod2 = GradientBooster.load_booster("mod2.json")
+# fmod2.predict(X)
+
+
+# # from sklearn.metrics import roc_auc_score
+# # print(roc_auc_score(y, fmod_preds))
+# # print(roc_auc_score(y, xmod_preds))
+
+# # from forust import GradientBoosterF32
+# # import sys
+# # flat_data = X.to_numpy().ravel(order="F")
+# # mod = GradientBoosterF32(
+# #     objective_type = "LogLoss",
+# #         iterations = 100,
+# #         learning_rate = 0.3,
+# #         max_depth = 5,
+# #         max_leaves = sys.maxsize,
+# #         l2 = 1.0,
+# #         gamma = 0.0,
+# #         min_leaf_weight = 0.0,
+# #         base_score = 0.5,
+# #         nbins = 256,
+# #         parallel = True
+# # )
+# # mod.fit(
+# #     flat_data, *X.shape, y.to_numpy(), np.ones(y.shape, "float32")
+# # )
+
+# # print(fmod.text_dump()[0])
+# # print(xmod.get_booster().get_dump(with_stats=True)[0])
+
+
+# fmod_preds[~np.isclose(fmod_preds, xmod_preds, rtol=0.001)]
+# xmod_preds[~np.isclose(fmod_preds, xmod_preds, atol=0.001)]
+# fmod_preds[~np.isclose(fmod_preds, xmod_preds, atol=0.001)]
+# assert np.allclose(fmod_preds, xmod_preds, rtol=0.001)
+
+
+# import numpy as np
+
+# # Trying regression
+# import pandas as pd
+# from xgboost import XGBClassifier
+
+# from forust import GradientBooster
+
+# df = (
+#     pd.read_csv("../resources/titanic.csv")
+#     .sample(100_000, replace=True, random_state=0)
+#     .reset_index(drop=True)
+# )
+# X = df.select_dtypes("number").drop(columns="fare").reset_index(drop=True)
+# y = df["fare"]
+
+# # X = X.fillna(0)
+# # w = X["fare"].to_numpy() + 1
+# from xgboost import XGBRegressor
+
+# xmod = XGBRegressor(
+#     n_estimators=100,
+#     learning_rate=0.3,
+#     max_depth=5,
+#     reg_lambda=1,
+#     min_child_weight=1.0,
+#     gamma=0.0,
+#     objective="reg:squarederror",
+#     eval_metric="auc",
+#     # tree_method="hist",
+#     # max_bin=1000,
+# )
+# xmod.fit(X, y)  # , sample_weight=w)
+# xmod_preds = xmod.predict(X, output_margin=True)
+
+# fmod = GradientBooster(
+#     iterations=100,
+#     learning_rate=0.3,
+#     max_depth=5,
+#     l2=1,
+#     min_leaf_weight=1.0,
+#     gamma=0.0,
+#     objective_type="SquaredLoss",
+# )
+# fmod.fit(X, y=y)  # , sample_weight=w)
+# fmod_preds = fmod.predict(X)
+
+# print(fmod_preds[0:10])
+# print(xmod_preds[0:10])
+
+# fmod.save_booster("mod2.json")
+# fmod2 = GradientBooster.load_booster("mod2.json")
+# fmod2.predict(X)
+
+# fmod.booster.json_dump()
```

### Comparing `forust-0.2.6/src/lib.rs` & `forust-0.2.7/src/lib.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,285 +1,370 @@
-use forust_ml::constraints::{Constraint, ConstraintMap};
-use forust_ml::data::Matrix;
-use forust_ml::gradientbooster::{ContributionsMethod, GradientBooster as CrateGradientBooster};
-use forust_ml::objective::ObjectiveType;
-use forust_ml::utils::percentiles as crate_percentiles;
-use numpy::{IntoPyArray, PyArray1, PyReadonlyArray1};
-use pyo3::exceptions::{PyKeyError, PyValueError};
-use pyo3::prelude::*;
-use pyo3::types::IntoPyDict;
-use pyo3::types::PyType;
-use std::collections::HashMap;
-
-fn int_map_to_constraint_map(int_map: HashMap<usize, i8>) -> PyResult<ConstraintMap> {
-    let mut constraints: ConstraintMap = HashMap::new();
-    for (f, c) in int_map.iter() {
-        let c_ = match c {
-                -1 => Ok(Constraint::Negative),
-                1 => Ok(Constraint::Positive),
-                0 => Ok(Constraint::Unconstrained),
-                _ => Err(PyValueError::new_err(format!("Valid monotone constraints are -1, 1 or 0, but '{}' was provided for feature number {}.", c, f))),
-            }?;
-        constraints.insert(*f, c_);
-    }
-    Ok(constraints)
-}
-
-// This macro is used to define the base implementation of
-// the booster.
-#[pyclass(subclass)]
-struct GradientBooster {
-    booster: CrateGradientBooster,
-}
-
-#[pymethods]
-impl GradientBooster {
-    #[new]
-    #[allow(clippy::too_many_arguments)]
-    pub fn new(
-        objective_type: &str,
-        iterations: usize,
-        learning_rate: f32,
-        max_depth: usize,
-        max_leaves: usize,
-        l2: f32,
-        gamma: f32,
-        min_leaf_weight: f32,
-        base_score: f64,
-        nbins: u16,
-        parallel: bool,
-        allow_missing_splits: bool,
-        monotone_constraints: HashMap<usize, i8>,
-        subsample: f32,
-        seed: u64,
-        missing: f64,
-        create_missing_branch: bool,
-    ) -> PyResult<Self> {
-        let constraints = int_map_to_constraint_map(monotone_constraints)?;
-        let objective_ = match objective_type {
-            "LogLoss" => Ok(ObjectiveType::LogLoss),
-            "SquaredLoss" => Ok(ObjectiveType::SquaredLoss),
-            _ => Err(PyValueError::new_err(format!("Not a valid objective type passed, expected one of 'LogLoss', 'SquaredLoss', but '{}' was provided.", objective_type))),
-        }?;
-        let booster = CrateGradientBooster::new(
-            objective_,
-            iterations,
-            learning_rate,
-            max_depth,
-            max_leaves,
-            l2,
-            gamma,
-            min_leaf_weight,
-            base_score,
-            nbins,
-            parallel,
-            allow_missing_splits,
-            Some(constraints),
-            subsample,
-            seed,
-            missing,
-            create_missing_branch,
-        );
-        Ok(GradientBooster { booster })
-    }
-
-    #[setter]
-    fn set_monotone_constraints(&mut self, value: HashMap<usize, i8>) -> PyResult<()> {
-        let map = int_map_to_constraint_map(value)?;
-        self.booster.monotone_constraints = Some(map);
-        Ok(())
-    }
-
-    pub fn fit(
-        &mut self,
-        flat_data: PyReadonlyArray1<f64>,
-        rows: usize,
-        cols: usize,
-        y: PyReadonlyArray1<f64>,
-        sample_weight: PyReadonlyArray1<f64>,
-    ) -> PyResult<()> {
-        let flat_data = flat_data.as_slice()?;
-        let data = Matrix::new(flat_data, rows, cols);
-        let y = y.as_slice()?;
-        let sample_weight = sample_weight.as_slice()?;
-        match self.booster.fit(&data, y, sample_weight) {
-            Ok(m) => Ok(m),
-            Err(e) => Err(PyValueError::new_err(e.to_string())),
-        }?;
-        Ok(())
-    }
-    pub fn predict<'py>(
-        &self,
-        py: Python<'py>,
-        flat_data: PyReadonlyArray1<f64>,
-        rows: usize,
-        cols: usize,
-        parallel: Option<bool>,
-    ) -> PyResult<&'py PyArray1<f64>> {
-        let flat_data = flat_data.as_slice()?;
-        let data = Matrix::new(flat_data, rows, cols);
-        let parallel = parallel.unwrap_or(true);
-        Ok(self.booster.predict(&data, parallel).into_pyarray(py))
-    }
-    pub fn predict_contributions<'py>(
-        &self,
-        py: Python<'py>,
-        flat_data: PyReadonlyArray1<f64>,
-        rows: usize,
-        cols: usize,
-        method: &str,
-        parallel: Option<bool>,
-    ) -> PyResult<&'py PyArray1<f64>> {
-        let flat_data = flat_data.as_slice()?;
-        let data = Matrix::new(flat_data, rows, cols);
-        let parallel = parallel.unwrap_or(true);
-        let method_ = match method {
-            "weight" => Ok(ContributionsMethod::Weight),
-            "average" => Ok(ContributionsMethod::Average),
-            _ => Err(PyValueError::new_err(format!("Not a valid contributions method passed, expected one of 'weight', 'average', but '{}' was provided.", method))),
-        }?;
-        Ok(self
-            .booster
-            .predict_contributions(&data, method_, parallel)
-            .into_pyarray(py))
-    }
-
-    pub fn value_partial_dependence(&self, feature: usize, value: f64) -> PyResult<f64> {
-        Ok(self.booster.value_partial_dependence(feature, value))
-    }
-
-    pub fn text_dump(&self) -> PyResult<Vec<String>> {
-        let mut trees = Vec::new();
-        for t in &self.booster.trees {
-            trees.push(format!("{}", t));
-        }
-        Ok(trees)
-    }
-
-    pub fn save_booster(&self, path: &str) -> PyResult<()> {
-        match self.booster.save_booster(path) {
-            Ok(_) => Ok(()),
-            Err(e) => Err(PyValueError::new_err(e.to_string())),
-        }
-    }
-
-    pub fn json_dump(&self) -> PyResult<String> {
-        match self.booster.json_dump() {
-            Ok(m) => Ok(m),
-            Err(e) => Err(PyValueError::new_err(e.to_string())),
-        }
-    }
-
-    pub fn insert_metadata(&mut self, key: String, value: String) -> PyResult<()> {
-        self.booster.insert_metadata(key, value);
-        Ok(())
-    }
-
-    pub fn get_metadata(&self, key: String) -> PyResult<String> {
-        match self.booster.get_metadata(&key) {
-            Some(m) => Ok(m),
-            None => Err(PyKeyError::new_err(
-                format!("No value associated with provided key {}", key).to_string(),
-            )),
-        }
-    }
-
-    #[classmethod]
-    pub fn load_booster(_: &PyType, path: String) -> PyResult<Self> {
-        let booster = match CrateGradientBooster::load_booster(path.as_str()) {
-            Ok(m) => Ok(m),
-            Err(e) => Err(PyValueError::new_err(e.to_string())),
-        }?;
-        Ok(GradientBooster { booster })
-    }
-
-    #[classmethod]
-    pub fn from_json(_: &PyType, json_str: &str) -> PyResult<Self> {
-        let booster = match CrateGradientBooster::from_json(json_str) {
-            Ok(m) => Ok(m),
-            Err(e) => Err(PyValueError::new_err(e.to_string())),
-        }?;
-        Ok(GradientBooster { booster })
-    }
-
-    pub fn get_params(&self, py: Python) -> PyResult<PyObject> {
-        let objective_ = match self.booster.objective_type {
-            ObjectiveType::LogLoss => "LogLoss",
-            ObjectiveType::SquaredLoss => "SquaredLoss",
-        };
-        let constraints: HashMap<usize, i8> = self
-            .booster
-            .monotone_constraints
-            .as_ref()
-            .unwrap()
-            .iter()
-            .map(|(f, c)| {
-                let c_ = match c {
-                    Constraint::Negative => -1,
-                    Constraint::Positive => 1,
-                    Constraint::Unconstrained => 0,
-                };
-                (*f, c_)
-            })
-            .collect();
-        let key_vals: Vec<(&str, PyObject)> = vec![
-            ("objective_type", objective_.to_object(py)),
-            ("iterations", self.booster.iterations.to_object(py)),
-            ("learning_rate", self.booster.learning_rate.to_object(py)),
-            ("max_depth", self.booster.max_depth.to_object(py)),
-            ("max_leaves", self.booster.max_leaves.to_object(py)),
-            ("l2", self.booster.l2.to_object(py)),
-            ("gamma", self.booster.gamma.to_object(py)),
-            (
-                "min_leaf_weight",
-                self.booster.min_leaf_weight.to_object(py),
-            ),
-            ("base_score", self.booster.base_score.to_object(py)),
-            ("nbins", self.booster.nbins.to_object(py)),
-            ("parallel", self.booster.parallel.to_object(py)),
-            (
-                "allow_missing_splits",
-                self.booster.allow_missing_splits.to_object(py),
-            ),
-            ("monotone_constraints", constraints.to_object(py)),
-            ("subsample", self.booster.subsample.to_object(py)),
-            ("seed", self.booster.seed.to_object(py)),
-            ("missing", self.booster.missing.to_object(py)),
-            (
-                "create_missing_branch",
-                self.booster.create_missing_branch.to_object(py),
-            ),
-        ];
-        let dict = key_vals.into_py_dict(py);
-        Ok(dict.to_object(py))
-    }
-}
-
-#[pyfunction]
-fn print_matrix(x: PyReadonlyArray1<f32>, rows: usize, cols: usize) -> PyResult<()> {
-    let m = Matrix::new(x.as_slice()?, rows, cols);
-    println!("{}", m);
-    Ok(())
-}
-
-#[pyfunction]
-fn percentiles<'py>(
-    py: Python<'py>,
-    v: PyReadonlyArray1<f64>,
-    sample_weight: PyReadonlyArray1<f64>,
-    percentiles: PyReadonlyArray1<f64>,
-) -> PyResult<&'py PyArray1<f64>> {
-    let v_ = v.as_slice()?;
-    let sample_weight_ = sample_weight.as_slice()?;
-    let percentiles_ = percentiles.as_slice()?;
-    let p = crate_percentiles(v_, sample_weight_, percentiles_);
-    Ok(p.into_pyarray(py))
-}
-
-/// A Python module implemented in Rust.
-#[pymodule]
-fn forust(_py: Python, m: &PyModule) -> PyResult<()> {
-    m.add_function(wrap_pyfunction!(print_matrix, m)?)?;
-    m.add_function(wrap_pyfunction!(percentiles, m)?)?;
-    m.add_class::<GradientBooster>()?;
-    Ok(())
-}
+use forust_ml::constraints::{Constraint, ConstraintMap};
+use forust_ml::data::Matrix;
+use forust_ml::errors::ForustError;
+use forust_ml::gradientbooster::EvaluationData;
+use forust_ml::gradientbooster::{ContributionsMethod, GradientBooster as CrateGradientBooster};
+use forust_ml::metric::Metric;
+use forust_ml::objective::ObjectiveType;
+use forust_ml::sampler::SampleMethod;
+use forust_ml::utils::percentiles as crate_percentiles;
+use numpy::{IntoPyArray, PyArray1, PyReadonlyArray1};
+use pyo3::exceptions::{PyKeyError, PyValueError};
+use pyo3::prelude::*;
+use pyo3::types::IntoPyDict;
+use pyo3::types::PyType;
+use std::collections::HashMap;
+use std::str::FromStr;
+
+type PyEvaluationData<'a> = (
+    PyReadonlyArray1<'a, f64>,
+    usize,
+    usize,
+    PyReadonlyArray1<'a, f64>,
+    PyReadonlyArray1<'a, f64>,
+);
+
+fn int_map_to_constraint_map(int_map: HashMap<usize, i8>) -> PyResult<ConstraintMap> {
+    let mut constraints: ConstraintMap = HashMap::new();
+    for (f, c) in int_map.iter() {
+        let c_ = match c {
+                -1 => Ok(Constraint::Negative),
+                1 => Ok(Constraint::Positive),
+                0 => Ok(Constraint::Unconstrained),
+                _ => Err(PyValueError::new_err(format!("Valid monotone constraints are -1, 1 or 0, but '{}' was provided for feature number {}.", c, f))),
+            }?;
+        constraints.insert(*f, c_);
+    }
+    Ok(constraints)
+}
+
+fn to_value_error<T>(value: Result<T, ForustError>) -> Result<T, PyErr> {
+    match value {
+        Ok(v) => Ok(v),
+        Err(e) => Err(PyValueError::new_err(e.to_string())),
+    }
+}
+
+#[pyclass(subclass)]
+struct GradientBooster {
+    booster: CrateGradientBooster,
+}
+
+#[pymethods]
+impl GradientBooster {
+    #[new]
+    #[allow(clippy::too_many_arguments)]
+    pub fn new(
+        objective_type: &str,
+        iterations: usize,
+        learning_rate: f32,
+        max_depth: usize,
+        max_leaves: usize,
+        l2: f32,
+        gamma: f32,
+        min_leaf_weight: f32,
+        base_score: f64,
+        nbins: u16,
+        parallel: bool,
+        allow_missing_splits: bool,
+        monotone_constraints: HashMap<usize, i8>,
+        subsample: f32,
+        seed: u64,
+        missing: f64,
+        create_missing_branch: bool,
+        sample_method: Option<&str>,
+        evaluation_metric: Option<&str>,
+        early_stopping_rounds: Option<usize>,
+    ) -> PyResult<Self> {
+        let constraints = int_map_to_constraint_map(monotone_constraints)?;
+        let objective_ = to_value_error(ObjectiveType::from_str(objective_type))?;
+        let sample_method_ = match sample_method {
+            Some(s) => to_value_error(SampleMethod::from_str(s))?,
+            None => SampleMethod::None,
+        };
+        let evaluation_metric_ = match evaluation_metric {
+            Some(s) => Some(to_value_error(Metric::from_str(s))?),
+            None => None,
+        };
+        let booster = CrateGradientBooster::new(
+            objective_,
+            iterations,
+            learning_rate,
+            max_depth,
+            max_leaves,
+            l2,
+            gamma,
+            min_leaf_weight,
+            base_score,
+            nbins,
+            parallel,
+            allow_missing_splits,
+            Some(constraints),
+            subsample,
+            seed,
+            missing,
+            create_missing_branch,
+            sample_method_,
+            evaluation_metric_,
+            early_stopping_rounds,
+        );
+        Ok(GradientBooster { booster })
+    }
+
+    #[setter]
+    fn set_monotone_constraints(&mut self, value: HashMap<usize, i8>) -> PyResult<()> {
+        let map = int_map_to_constraint_map(value)?;
+        self.booster.monotone_constraints = Some(map);
+        Ok(())
+    }
+
+    #[setter]
+    fn set_prediction_iteration(&mut self, value: Option<usize>) -> PyResult<()> {
+        self.booster.prediction_iteration = value;
+        Ok(())
+    }
+
+    #[getter]
+    fn best_iteration(&self) -> PyResult<Option<usize>> {
+        Ok(self.booster.best_iteration)
+    }
+
+    pub fn fit(
+        &mut self,
+        flat_data: PyReadonlyArray1<f64>,
+        rows: usize,
+        cols: usize,
+        y: PyReadonlyArray1<f64>,
+        sample_weight: PyReadonlyArray1<f64>,
+        evaluation_data: Option<Vec<PyEvaluationData>>,
+    ) -> PyResult<()> {
+        let flat_data = flat_data.as_slice()?;
+        let data = Matrix::new(flat_data, rows, cols);
+        let y = y.as_slice()?;
+        let sample_weight = sample_weight.as_slice()?;
+
+        let evaluation_data_: Option<Vec<EvaluationData>> = match evaluation_data.as_ref() {
+            None => None,
+            Some(values) => {
+                let mut eval_data = Vec::new();
+                for (a, r, c, y_, w_) in values.iter() {
+                    eval_data.push((
+                        Matrix::new(a.as_slice()?, *r, *c),
+                        y_.as_slice()?,
+                        w_.as_slice()?,
+                    ));
+                }
+                Some(eval_data)
+            }
+        };
+        match self.booster.fit(&data, y, sample_weight, evaluation_data_) {
+            Ok(m) => Ok(m),
+            Err(e) => Err(PyValueError::new_err(e.to_string())),
+        }?;
+        Ok(())
+    }
+    pub fn predict<'py>(
+        &self,
+        py: Python<'py>,
+        flat_data: PyReadonlyArray1<f64>,
+        rows: usize,
+        cols: usize,
+        parallel: Option<bool>,
+    ) -> PyResult<&'py PyArray1<f64>> {
+        let flat_data = flat_data.as_slice()?;
+        let data = Matrix::new(flat_data, rows, cols);
+        let parallel = parallel.unwrap_or(true);
+        Ok(self.booster.predict(&data, parallel).into_pyarray(py))
+    }
+    pub fn predict_contributions<'py>(
+        &self,
+        py: Python<'py>,
+        flat_data: PyReadonlyArray1<f64>,
+        rows: usize,
+        cols: usize,
+        method: &str,
+        parallel: Option<bool>,
+    ) -> PyResult<&'py PyArray1<f64>> {
+        let flat_data = flat_data.as_slice()?;
+        let data = Matrix::new(flat_data, rows, cols);
+        let parallel = parallel.unwrap_or(true);
+        let method_ = match method {
+            "weight" => Ok(ContributionsMethod::Weight),
+            "average" => Ok(ContributionsMethod::Average),
+            _ => Err(PyValueError::new_err(format!("Not a valid contributions method passed, expected one of 'weight', 'average', but '{}' was provided.", method))),
+        }?;
+        Ok(self
+            .booster
+            .predict_contributions(&data, method_, parallel)
+            .into_pyarray(py))
+    }
+
+    pub fn value_partial_dependence(&self, feature: usize, value: f64) -> PyResult<f64> {
+        Ok(self.booster.value_partial_dependence(feature, value))
+    }
+
+    pub fn text_dump(&self) -> PyResult<Vec<String>> {
+        let mut trees = Vec::new();
+        for t in &self.booster.trees {
+            trees.push(format!("{}", t));
+        }
+        Ok(trees)
+    }
+
+    pub fn save_booster(&self, path: &str) -> PyResult<()> {
+        match self.booster.save_booster(path) {
+            Ok(_) => Ok(()),
+            Err(e) => Err(PyValueError::new_err(e.to_string())),
+        }
+    }
+
+    pub fn json_dump(&self) -> PyResult<String> {
+        match self.booster.json_dump() {
+            Ok(m) => Ok(m),
+            Err(e) => Err(PyValueError::new_err(e.to_string())),
+        }
+    }
+
+    pub fn insert_metadata(&mut self, key: String, value: String) -> PyResult<()> {
+        self.booster.insert_metadata(key, value);
+        Ok(())
+    }
+
+    pub fn get_metadata(&self, key: String) -> PyResult<String> {
+        match self.booster.get_metadata(&key) {
+            Some(m) => Ok(m),
+            None => Err(PyKeyError::new_err(format!(
+                "No value associated with provided key {}",
+                key
+            ))),
+        }
+    }
+
+    #[classmethod]
+    pub fn load_booster(_: &PyType, path: String) -> PyResult<Self> {
+        let booster = match CrateGradientBooster::load_booster(path.as_str()) {
+            Ok(m) => Ok(m),
+            Err(e) => Err(PyValueError::new_err(e.to_string())),
+        }?;
+        Ok(GradientBooster { booster })
+    }
+
+    #[classmethod]
+    pub fn from_json(_: &PyType, json_str: &str) -> PyResult<Self> {
+        let booster = match CrateGradientBooster::from_json(json_str) {
+            Ok(m) => Ok(m),
+            Err(e) => Err(PyValueError::new_err(e.to_string())),
+        }?;
+        Ok(GradientBooster { booster })
+    }
+
+    pub fn get_params(&self, py: Python) -> PyResult<PyObject> {
+        let objective_ = match self.booster.objective_type {
+            ObjectiveType::LogLoss => "LogLoss",
+            ObjectiveType::SquaredLoss => "SquaredLoss",
+        };
+        let sample_method_: Option<&str> = match self.booster.sample_method {
+            SampleMethod::Random => Some("random"),
+            SampleMethod::Goss => Some("goss"),
+            SampleMethod::None => None,
+        };
+        let evaluation_metric_: Option<&str> = match self.booster.evaluation_metric {
+            Some(Metric::AUC) => Some("AUC"),
+            Some(Metric::LogLoss) => Some("LogLoss"),
+            Some(Metric::RootMeanSquaredLogError) => Some("RootMeanSquaredLogError"),
+            Some(Metric::RootMeanSquaredError) => Some("RootMeanSquaredError"),
+            _ => None,
+        };
+        let constraints: HashMap<usize, i8> = self
+            .booster
+            .monotone_constraints
+            .as_ref()
+            .unwrap()
+            .iter()
+            .map(|(f, c)| {
+                let c_ = match c {
+                    Constraint::Negative => -1,
+                    Constraint::Positive => 1,
+                    Constraint::Unconstrained => 0,
+                };
+                (*f, c_)
+            })
+            .collect();
+        let key_vals: Vec<(&str, PyObject)> = vec![
+            ("objective_type", objective_.to_object(py)),
+            ("iterations", self.booster.iterations.to_object(py)),
+            ("learning_rate", self.booster.learning_rate.to_object(py)),
+            ("max_depth", self.booster.max_depth.to_object(py)),
+            ("max_leaves", self.booster.max_leaves.to_object(py)),
+            ("l2", self.booster.l2.to_object(py)),
+            ("gamma", self.booster.gamma.to_object(py)),
+            (
+                "min_leaf_weight",
+                self.booster.min_leaf_weight.to_object(py),
+            ),
+            ("base_score", self.booster.base_score.to_object(py)),
+            ("nbins", self.booster.nbins.to_object(py)),
+            ("parallel", self.booster.parallel.to_object(py)),
+            (
+                "allow_missing_splits",
+                self.booster.allow_missing_splits.to_object(py),
+            ),
+            ("monotone_constraints", constraints.to_object(py)),
+            ("subsample", self.booster.subsample.to_object(py)),
+            ("seed", self.booster.seed.to_object(py)),
+            ("missing", self.booster.missing.to_object(py)),
+            (
+                "create_missing_branch",
+                self.booster.create_missing_branch.to_object(py),
+            ),
+            ("sample_method", sample_method_.to_object(py)),
+            ("evaluation_metric", evaluation_metric_.to_object(py)),
+            (
+                "early_stopping_rounds",
+                self.booster.early_stopping_rounds.to_object(py),
+            ),
+        ];
+        let dict = key_vals.into_py_dict(py);
+        Ok(dict.to_object(py))
+    }
+
+    pub fn get_evaluation_history<'py>(
+        &self,
+        py: Python<'py>,
+    ) -> PyResult<Option<(usize, usize, &'py PyArray1<f64>)>> {
+        if let Some(data) = &self.booster.evaluation_history {
+            let d = data.data.to_owned().into_pyarray(py);
+            return Ok(Some((data.rows, data.cols, d)));
+        }
+        Ok(None)
+    }
+}
+
+#[pyfunction]
+fn print_matrix(x: PyReadonlyArray1<f32>, rows: usize, cols: usize) -> PyResult<()> {
+    let m = Matrix::new(x.as_slice()?, rows, cols);
+    println!("{}", m);
+    Ok(())
+}
+
+#[pyfunction]
+fn percentiles<'py>(
+    py: Python<'py>,
+    v: PyReadonlyArray1<f64>,
+    sample_weight: PyReadonlyArray1<f64>,
+    percentiles: PyReadonlyArray1<f64>,
+) -> PyResult<&'py PyArray1<f64>> {
+    let v_ = v.as_slice()?;
+    let sample_weight_ = sample_weight.as_slice()?;
+    let percentiles_ = percentiles.as_slice()?;
+    let p = crate_percentiles(v_, sample_weight_, percentiles_);
+    Ok(p.into_pyarray(py))
+}
+
+/// A Python module implemented in Rust.
+#[pymodule]
+fn forust(_py: Python, m: &PyModule) -> PyResult<()> {
+    m.add_function(wrap_pyfunction!(print_matrix, m)?)?;
+    m.add_function(wrap_pyfunction!(percentiles, m)?)?;
+    m.add_class::<GradientBooster>()?;
+    Ok(())
+}
```

### Comparing `forust-0.2.6/tests/test_booster.py` & `forust-0.2.7/tests/test_booster.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,491 +1,545 @@
-from typing import Tuple
-
-import numpy as np
-import pandas as pd
-import pytest
-from xgboost import XGBClassifier, XGBRegressor
-
-from forust import GradientBooster
-
-
-@pytest.fixture
-def X_y() -> Tuple[pd.DataFrame, pd.Series]:
-    df = pd.read_csv("../resources/titanic.csv")
-    X = df.select_dtypes("number").drop(columns="survived").reset_index(drop=True)
-    y = df["survived"]
-    return X, y
-
-
-def test_booster_to_xgboosts(X_y):
-    X, y = X_y
-    X = X.fillna(0)
-    xmod = XGBClassifier(
-        n_estimators=100,
-        learning_rate=0.3,
-        max_depth=5,
-        reg_lambda=1,
-        min_child_weight=1.0,
-        gamma=0,
-        objective="binary:logitraw",
-        tree_method="hist",
-    )
-    xmod.fit(X, y)
-    xmod_preds = xmod.predict(X, output_margin=True)
-
-    fmod = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1.0,
-        gamma=0,
-        objective_type="LogLoss",
-    )
-    fmod.fit(X, y=y)
-    fmod_preds = fmod.predict(X)
-    assert np.allclose(fmod_preds, xmod_preds, atol=0.00001)
-
-
-def test_booster_to_xgboosts_with_missing(X_y):
-    X, y = X_y
-    X = X
-    xmod = XGBClassifier(
-        n_estimators=100,
-        learning_rate=0.3,
-        max_depth=5,
-        reg_lambda=1,
-        min_child_weight=1,
-        gamma=1,
-        objective="binary:logitraw",
-        eval_metric="auc",
-        tree_method="hist",
-        max_bin=10000,
-    )
-    xmod.fit(X, y)
-    xmod_preds = xmod.predict(X, output_margin=True)
-
-    fmod = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="LogLoss",
-        nbins=500,
-        parallel=True,
-    )
-    fmod.fit(X, y=y)
-    fmod_preds = fmod.predict(X)
-    assert np.allclose(fmod_preds, xmod_preds, atol=0.00001)
-
-
-def test_booster_to_xgboosts_with_missing_sl(X_y):
-    X, y = X_y
-    X = X
-    X["survived"] = y
-    y = X["fare"]
-    X = X.drop(columns=["fare"])
-    xmod = XGBRegressor(
-        n_estimators=100,
-        learning_rate=0.3,
-        max_depth=5,
-        reg_lambda=1,
-        min_child_weight=1,
-        gamma=1,
-        eval_metric="auc",
-        tree_method="hist",
-        max_bin=10000,
-    )
-    xmod.fit(X, y)
-    xmod_preds = xmod.predict(X, output_margin=True)
-
-    fmod = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="SquaredLoss",
-        nbins=500,
-        parallel=True,
-    )
-    fmod.fit(X, y=y)
-    fmod_preds = fmod.predict(X)
-    assert np.allclose(fmod_preds, xmod_preds, atol=0.00001)
-
-
-def test_booster_with_new_missing(X_y):
-    X, y = X_y
-    X = X
-    fmod = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="LogLoss",
-        nbins=500,
-        parallel=True,
-    )
-    fmod.fit(X, y=y)
-    fmod_preds = fmod.predict(X)
-
-    Xm = X.copy().fillna(-9999)
-    fmod2 = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="LogLoss",
-        nbins=500,
-        parallel=True,
-        missing=-9999,
-    )
-    fmod2.fit(Xm, y=y)
-    fmod_preds2 = fmod2.predict(Xm)
-    assert np.allclose(fmod_preds, fmod_preds2, atol=0.00001)
-
-
-def test_booster_with_seed(X_y):
-    X, y = X_y
-    X = X
-    fmod1 = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="LogLoss",
-        nbins=500,
-        parallel=True,
-        subsample=0.5,
-        seed=0,
-    )
-    fmod1.fit(X, y=y)
-    fmod1_preds = fmod1.predict(X)
-
-    fmod2 = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="LogLoss",
-        nbins=500,
-        parallel=True,
-        subsample=0.5,
-        seed=0,
-    )
-    fmod2.fit(X, y=y)
-    fmod2_preds = fmod2.predict(X)
-    assert np.allclose(fmod2_preds, fmod1_preds, atol=0.0000001)
-
-    fmod3 = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="LogLoss",
-        nbins=500,
-        parallel=True,
-        subsample=0.5,
-        seed=1,
-    )
-    fmod3.fit(X, y=y)
-    fmod3_preds = fmod3.predict(X)
-    assert not np.allclose(fmod3_preds, fmod2_preds, atol=0.0000001)
-
-    fmod4 = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="LogLoss",
-        nbins=500,
-        parallel=True,
-    )
-    fmod4.fit(X, y=y)
-    fmod4_preds = fmod4.predict(X)
-    assert not np.allclose(fmod4_preds, fmod2_preds, atol=0.00001)
-
-
-def test_booster_to_xgboosts_weighted(X_y):
-    X, y = X_y
-    X = X.fillna(0)
-    w = X["fare"].to_numpy() + 1
-    xmod = XGBClassifier(
-        n_estimators=100,
-        learning_rate=0.3,
-        max_depth=5,
-        reg_lambda=1,
-        min_child_weight=1,
-        gamma=0,
-        objective="binary:logitraw",
-        tree_method="hist",
-        max_bins=1000,
-    )
-    xmod.fit(X, y, sample_weight=w)
-    xmod_preds = xmod.predict(X, output_margin=True)
-
-    fmod = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=0,
-        objective_type="LogLoss",
-    )
-    fmod.fit(X, y=y, sample_weight=w)
-    fmod_preds = fmod.predict(X)
-    assert np.allclose(fmod_preds, xmod_preds, atol=0.0001)
-
-
-def test_booster_saving(X_y, tmp_path):
-    # squared loss
-    f64_model_path = tmp_path / "modelf64_sl.json"
-    X, y = X_y
-    X = X
-    fmod = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="SquaredLoss",
-        nbins=500,
-        parallel=True,
-    )
-    fmod.fit(X, y=y)
-    fmod_preds = fmod.predict(X)
-    fmod.save_booster(f64_model_path)
-    fmod_loaded = GradientBooster.load_booster(f64_model_path)
-    assert all(fmod_preds == fmod_loaded.predict(X))
-
-    # LogLoss
-    f64_model_path = tmp_path / "modelf64_ll.json"
-    X, y = X_y
-    X = X
-    fmod = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="LogLoss",
-        nbins=500,
-        parallel=True,
-    )
-    fmod.fit(X, y=y)
-    fmod_preds = fmod.predict(X)
-    fmod.save_booster(f64_model_path)
-    fmod_loaded = GradientBooster.load_booster(f64_model_path)
-    assert fmod_loaded.feature_names_in_ == fmod.feature_names_in_
-    assert fmod_loaded.feature_names_in_ == X.columns.to_list()
-    assert all(fmod_preds == fmod_loaded.predict(X))
-
-
-def test_booster_saving_with_montone_constraints(X_y, tmp_path):
-    # squared loss
-    f64_model_path = tmp_path / "modelf64_sl.json"
-    X, y = X_y
-    X = X
-    mono_ = X.apply(lambda x: int(np.sign(x.corr(y)))).to_dict()
-    fmod = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="SquaredLoss",
-        nbins=500,
-        parallel=True,
-        monotone_constraints=mono_,
-    )
-    fmod.fit(X, y=y)
-    fmod_preds = fmod.predict(X)
-    fmod.save_booster(f64_model_path)
-    fmod_loaded = GradientBooster.load_booster(f64_model_path)
-    assert fmod_loaded.feature_names_in_ == fmod.feature_names_in_
-    assert fmod_loaded.feature_names_in_ == X.columns.to_list()
-    assert all(fmod_preds == fmod_loaded.predict(X))
-
-    # LogLoss
-    f64_model_path = tmp_path / "modelf64_ll.json"
-    X, y = X_y
-    X = X
-    fmod = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="LogLoss",
-        nbins=500,
-        parallel=True,
-        monotone_constraints=mono_,
-    )
-    fmod.fit(X, y=y)
-    fmod_preds = fmod.predict(X)
-    fmod.save_booster(f64_model_path)
-    fmod_loaded = GradientBooster.load_booster(f64_model_path)
-    assert all(fmod_preds == fmod_loaded.predict(X))
-
-
-def test_monotone_constraints(X_y):
-    X, y = X_y
-    X = X
-    mono_ = X.apply(lambda x: int(np.sign(x.corr(y)))).to_dict()
-    fmod = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="SquaredLoss",
-        nbins=500,
-        parallel=True,
-        monotone_constraints=mono_,
-    )
-    fmod.fit(X, y=y)
-    for f, m in mono_.items():
-        p_d = fmod.partial_dependence(X, feature=f)
-        p_d = p_d[~np.isnan(p_d[:, 0])]
-        if m < 0:
-            assert np.all(p_d[0:-1, 1] >= p_d[1:, 1])
-        else:
-            assert np.all(p_d[0:-1, 1] <= p_d[1:, 1])
-
-
-def test_booster_to_xgboosts_with_contributions(X_y):
-    X, y = X_y
-    X = X
-    fmod = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="LogLoss",
-        nbins=500,
-        parallel=True,
-        base_score=0.5,
-    )
-    fmod.fit(X, y=y)
-    fmod_preds = fmod.predict(X)
-    fmod_contribs = fmod.predict_contributions(X)
-    fmod_preds[~np.isclose(fmod_contribs.sum(1), fmod_preds, rtol=5)]
-    fmod_contribs.sum(1)[~np.isclose(fmod_contribs.sum(1), fmod_preds, rtol=5)]
-    assert fmod_contribs.shape[1] == X.shape[1] + 1
-    assert np.allclose(fmod_contribs.sum(1), fmod_preds)
-
-    xmod = XGBClassifier(
-        n_estimators=100,
-        learning_rate=0.3,
-        max_depth=5,
-        reg_lambda=1,
-        min_child_weight=1,
-        gamma=1,
-        objective="binary:logitraw",
-        eval_metric="auc",
-        tree_method="hist",
-        max_bin=10000,
-        base_score=0.5,
-    )
-    xmod.fit(X, y)
-    xmod_preds = xmod.predict(X, output_margin=True)
-    import xgboost as xgb
-
-    xmod_contribs = xmod.get_booster().predict(
-        xgb.DMatrix(X), approx_contribs=True, pred_contribs=True
-    )
-    assert np.allclose(fmod_contribs, xmod_contribs, atol=0.000001)
-
-
-def test_missing_branch_with_contributions(X_y):
-    X, y = X_y
-    X = X
-    fmod_miss_leaf = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="LogLoss",
-        nbins=500,
-        parallel=True,
-        base_score=0.5,
-        allow_missing_splits=False,
-        create_missing_branch=True,
-    )
-    fmod_miss_leaf.fit(X, y)
-    fmod_miss_leaf_preds = fmod_miss_leaf.predict(X)
-    fmod_miss_leaf_conts = fmod_miss_leaf.predict_contributions(X)
-    assert np.allclose(fmod_miss_leaf_conts.sum(1), fmod_miss_leaf_preds)
-
-    fmod_miss_branch = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="LogLoss",
-        nbins=500,
-        parallel=True,
-        base_score=0.5,
-        allow_missing_splits=True,
-        create_missing_branch=True,
-    )
-    fmod_miss_branch.fit(X, y)
-    fmod_miss_branch_preds = fmod_miss_branch.predict(X)
-    fmod_miss_branch_conts = fmod_miss_branch.predict_contributions(X)
-    assert np.allclose(fmod_miss_branch_conts.sum(1), fmod_miss_branch_preds)
-    assert not np.allclose(fmod_miss_branch_preds, fmod_miss_leaf_preds)
-
-
-def test_booster_metadata(X_y, tmp_path):
-    f64_model_path = tmp_path / "modelf64_sl.json"
-    X, y = X_y
-    X = X
-    fmod = GradientBooster(
-        iterations=100,
-        learning_rate=0.3,
-        max_depth=5,
-        l2=1,
-        min_leaf_weight=1,
-        gamma=1,
-        objective_type="SquaredLoss",
-        nbins=500,
-        parallel=True,
-    )
-    fmod.fit(X, y=y)
-    fmod_preds = fmod.predict(X)
-    fmod.save_booster(f64_model_path)
-    fmod.insert_metadata("test-info", "some-info")
-    assert fmod.get_metadata("test-info") == "some-info"
-    fmod.save_booster(f64_model_path)
-
-    loaded = GradientBooster.load_booster(f64_model_path)
-    assert loaded.get_metadata("test-info") == "some-info"
-
-    with pytest.raises(KeyError):
-        loaded.get_metadata("No-key")
+from typing import Tuple
+
+import numpy as np
+import pandas as pd
+import pytest
+from sklearn.metrics import roc_auc_score
+from xgboost import XGBClassifier, XGBRegressor
+
+import forust
+from forust import GradientBooster
+
+
+@pytest.fixture
+def X_y() -> Tuple[pd.DataFrame, pd.Series]:
+    df = pd.read_csv("../resources/titanic.csv")
+    X = df.select_dtypes("number").drop(columns="survived").reset_index(drop=True)
+    y = df["survived"]
+    return X, y
+
+
+def test_booster_to_xgboosts(X_y):
+    X, y = X_y
+    X = X.fillna(0)
+    xmod = XGBClassifier(
+        n_estimators=100,
+        learning_rate=0.3,
+        max_depth=5,
+        reg_lambda=1,
+        min_child_weight=1.0,
+        gamma=0,
+        objective="binary:logitraw",
+        tree_method="hist",
+    )
+    xmod.fit(X, y)
+    xmod_preds = xmod.predict(X, output_margin=True)
+
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1.0,
+        gamma=0,
+        objective_type="LogLoss",
+    )
+    fmod.fit(X, y=y)
+    fmod_preds = fmod.predict(X)
+    assert np.allclose(fmod_preds, xmod_preds, atol=0.00001)
+
+
+def test_booster_to_xgboosts_with_missing(X_y):
+    X, y = X_y
+    X = X
+    xmod = XGBClassifier(
+        n_estimators=100,
+        learning_rate=0.3,
+        max_depth=5,
+        reg_lambda=1,
+        min_child_weight=1,
+        gamma=1,
+        objective="binary:logitraw",
+        eval_metric="auc",
+        tree_method="hist",
+        max_bin=10000,
+    )
+    xmod.fit(X, y)
+    xmod_preds = xmod.predict(X, output_margin=True)
+
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+    )
+    fmod.fit(X, y=y)
+    fmod_preds = fmod.predict(X)
+    assert np.allclose(fmod_preds, xmod_preds, atol=0.00001)
+
+
+def test_booster_to_xgboosts_with_missing_sl(X_y):
+    X, y = X_y
+    X = X
+    X["survived"] = y
+    y = X["fare"]
+    X = X.drop(columns=["fare"])
+    xmod = XGBRegressor(
+        n_estimators=100,
+        learning_rate=0.3,
+        max_depth=5,
+        reg_lambda=1,
+        min_child_weight=1,
+        gamma=1,
+        eval_metric="auc",
+        tree_method="hist",
+        max_bin=10000,
+    )
+    xmod.fit(X, y)
+    xmod_preds = xmod.predict(X, output_margin=True)
+
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="SquaredLoss",
+        nbins=500,
+        parallel=True,
+    )
+    fmod.fit(X, y=y)
+    fmod_preds = fmod.predict(X)
+    assert np.allclose(fmod_preds, xmod_preds, atol=0.00001)
+
+
+def test_booster_with_new_missing(X_y):
+    X, y = X_y
+    X = X
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+    )
+    fmod.fit(X, y=y)
+    fmod_preds = fmod.predict(X)
+
+    Xm = X.copy().fillna(-9999)
+    fmod2 = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        missing=-9999,
+    )
+    fmod2.fit(Xm, y=y)
+    fmod_preds2 = fmod2.predict(Xm)
+    assert np.allclose(fmod_preds, fmod_preds2, atol=0.00001)
+
+
+def test_booster_with_seed(X_y):
+    X, y = X_y
+    X = X
+    fmod1 = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        subsample=0.5,
+        seed=0,
+    )
+    fmod1.fit(X, y=y)
+    fmod1_preds = fmod1.predict(X)
+
+    fmod2 = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        subsample=0.5,
+        seed=0,
+    )
+    fmod2.fit(X, y=y)
+    fmod2_preds = fmod2.predict(X)
+    assert np.allclose(fmod2_preds, fmod1_preds, atol=0.0000001)
+
+    fmod3 = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        subsample=0.5,
+        seed=1,
+    )
+    fmod3.fit(X, y=y)
+    fmod3_preds = fmod3.predict(X)
+    assert not np.allclose(fmod3_preds, fmod2_preds, atol=0.0000001)
+
+    fmod4 = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+    )
+    fmod4.fit(X, y=y)
+    fmod4_preds = fmod4.predict(X)
+    assert not np.allclose(fmod4_preds, fmod2_preds, atol=0.00001)
+
+
+def test_booster_to_xgboosts_weighted(X_y):
+    X, y = X_y
+    X = X.fillna(0)
+    w = X["fare"].to_numpy() + 1
+    xmod = XGBClassifier(
+        n_estimators=100,
+        learning_rate=0.3,
+        max_depth=5,
+        reg_lambda=1,
+        min_child_weight=1,
+        gamma=0,
+        objective="binary:logitraw",
+        tree_method="hist",
+        max_bins=1000,
+    )
+    xmod.fit(X, y, sample_weight=w)
+    xmod_preds = xmod.predict(X, output_margin=True)
+
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=0,
+        objective_type="LogLoss",
+    )
+    fmod.fit(X, y=y, sample_weight=w)
+    fmod_preds = fmod.predict(X)
+    assert np.allclose(fmod_preds, xmod_preds, atol=0.0001)
+
+
+def test_booster_saving(X_y, tmp_path):
+    # squared loss
+    f64_model_path = tmp_path / "modelf64_sl.json"
+    X, y = X_y
+    X = X
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="SquaredLoss",
+        nbins=500,
+        parallel=True,
+    )
+    fmod.fit(X, y=y)
+    fmod_preds = fmod.predict(X)
+    fmod.save_booster(f64_model_path)
+    fmod_loaded = GradientBooster.load_booster(f64_model_path)
+    assert all(fmod_preds == fmod_loaded.predict(X))
+
+    # LogLoss
+    f64_model_path = tmp_path / "modelf64_ll.json"
+    X, y = X_y
+    X = X
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+    )
+    fmod.fit(X, y=y)
+    fmod_preds = fmod.predict(X)
+    fmod.save_booster(f64_model_path)
+    fmod_loaded = GradientBooster.load_booster(f64_model_path)
+    assert fmod_loaded.feature_names_in_ == fmod.feature_names_in_
+    assert fmod_loaded.feature_names_in_ == X.columns.to_list()
+    assert all(fmod_preds == fmod_loaded.predict(X))
+
+
+def test_booster_saving_with_montone_constraints(X_y, tmp_path):
+    # squared loss
+    f64_model_path = tmp_path / "modelf64_sl.json"
+    X, y = X_y
+    X = X
+    mono_ = X.apply(lambda x: int(np.sign(x.corr(y)))).to_dict()
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="SquaredLoss",
+        nbins=500,
+        parallel=True,
+        monotone_constraints=mono_,
+    )
+    fmod.fit(X, y=y)
+    fmod_preds = fmod.predict(X)
+    fmod.save_booster(f64_model_path)
+    fmod_loaded = GradientBooster.load_booster(f64_model_path)
+    assert fmod_loaded.feature_names_in_ == fmod.feature_names_in_
+    assert fmod_loaded.feature_names_in_ == X.columns.to_list()
+    assert all(fmod_preds == fmod_loaded.predict(X))
+
+    # LogLoss
+    f64_model_path = tmp_path / "modelf64_ll.json"
+    X, y = X_y
+    X = X
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        monotone_constraints=mono_,
+    )
+    fmod.fit(X, y=y)
+    fmod_preds = fmod.predict(X)
+    fmod.save_booster(f64_model_path)
+    fmod_loaded = GradientBooster.load_booster(f64_model_path)
+    assert all(fmod_preds == fmod_loaded.predict(X))
+
+
+def test_monotone_constraints(X_y):
+    X, y = X_y
+    X = X
+    mono_ = X.apply(lambda x: int(np.sign(x.corr(y)))).to_dict()
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="SquaredLoss",
+        nbins=500,
+        parallel=True,
+        monotone_constraints=mono_,
+    )
+    fmod.fit(X, y=y)
+    for f, m in mono_.items():
+        p_d = fmod.partial_dependence(X, feature=f)
+        p_d = p_d[~np.isnan(p_d[:, 0])]
+        if m < 0:
+            assert np.all(p_d[0:-1, 1] >= p_d[1:, 1])
+        else:
+            assert np.all(p_d[0:-1, 1] <= p_d[1:, 1])
+
+
+def test_booster_to_xgboosts_with_contributions(X_y):
+    X, y = X_y
+    X = X
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        base_score=0.5,
+    )
+    fmod.fit(X, y=y)
+    fmod_preds = fmod.predict(X)
+    fmod_contribs = fmod.predict_contributions(X)
+    fmod_preds[~np.isclose(fmod_contribs.sum(1), fmod_preds, rtol=5)]
+    fmod_contribs.sum(1)[~np.isclose(fmod_contribs.sum(1), fmod_preds, rtol=5)]
+    assert fmod_contribs.shape[1] == X.shape[1] + 1
+    assert np.allclose(fmod_contribs.sum(1), fmod_preds)
+
+    xmod = XGBClassifier(
+        n_estimators=100,
+        learning_rate=0.3,
+        max_depth=5,
+        reg_lambda=1,
+        min_child_weight=1,
+        gamma=1,
+        objective="binary:logitraw",
+        eval_metric="auc",
+        tree_method="hist",
+        max_bin=10000,
+        base_score=0.5,
+    )
+    xmod.fit(X, y)
+    xmod_preds = xmod.predict(X, output_margin=True)
+    import xgboost as xgb
+
+    xmod_contribs = xmod.get_booster().predict(
+        xgb.DMatrix(X), approx_contribs=True, pred_contribs=True
+    )
+    assert np.allclose(fmod_contribs, xmod_contribs, atol=0.000001)
+
+
+def test_missing_branch_with_contributions(X_y):
+    X, y = X_y
+    X = X
+    fmod_miss_leaf = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        base_score=0.5,
+        allow_missing_splits=False,
+        create_missing_branch=True,
+    )
+    fmod_miss_leaf.fit(X, y)
+    fmod_miss_leaf_preds = fmod_miss_leaf.predict(X)
+    fmod_miss_leaf_conts = fmod_miss_leaf.predict_contributions(X)
+    assert np.allclose(fmod_miss_leaf_conts.sum(1), fmod_miss_leaf_preds)
+
+    fmod_miss_branch = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        base_score=0.5,
+        allow_missing_splits=True,
+        create_missing_branch=True,
+    )
+    fmod_miss_branch.fit(X, y)
+    fmod_miss_branch_preds = fmod_miss_branch.predict(X)
+    fmod_miss_branch_conts = fmod_miss_branch.predict_contributions(X)
+    assert np.allclose(fmod_miss_branch_conts.sum(1), fmod_miss_branch_preds)
+    assert not np.allclose(fmod_miss_branch_preds, fmod_miss_leaf_preds)
+
+
+def test_booster_metadata(X_y, tmp_path):
+    f64_model_path = tmp_path / "modelf64_sl.json"
+    X, y = X_y
+    X = X
+    fmod = GradientBooster(
+        iterations=100,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="SquaredLoss",
+        nbins=500,
+        parallel=True,
+    )
+    fmod.fit(X, y=y)
+    fmod_preds = fmod.predict(X)
+    fmod.save_booster(f64_model_path)
+    fmod.insert_metadata("test-info", "some-info")
+    assert fmod.get_metadata("test-info") == "some-info"
+    fmod.save_booster(f64_model_path)
+
+    loaded = GradientBooster.load_booster(f64_model_path)
+    assert loaded.get_metadata("test-info") == "some-info"
+
+    with pytest.raises(KeyError):
+        loaded.get_metadata("No-key")
+
+    loaded_dict = loaded.__dict__
+    fmod_dict = fmod.__dict__
+    assert sorted(loaded_dict.keys()) == sorted(fmod_dict.keys())
+    for k, v in loaded_dict.items():
+        c_v = fmod_dict[k]
+        if isinstance(v, float):
+            if np.isnan(v):
+                assert np.isnan(c_v)
+            else:
+                assert np.allclose(v, c_v)
+        elif isinstance(v, forust.CrateGradientBooster):
+            assert isinstance(c_v, forust.CrateGradientBooster)
+        else:
+            assert v == c_v
+
+
+def test_early_stopping_rounds(X_y, tmp_path):
+    X, y = X_y
+    X = X
+    fmod = GradientBooster(
+        iterations=200,
+        learning_rate=0.3,
+        max_depth=5,
+        l2=1,
+        min_leaf_weight=1,
+        gamma=1,
+        objective_type="LogLoss",
+        nbins=500,
+        parallel=True,
+        base_score=0.5,
+        early_stopping_rounds=2,
+        evaluation_metric="AUC",
+    )
+    fmod.fit(X, y, evaluation_data=[(X, y)])
+    preds = fmod.predict(X)
+    mod_path = tmp_path / "early_stopping_model.json"
+    fmod.save_booster(mod_path)
+    loaded = GradientBooster.load_booster(mod_path)
+    assert np.allclose(loaded.predict(X), preds)
+    history = fmod.get_evaluation_history()
+    assert history is not None
+    assert np.isclose(roc_auc_score(y, preds), history.max())
+    best_iteration = fmod.get_best_iteration()
+    assert best_iteration is not None
+    assert best_iteration < history.shape[0]
+    fmod.set_prediction_iteration(4)
+    new_preds = fmod.predict(X)
+    assert not np.allclose(new_preds, preds)
+    fmod.save_booster(mod_path)
+    loaded = GradientBooster.load_booster(mod_path)
+    assert np.allclose(loaded.predict(X), new_preds)
```

### Comparing `forust-0.2.6/LICENSE` & `forust-0.2.7/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2022 James Inlow
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2022 James Inlow
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `forust-0.2.6/PKG-INFO` & `forust-0.2.7/local_dependencies/forust-ml/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,209 +1,207 @@
-Metadata-Version: 2.1
-Name: forust
-Version: 0.2.6
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: numpy>=1.21
-Requires-Dist: pandas>=1.3
-Requires-Dist: maturin; extra == 'dev'
-Requires-Dist: pytest; extra == 'dev'
-Requires-Dist: seaborn; extra == 'dev'
-Requires-Dist: xgboost==1.6.1; extra == 'dev'
-Requires-Dist: scikit-learn; extra == 'dev'
-Provides-Extra: dev
-License-File: LICENSE
-Summary: A lightweight gradient boosting implementation in Rust.
-Keywords: rust,forust,machine learning,xgboost,tree model,decision tree
-Author: James Inlow
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-
-<p align="center">
-  <img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/tree-image-crop.png">
-</p>
-
-
-<div align="center">
-
-  <a href="https://pypi.org/project/forust/">![PyPI](https://img.shields.io/pypi/v/forust?color=gr&style=for-the-badge)</a>
-  <a href="https://crates.io/crates/forust-ml">![Crates.io](https://img.shields.io/crates/v/forust-ml?color=gr&style=for-the-badge)</a>
-
-</div>
-
-# Forust
-## _A lightweight gradient boosting package_
-Forust, is a lightweight package for building gradient boosted decision tree ensembles. All of the algorithm code is written in [Rust](https://www.rust-lang.org/), with a python wrapper. The rust package can be used directly, however, most examples shown here will be for the python wrapper. For a self contained rust example, [see here](rs-example.md). It implements the same algorithm as the [XGBoost](https://xgboost.readthedocs.io/en/stable/) package, and in many cases will give nearly identical results.
-
-I developed this package for a few reasons, mainly to better understand the XGBoost algorithm, additionally to have a fun project to work on in rust, and because I wanted to be able to experiment with adding new features to the algorithm in a smaller simpler codebase.
-
-All of the rust code for the package can be found in the [src](src/) directory, while all of the python wrapper code is in the [py-forust](py-forust/) directory.
-
-## Installation
-The package can be installed directly from [pypi](https://pypi.org/project/forust/).
-```shell
-pip install forust
-```
-
-To use in a rust project add the following to your Cargo.toml file.
-```toml
-forust-ml = "0.2.6"
-```
-
-## Usage
-The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
-
-It can be initialized with the following arguments.
-
- - `objective_type` ***(str, optional)***: The name of objective function used to optimize.
-    Valid options include "LogLoss" to use logistic loss as the objective function (binary classification),
-    or "SquaredLoss" to use Squared Error as the objective function (continuous regression).
-    Defaults to "LogLoss".
- - `iterations` ***(int, optional)***: Total number of trees to train in the ensemble.
-    Defaults to 100.
- - `learning_rate` ***(float, optional)***: Step size to use at each iteration. Each
-    leaf weight is multiplied by this number. The smaller the value, the more
-    conservative the weights will be. Defaults to 0.3.
- - `max_depth` ***(int, optional)***: Maximum depth of an individual tree. Valid values
-    are 0 to infinity. Defaults to 5.
- - `max_leaves` ***(int, optional)***: Maximum number of leaves allowed on a tree. Valid values
-    are 0 to infinity. This is the total number of final nodes. Defaults to sys.maxsize.
- - `l2` ***(float, optional)***: L2 regularization term applied to the weights of the tree. Valid values
-    are 0 to infinity. Defaults to 1.0.
- - `gamma` ***(float, optional)***: The minimum amount of loss required to further split a node.
-    Valid values are 0 to infinity. Defaults to 0.0.
- - `min_leaf_weight` ***(float, optional)***: Minimum sum of the hessian values of the loss function
-    required to be in a node. Defaults to 1.0.
- - `base_score` ***(float, optional)***: The initial prediction value of the model. Defaults to 0.5.
- - `nbins` ***(int, optional)***: Number of bins to calculate to partition the data. Setting this to
-    a smaller number, will result in faster training time, while potentially sacrificing
-    accuracy. If there are more bins, than unique values in a column, all unique values
-    will be used. Defaults to 256.
- - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
-    with this model? Defaults to `True`.
- - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. If `create_missing_branch` is set to `True` having this parameter be set to `True` will result in the missing branch further split, if this parameter is `False` then in that case the missing branch will always be a terminal node. Defaults to `True`.
- - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
- - `subsample` ***(float, optional)***: Percent of records to randomly sample at each iteration when
-      training a tree. Defaults to 1.0, meaning all data is used for training.
- - `seed` ***(integer, optional)***: Integer value used to seed any randomness used in the
-      algorithm. Defaults to 0.
- - `missing` ***(float, optional)***: Value to consider missing, when training and predicting with the booster. Defaults to `np.nan`.
- - `create_missing_branch` ***(bool, optional)***: An experimental parameter, that if `True`, will create a separate branch for missing, creating a ternary tree, the missing node will be given the same weight value as the parent node. If this parameter is `False`, missing will be sent down either the left or right branch, creating a binary tree. Defaults to `False`.
-
-### Training and Predicting
-
-Once, the booster has been initialized, it can be fit on a provided dataset, and performance field. After fitting, the model can be used to predict on a dataset.
-In the case of this example, the predictions are the log odds of a given record being 1.
-
-```python
-# Small example dataset
-from seaborn import load_dataset
-
-df = load_dataset("titanic")
-X = df.select_dtypes("number").drop(columns=["survived"])
-y = df["survived"]
-
-# Initialize a booster with defaults.
-from forust import GradientBooster
-model = GradientBooster(objective_type="LogLoss")
-model.fit(X, y)
-
-# Predict on data
-model.predict(X.head())
-# array([-1.94919663,  2.25863229,  0.32963671,  2.48732194, -3.00371813])
-
-# predict contributions
-model.predict_contributions(X.head())
-# array([[-0.63014213,  0.33880048, -0.16520798, -0.07798772, -0.85083578,
-#        -1.07720813],
-#       [ 1.05406709,  0.08825999,  0.21662544, -0.12083538,  0.35209258,
-#        -1.07720813],
-```
-
-The `fit` method accepts the following arguments.
- - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
- - `y` ***(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If "LogLoss" was
-   the objective type specified, then this should only contain 1 or 0 values, where 1 is the positive class being predicted. If "SquaredLoss" is the objective type, then any continuous variable can be provided.
- - `sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use when training the model. If None is passed, a weight of 1 will be used for every record. Defaults to None.
-
-The predict method accepts the following arguments.
- - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
- - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict function should run in parallel on multiple threads. If `None` is passed, the `parallel` attribute of the booster will be used. Defaults to `None`.
-
-The `predict_contributions` method will predict with the fitted booster on new data, returning the feature contribution matrix. The last column is the bias term.
- - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
- - `method` ***(str, optional)***: Method to calculate the contributions, if "average" is specified, the average internal node values are calculated, this is equivalent to the `approx_contribs` parameter in XGBoost. The other supported method is "weight", this will use the internal leaf weights, to calculate the contributions. This is the same as what is described by Saabas [here](https://blog.datadive.net/interpreting-random-forests/).
- - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict function should run in parallel on multiple threads. If `None` is passed, the `parallel` attribute of the booster will be used. Defaults to `None`.
-
-### Inspecting the Model
-
-Once the booster has been fit, each individual tree structure can be retrieved in text form, using the `text_dump` method. This method returns a list, the same length as the number of trees in the model.
-
-```python
-model.text_dump()[0]
-# 0:[0 < 3] yes=1,no=2,missing=2,gain=91.50833,cover=209.388307
-#       1:[4 < 13.7917] yes=3,no=4,missing=4,gain=28.185467,cover=94.00148
-#             3:[1 < 18] yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348
-#                   7:[1 < 17] yes=15,no=16,missing=16,gain=0.691266,cover=0.705011
-#                         15:leaf=-0.15120,cover=0.23500
-#                         16:leaf=0.154097,cover=0.470007
-```
-
-The `json_dump` method performs the same action, but returns the model as a json representation rather than a text string.
-
-To see an estimate for how a given feature is used in the model, the `partial_dependence` method is provided. This method calculates the partial dependence values of a feature. For each unique value of the feature, this gives the estimate of the predicted value for that feature, with the effects of all features averaged out. This information gives an estimate of how a given feature impacts the model.
-
-The `partial_dependence` method takes the following parameters...
-
- - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array. This should be the same data passed into the models fit, or predict, with the columns in the same order.
- - `feature` ***(Union[str, int])***: The feature for which to calculate the partial dependence values. This can be the name of a column, if the provided X is a pandas DataFrame, or the index of the feature.
- - `samples` ***(int | None, optional)***: Number of evenly spaced samples to select. If None is passed all unique values will be used. Defaults to 100.
- - `exclude_missing` ***(bool, optional)***: Should missing excluded from the features? Defaults to True.
- - `percentile_bounds` ***(tuple[float, float], optional)***: Upper and lower percentiles to start at  when calculating the samples. Defaults to (0.2, 0.98) to cap the samples selected  at the 5th and 95th percentiles respectively.
-This method returns a 2 dimensional numpy array, where the first column is the sorted unique values of the feature, and then the second column is the partial dependence values for each feature value.
-
-This information can be plotted to visualize how a feature is used in the model, like so.
-
-```python
-from seaborn import lineplot
-import matplotlib.pyplot as plt
-
-pd_values = model.partial_dependence(X=X, feature="age", samples=None)
-
-fig = lineplot(x=pd_values[:,0], y=pd_values[:,1],)
-plt.title("Partial Dependence Plot")
-plt.xlabel("Age")
-plt.ylabel("Log Odds")
-```
-<img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/pdp_plot_age.png">
-
-We can see how this is impacted if a model is created, where a specific constraint is applied to the feature using the `monotone_constraint` parameter.
-
-```python
-model = GradientBooster(
-    objective_type="LogLoss",
-    monotone_constraints={"age": -1},
-)
-model.fit(X, y)
-
-pd_values = model.partial_dependence(X=X, feature="age")
-fig = lineplot(
-    x=pd_values[:, 0],
-    y=pd_values[:, 1],
-)
-plt.title("Partial Dependence Plot with Monotonicity")
-plt.xlabel("Age")
-plt.ylabel("Log Odds")
-```
-<img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/pdp_plot_age_mono.png">
-
-### Saving the model
-To save and subsequently load a trained booster, the `save_booster` and `load_booster` methods can be used. Each accepts a path, which is used to write the model to. The model is saved and loaded as a json object.
-
-```python
-trained_model.save_booster("model_path.json")
-
-# To load a model from a json path.
-loaded_model = GradientBooster.load_model("model_path.json")
-```
+<p align="center">
+  <img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/tree-image-crop.png">
+</p>
 
+
+<div align="center">
+
+  <a href="https://pypi.org/project/forust/">![PyPI](https://img.shields.io/pypi/v/forust?color=gr&style=for-the-badge)</a>
+  <a href="https://crates.io/crates/forust-ml">![Crates.io](https://img.shields.io/crates/v/forust-ml?color=gr&style=for-the-badge)</a>
+
+</div>
+
+# Forust
+## _A lightweight gradient boosting package_
+Forust, is a lightweight package for building gradient boosted decision tree ensembles. All of the algorithm code is written in [Rust](https://www.rust-lang.org/), with a python wrapper. The rust package can be used directly, however, most examples shown here will be for the python wrapper. For a self contained rust example, [see here](rs-example.md). It implements the same algorithm as the [XGBoost](https://xgboost.readthedocs.io/en/stable/) package, and in many cases will give nearly identical results.
+
+I developed this package for a few reasons, mainly to better understand the XGBoost algorithm, additionally to have a fun project to work on in rust, and because I wanted to be able to experiment with adding new features to the algorithm in a smaller simpler codebase.
+
+All of the rust code for the package can be found in the [src](src/) directory, while all of the python wrapper code is in the [py-forust](py-forust/) directory.
+
+## Installation
+The package can be installed directly from [pypi](https://pypi.org/project/forust/).
+```shell
+pip install forust
+```
+
+To use in a rust project add the following to your Cargo.toml file.
+```toml
+forust-ml = "0.2.7"
+```
+
+## Usage
+The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
+
+It can be initialized with the following arguments.
+
+ - `objective_type` ***(str, optional)***: The name of objective function used to optimize.
+    Valid options include "LogLoss" to use logistic loss as the objective function (binary classification),
+    or "SquaredLoss" to use Squared Error as the objective function (continuous regression).
+    Defaults to "LogLoss".
+ - `iterations` ***(int, optional)***: Total number of trees to train in the ensemble.
+    Defaults to 100.
+ - `learning_rate` ***(float, optional)***: Step size to use at each iteration. Each
+    leaf weight is multiplied by this number. The smaller the value, the more
+    conservative the weights will be. Defaults to 0.3.
+ - `max_depth` ***(int, optional)***: Maximum depth of an individual tree. Valid values
+    are 0 to infinity. Defaults to 5.
+ - `max_leaves` ***(int, optional)***: Maximum number of leaves allowed on a tree. Valid values
+    are 0 to infinity. This is the total number of final nodes. Defaults to sys.maxsize.
+ - `l2` ***(float, optional)***: L2 regularization term applied to the weights of the tree. Valid values
+    are 0 to infinity. Defaults to 1.0.
+ - `gamma` ***(float, optional)***: The minimum amount of loss required to further split a node.
+    Valid values are 0 to infinity. Defaults to 0.0.
+ - `min_leaf_weight` ***(float, optional)***: Minimum sum of the hessian values of the loss function
+    required to be in a node. Defaults to 1.0.
+ - `base_score` ***(float, optional)***: The initial prediction value of the model. Defaults to 0.5.
+ - `nbins` ***(int, optional)***: Number of bins to calculate to partition the data. Setting this to
+    a smaller number, will result in faster training time, while potentially sacrificing
+    accuracy. If there are more bins, than unique values in a column, all unique values
+    will be used. Defaults to 256.
+ - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
+    with this model? Defaults to `True`.
+ - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. If `create_missing_branch` is set to `True` having this parameter be set to `True` will result in the missing branch further split, if this parameter is `False` then in that case the missing branch will always be a terminal node. Defaults to `True`.
+ - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
+ - `subsample` ***(float, optional)***: Percent of records to randomly sample at each iteration when
+      training a tree. Defaults to 1.0, meaning all data is used for training.
+ - `seed` ***(integer, optional)***: Integer value used to seed any randomness used in the
+      algorithm. Defaults to 0.
+ - `missing` ***(float, optional)***: Value to consider missing, when training and predicting with the booster. Defaults to `np.nan`.
+ - `create_missing_branch` ***(bool, optional)***: An experimental parameter, that if `True`, will create a separate branch for missing, creating a ternary tree, the missing node will be given the same weight value as the parent node. If this parameter is `False`, missing will be sent down either the left or right branch, creating a binary tree. Defaults to `False`.
+ - `sample_method` ***(str | None, optional)***: Optional string value to use to determine the method to use to sample the data while training. If this is None, no sample method will be used. If the `subsample` parameter is less than 1 and no sample_method is provided this `sample_method` will be automatically set to "random". Valid options are "goss" and "random". Defaults to `None`.
+ - `evaluation_metric` ***(str | None, optional)***: Optional string value used to define an evaluation metric that will be calculated at each iteration if a `evaluation_dataset` is provided at fit time. The metric can be one of "AUC", "LogLoss", "RootMeanSquaredLogError", or "RootMeanSquaredError". If no `evaluation_metric` is passed, but an `evaluation_dataset` is passed, then "LogLoss", will be used with the "LogLoss" objective function, and "RootMeanSquaredLogError" will be used with "SquaredLoss".
+ - `early_stopping_rounds` ***(int | None, optional)***: If this is specified, and an `evaluation_dataset` is passed during fit, then an improvement in the `evaluation_metric` must be seen after at least this many iterations of training, otherwise training will be cut short.
+
+### Training and Predicting
+
+Once, the booster has been initialized, it can be fit on a provided dataset, and performance field. After fitting, the model can be used to predict on a dataset.
+In the case of this example, the predictions are the log odds of a given record being 1.
+
+```python
+# Small example dataset
+from seaborn import load_dataset
+
+df = load_dataset("titanic")
+X = df.select_dtypes("number").drop(columns=["survived"])
+y = df["survived"]
+
+# Initialize a booster with defaults.
+from forust import GradientBooster
+model = GradientBooster(objective_type="LogLoss")
+model.fit(X, y)
+
+# Predict on data
+model.predict(X.head())
+# array([-1.94919663,  2.25863229,  0.32963671,  2.48732194, -3.00371813])
+
+# predict contributions
+model.predict_contributions(X.head())
+# array([[-0.63014213,  0.33880048, -0.16520798, -0.07798772, -0.85083578,
+#        -1.07720813],
+#       [ 1.05406709,  0.08825999,  0.21662544, -0.12083538,  0.35209258,
+#        -1.07720813],
+```
+
+The `fit` method accepts the following arguments.
+ - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
+ - `y` ***(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If "LogLoss" was
+   the objective type specified, then this should only contain 1 or 0 values, where 1 is the positive class being predicted. If "SquaredLoss" is the objective type, then any continuous variable can be provided.
+ - `sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use when training the model. If None is passed, a weight of 1 will be used for every record. Defaults to None.
+ - `evaluation_data` ***(tuple[FrameLike, ArrayLike, ArrayLike] | tuple[FrameLike, ArrayLike], optional)***: An optional list of tuples, where each tuple should contain a dataset, and equal length target array, and optional an equal length sample weight array. If this is provided metric values will be calculated at each iteration of training. If `early_stopping_rounds` is supplied, the first entry of this list will be used to determine if performance has improved over the last set of iterations, for which if no improvement is not seen in `early_stopping_rounds` training will be cut short.
+
+The predict method accepts the following arguments.
+ - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
+ - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict function should run in parallel on multiple threads. If `None` is passed, the `parallel` attribute of the booster will be used. Defaults to `None`.
+
+The `predict_contributions` method will predict with the fitted booster on new data, returning the feature contribution matrix. The last column is the bias term.
+ - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
+ - `method` ***(str, optional)***: Method to calculate the contributions, if "average" is specified, the average internal node values are calculated, this is equivalent to the `approx_contribs` parameter in XGBoost. The other supported method is "weight", this will use the internal leaf weights, to calculate the contributions. This is the same as what is described by Saabas [here](https://blog.datadive.net/interpreting-random-forests/).
+ - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict function should run in parallel on multiple threads. If `None` is passed, the `parallel` attribute of the booster will be used. Defaults to `None`.
+
+When predicting with the data, the maximum iteration that will be used when predicting can be set using the `set_prediction_iteration` method. If `early_stopping_rounds` has been set, this will default to the best iteration, otherwise all of the trees will be used. It accepts a single value.
+ - `iteration` (int): Iteration number to use, this will use all trees, up to and including this index.
+
+If early stopping was used, the evaluation history can be retrieved with the `get_evaluation_history` method.
+
+```python
+model = GradientBooster(objective_type="LogLoss")
+model.fit(X, y, evaluation_data=[(X, y)])
+
+model.get_evaluation_history()[0:3]
+
+# array([[588.9158873 ],
+#        [532.01055803],
+#        [496.76933646]])
+```
+
+### Inspecting the Model
+
+Once the booster has been fit, each individual tree structure can be retrieved in text form, using the `text_dump` method. This method returns a list, the same length as the number of trees in the model.
+
+```python
+model.text_dump()[0]
+# 0:[0 < 3] yes=1,no=2,missing=2,gain=91.50833,cover=209.388307
+#       1:[4 < 13.7917] yes=3,no=4,missing=4,gain=28.185467,cover=94.00148
+#             3:[1 < 18] yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348
+#                   7:[1 < 17] yes=15,no=16,missing=16,gain=0.691266,cover=0.705011
+#                         15:leaf=-0.15120,cover=0.23500
+#                         16:leaf=0.154097,cover=0.470007
+```
+
+The `json_dump` method performs the same action, but returns the model as a json representation rather than a text string.
+
+To see an estimate for how a given feature is used in the model, the `partial_dependence` method is provided. This method calculates the partial dependence values of a feature. For each unique value of the feature, this gives the estimate of the predicted value for that feature, with the effects of all features averaged out. This information gives an estimate of how a given feature impacts the model.
+
+The `partial_dependence` method takes the following parameters...
+
+ - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array. This should be the same data passed into the models fit, or predict, with the columns in the same order.
+ - `feature` ***(Union[str, int])***: The feature for which to calculate the partial dependence values. This can be the name of a column, if the provided X is a pandas DataFrame, or the index of the feature.
+ - `samples` ***(int | None, optional)***: Number of evenly spaced samples to select. If None is passed all unique values will be used. Defaults to 100.
+ - `exclude_missing` ***(bool, optional)***: Should missing excluded from the features? Defaults to True.
+ - `percentile_bounds` ***(tuple[float, float], optional)***: Upper and lower percentiles to start at  when calculating the samples. Defaults to (0.2, 0.98) to cap the samples selected  at the 5th and 95th percentiles respectively.
+This method returns a 2 dimensional numpy array, where the first column is the sorted unique values of the feature, and then the second column is the partial dependence values for each feature value.
+
+This information can be plotted to visualize how a feature is used in the model, like so.
+
+```python
+from seaborn import lineplot
+import matplotlib.pyplot as plt
+
+pd_values = model.partial_dependence(X=X, feature="age", samples=None)
+
+fig = lineplot(x=pd_values[:,0], y=pd_values[:,1],)
+plt.title("Partial Dependence Plot")
+plt.xlabel("Age")
+plt.ylabel("Log Odds")
+```
+<img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/pdp_plot_age.png">
+
+We can see how this is impacted if a model is created, where a specific constraint is applied to the feature using the `monotone_constraint` parameter.
+
+```python
+model = GradientBooster(
+    objective_type="LogLoss",
+    monotone_constraints={"age": -1},
+)
+model.fit(X, y)
+
+pd_values = model.partial_dependence(X=X, feature="age")
+fig = lineplot(
+    x=pd_values[:, 0],
+    y=pd_values[:, 1],
+)
+plt.title("Partial Dependence Plot with Monotonicity")
+plt.xlabel("Age")
+plt.ylabel("Log Odds")
+```
+<img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/pdp_plot_age_mono.png">
+
+### Saving the model
+To save and subsequently load a trained booster, the `save_booster` and `load_booster` methods can be used. Each accepts a path, which is used to write the model to. The model is saved and loaded as a json object.
+
+```python
+trained_model.save_booster("model_path.json")
+
+# To load a model from a json path.
+loaded_model = GradientBooster.load_model("model_path.json")
+```
```

#### html2text {}

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1 Name: forust Version: 0.2.6 Classifier: Programming
-Language :: Rust Classifier: Programming Language :: Python :: Implementation
-:: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: numpy>=1.21 Requires-Dist: pandas>=1.3 Requires-Dist: maturin;
-extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist: seaborn;
-extra == 'dev' Requires-Dist: xgboost==1.6.1; extra == 'dev' Requires-Dist:
-scikit-learn; extra == 'dev' Provides-Extra: dev License-File: LICENSE Summary:
-A lightweight gradient boosting implementation in Rust. Keywords:
-rust,forust,machine learning,xgboost,tree model,decision tree Author: James
-Inlow Requires-Python: >=3.8 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM
    [https://github.com/jinlow/forust/raw/main/resources/tree-image-crop.png]
  ![PyPI](https://img.shields.io/pypi/v/forust?color=gr&style=for-the-badge) !
  [Crates.io](https://img.shields.io/crates/v/forust-ml?color=gr&style=for-the-
                                     badge)
 # Forust ## _A lightweight gradient boosting package_ Forust, is a lightweight
 package for building gradient boosted decision tree ensembles. All of the
 algorithm code is written in [Rust](https://www.rust-lang.org/), with a python
@@ -24,15 +13,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.6" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.7" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -81,56 +70,89 @@
 used in the algorithm. Defaults to 0. - `missing` ***(float, optional)***:
 Value to consider missing, when training and predicting with the booster.
 Defaults to `np.nan`. - `create_missing_branch` ***(bool, optional)***: An
 experimental parameter, that if `True`, will create a separate branch for
 missing, creating a ternary tree, the missing node will be given the same
 weight value as the parent node. If this parameter is `False`, missing will be
 sent down either the left or right branch, creating a binary tree. Defaults to
-`False`. ### Training and Predicting Once, the booster has been initialized, it
-can be fit on a provided dataset, and performance field. After fitting, the
-model can be used to predict on a dataset. In the case of this example, the
-predictions are the log odds of a given record being 1. ```python # Small
-example dataset from seaborn import load_dataset df = load_dataset("titanic") X
-= df.select_dtypes("number").drop(columns=["survived"]) y = df["survived"] #
-Initialize a booster with defaults. from forust import GradientBooster model =
-GradientBooster(objective_type="LogLoss") model.fit(X, y) # Predict on data
-model.predict(X.head()) # array([-1.94919663, 2.25863229, 0.32963671,
-2.48732194, -3.00371813]) # predict contributions model.predict_contributions
-(X.head()) # array([[-0.63014213, 0.33880048, -0.16520798, -0.07798772, -
-0.85083578, # -1.07720813], # [ 1.05406709, 0.08825999, 0.21662544, -
-0.12083538, 0.35209258, # -1.07720813], ``` The `fit` method accepts the
-following arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2
-dimensional numpy array, with numeric data. - `y` ***(ArrayLike)***: Either a
-pandas Series, or a 1 dimensional numpy array. If "LogLoss" was the objective
-type specified, then this should only contain 1 or 0 values, where 1 is the
-positive class being predicted. If "SquaredLoss" is the objective type, then
-any continuous variable can be provided. - `sample_weight` ***(Optional
-[ArrayLike], optional)***: Instance weights to use when training the model. If
-None is passed, a weight of 1 will be used for every record. Defaults to None.
-The predict method accepts the following arguments. - `X` ***(FrameLike)***:
+`False`. - `sample_method` ***(str | None, optional)***: Optional string value
+to use to determine the method to use to sample the data while training. If
+this is None, no sample method will be used. If the `subsample` parameter is
+less than 1 and no sample_method is provided this `sample_method` will be
+automatically set to "random". Valid options are "goss" and "random". Defaults
+to `None`. - `evaluation_metric` ***(str | None, optional)***: Optional string
+value used to define an evaluation metric that will be calculated at each
+iteration if a `evaluation_dataset` is provided at fit time. The metric can be
+one of "AUC", "LogLoss", "RootMeanSquaredLogError", or "RootMeanSquaredError".
+If no `evaluation_metric` is passed, but an `evaluation_dataset` is passed,
+then "LogLoss", will be used with the "LogLoss" objective function, and
+"RootMeanSquaredLogError" will be used with "SquaredLoss". -
+`early_stopping_rounds` ***(int | None, optional)***: If this is specified, and
+an `evaluation_dataset` is passed during fit, then an improvement in the
+`evaluation_metric` must be seen after at least this many iterations of
+training, otherwise training will be cut short. ### Training and Predicting
+Once, the booster has been initialized, it can be fit on a provided dataset,
+and performance field. After fitting, the model can be used to predict on a
+dataset. In the case of this example, the predictions are the log odds of a
+given record being 1. ```python # Small example dataset from seaborn import
+load_dataset df = load_dataset("titanic") X = df.select_dtypes("number").drop
+(columns=["survived"]) y = df["survived"] # Initialize a booster with defaults.
+from forust import GradientBooster model = GradientBooster
+(objective_type="LogLoss") model.fit(X, y) # Predict on data model.predict
+(X.head()) # array([-1.94919663, 2.25863229, 0.32963671, 2.48732194, -
+3.00371813]) # predict contributions model.predict_contributions(X.head()) #
+array([[-0.63014213, 0.33880048, -0.16520798, -0.07798772, -0.85083578, # -
+1.07720813], # [ 1.05406709, 0.08825999, 0.21662544, -0.12083538, 0.35209258, #
+-1.07720813], ``` The `fit` method accepts the following arguments. - `X` ***
+(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with
+numeric data. - `y` ***(ArrayLike)***: Either a pandas Series, or a 1
+dimensional numpy array. If "LogLoss" was the objective type specified, then
+this should only contain 1 or 0 values, where 1 is the positive class being
+predicted. If "SquaredLoss" is the objective type, then any continuous variable
+can be provided. - `sample_weight` ***(Optional[ArrayLike], optional)***:
+Instance weights to use when training the model. If None is passed, a weight of
+1 will be used for every record. Defaults to None. - `evaluation_data` ***
+(tuple[FrameLike, ArrayLike, ArrayLike] | tuple[FrameLike, ArrayLike],
+optional)***: An optional list of tuples, where each tuple should contain a
+dataset, and equal length target array, and optional an equal length sample
+weight array. If this is provided metric values will be calculated at each
+iteration of training. If `early_stopping_rounds` is supplied, the first entry
+of this list will be used to determine if performance has improved over the
+last set of iterations, for which if no improvement is not seen in
+`early_stopping_rounds` training will be cut short. The predict method accepts
+the following arguments. - `X` ***(FrameLike)***: Either a pandas DataFrame, or
+a 2 dimensional numpy array, with numeric data. - `parallel` ***(Optional
+[bool], optional)***: Optionally specify if the predict function should run in
+parallel on multiple threads. If `None` is passed, the `parallel` attribute of
+the booster will be used. Defaults to `None`. The `predict_contributions`
+method will predict with the fitted booster on new data, returning the feature
+contribution matrix. The last column is the bias term. - `X` ***(FrameLike)***:
 Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data. -
-`parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
-function should run in parallel on multiple threads. If `None` is passed, the
-`parallel` attribute of the booster will be used. Defaults to `None`. The
-`predict_contributions` method will predict with the fitted booster on new
-data, returning the feature contribution matrix. The last column is the bias
-term. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional
-numpy array, with numeric data. - `method` ***(str, optional)***: Method to
-calculate the contributions, if "average" is specified, the average internal
-node values are calculated, this is equivalent to the `approx_contribs`
-parameter in XGBoost. The other supported method is "weight", this will use the
-internal leaf weights, to calculate the contributions. This is the same as what
-is described by Saabas [here](https://blog.datadive.net/interpreting-random-
-forests/). - `parallel` ***(Optional[bool], optional)***: Optionally specify if
-the predict function should run in parallel on multiple threads. If `None` is
-passed, the `parallel` attribute of the booster will be used. Defaults to
-`None`. ### Inspecting the Model Once the booster has been fit, each individual
-tree structure can be retrieved in text form, using the `text_dump` method.
-This method returns a list, the same length as the number of trees in the
-model. ```python model.text_dump()[0] # 0:[0 < 3]
+`method` ***(str, optional)***: Method to calculate the contributions, if
+"average" is specified, the average internal node values are calculated, this
+is equivalent to the `approx_contribs` parameter in XGBoost. The other
+supported method is "weight", this will use the internal leaf weights, to
+calculate the contributions. This is the same as what is described by Saabas
+[here](https://blog.datadive.net/interpreting-random-forests/). - `parallel`
+***(Optional[bool], optional)***: Optionally specify if the predict function
+should run in parallel on multiple threads. If `None` is passed, the `parallel`
+attribute of the booster will be used. Defaults to `None`. When predicting with
+the data, the maximum iteration that will be used when predicting can be set
+using the `set_prediction_iteration` method. If `early_stopping_rounds` has
+been set, this will default to the best iteration, otherwise all of the trees
+will be used. It accepts a single value. - `iteration` (int): Iteration number
+to use, this will use all trees, up to and including this index. If early
+stopping was used, the evaluation history can be retrieved with the
+`get_evaluation_history` method. ```python model = GradientBooster
+(objective_type="LogLoss") model.fit(X, y, evaluation_data=[(X, y)])
+model.get_evaluation_history()[0:3] # array([[588.9158873 ], # [532.01055803],
+# [496.76933646]]) ``` ### Inspecting the Model Once the booster has been fit,
+each individual tree structure can be retrieved in text form, using the
+`text_dump` method. This method returns a list, the same length as the number
+of trees in the model. ```python model.text_dump()[0] # 0:[0 < 3]
 yes=1,no=2,missing=2,gain=91.50833,cover=209.388307 # 1:[4 < 13.7917]
 yes=3,no=4,missing=4,gain=28.185467,cover=94.00148 # 3:[1 < 18]
 yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348 # 7:[1 < 17]
 yes=15,no=16,missing=16,gain=0.691266,cover=0.705011 # 15:leaf=-
 0.15120,cover=0.23500 # 16:leaf=0.154097,cover=0.470007 ``` The `json_dump`
 method performs the same action, but returns the model as a json representation
 rather than a text string. To see an estimate for how a given feature is used
```

