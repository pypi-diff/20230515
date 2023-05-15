# Comparing `tmp/lophat-0.8.3.tar.gz` & `tmp/lophat-0.9.0.tar.gz`

## Comparing `lophat-0.8.3.tar` & `lophat-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 lophat-0.8.3/Cargo.toml
--rw-r--r--   0     1000     1001      691 2023-03-09 14:38:58.000000 lophat-0.8.3/.gitignore
--rw-r--r--   0     1000     1001     1071 2023-03-07 14:26:14.000000 lophat-0.8.3/LICENSE
--rw-r--r--   0     1000     1001     4365 2023-04-12 13:01:54.000000 lophat-0.8.3/README.md
--rw-r--r--   0     1000     1001     1154 2023-03-27 07:14:32.000000 lophat-0.8.3/example.py
--rw-r--r--   0     1000     1001     2249 2023-03-24 12:16:44.000000 lophat-0.8.3/lophat.pyi
--rw-r--r--   0     1000     1001      316 2023-03-09 07:17:41.000000 lophat-0.8.3/pyproject.toml
--rw-r--r--   0     1000     1001     4020 2023-04-14 09:38:24.000000 lophat-0.8.3/src/anti_transpose.rs
--rw-r--r--   0     1000     1001     6683 2023-04-14 10:16:52.000000 lophat-0.8.3/src/column.rs
--rw-r--r--   0     1000     1001     5905 2023-03-31 10:49:18.000000 lophat-0.8.3/src/decomposition.rs
--rw-r--r--   0     1000     1001     1342 2023-04-12 13:01:54.000000 lophat-0.8.3/src/diagram.rs
--rw-r--r--   0     1000     1001     1360 2023-03-24 12:16:44.000000 lophat-0.8.3/src/indexing.rs
--rw-r--r--   0     1000     1001     5018 2023-04-18 07:35:51.000000 lophat-0.8.3/src/lib.rs
--rw-r--r--   0     1000     1001    11898 2023-04-18 07:39:38.000000 lophat-0.8.3/src/lock_free.rs
--rw-r--r--   0     1000     1001    12379 2023-04-17 07:42:42.000000 lophat-0.8.3/src/locking.rs
--rw-r--r--   0     1000     1001     2097 2023-04-12 13:01:54.000000 lophat-0.8.3/src/options.rs
--rw-r--r--   0     1000     1001     2416 2023-04-18 07:14:49.000000 lophat-0.8.3/timing_test.py
--rw-r--r--   0     1000     1001    19352 2023-04-18 09:32:34.000000 lophat-0.8.3/Cargo.lock
--rw-r--r--   0        0        0     4892 1970-01-01 00:00:00.000000 lophat-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 lophat-0.9.0/Cargo.toml
+-rw-r--r--   0     1000     1001      691 2023-03-09 14:38:58.000000 lophat-0.9.0/.gitignore
+-rw-r--r--   0     1000     1001     1071 2023-03-07 14:26:14.000000 lophat-0.9.0/LICENSE
+-rw-r--r--   0     1000     1001     4608 2023-04-19 10:41:37.000000 lophat-0.9.0/README.md
+-rw-r--r--   0     1000     1001     1154 2023-03-27 07:14:32.000000 lophat-0.9.0/example.py
+-rw-r--r--   0     1000     1001     2181 2023-04-19 13:33:57.000000 lophat-0.9.0/lophat.pyi
+-rw-r--r--   0     1000     1001      316 2023-03-09 07:17:41.000000 lophat-0.9.0/pyproject.toml
+-rw-r--r--   0     1000     1001    13047 2023-04-19 10:41:39.000000 lophat-0.9.0/src/algorithms/lock_free.rs
+-rw-r--r--   0     1000     1001    11987 2023-04-19 10:38:16.000000 lophat-0.9.0/src/algorithms/locking.rs
+-rw-r--r--   0     1000     1001     3213 2023-04-19 10:03:29.000000 lophat-0.9.0/src/algorithms/mod.rs
+-rw-r--r--   0     1000     1001     5109 2023-04-19 10:37:51.000000 lophat-0.9.0/src/algorithms/serial.rs
+-rw-r--r--   0     1000     1001     2761 2023-04-19 13:34:49.000000 lophat-0.9.0/src/bindings.rs
+-rw-r--r--   0     1000     1001     1991 2023-04-19 09:58:40.000000 lophat-0.9.0/src/columns/bit_set.rs
+-rw-r--r--   0     1000     1001     4027 2023-04-19 10:54:59.000000 lophat-0.9.0/src/columns/hybrid.rs
+-rw-r--r--   0     1000     1001     3580 2023-04-19 10:20:09.000000 lophat-0.9.0/src/columns/mod.rs
+-rw-r--r--   0     1000     1001     2931 2023-04-19 10:02:48.000000 lophat-0.9.0/src/columns/vec.rs
+-rw-r--r--   0     1000     1001     3195 2023-04-19 10:41:41.000000 lophat-0.9.0/src/lib.rs
+-rw-r--r--   0     1000     1001     2276 2023-04-19 11:02:43.000000 lophat-0.9.0/src/options.rs
+-rw-r--r--   0     1000     1001     3300 2023-04-19 07:32:06.000000 lophat-0.9.0/src/utils/anti_transpose.rs
+-rw-r--r--   0     1000     1001     1966 2023-04-19 10:06:47.000000 lophat-0.9.0/src/utils/diagram.rs
+-rw-r--r--   0     1000     1001      511 2023-04-19 10:39:55.000000 lophat-0.9.0/src/utils/mod.rs
+-rw-r--r--   0     1000     1001     2416 2023-04-18 07:14:49.000000 lophat-0.9.0/timing_test.py
+-rw-r--r--   0     1000     1001    19352 2023-04-19 12:11:06.000000 lophat-0.9.0/Cargo.lock
+-rw-r--r--   0        0        0     5135 1970-01-01 00:00:00.000000 lophat-0.9.0/PKG-INFO
```

### Comparing `lophat-0.8.3/Cargo.toml` & `lophat-0.9.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "lophat"
-version = "0.8.3"
+version = "0.9.0"
 edition = "2021"
 license = "MIT"
 description = "Lockfree Persistent Homology Algorithm Toolbox"
 homepage = "https://github.com/tomchaplin/lophat"
 repository = "https://github.com/tomchaplin/lophat"
 readme = "README.md"
 exclude = ["scripts/**/*", "docs/**/*"]
```

### Comparing `lophat-0.8.3/.gitignore` & `lophat-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lophat-0.8.3/LICENSE` & `lophat-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lophat-0.8.3/README.md` & `lophat-0.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 The primary goal of this library is to make the algorithm accessible to those wishing to compute PH of ___arbitrary filtered chain complexes___.
 In particular, LoPHAT is **not** specialised to compute PH of common filtrations or even filtered simplicial complexes.
 As such, you should expect LoPHAT to under-perform as compared to [giotto-ph [3]](#3) or [oineus  [4]](#4), both of which use the algorithm of [[1]](#1).
 
 The only changes from the algorithm described in [[1]](#1) are:
 * We use the `pinboard` library for epoch-based memory management of the matrices.
 * We store the $j^{th}$ column of $R$ and $V$ alongside each other in memory, allowing a full $R=DV$ decomposition (rather than just computing pairings).
+* We additionally employ the clearing optimisation [[5]](#5) and provide methods for anti-transpotion (so as to compute persistent cohomology).
 * We distribute chunks via work-stealing, using the `rayon` library.
 
 > **Warning**
 > LoPHAT is currently in beta.
 > The implementation is not optimised, the API is not fixed and tests are limited.
 
 ## Usage in Rust
@@ -55,24 +56,22 @@
 To use serial algorithm or limit number of threads, additionally provide a `LoPhatOptions` object.
 
 For more details, please consult [the Python docs](https://lophat.readthedocs.io/en/latest/).
 For example usage, see the file `example.py` or [this Google colab notebook](https://colab.research.google.com/drive/1y0_wZfvuUZfRreYPO50mo4rBlflkMcfj?usp=sharing).
 
 ## TODO
 
+- [ ] Change options struct for each algorithm
+- [ ] Decide on new Python bindings
 - [ ] Increase property testing
 - [ ] Write unit tests
 - [ ] Write integration tests (testing V) 
 - [ ] Benchmark
-- [ ] Add alternative column representations
-- [ ] Implement a `LoPhatOptionsBuilder` in Rust and Python
-- [ ] Abstract out matrix trait
+- [ ] Abstract out matrix trait?
 - [ ] Reduce memory usage when V not maintained
-- [ ] Add example Rust usage
-- [ ] Add support for returning generators (needs different logic depending on whether homology or cohomology was computed).
 
 ## References
 
 <a id="1">[1]</a> Morozov, Dmitriy, and Arnur Nigmetov.
 "Towards lockfree persistent homology."
 Proceedings of the 32nd ACM Symposium on Parallelism in Algorithms and Architectures. 2020.
 
@@ -85,7 +84,13 @@
 arXiv preprint [arXiv:2107.05412](https://arxiv.org/abs/2107.05412) (2021).
 [GitHub](https://github.com/giotto-ai/giotto-ph)
 
 <a id="4">[4]</a> Nigmetov, Arnur, Morozov, Dmitriy, and USDOE.
 Oineus v1.0. Computer software.
 [https://www.osti.gov//servlets/purl/1774764](https://www.osti.gov//servlets/purl/1774764). USDOE. 1 Apr. 2021.
 Web. [doi:10.11578/dc.20210407.1](https://doi.org/10.11578/dc.20210407.1). [GitHub](https://github.com/anigmetov/oineus)
+
+<a id="5">[5]</a> Bauer, Ulrich, Michael Kerber, and Jan Reininghaus.
+"Clear and compress: Computing persistent homology in chunks."
+Topological Methods in Data Analysis and Visualization III: Theory, Algorithms, and Applications.
+Springer International Publishing, 2014.
+
```

### Comparing `lophat-0.8.3/example.py` & `lophat-0.9.0/example.py`

 * *Files identical despite different names*

### Comparing `lophat-0.8.3/lophat.pyi` & `lophat-0.9.0/lophat.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 from typing import Iterator, List, Set, Tuple
 
+
 def compute_pairings(
     matrix: List[Tuple[int, List[int]]] | Iterator[Tuple[int, List[int]]],
     anti_transpose: bool = True,
     options: LoPhatOptions | None = None,
 ) -> PersistenceDiagram:
     """
-    Decomposes the input matrix, using the lockfree or standard algorithm (according to options).
+    Decomposes the input matrix, using the lockfree algorithm.
 
     :param matrix: The boundary matrix, provided in sparse column format. Each column is a tuple of (dimension, boundary) where boundary is the list of non-zero indices.
     :param anti_transpose: Whether to anti-transpose the matrix first. Best left True with clearing on. Set to False if input matrix non-square.
     :param options: Options to control the R=DV decomposition algorithm.
     :returns: The persistence pairings read off from the R=DV decomposition.
     """
 
+
 class LoPhatOptions:
     """
     A class representing the persistence diagram computed by LoPHAT.
     Each column index in the input matrix appears exactly once, either in a pairing or as unpaired.
 
     :param maintain_v: Whether to maintain_v during decompositon, usually best left False.
-    :param num_threads: Max number of threads to use. Set at 0 to use all threads. Set at 1 to use standard, serial algorithm.
+    :param num_threads: Max number of threads to use. Set at 0 to use all threads.
     :param column_height: Optional hint to height of columns. If None, assumed that matrix is square.
     :param min_chunk_len: When splitting work, don't reduce chunks to smaller than this size.
     :param clearing: Whether to employ the clearing optimisation. Cannot use if input non-square.
     """
 
     def __init__(
         self,
         maintain_v: bool = False,
         num_threads: int = 0,
         column_height: int | None = None,
         min_chunk_len: int = 1,
         clearing: bool = True,
-    ) -> None: ...
+    ) -> None:
+        ...
+
 
 class PersistenceDiagram:
     """
     A class representing the persistence diagram computed by LoPHAT.
     Each column index in the input matrix appears exactly once, either in a pairing or as unpaired.
 
     :param unpaired: The set of input column indices that were not paired in the R=DV decomposition.
```

### Comparing `lophat-0.8.3/src/anti_transpose.rs` & `lophat-0.9.0/src/utils/anti_transpose.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,8 @@
-use crate::{Column, PersistenceDiagram};
-
-/// Re-indexes a persistence diagram, assuming that it was produced from an anti-transposed matrix.
-/// * `diagram` - the diagram to reindex.
-/// * `matrix_size` - the size of the decomposed matrix, assumed to be square.
-pub fn anti_transpose_diagram(
-    mut diagram: PersistenceDiagram,
-    matrix_size: usize,
-) -> PersistenceDiagram {
-    let new_paired = diagram
-        .paired
-        .into_iter()
-        .map(|(b, d)| (matrix_size - 1 - d, matrix_size - 1 - b))
-        .collect();
-    let new_unpaired = diagram
-        .unpaired
-        .into_iter()
-        .map(|idx| matrix_size - 1 - idx)
-        .collect();
-    diagram.paired = new_paired;
-    diagram.unpaired = new_unpaired;
-    diagram
-}
+use crate::columns::Column;
 
 /// Anti-transposes the input matrix (e.g. to compute cohomology).
 /// * `matrix` - a reference to a collected matrix (vector of columns).
 /// Assumes that input matrix is square.
 pub fn anti_transpose<C: Column>(matrix: &Vec<C>) -> Vec<C> {
     let matrix_width = matrix.len();
     let max_dim = matrix.iter().map(|col| col.dimension()).max().unwrap();
@@ -40,15 +18,15 @@
     }
     return_matrix
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
-    use crate::column::VecColumn;
+    use crate::columns::VecColumn;
 
     fn build_sphere_triangulation() -> Vec<VecColumn> {
         vec![
             (0, vec![]),
             (0, vec![]),
             (0, vec![]),
             (0, vec![]),
```

### Comparing `lophat-0.8.3/src/decomposition.rs` & `lophat-0.9.0/src/algorithms/serial.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,118 +1,111 @@
-use crate::{Column, DiagramReadOff, LoPhatOptions, PersistenceDiagram};
-use hashbrown::HashSet;
-use rayon::prelude::*;
+use crate::{
+    algorithms::RVDecomposition,
+    columns::{Column, ColumnMode},
+    options::LoPhatOptions,
+};
+
 use std::collections::HashMap;
 
-/// Stores the matrices R and V resulting from and R=DV decomposition as vectors of structs implementing [`Column`].
-#[derive(Debug, Default)]
-pub struct RVDecomposition<C: Column> {
-    pub r: Vec<C>,
-    pub v: Option<Vec<C>>,
+/// Implements the standard left-to-right column additional algorithm of [Edelsbrunner et al.](https://doi.org/10.1109/SFCS.2000.892133).
+/// No optimisations have been implemented.
+#[derive(Debug)]
+pub struct SerialAlgorithm<C: Column> {
+    r: Vec<C>,
+    v: Option<Vec<C>>,
+    low_inverse: HashMap<usize, usize>,
 }
 
-fn col_idx_with_same_low<C: Column>(col: &C, low_inverse: &HashMap<usize, usize>) -> Option<usize> {
-    let pivot = col.pivot()?;
-    low_inverse.get(&pivot).copied()
-}
+impl<C: Column> SerialAlgorithm<C> {
+    fn new(options: LoPhatOptions) -> Self {
+        Self {
+            r: vec![],
+            v: options.maintain_v.then_some(vec![]),
+            low_inverse: HashMap::new(),
+        }
+    }
 
-impl<C: Column> RVDecomposition<C> {
-    /// Uses the decomposition so far to reduce the next column of D.
-    /// 1. Receives `column`, assumed to be the next column of D.
-    /// 2. Reduces it with left-to-right addition from R.
-    /// 3. Pushes the reduced column to R and the correct corrsponding column to V to maintain a R=DV decomposition.
-    /// 4. Updates low_invese if the reduced column is non-zero.
-    ///
-    /// Note: `low_inverse` should be a mainted list of pivots so that if `self.r[j]` is non-empty then
-    /// ```ignore
-    /// low_inverse.get(&self.r[j].pivot().unwrap()) == j
-    /// ```
-    /// If you pass the same `HashMap` into `reduce_column` every time, it will maintain this map.
-    pub fn reduce_column(&mut self, mut column: C, low_inverse: &mut HashMap<usize, usize>) {
+    fn col_idx_with_same_low(&self, col: &C) -> Option<usize> {
+        let pivot = col.pivot()?;
+        self.low_inverse.get(&pivot).copied()
+    }
+    /// Uses the decomposition so far to reduce the next column of D with left-to-right columns addition.
+    pub fn reduce_column(&mut self, mut column: C) {
+        column.set_mode(ColumnMode::Working);
         // v_col tracks how the final reduced column is built up
         // Currently column contains 1 lot of the latest column in D
         let maintain_v = self.v.is_some();
         let mut v_col: Option<C> = None;
         if maintain_v {
             let mut v_col_internal = C::new_with_dimension(column.dimension());
+            v_col_internal.set_mode(ColumnMode::Working);
             v_col_internal.add_entry(self.r.len());
             v_col = Some(v_col_internal);
         }
         // Reduce the column, keeping track of how we do this in V
-        while let Some(col_idx) = col_idx_with_same_low(&column, &low_inverse) {
+        while let Some(col_idx) = self.col_idx_with_same_low(&column) {
             column.add_col(&self.r[col_idx]);
             if maintain_v {
                 v_col
                     .as_mut()
                     .unwrap()
                     .add_col(&self.v.as_mut().unwrap()[col_idx]);
             }
         }
         // Update low inverse
         let final_pivot = column.pivot();
         if let Some(final_pivot) = final_pivot {
             // This column has a lowest 1 and is being inserted at the end of R
-            low_inverse.insert(final_pivot, self.r.len());
+            self.low_inverse.insert(final_pivot, self.r.len());
         }
         // Push to decomposition
+        column.set_mode(ColumnMode::Storage);
         self.r.push(column);
         if maintain_v {
-            self.v.as_mut().unwrap().push(v_col.unwrap());
+            let mut v_col = v_col.unwrap();
+            v_col.set_mode(ColumnMode::Storage);
+            self.v.as_mut().unwrap().push(v_col);
         }
     }
 }
 
-impl<C: Column> DiagramReadOff for RVDecomposition<C> {
-    /// Constructs a persistence diagram from the R=DV decomposition via the usual
-    /// algorithm, reading off lowest-ones.
-    fn diagram(&self) -> PersistenceDiagram {
-        let paired: HashSet<(usize, usize)> = self
-            .r
-            .par_iter()
-            .enumerate()
-            .filter_map(|(idx, col)| {
-                let lowest_idx = col.pivot()?;
-                Some((lowest_idx, idx))
-            })
-            .collect();
-        let mut unpaired: HashSet<usize> = (0..self.r.len()).collect();
-        for (birth, death) in paired.iter() {
-            unpaired.remove(birth);
-            unpaired.remove(death);
-        }
-        PersistenceDiagram { unpaired, paired }
+impl<C: Column> RVDecomposition<C> for SerialAlgorithm<C> {
+    fn get_r_col(&self, index: usize) -> &C {
+        &self.r[index]
     }
-}
 
-/// Decomposes the input matrix, using the standard, serial algorithm.
-///
-/// * `matrix` - iterator over columns of the matrix you wish to decompose.
-/// * `options` - additional options to control decompositon, see [`LoPhatOptions`].
-pub fn rv_decompose_serial<C: Column>(
-    matrix: impl Iterator<Item = C>,
-    options: &LoPhatOptions,
-) -> RVDecomposition<C> {
-    let mut low_inverse = HashMap::new();
-    let init_rv = if options.maintain_v {
-        RVDecomposition {
-            r: vec![],
-            v: Some(vec![]),
-        }
-    } else {
-        RVDecomposition { r: vec![], v: None }
-    };
-    matrix.fold(init_rv, |mut accum, next_col| {
-        accum.reduce_column(next_col, &mut low_inverse);
-        accum
-    })
+    fn get_v_col(&self, index: usize) -> Option<&C> {
+        Some(&self.v.as_ref()?[index])
+    }
+
+    fn n_cols(&self) -> usize {
+        self.r.len()
+    }
+
+    type RColRef<'a> = &'a C where Self : 'a;
+
+    type VColRef<'a> = &'a C where Self: 'a;
+
+    type Options = LoPhatOptions;
+
+    fn decompose(matrix: impl Iterator<Item = C>, options: Option<Self::Options>) -> Self {
+        let options = options.unwrap_or_default();
+        let algo = SerialAlgorithm::new(options);
+        matrix.fold(algo, |mut accum, next_col| {
+            accum.reduce_column(next_col);
+            accum
+        })
+    }
 }
 
 #[cfg(test)]
 mod tests {
-    use crate::column::VecColumn;
+    use hashbrown::HashSet;
+
+    use crate::{columns::VecColumn, utils::PersistenceDiagram};
 
     use super::*;
 
     fn build_sphere_triangulation() -> impl Iterator<Item = VecColumn> {
         vec![
             (0, vec![]),
             (0, vec![]),
@@ -137,28 +130,28 @@
     fn sphere_triangulation_correct() {
         let matrix = build_sphere_triangulation();
         let correct_diagram = PersistenceDiagram {
             unpaired: HashSet::from_iter(vec![0, 13]),
             paired: HashSet::from_iter(vec![(1, 4), (2, 5), (3, 7), (6, 12), (8, 10), (9, 11)]),
         };
         let options = LoPhatOptions::default();
-        let computed_diagram = rv_decompose_serial(matrix, &options).diagram();
+        let computed_diagram = SerialAlgorithm::decompose(matrix, Some(options)).diagram();
         assert_eq!(computed_diagram, correct_diagram)
     }
 
     #[test]
     fn test_v_maintain() {
         let matrix = build_sphere_triangulation();
         let mut options = LoPhatOptions::default();
         options.maintain_v = true;
         let correct_diagram = PersistenceDiagram {
             unpaired: HashSet::from_iter(vec![0, 13]),
             paired: HashSet::from_iter(vec![(1, 4), (2, 5), (3, 7), (6, 12), (8, 10), (9, 11)]),
         };
-        let decomp = rv_decompose_serial(matrix, &options);
+        let decomp = SerialAlgorithm::decompose(matrix, Some(options));
         let computed_diagram = decomp.diagram();
         for col in decomp.v.unwrap() {
             println!("{:?}", col);
         }
         assert_eq!(computed_diagram, correct_diagram)
     }
 }
```

### Comparing `lophat-0.8.3/src/lock_free.rs` & `lophat-0.9.0/src/algorithms/lock_free.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-use crate::Column;
-use crate::DiagramReadOff;
-use crate::LoPhatOptions;
-use crate::PersistenceDiagram;
-use crate::RVDecomposition;
+use std::ops::Deref;
+
+use crate::columns::Column;
+use crate::columns::ColumnMode::{Storage, Working};
+use crate::options::LoPhatOptions;
+use crate::utils::set_mode_of_pair;
 
 use crossbeam::atomic::AtomicCell;
-use hashbrown::HashSet;
 use pinboard::GuardedRef;
 use pinboard::NonEmptyPinboard;
 use rayon::prelude::*;
 #[cfg(feature = "local_thread_pool")]
 use rayon::ThreadPoolBuilder;
 
+use super::RVDecomposition;
+
 enum LoPhatThreadPool {
     #[cfg(not(feature = "local_thread_pool"))]
     Global(),
     #[cfg(feature = "local_thread_pool")]
     Local(rayon::ThreadPool),
 }
 
@@ -30,27 +32,28 @@
             LoPhatThreadPool::Global() => op(),
             #[cfg(feature = "local_thread_pool")]
             LoPhatThreadPool::Local(pool) => pool.install(op),
         }
     }
 }
 
-/// Stores the matrix and pivot vector behind appropriate atomic data types, as well as the algorithm options.
-/// Provides methods for reducing the matrix in parallel.
-pub struct LockFreeAlgorithm<'a, C: Column + 'static> {
+/// Implements the parallel, lockfree algorithm introduced by [Morozov and Nigmetov](https://doi.org/10.1145/3350755.3400244).
+/// Also able to employ the clearing optimisation of [Bauer et al.](https://doi.org/10.1007/978-3-319-04099-8_7).
+pub struct LockFreeAlgorithm<C: Column + 'static> {
     matrix: Vec<NonEmptyPinboard<(C, Option<C>)>>,
     pivots: Vec<AtomicCell<Option<usize>>>,
-    options: &'a LoPhatOptions,
+    options: LoPhatOptions,
     thread_pool: LoPhatThreadPool,
     max_dim: usize,
 }
 
-impl<'a, C: Column + 'static> LockFreeAlgorithm<'a, C> {
+impl<C: Column + 'static> LockFreeAlgorithm<C> {
     /// Initialise atomic data structure with provided `matrix`, store algorithm options and init thread pool.
-    pub fn new(matrix: impl Iterator<Item = C>, options: &'a LoPhatOptions) -> Self {
+    fn new(matrix: impl Iterator<Item = C>, options: LoPhatOptions) -> Self {
+        Self::warn_if_not_lockfree();
         let mut max_dim = 0;
         let matrix: Vec<_> = matrix
             .enumerate()
             .map(|(idx, r_col)| {
                 max_dim = max_dim.max(r_col.dimension());
                 if options.maintain_v {
                     let mut v_col = C::new_with_dimension(r_col.dimension());
@@ -86,14 +89,20 @@
             pivots,
             options,
             thread_pool,
             max_dim,
         }
     }
 
+    fn warn_if_not_lockfree() {
+        if !AtomicCell::<Option<usize>>::is_lock_free() {
+            eprintln!("WARNING: The pivot vector is locking");
+        }
+    }
+
     /// Return a column with index `l`, if one exists.
     /// If found, returns `(col_idx, col)`, where col is a tuple consisting of the corresponding column in R and V.
     /// If not maintaining V, second entry of tuple is `None`.
     pub fn get_col_with_pivot(&self, l: usize) -> Option<(usize, GuardedRef<(C, Option<C>)>)> {
         loop {
             let piv = self.pivots[l].load();
             if let Some(piv) = piv {
@@ -115,76 +124,82 @@
     /// If a pivot is found to the right of `j` (e.g. redued by another thread)
     /// then will switch to reducing that column.
     /// It is safe to reduce all columns in parallel.
     pub fn reduce_column(&self, j: usize) {
         let mut working_j = j;
         'outer: loop {
             // We make a copy of the column because we want to mutate our local copy
-            // without locking other threads from reading
             let mut curr_column = self.matrix[working_j].read();
+            set_mode_of_pair(&mut curr_column, Working);
             while let Some(l) = (&curr_column).0.pivot() {
                 let piv_with_column_opt = self.get_col_with_pivot(l);
                 if let Some((piv, piv_column)) = piv_with_column_opt {
                     // Lines 17-24
                     if piv < working_j {
                         curr_column.0.add_col(&piv_column.0);
                         // Only add V columns if we need to
                         if self.options.maintain_v {
                             let curr_v_col = curr_column.1.as_mut().unwrap();
                             curr_v_col.add_col(piv_column.1.as_ref().unwrap());
                         }
                     } else if piv > working_j {
-                        self.matrix[working_j].set(curr_column);
+                        self.write_to_matrix(working_j, curr_column);
                         if self.pivots[l]
                             .compare_exchange(Some(piv), Some(working_j))
                             .is_ok()
                         {
                             working_j = piv;
                         }
                         continue 'outer;
                     } else {
                         panic!()
                     }
                 } else {
                     // piv = -1 case
-                    self.matrix[working_j].set(curr_column);
+                    self.write_to_matrix(working_j, curr_column);
                     if self.pivots[l]
                         .compare_exchange(None, Some(working_j))
                         .is_ok()
                     {
                         return;
                     } else {
                         continue 'outer;
                     }
                 }
             }
             // Lines 25-27 (curr_column = 0 clause)
             if (&curr_column.0).is_cycle() {
-                self.matrix[working_j].set(curr_column);
+                self.write_to_matrix(working_j, curr_column);
                 return;
             }
         }
     }
 
+    fn write_to_matrix(&self, index: usize, mut to_write: (C, Option<C>)) {
+        set_mode_of_pair(&mut to_write, Storage);
+        self.matrix[index].set(to_write);
+    }
+
     /// Uses the boundary built up in column `boudary_idx` to clear the column corresponding to its pivot
     pub fn clear_with_column(&self, boudary_idx: usize) {
         let boundary = self.matrix[boudary_idx].get_ref();
         let boundary_r = &boundary.0;
         let clearing_idx = boundary_r
             .pivot()
             .expect("Attempted to clear using cycle column");
         let clearing_dimension = self.matrix[clearing_idx].get_ref().0.dimension();
         // The cleared R column is empty
         let r_col = C::new_with_dimension(clearing_dimension);
-        // The corresponding R column should be the R column of the boundary
-        let v_col = self
-            .options
-            .maintain_v
-            .then_some(boundary_r.clone().with_dimension(clearing_dimension));
-        self.matrix[clearing_idx].set((r_col, v_col));
+        // The corresponding V column should be the R column of the boundary
+        let v_col = self.options.maintain_v.then(|| {
+            let mut br = boundary_r.clone();
+            br.set_dimension(clearing_dimension);
+            br
+        });
+        self.write_to_matrix(clearing_idx, (r_col, v_col));
     }
 
     /// Reduce all columns of given dimension in parallel, according to `options`.
     pub fn reduce_dimension(&self, dimension: usize) {
         // Reduce matrix for columns of that dimension
         self.thread_pool.install(|| {
             (0..self.matrix.len())
@@ -215,91 +230,110 @@
             if self.options.clearing && dimension > 0 {
                 self.clear_dimension(dimension)
             }
         }
     }
 }
 
-impl<'a, C: Column + 'static> DiagramReadOff for LockFreeAlgorithm<'a, C> {
-    fn diagram(&self) -> crate::PersistenceDiagram {
-        let paired: HashSet<(usize, usize)> = self
-            .matrix
-            .par_iter()
-            .enumerate()
-            .filter_map(|(idx, col)| {
-                let lowest_idx = col.get_ref().0.pivot()?;
-                Some((lowest_idx, idx))
-            })
-            .collect();
-        let mut unpaired: HashSet<usize> = (0..self.matrix.len()).collect();
-        for (birth, death) in paired.iter() {
-            unpaired.remove(birth);
-            unpaired.remove(death);
-        }
-        PersistenceDiagram { unpaired, paired }
+pub struct LockFreeRRef<C>(GuardedRef<(C, Option<C>)>);
+
+impl<C> Deref for LockFreeRRef<C> {
+    type Target = C;
+
+    fn deref(&self) -> &Self::Target {
+        &self.0.deref().0
     }
 }
 
-impl<'a, C: Column + 'static> From<LockFreeAlgorithm<'a, C>> for RVDecomposition<C> {
-    fn from(algo: LockFreeAlgorithm<C>) -> Self {
-        let (r, v) = if algo.options.maintain_v {
-            let (r_sub, v_sub) = algo
-                .matrix
-                .into_iter()
-                .map(|pinboard| pinboard.read())
-                .map(|(r_col, v_col)| (r_col, v_col.unwrap()))
-                .unzip();
-            (r_sub, Some(v_sub))
-        } else {
-            (
-                algo.matrix
-                    .into_iter()
-                    .map(|pinboard| pinboard.read())
-                    .map(|(r_col, _v_col)| r_col)
-                    .collect(),
-                None,
-            )
-        };
-        RVDecomposition { r, v }
+pub struct LockFreeVRef<C>(GuardedRef<(C, Option<C>)>);
+
+impl<C> Deref for LockFreeVRef<C> {
+    type Target = C;
+
+    fn deref(&self) -> &Self::Target {
+        &self.0.deref().1.as_ref().unwrap()
     }
 }
 
-/// Decomposes the input matrix, using the lockfree, parallel algoirhtm of Morozov and Nigmetov.
-///
-/// * `matrix` - iterator over columns of the matrix you wish to decompose.
-/// * `options` - additional options to control decompositon, see [`LoPhatOptions`].
-pub fn rv_decompose_lock_free<C: Column + 'static>(
-    matrix: impl Iterator<Item = C>,
-    options: &LoPhatOptions,
-) -> LockFreeAlgorithm<C> {
-    let algo = LockFreeAlgorithm::new(matrix, options);
-    algo.reduce();
-    algo
+impl<C: Column + 'static> RVDecomposition<C> for LockFreeAlgorithm<C> {
+    type RColRef<'a> = LockFreeRRef<C>;
+    fn get_r_col<'a>(&'a self, index: usize) -> Self::RColRef<'a> {
+        LockFreeRRef(self.matrix[index].get_ref())
+    }
+
+    type VColRef<'a> = LockFreeVRef<C>;
+    fn get_v_col<'a>(&'a self, index: usize) -> Option<Self::VColRef<'a>> {
+        self.options
+            .maintain_v
+            .then_some(LockFreeVRef(self.matrix[index].get_ref()))
+    }
+
+    fn n_cols(&self) -> usize {
+        self.matrix.len()
+    }
+
+    type Options = LoPhatOptions;
+
+    fn decompose(matrix: impl Iterator<Item = C>, options: Option<Self::Options>) -> Self {
+        let options = options.unwrap_or_default();
+        let algo = LockFreeAlgorithm::new(matrix, options);
+        algo.reduce();
+        algo
+    }
 }
 
 #[cfg(test)]
 mod tests {
 
     use super::*;
-    use crate::column::VecColumn;
-    use crate::rv_decompose_serial;
-    use crate::DiagramReadOff;
+    use crate::algorithms::SerialAlgorithm;
+    use crate::columns::{BitSetColumn, BitSetVecHybridColumn, VecColumn};
     use proptest::collection::hash_set;
     use proptest::prelude::*;
 
     proptest! {
         #[test]
         fn lockfree_agrees_with_serial( matrix in sut_matrix(100) ) {
             let options = LoPhatOptions::default();
-            let serial_dgm = rv_decompose_serial(matrix.iter().cloned(), &options).diagram();
-            let parallel_dgm = rv_decompose_lock_free(matrix.into_iter(), &options).diagram();
+            let serial_dgm = SerialAlgorithm::decompose(matrix.iter().cloned(), Some(options)).diagram();
+            let parallel_dgm = LockFreeAlgorithm::decompose(matrix.into_iter(), Some(options)).diagram();
             assert_eq!(serial_dgm, parallel_dgm);
         }
     }
 
+    proptest! {
+        #[test]
+        fn hybrid_cols_work( matrix in sut_matrix(100) ) {
+            let hybrid_matrix = matrix.iter().map(|col| {
+                let mut hybrid_col = BitSetVecHybridColumn::new_with_dimension(col.dimension());
+                hybrid_col.add_entries(col.entries());
+                hybrid_col
+            });
+            let options = LoPhatOptions::default();
+            let hybrid_dgm = LockFreeAlgorithm::decompose(hybrid_matrix, Some(options)).diagram();
+            let vec_dgm = LockFreeAlgorithm::decompose(matrix.into_iter(), Some(options)).diagram();
+            assert_eq!(vec_dgm, hybrid_dgm);
+        }
+    }
+
+    proptest! {
+        #[test]
+        fn bit_set_cols_work( matrix in sut_matrix(100) ) {
+            let bit_set_matrix = matrix.iter().map(|col| {
+                let mut bit_set_col = BitSetColumn::new_with_dimension(col.dimension());
+                bit_set_col.add_entries(col.entries());
+                bit_set_col
+            });
+            let options = LoPhatOptions::default();
+            let bit_set_dgm = LockFreeAlgorithm::decompose(bit_set_matrix, Some(options)).diagram();
+            let vec_dgm = LockFreeAlgorithm::decompose(matrix.into_iter(), Some(options)).diagram();
+            assert_eq!(vec_dgm, bit_set_dgm);
+        }
+    }
+
     // Generates a strict upper triangular matrix of VecColumns with given size
     fn sut_matrix(size: usize) -> impl Strategy<Value = Vec<VecColumn>> {
         let mut matrix = vec![];
         for i in 1..size {
             matrix.push(veccolum_with_idxs_below(i));
         }
         matrix
```

### Comparing `lophat-0.8.3/src/locking.rs` & `lophat-0.9.0/src/algorithms/locking.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+use std::ops::Deref;
 use std::sync::RwLock;
 use std::sync::RwLockReadGuard;
 
-use crate::Column;
-use crate::DiagramReadOff;
-use crate::LoPhatOptions;
-use crate::PersistenceDiagram;
-use crate::RVDecomposition;
+use crate::algorithms::RVDecomposition;
+use crate::columns::Column;
+use crate::columns::ColumnMode::{Storage, Working};
+use crate::options::LoPhatOptions;
+use crate::utils::set_mode_of_pair;
 
 use crossbeam::atomic::AtomicCell;
-use hashbrown::HashSet;
 use rayon::prelude::*;
 #[cfg(feature = "local_thread_pool")]
 use rayon::ThreadPoolBuilder;
 
 enum LoPhatThreadPool {
     #[cfg(not(feature = "local_thread_pool"))]
     Global(),
@@ -31,27 +31,28 @@
             LoPhatThreadPool::Global() => op(),
             #[cfg(feature = "local_thread_pool")]
             LoPhatThreadPool::Local(pool) => pool.install(op),
         }
     }
 }
 
-/// Stores the matrix and pivot vector behind appropriate atomic data types, as well as the algorithm options.
-/// Provides methods for reducing the matrix in parallel.
-pub struct LockingAlgorithm<'a, C: Column + 'static> {
+/// Implements a locking version of the parallel, lockfree algorithm introduced by [Morozov and Nigmetov](https://doi.org/10.1145/3350755.3400244).
+/// Rather than using atomic pointers to store columns, each column is stored behind a [`RwLock`](std::sync::RwLock).
+/// Also able to employ the clearing optimisation of [Bauer et al.](https://doi.org/10.1007/978-3-319-04099-8_7).
+pub struct LockingAlgorithm<C: Column + 'static> {
     matrix: Vec<RwLock<(C, Option<C>)>>,
     pivots: Vec<AtomicCell<Option<usize>>>,
-    options: &'a LoPhatOptions,
+    options: LoPhatOptions,
     thread_pool: LoPhatThreadPool,
     max_dim: usize,
 }
 
-impl<'a, C: Column + 'static> LockingAlgorithm<'a, C> {
+impl<'a, C: Column> LockingAlgorithm<C> {
     /// Initialise atomic data structure with provided `matrix`, store algorithm options and init thread pool.
-    pub fn new(matrix: impl Iterator<Item = C>, options: &'a LoPhatOptions) -> Self {
+    fn new(matrix: impl Iterator<Item = C>, options: LoPhatOptions) -> Self {
         let mut max_dim = 0;
         let matrix: Vec<_> = matrix
             .enumerate()
             .map(|(idx, r_col)| {
                 max_dim = max_dim.max(r_col.dimension());
                 if options.maintain_v {
                     let mut v_col = C::new_with_dimension(r_col.dimension());
@@ -121,14 +122,15 @@
     /// It is safe to reduce all columns in parallel.
     pub fn reduce_column(&self, j: usize) {
         let mut working_j = j;
         'outer: loop {
             // We make a copy of the column because we want to mutate our local copy
             // without locking other threads from reading
             let mut curr_column = self.matrix[working_j].read().unwrap().clone();
+            set_mode_of_pair(&mut curr_column, Working);
             while let Some(l) = (&curr_column).0.pivot() {
                 let piv_with_column_opt = self.get_col_with_pivot(l);
                 if let Some((piv, piv_column)) = piv_with_column_opt {
                     // Lines 17-24
                     if piv < working_j {
                         curr_column.0.add_col(&piv_column.0);
                         // Only add V columns if we need to
@@ -167,34 +169,36 @@
                 return;
             }
         }
     }
 
     // Write to matrix; might lock until no read locks present
     // Make sure write lock is dropped quickly
-    fn write_to_matrix(&self, index: usize, to_write: (C, Option<C>)) {
+    fn write_to_matrix(&self, index: usize, mut to_write: (C, Option<C>)) {
+        set_mode_of_pair(&mut to_write, Storage);
         let mut in_matrix = self.matrix[index].write().unwrap();
         *in_matrix = to_write;
     }
 
     /// Uses the boundary built up in column `boudary_idx` to clear the column corresponding to its pivot
     pub fn clear_with_column(&self, boudary_idx: usize) {
         let boundary = self.matrix[boudary_idx].read().unwrap();
         let boundary_r = &boundary.0;
         let clearing_idx = boundary_r
             .pivot()
             .expect("Attempted to clear using cycle column");
         let clearing_dimension = self.matrix[clearing_idx].read().unwrap().0.dimension();
         // The cleared R column is empty
         let r_col = C::new_with_dimension(clearing_dimension);
-        // The corresponding R column should be the R column of the boundary
-        let v_col = self
-            .options
-            .maintain_v
-            .then_some(boundary_r.clone().with_dimension(clearing_dimension));
+        // The corresponding V column should be the R column of the boundary
+        let v_col = self.options.maintain_v.then(|| {
+            let mut br = boundary_r.clone();
+            br.set_dimension(clearing_dimension);
+            br
+        });
         self.write_to_matrix(clearing_idx, (r_col, v_col));
     }
 
     /// Reduce all columns of given dimension in parallel, according to `options`.
     pub fn reduce_dimension(&self, dimension: usize) {
         // Reduce matrix for columns of that dimension
         self.thread_pool.install(|| {
@@ -226,88 +230,76 @@
             if self.options.clearing && dimension > 0 {
                 self.clear_dimension(dimension)
             }
         }
     }
 }
 
-impl<'a, C: Column + 'static> DiagramReadOff for LockingAlgorithm<'a, C> {
-    fn diagram(&self) -> crate::PersistenceDiagram {
-        let paired: HashSet<(usize, usize)> = self
-            .matrix
-            .par_iter()
-            .enumerate()
-            .filter_map(|(idx, col)| {
-                let lowest_idx = col.read().unwrap().0.pivot()?;
-                Some((lowest_idx, idx))
-            })
-            .collect();
-        let mut unpaired: HashSet<usize> = (0..self.matrix.len()).collect();
-        for (birth, death) in paired.iter() {
-            unpaired.remove(birth);
-            unpaired.remove(death);
-        }
-        PersistenceDiagram { unpaired, paired }
+pub struct LockingRRef<'a, C>(RwLockReadGuard<'a, (C, Option<C>)>);
+
+impl<'a, C> Deref for LockingRRef<'a, C> {
+    type Target = C;
+
+    fn deref(&self) -> &Self::Target {
+        &self.0.deref().0
     }
 }
 
-impl<'a, C: Column + 'static> From<LockingAlgorithm<'a, C>> for RVDecomposition<C> {
-    fn from(algo: LockingAlgorithm<C>) -> Self {
-        let (r, v) = if algo.options.maintain_v {
-            let (r_sub, v_sub) = algo
-                .matrix
-                .into_iter()
-                .map(|rwlock_cols| rwlock_cols.into_inner().unwrap())
-                .map(|(r_col, v_col)| (r_col, v_col.unwrap()))
-                .unzip();
-            (r_sub, Some(v_sub))
-        } else {
-            (
-                algo.matrix
-                    .into_iter()
-                    .map(|rwlock_cols| rwlock_cols.into_inner().unwrap())
-                    .map(|(r_col, _v_col)| r_col)
-                    .collect(),
-                None,
-            )
-        };
-        RVDecomposition { r, v }
+pub struct LockingVRef<'a, C>(RwLockReadGuard<'a, (C, Option<C>)>);
+
+impl<'a, C> Deref for LockingVRef<'a, C> {
+    type Target = C;
+
+    fn deref(&self) -> &Self::Target {
+        &self.0.deref().1.as_ref().unwrap()
     }
 }
 
-/// Decomposes the input matrix, using the parallel algoirhtm of Morozov and Nigmetov
-/// but storing each column behind a [`RwLock`], to reduce cloning at the expense of locking.
-///
-/// * `matrix` - iterator over columns of the matrix you wish to decompose.
-/// * `options` - additional options to control decompositon, see [`LoPhatOptions`].
-pub fn rv_decompose_locking<C: Column + 'static>(
-    matrix: impl Iterator<Item = C>,
-    options: &LoPhatOptions,
-) -> LockingAlgorithm<C> {
-    let algo = LockingAlgorithm::new(matrix, options);
-    algo.reduce();
-    algo
+impl<C: Column + 'static> RVDecomposition<C> for LockingAlgorithm<C> {
+    type RColRef<'a> = LockingRRef<'a, C> where Self : 'a;
+    fn get_r_col<'a>(&'a self, index: usize) -> Self::RColRef<'a> {
+        LockingRRef(self.matrix[index].read().unwrap())
+    }
+
+    type VColRef<'a> = LockingVRef<'a, C> where Self : 'a;
+    fn get_v_col<'a>(&'a self, index: usize) -> Option<Self::VColRef<'a>> {
+        self.options
+            .maintain_v
+            .then_some(LockingVRef(self.matrix[index].read().unwrap()))
+    }
+
+    fn n_cols(&self) -> usize {
+        self.matrix.len()
+    }
+
+    type Options = LoPhatOptions;
+
+    fn decompose(matrix: impl Iterator<Item = C>, options: Option<Self::Options>) -> Self {
+        let options = options.unwrap_or_default();
+        let algo = LockingAlgorithm::new(matrix, options);
+        algo.reduce();
+        algo
+    }
 }
 
 #[cfg(test)]
 mod tests {
 
     use super::*;
-    use crate::column::VecColumn;
-    use crate::rv_decompose_serial;
-    use crate::DiagramReadOff;
+    use crate::algorithms::SerialAlgorithm;
+    use crate::columns::VecColumn;
     use proptest::collection::hash_set;
     use proptest::prelude::*;
 
     proptest! {
         #[test]
         fn locking_agrees_with_serial( matrix in sut_matrix(100) ) {
             let options = LoPhatOptions::default();
-            let serial_dgm = rv_decompose_serial(matrix.iter().cloned(), &options).diagram();
-            let parallel_dgm = rv_decompose_locking(matrix.into_iter(), &options).diagram();
+            let serial_dgm = SerialAlgorithm::decompose(matrix.iter().cloned(), Some(options)).diagram();
+            let parallel_dgm = LockingAlgorithm::decompose(matrix.into_iter(), Some(options)).diagram();
             assert_eq!(serial_dgm, parallel_dgm);
         }
     }
 
     // Generates a strict upper triangular matrix of VecColumns with given size
     fn sut_matrix(size: usize) -> impl Strategy<Value = Vec<VecColumn>> {
         let mut matrix = vec![];
```

### Comparing `lophat-0.8.3/src/options.rs` & `lophat-0.9.0/src/options.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,35 @@
+//! Options for all algorithms.
+//! Soon to be deprecated in favour of an option struct per algorithm.
+
 #[cfg(feature = "python")]
 use pyo3::prelude::*;
 
-/// A simple struct for specifying options for R=DV decompositions
-///
-/// * `maintain_v` - if true, returns full R=DV decomposition,
-///   otherwise returns [`RVDecomposition`](crate::RVDecomposition) with field `v` set to `None`.
-/// * `n_threads` - number of threads to use in thread pool; ignored by serial algorithms.
-///   see [`num_threads`](rayon::ThreadPoolBuilder::num_threads) for more details.
-///   Only relevant for lockfree algorithm.
-/// * `column_height` - an optional hint to the height of the columns.
-///   If `None`, assumed to be `matrix.collect().len()`.
-///   All indices must lie in the range `0..column_height`.
-///   Only relevant for lockfree algorithm.
-/// * `min_chunk_len` - When splitting work, don't reduce chunks to smaller than this size.
-///   Only relevant for lockfree algorithm.
-/// * `clearing` - Whether to employ the clearing optimisation.
-///   Note, if input matrix is not square then can't use this optimisation since it assumes D*D = 0.
-///   Only relevant for lockfree algorithm.
+/// A simple struct for specifying options for R=DV decompositions.
+/// Soon to be deprecated in favour of an option struct per algorithm.
 #[cfg_attr(feature = "python", pyclass(get_all, set_all))]
-#[derive(Clone)]
+#[derive(Copy, Clone)]
 pub struct LoPhatOptions {
+    /// If true, returns full R=DV decomposition, otherwise the resulting decomposition will always return `None` from [`get_v_col`](crate::algorithms::RVDecomposition::get_v_col).
     pub maintain_v: bool,
+    ///  Number of threads to use in thread pool; ignored by serial algorithms.
+    ///   see [`num_threads`](rayon::ThreadPoolBuilder::num_threads) for more details.
+    ///   Only relevant for lockfree algorithm.
     pub num_threads: usize,
+    ///  An optional hint to the height of the columns.
+    ///   If `None`, assumed to be `matrix.collect().len()`.
+    ///   All indices must lie in the range `0..column_height`.
+    ///   Only relevant for lockfree algorithm.
     pub column_height: Option<usize>,
+    ///  When splitting work, don't reduce chunks to smaller than this size.
+    ///   Only relevant for lockfree algorithm.
     pub min_chunk_len: usize,
+    ///  Whether to employ the clearing optimisation.
+    ///   Note, if input matrix is not square then can't use this optimisation since it assumes D*D = 0.
+    ///   Only relevant for lockfree algorithm.
     pub clearing: bool,
 }
 
 #[cfg(feature = "python")]
 #[pymethods]
 impl LoPhatOptions {
     #[new]
```

### Comparing `lophat-0.8.3/timing_test.py` & `lophat-0.9.0/timing_test.py`

 * *Files identical despite different names*

### Comparing `lophat-0.8.3/Cargo.lock` & `lophat-0.9.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "lophat"
-version = "0.8.3"
+version = "0.9.0"
 dependencies = [
  "bit-set",
  "crossbeam",
  "hashbrown",
  "pinboard",
  "proptest",
  "pyo3",
```

### Comparing `lophat-0.8.3/PKG-INFO` & `lophat-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lophat
-Version: 0.8.3
+Version: 0.9.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Lockfree Persistent Homology Algorithm Toolbox
 Home-Page: https://github.com/tomchaplin/lophat
 License: MIT
@@ -35,14 +35,15 @@
 The primary goal of this library is to make the algorithm accessible to those wishing to compute PH of ___arbitrary filtered chain complexes___.
 In particular, LoPHAT is **not** specialised to compute PH of common filtrations or even filtered simplicial complexes.
 As such, you should expect LoPHAT to under-perform as compared to [giotto-ph [3]](#3) or [oineus  [4]](#4), both of which use the algorithm of [[1]](#1).
 
 The only changes from the algorithm described in [[1]](#1) are:
 * We use the `pinboard` library for epoch-based memory management of the matrices.
 * We store the $j^{th}$ column of $R$ and $V$ alongside each other in memory, allowing a full $R=DV$ decomposition (rather than just computing pairings).
+* We additionally employ the clearing optimisation [[5]](#5) and provide methods for anti-transpotion (so as to compute persistent cohomology).
 * We distribute chunks via work-stealing, using the `rayon` library.
 
 > **Warning**
 > LoPHAT is currently in beta.
 > The implementation is not optimised, the API is not fixed and tests are limited.
 
 ## Usage in Rust
@@ -69,24 +70,22 @@
 To use serial algorithm or limit number of threads, additionally provide a `LoPhatOptions` object.
 
 For more details, please consult [the Python docs](https://lophat.readthedocs.io/en/latest/).
 For example usage, see the file `example.py` or [this Google colab notebook](https://colab.research.google.com/drive/1y0_wZfvuUZfRreYPO50mo4rBlflkMcfj?usp=sharing).
 
 ## TODO
 
+- [ ] Change options struct for each algorithm
+- [ ] Decide on new Python bindings
 - [ ] Increase property testing
 - [ ] Write unit tests
 - [ ] Write integration tests (testing V) 
 - [ ] Benchmark
-- [ ] Add alternative column representations
-- [ ] Implement a `LoPhatOptionsBuilder` in Rust and Python
-- [ ] Abstract out matrix trait
+- [ ] Abstract out matrix trait?
 - [ ] Reduce memory usage when V not maintained
-- [ ] Add example Rust usage
-- [ ] Add support for returning generators (needs different logic depending on whether homology or cohomology was computed).
 
 ## References
 
 <a id="1">[1]</a> Morozov, Dmitriy, and Arnur Nigmetov.
 "Towards lockfree persistent homology."
 Proceedings of the 32nd ACM Symposium on Parallelism in Algorithms and Architectures. 2020.
 
@@ -100,7 +99,13 @@
 [GitHub](https://github.com/giotto-ai/giotto-ph)
 
 <a id="4">[4]</a> Nigmetov, Arnur, Morozov, Dmitriy, and USDOE.
 Oineus v1.0. Computer software.
 [https://www.osti.gov//servlets/purl/1774764](https://www.osti.gov//servlets/purl/1774764). USDOE. 1 Apr. 2021.
 Web. [doi:10.11578/dc.20210407.1](https://doi.org/10.11578/dc.20210407.1). [GitHub](https://github.com/anigmetov/oineus)
 
+<a id="5">[5]</a> Bauer, Ulrich, Michael Kerber, and Jan Reininghaus.
+"Clear and compress: Computing persistent homology in chunks."
+Topological Methods in Data Analysis and Visualization III: Theory, Algorithms, and Applications.
+Springer International Publishing, 2014.
+
+
```

