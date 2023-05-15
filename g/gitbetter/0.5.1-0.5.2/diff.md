# Comparing `tmp/gitbetter-0.5.1.tar.gz` & `tmp/gitbetter-0.5.2.tar.gz`

## Comparing `gitbetter-0.5.1.tar` & `gitbetter-0.5.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 gitbetter-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0    34124 2020-02-02 00:00:00.000000 gitbetter-0.5.1/docs/gitbetter.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-0.5.1/docs/index.html
--rw-r--r--   0        0        0    57989 2020-02-02 00:00:00.000000 gitbetter-0.5.1/docs/search.js
--rw-r--r--   0        0        0   138245 2020-02-02 00:00:00.000000 gitbetter-0.5.1/docs/gitbetter/git.html
--rw-r--r--   0        0        0   248978 2020-02-02 00:00:00.000000 gitbetter-0.5.1/docs/gitbetter/gitbetter.html
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gitbetter-0.5.1/src/gitbetter/__init__.py
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 gitbetter-0.5.1/src/gitbetter/git.py
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 gitbetter-0.5.1/src/gitbetter/gitbetter.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-0.5.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-0.5.1/LICENSE.txt
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 gitbetter-0.5.1/README.md
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 gitbetter-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 gitbetter-0.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0    34124 2020-02-02 00:00:00.000000 gitbetter-0.5.2/docs/gitbetter.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-0.5.2/docs/index.html
+-rw-r--r--   0        0        0    57989 2020-02-02 00:00:00.000000 gitbetter-0.5.2/docs/search.js
+-rw-r--r--   0        0        0   138514 2020-02-02 00:00:00.000000 gitbetter-0.5.2/docs/gitbetter/git.html
+-rw-r--r--   0        0        0   248978 2020-02-02 00:00:00.000000 gitbetter-0.5.2/docs/gitbetter/gitbetter.html
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gitbetter-0.5.2/src/gitbetter/__init__.py
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 gitbetter-0.5.2/src/gitbetter/git.py
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 gitbetter-0.5.2/src/gitbetter/gitbetter.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-0.5.2/LICENSE.txt
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 gitbetter-0.5.2/README.md
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 gitbetter-0.5.2/PKG-INFO
```

### Comparing `gitbetter-0.5.1/CHANGELOG.md` & `gitbetter-0.5.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 # Changelog
 
-## 0.5.0 (2023-05-11)
+## 0.5.1 (2023-05-13)
+
+#### Fixes
+
+* fix  create_remote_from_cwd() not setting remote to upstream
+
+
+## v0.5.0 (2023-05-11)
 
 #### New Features
 
 * add create_remote_from_cwd()
 #### Refactorings
 
 * rename do_list_branches() to do_branches()
 * do_new_gh_remote invokes create_remote_from_cwd so url no longer needs to be added manually after creating remote
 #### Docs
 
 * update readme
 * update doc string
+#### Others
+
+* build v0.5.0
+* update changelog
 
 
 ## v0.4.0 (2023-05-04)
 
 #### New Features
 
 * add status command
```

### Comparing `gitbetter-0.5.1/docs/gitbetter.html` & `gitbetter-0.5.2/docs/gitbetter.html`

 * *Files identical despite different names*

### Comparing `gitbetter-0.5.1/docs/search.js` & `gitbetter-0.5.2/docs/search.js`

 * *Files identical despite different names*

### Comparing `gitbetter-0.5.1/docs/gitbetter/git.html` & `gitbetter-0.5.2/docs/gitbetter/git.html`

 * *Files 0% similar despite different names*

```diff
@@ -133,227 +133,229 @@
                 
                         <input id="mod-git-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-git-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">os</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a>
-</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a>
-</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a>    <span class="sd">&quot;&quot;&quot;Execute git command.</span>
-</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>
-</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="sd">    Equivalent to `os.system(f&quot;git {command}&quot;)`</span>
+</span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
+</span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a>
+</span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a>
+</span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a><span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a>    <span class="sd">&quot;&quot;&quot;Execute git command.</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="sd">    Returns the output of the `os.system` call.&quot;&quot;&quot;</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>    <span class="k">return</span> <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git </span><span class="si">{</span><span class="n">command</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="k">def</span> <span class="nf">new_repo</span><span class="p">():</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>    <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git init -b main&quot;&quot;&quot;</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;init -b main&quot;</span><span class="p">)</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a><span class="k">def</span> <span class="nf">loggy</span><span class="p">():</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git log --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;log --oneline --name-only --abbrev-commit --graph&quot;</span><span class="p">)</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a><span class="k">def</span> <span class="nf">status</span><span class="p">():</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>    <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;status&quot;</span><span class="p">)</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a><span class="c1"># ======================================Staging/Committing======================================</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a><span class="k">def</span> <span class="nf">commit</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>    <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git commit {args}&quot;&quot;&quot;</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;commit </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="k">def</span> <span class="nf">add</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>    <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="sd">    If no files are given (`files=None`), all files will be staged.&quot;&quot;&quot;</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;add .&quot;</span><span class="p">)</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;add </span><span class="si">{</span><span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">files</span><span class="p">)</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a><span class="k">def</span> <span class="nf">commit_files</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit a list of files with commit message `message`.&quot;&quot;&quot;</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a><span class="k">def</span> <span class="nf">initcommit</span><span class="p">():</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="sd">    &gt;&gt;&gt; git add .</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="sd">    &gt;&gt;&gt; git commit -m &quot;Initial commit&quot; &quot;&quot;&quot;</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="n">add</span><span class="p">()</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s1">&#39;-m &quot;Initial commit&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a><span class="k">def</span> <span class="nf">amend</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="sd">    If `files` is `None`, all files will be staged.</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="sd">    Equivalent to `os.system(f&quot;git {command}&quot;)`</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="sd">    Returns the output of the `os.system` call.&quot;&quot;&quot;</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>    <span class="k">return</span> <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git </span><span class="si">{</span><span class="n">command</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a><span class="k">def</span> <span class="nf">new_repo</span><span class="p">():</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>    <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git init -b main&quot;&quot;&quot;</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;init -b main&quot;</span><span class="p">)</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a><span class="k">def</span> <span class="nf">loggy</span><span class="p">():</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git log --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;log --oneline --name-only --abbrev-commit --graph&quot;</span><span class="p">)</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a><span class="k">def</span> <span class="nf">status</span><span class="p">():</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>    <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;status&quot;</span><span class="p">)</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a><span class="c1"># ======================================Staging/Committing======================================</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a><span class="k">def</span> <span class="nf">commit</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>    <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git commit {args}&quot;&quot;&quot;</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;commit </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="k">def</span> <span class="nf">add</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a><span class="sd">    If no files are given (`files=None`), all files will be staged.&quot;&quot;&quot;</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;add .&quot;</span><span class="p">)</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>        <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;add </span><span class="si">{</span><span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">files</span><span class="p">)</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a><span class="k">def</span> <span class="nf">commit_files</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit a list of files with commit message `message`.&quot;&quot;&quot;</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>    <span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="k">def</span> <span class="nf">initcommit</span><span class="p">():</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a><span class="sd">    &gt;&gt;&gt; git add .</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a><span class="sd">    &gt;&gt;&gt; git commit -m &quot;Initial commit&quot; &quot;&quot;&quot;</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="n">add</span><span class="p">()</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s1">&#39;-m &quot;Initial commit&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="k">def</span> <span class="nf">amend</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
 </span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="sd">    Equivalent to:</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="sd">    &gt;&gt;&gt; git add {files}</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="sd">    &gt;&gt;&gt; git commit --amend --no-edit</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a><span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="n">id_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>    <span class="sd">&quot;&quot;&quot;Tag the current commit with `id_`.</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="sd">    Equivalent to `git tag {id_}`.&quot;&quot;&quot;</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">id_</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="c1"># ==========================================Push/Pull==========================================</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">):</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a><span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">    Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a><span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a><span class="c1"># ============================================Checkout/Branches============================================</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a><span class="k">def</span> <span class="nf">list_branches</span><span class="p">():</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a><span class="sd">    Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a><span class="sd">    Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a><span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>    <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="sd">    If `files` is `None`, all files will be staged.</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="sd">    Equivalent to:</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a><span class="sd">    &gt;&gt;&gt; git add {files}</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a><span class="sd">    &gt;&gt;&gt; git commit --amend --no-edit</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a><span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="n">id_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>    <span class="sd">&quot;&quot;&quot;Tag the current commit with `id_`.</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a><span class="sd">    Equivalent to `git tag {id_}`.&quot;&quot;&quot;</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">id_</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a><span class="c1"># ==========================================Push/Pull==========================================</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">):</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a><span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a><span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="sd">    Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a><span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="c1"># ============================================Checkout/Branches============================================</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a><span class="k">def</span> <span class="nf">list_branches</span><span class="p">():</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a><span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a><span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">    Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a><span class="sd">    Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a><span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>    <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
 </span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a><span class="sd">    `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a><span class="k">def</span> <span class="nf">undo</span><span class="p">():</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a><span class="sd">    Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a><span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>    <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a><span class="c1"># ===============================Requires GitHub CLI to be installed and configured===============================</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a><span class="sd">    `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>    <span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>        <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a><span class="k">def</span> <span class="nf">undo</span><span class="p">():</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>    <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a><span class="sd">    Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a><span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>
 </span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a><span class="c1"># ===============================Requires GitHub CLI to be installed and configured===============================</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a><span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
 </span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a><span class="sd">    `name`: The name for the repo.</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a><span class="sd">    #### :params:</span>
 </span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a><span class="sd">    `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>    <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a><span class="sd">    the current working directory repo and add its url as this repo&#39;s remote origin.</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a><span class="sd">    `name`: The name for the repo.</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a><span class="sd">    `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a><span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>    <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">    the current working directory repo and add its url as this repo&#39;s remote origin.</span>
 </span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a><span class="sd">    `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create --source=. --remote=upstream --</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a><span class="sd">    `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create --source . --</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2"> --push&quot;</span><span class="p">)</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
 </span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="sd">    #### :params:</span>
 </span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility private&quot;</span><span class="p">)</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a><span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility private&quot;</span><span class="p">)</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a><span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
 </span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">    #### :params:</span>
 </span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility public&quot;</span><span class="p">)</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a><span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility public&quot;</span><span class="p">)</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a><span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
 </span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">    #### :params:</span>
 </span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">    `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo delete </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --yes&quot;</span><span class="p">)</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">    `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo delete </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --yes&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             </section>
                 <section id="execute">
                             <input id="execute-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -361,21 +363,21 @@
         <span class="def">def</span>
         <span class="name">execute</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">command</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="execute-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#execute"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="execute-5"><a href="#execute-5"><span class="linenos"> 5</span></a><span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="execute-6"><a href="#execute-6"><span class="linenos"> 6</span></a>    <span class="sd">&quot;&quot;&quot;Execute git command.</span>
-</span><span id="execute-7"><a href="#execute-7"><span class="linenos"> 7</span></a>
-</span><span id="execute-8"><a href="#execute-8"><span class="linenos"> 8</span></a><span class="sd">    Equivalent to `os.system(f&quot;git {command}&quot;)`</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="execute-7"><a href="#execute-7"><span class="linenos"> 7</span></a><span class="k">def</span> <span class="nf">execute</span><span class="p">(</span><span class="n">command</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="execute-8"><a href="#execute-8"><span class="linenos"> 8</span></a>    <span class="sd">&quot;&quot;&quot;Execute git command.</span>
 </span><span id="execute-9"><a href="#execute-9"><span class="linenos"> 9</span></a>
-</span><span id="execute-10"><a href="#execute-10"><span class="linenos">10</span></a><span class="sd">    Returns the output of the `os.system` call.&quot;&quot;&quot;</span>
-</span><span id="execute-11"><a href="#execute-11"><span class="linenos">11</span></a>    <span class="k">return</span> <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git </span><span class="si">{</span><span class="n">command</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="execute-10"><a href="#execute-10"><span class="linenos">10</span></a><span class="sd">    Equivalent to `os.system(f&quot;git {command}&quot;)`</span>
+</span><span id="execute-11"><a href="#execute-11"><span class="linenos">11</span></a>
+</span><span id="execute-12"><a href="#execute-12"><span class="linenos">12</span></a><span class="sd">    Returns the output of the `os.system` call.&quot;&quot;&quot;</span>
+</span><span id="execute-13"><a href="#execute-13"><span class="linenos">13</span></a>    <span class="k">return</span> <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;git </span><span class="si">{</span><span class="n">command</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute git command.</p>
 
 <p>Equivalent to <code>os.system(f"git {command}")</code></p>
 
@@ -391,17 +393,17 @@
         <span class="def">def</span>
         <span class="name">new_repo</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="new_repo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#new_repo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="new_repo-14"><a href="#new_repo-14"><span class="linenos">14</span></a><span class="k">def</span> <span class="nf">new_repo</span><span class="p">():</span>
-</span><span id="new_repo-15"><a href="#new_repo-15"><span class="linenos">15</span></a>    <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git init -b main&quot;&quot;&quot;</span>
-</span><span id="new_repo-16"><a href="#new_repo-16"><span class="linenos">16</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;init -b main&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="new_repo-16"><a href="#new_repo-16"><span class="linenos">16</span></a><span class="k">def</span> <span class="nf">new_repo</span><span class="p">():</span>
+</span><span id="new_repo-17"><a href="#new_repo-17"><span class="linenos">17</span></a>    <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git init -b main&quot;&quot;&quot;</span>
+</span><span id="new_repo-18"><a href="#new_repo-18"><span class="linenos">18</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;init -b main&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">git</span> <span class="n">init</span> <span class="o">-</span><span class="n">b</span> <span class="n">main</span>
 </code></pre>
 </div>
@@ -416,17 +418,17 @@
         <span class="def">def</span>
         <span class="name">loggy</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="loggy-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#loggy"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="loggy-19"><a href="#loggy-19"><span class="linenos">19</span></a><span class="k">def</span> <span class="nf">loggy</span><span class="p">():</span>
-</span><span id="loggy-20"><a href="#loggy-20"><span class="linenos">20</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git log --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="loggy-21"><a href="#loggy-21"><span class="linenos">21</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;log --oneline --name-only --abbrev-commit --graph&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="loggy-21"><a href="#loggy-21"><span class="linenos">21</span></a><span class="k">def</span> <span class="nf">loggy</span><span class="p">():</span>
+</span><span id="loggy-22"><a href="#loggy-22"><span class="linenos">22</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git log --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="loggy-23"><a href="#loggy-23"><span class="linenos">23</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;log --oneline --name-only --abbrev-commit --graph&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git log --oneline --name-only --abbrev-commit --graph</code>.</p>
 </div>
 
 
@@ -438,17 +440,17 @@
         <span class="def">def</span>
         <span class="name">status</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="status-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#status"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="status-24"><a href="#status-24"><span class="linenos">24</span></a><span class="k">def</span> <span class="nf">status</span><span class="p">():</span>
-</span><span id="status-25"><a href="#status-25"><span class="linenos">25</span></a>    <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
-</span><span id="status-26"><a href="#status-26"><span class="linenos">26</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;status&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="status-26"><a href="#status-26"><span class="linenos">26</span></a><span class="k">def</span> <span class="nf">status</span><span class="p">():</span>
+</span><span id="status-27"><a href="#status-27"><span class="linenos">27</span></a>    <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="status-28"><a href="#status-28"><span class="linenos">28</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;status&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git status</code>.</p>
 </div>
 
 
@@ -460,17 +462,17 @@
         <span class="def">def</span>
         <span class="name">commit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="commit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#commit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="commit-30"><a href="#commit-30"><span class="linenos">30</span></a><span class="k">def</span> <span class="nf">commit</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="commit-31"><a href="#commit-31"><span class="linenos">31</span></a>    <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git commit {args}&quot;&quot;&quot;</span>
-</span><span id="commit-32"><a href="#commit-32"><span class="linenos">32</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;commit </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="commit-32"><a href="#commit-32"><span class="linenos">32</span></a><span class="k">def</span> <span class="nf">commit</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="commit-33"><a href="#commit-33"><span class="linenos">33</span></a>    <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git commit {args}&quot;&quot;&quot;</span>
+</span><span id="commit-34"><a href="#commit-34"><span class="linenos">34</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;commit </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">git</span> <span class="n">commit</span> <span class="p">{</span><span class="n">args</span><span class="p">}</span>
 </code></pre>
 </div>
@@ -485,22 +487,22 @@
         <span class="def">def</span>
         <span class="name">add</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="add-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#add"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="add-35"><a href="#add-35"><span class="linenos">35</span></a><span class="k">def</span> <span class="nf">add</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="add-36"><a href="#add-36"><span class="linenos">36</span></a>    <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="add-37"><a href="#add-37"><span class="linenos">37</span></a>
-</span><span id="add-38"><a href="#add-38"><span class="linenos">38</span></a><span class="sd">    If no files are given (`files=None`), all files will be staged.&quot;&quot;&quot;</span>
-</span><span id="add-39"><a href="#add-39"><span class="linenos">39</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="add-40"><a href="#add-40"><span class="linenos">40</span></a>        <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;add .&quot;</span><span class="p">)</span>
-</span><span id="add-41"><a href="#add-41"><span class="linenos">41</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="add-42"><a href="#add-42"><span class="linenos">42</span></a>        <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;add </span><span class="si">{</span><span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">files</span><span class="p">)</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="add-37"><a href="#add-37"><span class="linenos">37</span></a><span class="k">def</span> <span class="nf">add</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="add-38"><a href="#add-38"><span class="linenos">38</span></a>    <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="add-39"><a href="#add-39"><span class="linenos">39</span></a>
+</span><span id="add-40"><a href="#add-40"><span class="linenos">40</span></a><span class="sd">    If no files are given (`files=None`), all files will be staged.&quot;&quot;&quot;</span>
+</span><span id="add-41"><a href="#add-41"><span class="linenos">41</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="add-42"><a href="#add-42"><span class="linenos">42</span></a>        <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;add .&quot;</span><span class="p">)</span>
+</span><span id="add-43"><a href="#add-43"><span class="linenos">43</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="add-44"><a href="#add-44"><span class="linenos">44</span></a>        <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;add </span><span class="si">{</span><span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">files</span><span class="p">)</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage a list of files.</p>
 
 <p>If no files are given (<code>files=None</code>), all files will be staged.</p>
 </div>
@@ -514,18 +516,18 @@
         <span class="def">def</span>
         <span class="name">commit_files</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>, </span><span class="param"><span class="n">message</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="commit_files-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#commit_files"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="commit_files-45"><a href="#commit_files-45"><span class="linenos">45</span></a><span class="k">def</span> <span class="nf">commit_files</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="commit_files-46"><a href="#commit_files-46"><span class="linenos">46</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit a list of files with commit message `message`.&quot;&quot;&quot;</span>
-</span><span id="commit_files-47"><a href="#commit_files-47"><span class="linenos">47</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
-</span><span id="commit_files-48"><a href="#commit_files-48"><span class="linenos">48</span></a>    <span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="commit_files-47"><a href="#commit_files-47"><span class="linenos">47</span></a><span class="k">def</span> <span class="nf">commit_files</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="commit_files-48"><a href="#commit_files-48"><span class="linenos">48</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit a list of files with commit message `message`.&quot;&quot;&quot;</span>
+</span><span id="commit_files-49"><a href="#commit_files-49"><span class="linenos">49</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
+</span><span id="commit_files-50"><a href="#commit_files-50"><span class="linenos">50</span></a>    <span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit a list of files with commit message <code>message</code>.</p>
 </div>
 
 
@@ -537,20 +539,20 @@
         <span class="def">def</span>
         <span class="name">initcommit</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="initcommit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#initcommit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="initcommit-51"><a href="#initcommit-51"><span class="linenos">51</span></a><span class="k">def</span> <span class="nf">initcommit</span><span class="p">():</span>
-</span><span id="initcommit-52"><a href="#initcommit-52"><span class="linenos">52</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to</span>
-</span><span id="initcommit-53"><a href="#initcommit-53"><span class="linenos">53</span></a><span class="sd">    &gt;&gt;&gt; git add .</span>
-</span><span id="initcommit-54"><a href="#initcommit-54"><span class="linenos">54</span></a><span class="sd">    &gt;&gt;&gt; git commit -m &quot;Initial commit&quot; &quot;&quot;&quot;</span>
-</span><span id="initcommit-55"><a href="#initcommit-55"><span class="linenos">55</span></a>    <span class="n">add</span><span class="p">()</span>
-</span><span id="initcommit-56"><a href="#initcommit-56"><span class="linenos">56</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s1">&#39;-m &quot;Initial commit&quot;&#39;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="initcommit-53"><a href="#initcommit-53"><span class="linenos">53</span></a><span class="k">def</span> <span class="nf">initcommit</span><span class="p">():</span>
+</span><span id="initcommit-54"><a href="#initcommit-54"><span class="linenos">54</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to</span>
+</span><span id="initcommit-55"><a href="#initcommit-55"><span class="linenos">55</span></a><span class="sd">    &gt;&gt;&gt; git add .</span>
+</span><span id="initcommit-56"><a href="#initcommit-56"><span class="linenos">56</span></a><span class="sd">    &gt;&gt;&gt; git commit -m &quot;Initial commit&quot; &quot;&quot;&quot;</span>
+</span><span id="initcommit-57"><a href="#initcommit-57"><span class="linenos">57</span></a>    <span class="n">add</span><span class="p">()</span>
+</span><span id="initcommit-58"><a href="#initcommit-58"><span class="linenos">58</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s1">&#39;-m &quot;Initial commit&quot;&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">git</span> <span class="n">add</span> <span class="o">.</span>
@@ -568,25 +570,25 @@
         <span class="def">def</span>
         <span class="name">amend</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="amend-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#amend"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="amend-59"><a href="#amend-59"><span class="linenos">59</span></a><span class="k">def</span> <span class="nf">amend</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="amend-60"><a href="#amend-60"><span class="linenos">60</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
-</span><span id="amend-61"><a href="#amend-61"><span class="linenos">61</span></a>
-</span><span id="amend-62"><a href="#amend-62"><span class="linenos">62</span></a><span class="sd">    If `files` is `None`, all files will be staged.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="amend-61"><a href="#amend-61"><span class="linenos">61</span></a><span class="k">def</span> <span class="nf">amend</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="amend-62"><a href="#amend-62"><span class="linenos">62</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
 </span><span id="amend-63"><a href="#amend-63"><span class="linenos">63</span></a>
-</span><span id="amend-64"><a href="#amend-64"><span class="linenos">64</span></a><span class="sd">    Equivalent to:</span>
-</span><span id="amend-65"><a href="#amend-65"><span class="linenos">65</span></a><span class="sd">    &gt;&gt;&gt; git add {files}</span>
-</span><span id="amend-66"><a href="#amend-66"><span class="linenos">66</span></a><span class="sd">    &gt;&gt;&gt; git commit --amend --no-edit</span>
-</span><span id="amend-67"><a href="#amend-67"><span class="linenos">67</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="amend-68"><a href="#amend-68"><span class="linenos">68</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
-</span><span id="amend-69"><a href="#amend-69"><span class="linenos">69</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>
+</span><span id="amend-64"><a href="#amend-64"><span class="linenos">64</span></a><span class="sd">    If `files` is `None`, all files will be staged.</span>
+</span><span id="amend-65"><a href="#amend-65"><span class="linenos">65</span></a>
+</span><span id="amend-66"><a href="#amend-66"><span class="linenos">66</span></a><span class="sd">    Equivalent to:</span>
+</span><span id="amend-67"><a href="#amend-67"><span class="linenos">67</span></a><span class="sd">    &gt;&gt;&gt; git add {files}</span>
+</span><span id="amend-68"><a href="#amend-68"><span class="linenos">68</span></a><span class="sd">    &gt;&gt;&gt; git commit --amend --no-edit</span>
+</span><span id="amend-69"><a href="#amend-69"><span class="linenos">69</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="amend-70"><a href="#amend-70"><span class="linenos">70</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
+</span><span id="amend-71"><a href="#amend-71"><span class="linenos">71</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit changes to the previous commit.</p>
 
 <p>If <code>files</code> is <code>None</code>, all files will be staged.</p>
 
@@ -608,19 +610,19 @@
         <span class="def">def</span>
         <span class="name">tag</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">id_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="tag-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#tag"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="tag-72"><a href="#tag-72"><span class="linenos">72</span></a><span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="n">id_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="tag-73"><a href="#tag-73"><span class="linenos">73</span></a>    <span class="sd">&quot;&quot;&quot;Tag the current commit with `id_`.</span>
-</span><span id="tag-74"><a href="#tag-74"><span class="linenos">74</span></a>
-</span><span id="tag-75"><a href="#tag-75"><span class="linenos">75</span></a><span class="sd">    Equivalent to `git tag {id_}`.&quot;&quot;&quot;</span>
-</span><span id="tag-76"><a href="#tag-76"><span class="linenos">76</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">id_</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="tag-74"><a href="#tag-74"><span class="linenos">74</span></a><span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="n">id_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="tag-75"><a href="#tag-75"><span class="linenos">75</span></a>    <span class="sd">&quot;&quot;&quot;Tag the current commit with `id_`.</span>
+</span><span id="tag-76"><a href="#tag-76"><span class="linenos">76</span></a>
+</span><span id="tag-77"><a href="#tag-77"><span class="linenos">77</span></a><span class="sd">    Equivalent to `git tag {id_}`.&quot;&quot;&quot;</span>
+</span><span id="tag-78"><a href="#tag-78"><span class="linenos">78</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">id_</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Tag the current commit with <code>id_</code>.</p>
 
 <p>Equivalent to <code>git tag {id_}</code>.</p>
 </div>
@@ -634,17 +636,17 @@
         <span class="def">def</span>
         <span class="name">add_remote_url</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">url</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;origin&#39;</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="add_remote_url-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#add_remote_url"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="add_remote_url-80"><a href="#add_remote_url-80"><span class="linenos">80</span></a><span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">):</span>
-</span><span id="add_remote_url-81"><a href="#add_remote_url-81"><span class="linenos">81</span></a>    <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
-</span><span id="add_remote_url-82"><a href="#add_remote_url-82"><span class="linenos">82</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="add_remote_url-82"><a href="#add_remote_url-82"><span class="linenos">82</span></a><span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">):</span>
+</span><span id="add_remote_url-83"><a href="#add_remote_url-83"><span class="linenos">83</span></a>    <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
+</span><span id="add_remote_url-84"><a href="#add_remote_url-84"><span class="linenos">84</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add remote url to repo.</p>
 </div>
 
 
@@ -656,17 +658,17 @@
         <span class="def">def</span>
         <span class="name">push</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="push-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#push"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="push-85"><a href="#push-85"><span class="linenos">85</span></a><span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
-</span><span id="push-86"><a href="#push-86"><span class="linenos">86</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
-</span><span id="push-87"><a href="#push-87"><span class="linenos">87</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="push-87"><a href="#push-87"><span class="linenos">87</span></a><span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
+</span><span id="push-88"><a href="#push-88"><span class="linenos">88</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
+</span><span id="push-89"><a href="#push-89"><span class="linenos">89</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git push {args}</code>.</p>
 </div>
 
 
@@ -678,17 +680,17 @@
         <span class="def">def</span>
         <span class="name">pull</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="pull-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#pull"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="pull-90"><a href="#pull-90"><span class="linenos">90</span></a><span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
-</span><span id="pull-91"><a href="#pull-91"><span class="linenos">91</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
-</span><span id="pull-92"><a href="#pull-92"><span class="linenos">92</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="pull-92"><a href="#pull-92"><span class="linenos">92</span></a><span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
+</span><span id="pull-93"><a href="#pull-93"><span class="linenos">93</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
+</span><span id="pull-94"><a href="#pull-94"><span class="linenos">94</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git pull {args}</code>.</p>
 </div>
 
 
@@ -700,19 +702,19 @@
         <span class="def">def</span>
         <span class="name">push_new_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="push_new_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#push_new_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="push_new_branch-95"><a href="#push_new_branch-95"><span class="linenos">95</span></a><span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="push_new_branch-96"><a href="#push_new_branch-96"><span class="linenos">96</span></a>    <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
-</span><span id="push_new_branch-97"><a href="#push_new_branch-97"><span class="linenos">97</span></a>
-</span><span id="push_new_branch-98"><a href="#push_new_branch-98"><span class="linenos">98</span></a><span class="sd">    Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
-</span><span id="push_new_branch-99"><a href="#push_new_branch-99"><span class="linenos">99</span></a>    <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="push_new_branch-97"><a href="#push_new_branch-97"><span class="linenos"> 97</span></a><span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="push_new_branch-98"><a href="#push_new_branch-98"><span class="linenos"> 98</span></a>    <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
+</span><span id="push_new_branch-99"><a href="#push_new_branch-99"><span class="linenos"> 99</span></a>
+</span><span id="push_new_branch-100"><a href="#push_new_branch-100"><span class="linenos">100</span></a><span class="sd">    Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
+</span><span id="push_new_branch-101"><a href="#push_new_branch-101"><span class="linenos">101</span></a>    <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Push a new branch to origin with tracking.</p>
 
 <p>Equivalent to <code>git push -u origin {branch}</code>.</p>
 </div>
@@ -726,17 +728,17 @@
         <span class="def">def</span>
         <span class="name">pull_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="pull_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#pull_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="pull_branch-102"><a href="#pull_branch-102"><span class="linenos">102</span></a><span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="pull_branch-103"><a href="#pull_branch-103"><span class="linenos">103</span></a>    <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
-</span><span id="pull_branch-104"><a href="#pull_branch-104"><span class="linenos">104</span></a>    <span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="pull_branch-104"><a href="#pull_branch-104"><span class="linenos">104</span></a><span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="pull_branch-105"><a href="#pull_branch-105"><span class="linenos">105</span></a>    <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
+</span><span id="pull_branch-106"><a href="#pull_branch-106"><span class="linenos">106</span></a>    <span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Pull <code><a href="#branch">branch</a></code> from origin.</p>
 </div>
 
 
@@ -748,17 +750,17 @@
         <span class="def">def</span>
         <span class="name">branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="branch-108"><a href="#branch-108"><span class="linenos">108</span></a><span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="branch-109"><a href="#branch-109"><span class="linenos">109</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
-</span><span id="branch-110"><a href="#branch-110"><span class="linenos">110</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="branch-110"><a href="#branch-110"><span class="linenos">110</span></a><span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="branch-111"><a href="#branch-111"><span class="linenos">111</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
+</span><span id="branch-112"><a href="#branch-112"><span class="linenos">112</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git branch {args}</code>.</p>
 </div>
 
 
@@ -770,17 +772,17 @@
         <span class="def">def</span>
         <span class="name">list_branches</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="list_branches-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#list_branches"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="list_branches-113"><a href="#list_branches-113"><span class="linenos">113</span></a><span class="k">def</span> <span class="nf">list_branches</span><span class="p">():</span>
-</span><span id="list_branches-114"><a href="#list_branches-114"><span class="linenos">114</span></a>    <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
-</span><span id="list_branches-115"><a href="#list_branches-115"><span class="linenos">115</span></a>    <span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="list_branches-115"><a href="#list_branches-115"><span class="linenos">115</span></a><span class="k">def</span> <span class="nf">list_branches</span><span class="p">():</span>
+</span><span id="list_branches-116"><a href="#list_branches-116"><span class="linenos">116</span></a>    <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
+</span><span id="list_branches-117"><a href="#list_branches-117"><span class="linenos">117</span></a>    <span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Print a list of branches.</p>
 </div>
 
 
@@ -792,17 +794,17 @@
         <span class="def">def</span>
         <span class="name">checkout</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="checkout-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#checkout"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="checkout-118"><a href="#checkout-118"><span class="linenos">118</span></a><span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="checkout-119"><a href="#checkout-119"><span class="linenos">119</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
-</span><span id="checkout-120"><a href="#checkout-120"><span class="linenos">120</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="checkout-120"><a href="#checkout-120"><span class="linenos">120</span></a><span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="checkout-121"><a href="#checkout-121"><span class="linenos">121</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
+</span><span id="checkout-122"><a href="#checkout-122"><span class="linenos">122</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git checkout {args}</code>.</p>
 </div>
 
 
@@ -814,19 +816,19 @@
         <span class="def">def</span>
         <span class="name">switch_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="switch_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#switch_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="switch_branch-123"><a href="#switch_branch-123"><span class="linenos">123</span></a><span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="switch_branch-124"><a href="#switch_branch-124"><span class="linenos">124</span></a>    <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
-</span><span id="switch_branch-125"><a href="#switch_branch-125"><span class="linenos">125</span></a>
-</span><span id="switch_branch-126"><a href="#switch_branch-126"><span class="linenos">126</span></a><span class="sd">    Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
-</span><span id="switch_branch-127"><a href="#switch_branch-127"><span class="linenos">127</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="switch_branch-125"><a href="#switch_branch-125"><span class="linenos">125</span></a><span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="switch_branch-126"><a href="#switch_branch-126"><span class="linenos">126</span></a>    <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
+</span><span id="switch_branch-127"><a href="#switch_branch-127"><span class="linenos">127</span></a>
+</span><span id="switch_branch-128"><a href="#switch_branch-128"><span class="linenos">128</span></a><span class="sd">    Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
+</span><span id="switch_branch-129"><a href="#switch_branch-129"><span class="linenos">129</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Switch to the branch specified by <code>branch_name</code>.</p>
 
 <p>Equivalent to <code>git checkout {branch_name}</code>.</p>
 </div>
@@ -840,19 +842,19 @@
         <span class="def">def</span>
         <span class="name">create_new_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_new_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_new_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_new_branch-130"><a href="#create_new_branch-130"><span class="linenos">130</span></a><span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="create_new_branch-131"><a href="#create_new_branch-131"><span class="linenos">131</span></a>    <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
-</span><span id="create_new_branch-132"><a href="#create_new_branch-132"><span class="linenos">132</span></a>
-</span><span id="create_new_branch-133"><a href="#create_new_branch-133"><span class="linenos">133</span></a><span class="sd">    Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
-</span><span id="create_new_branch-134"><a href="#create_new_branch-134"><span class="linenos">134</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_new_branch-132"><a href="#create_new_branch-132"><span class="linenos">132</span></a><span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="create_new_branch-133"><a href="#create_new_branch-133"><span class="linenos">133</span></a>    <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
+</span><span id="create_new_branch-134"><a href="#create_new_branch-134"><span class="linenos">134</span></a>
+</span><span id="create_new_branch-135"><a href="#create_new_branch-135"><span class="linenos">135</span></a><span class="sd">    Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
+</span><span id="create_new_branch-136"><a href="#create_new_branch-136"><span class="linenos">136</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create and switch to a new branch named with <code>branch_name</code>.</p>
 
 <p>Equivalent to <code>git checkout -b {branch_name} --track</code>.</p>
 </div>
@@ -866,23 +868,23 @@
         <span class="def">def</span>
         <span class="name">delete_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="delete_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#delete_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_branch-137"><a href="#delete_branch-137"><span class="linenos">137</span></a><span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="delete_branch-138"><a href="#delete_branch-138"><span class="linenos">138</span></a>    <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
-</span><span id="delete_branch-139"><a href="#delete_branch-139"><span class="linenos">139</span></a>
-</span><span id="delete_branch-140"><a href="#delete_branch-140"><span class="linenos">140</span></a><span class="sd">    #### :params:</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_branch-139"><a href="#delete_branch-139"><span class="linenos">139</span></a><span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="delete_branch-140"><a href="#delete_branch-140"><span class="linenos">140</span></a>    <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
 </span><span id="delete_branch-141"><a href="#delete_branch-141"><span class="linenos">141</span></a>
-</span><span id="delete_branch-142"><a href="#delete_branch-142"><span class="linenos">142</span></a><span class="sd">    `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
-</span><span id="delete_branch-143"><a href="#delete_branch-143"><span class="linenos">143</span></a>    <span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="delete_branch-144"><a href="#delete_branch-144"><span class="linenos">144</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
-</span><span id="delete_branch-145"><a href="#delete_branch-145"><span class="linenos">145</span></a>        <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="delete_branch-142"><a href="#delete_branch-142"><span class="linenos">142</span></a><span class="sd">    #### :params:</span>
+</span><span id="delete_branch-143"><a href="#delete_branch-143"><span class="linenos">143</span></a>
+</span><span id="delete_branch-144"><a href="#delete_branch-144"><span class="linenos">144</span></a><span class="sd">    `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
+</span><span id="delete_branch-145"><a href="#delete_branch-145"><span class="linenos">145</span></a>    <span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="delete_branch-146"><a href="#delete_branch-146"><span class="linenos">146</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
+</span><span id="delete_branch-147"><a href="#delete_branch-147"><span class="linenos">147</span></a>        <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete <code>branch_name</code> from repo.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -898,19 +900,19 @@
         <span class="def">def</span>
         <span class="name">undo</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="undo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#undo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="undo-148"><a href="#undo-148"><span class="linenos">148</span></a><span class="k">def</span> <span class="nf">undo</span><span class="p">():</span>
-</span><span id="undo-149"><a href="#undo-149"><span class="linenos">149</span></a>    <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
-</span><span id="undo-150"><a href="#undo-150"><span class="linenos">150</span></a>
-</span><span id="undo-151"><a href="#undo-151"><span class="linenos">151</span></a><span class="sd">    Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
-</span><span id="undo-152"><a href="#undo-152"><span class="linenos">152</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="undo-150"><a href="#undo-150"><span class="linenos">150</span></a><span class="k">def</span> <span class="nf">undo</span><span class="p">():</span>
+</span><span id="undo-151"><a href="#undo-151"><span class="linenos">151</span></a>    <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
+</span><span id="undo-152"><a href="#undo-152"><span class="linenos">152</span></a>
+</span><span id="undo-153"><a href="#undo-153"><span class="linenos">153</span></a><span class="sd">    Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
+</span><span id="undo-154"><a href="#undo-154"><span class="linenos">154</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Undo uncommitted changes.</p>
 
 <p>Equivalent to <code>git checkout .</code>.</p>
 </div>
@@ -924,17 +926,17 @@
         <span class="def">def</span>
         <span class="name">merge</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="merge-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#merge"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="merge-155"><a href="#merge-155"><span class="linenos">155</span></a><span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="merge-156"><a href="#merge-156"><span class="linenos">156</span></a>    <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
-</span><span id="merge-157"><a href="#merge-157"><span class="linenos">157</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="merge-157"><a href="#merge-157"><span class="linenos">157</span></a><span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="merge-158"><a href="#merge-158"><span class="linenos">158</span></a>    <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
+</span><span id="merge-159"><a href="#merge-159"><span class="linenos">159</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Merge branch <code>branch_name</code> with currently active branch.</p>
 </div>
 
 
@@ -946,24 +948,24 @@
         <span class="def">def</span>
         <span class="name">create_remote</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_remote-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_remote"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_remote-163"><a href="#create_remote-163"><span class="linenos">163</span></a><span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
-</span><span id="create_remote-164"><a href="#create_remote-164"><span class="linenos">164</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
-</span><span id="create_remote-165"><a href="#create_remote-165"><span class="linenos">165</span></a>
-</span><span id="create_remote-166"><a href="#create_remote-166"><span class="linenos">166</span></a><span class="sd">    #### :params:</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_remote-165"><a href="#create_remote-165"><span class="linenos">165</span></a><span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
+</span><span id="create_remote-166"><a href="#create_remote-166"><span class="linenos">166</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
 </span><span id="create_remote-167"><a href="#create_remote-167"><span class="linenos">167</span></a>
-</span><span id="create_remote-168"><a href="#create_remote-168"><span class="linenos">168</span></a><span class="sd">    `name`: The name for the repo.</span>
+</span><span id="create_remote-168"><a href="#create_remote-168"><span class="linenos">168</span></a><span class="sd">    #### :params:</span>
 </span><span id="create_remote-169"><a href="#create_remote-169"><span class="linenos">169</span></a>
-</span><span id="create_remote-170"><a href="#create_remote-170"><span class="linenos">170</span></a><span class="sd">    `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
-</span><span id="create_remote-171"><a href="#create_remote-171"><span class="linenos">171</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
-</span><span id="create_remote-172"><a href="#create_remote-172"><span class="linenos">172</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="create_remote-170"><a href="#create_remote-170"><span class="linenos">170</span></a><span class="sd">    `name`: The name for the repo.</span>
+</span><span id="create_remote-171"><a href="#create_remote-171"><span class="linenos">171</span></a>
+</span><span id="create_remote-172"><a href="#create_remote-172"><span class="linenos">172</span></a><span class="sd">    `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
+</span><span id="create_remote-173"><a href="#create_remote-173"><span class="linenos">173</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
+</span><span id="create_remote-174"><a href="#create_remote-174"><span class="linenos">174</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -981,23 +983,23 @@
         <span class="def">def</span>
         <span class="name">create_remote_from_cwd</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_remote_from_cwd-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_remote_from_cwd"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_remote_from_cwd-175"><a href="#create_remote_from_cwd-175"><span class="linenos">175</span></a><span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
-</span><span id="create_remote_from_cwd-176"><a href="#create_remote_from_cwd-176"><span class="linenos">176</span></a>    <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
-</span><span id="create_remote_from_cwd-177"><a href="#create_remote_from_cwd-177"><span class="linenos">177</span></a><span class="sd">    the current working directory repo and add its url as this repo&#39;s remote origin.</span>
-</span><span id="create_remote_from_cwd-178"><a href="#create_remote_from_cwd-178"><span class="linenos">178</span></a>
-</span><span id="create_remote_from_cwd-179"><a href="#create_remote_from_cwd-179"><span class="linenos">179</span></a><span class="sd">    #### :params:</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_remote_from_cwd-177"><a href="#create_remote_from_cwd-177"><span class="linenos">177</span></a><span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
+</span><span id="create_remote_from_cwd-178"><a href="#create_remote_from_cwd-178"><span class="linenos">178</span></a>    <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
+</span><span id="create_remote_from_cwd-179"><a href="#create_remote_from_cwd-179"><span class="linenos">179</span></a><span class="sd">    the current working directory repo and add its url as this repo&#39;s remote origin.</span>
 </span><span id="create_remote_from_cwd-180"><a href="#create_remote_from_cwd-180"><span class="linenos">180</span></a>
-</span><span id="create_remote_from_cwd-181"><a href="#create_remote_from_cwd-181"><span class="linenos">181</span></a><span class="sd">    `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
-</span><span id="create_remote_from_cwd-182"><a href="#create_remote_from_cwd-182"><span class="linenos">182</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
-</span><span id="create_remote_from_cwd-183"><a href="#create_remote_from_cwd-183"><span class="linenos">183</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create --source=. --remote=upstream --</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="create_remote_from_cwd-181"><a href="#create_remote_from_cwd-181"><span class="linenos">181</span></a><span class="sd">    #### :params:</span>
+</span><span id="create_remote_from_cwd-182"><a href="#create_remote_from_cwd-182"><span class="linenos">182</span></a>
+</span><span id="create_remote_from_cwd-183"><a href="#create_remote_from_cwd-183"><span class="linenos">183</span></a><span class="sd">    `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
+</span><span id="create_remote_from_cwd-184"><a href="#create_remote_from_cwd-184"><span class="linenos">184</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
+</span><span id="create_remote_from_cwd-185"><a href="#create_remote_from_cwd-185"><span class="linenos">185</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create --source . --</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2"> --push&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from
 the current working directory repo and add its url as this repo's remote origin.</p>
 
 <h4 id="params">:params:</h4>
@@ -1014,23 +1016,23 @@
         <span class="def">def</span>
         <span class="name">make_private</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="make_private-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#make_private"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="make_private-186"><a href="#make_private-186"><span class="linenos">186</span></a><span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="make_private-187"><a href="#make_private-187"><span class="linenos">187</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
-</span><span id="make_private-188"><a href="#make_private-188"><span class="linenos">188</span></a>
-</span><span id="make_private-189"><a href="#make_private-189"><span class="linenos">189</span></a><span class="sd">    #### :params:</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="make_private-188"><a href="#make_private-188"><span class="linenos">188</span></a><span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="make_private-189"><a href="#make_private-189"><span class="linenos">189</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
 </span><span id="make_private-190"><a href="#make_private-190"><span class="linenos">190</span></a>
-</span><span id="make_private-191"><a href="#make_private-191"><span class="linenos">191</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="make_private-191"><a href="#make_private-191"><span class="linenos">191</span></a><span class="sd">    #### :params:</span>
 </span><span id="make_private-192"><a href="#make_private-192"><span class="linenos">192</span></a>
-</span><span id="make_private-193"><a href="#make_private-193"><span class="linenos">193</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="make_private-194"><a href="#make_private-194"><span class="linenos">194</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility private&quot;</span><span class="p">)</span>
+</span><span id="make_private-193"><a href="#make_private-193"><span class="linenos">193</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="make_private-194"><a href="#make_private-194"><span class="linenos">194</span></a>
+</span><span id="make_private-195"><a href="#make_private-195"><span class="linenos">195</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="make_private-196"><a href="#make_private-196"><span class="linenos">196</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility private&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be installed and configured) to set the repo's visibility to private.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1048,23 +1050,23 @@
         <span class="def">def</span>
         <span class="name">make_public</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="make_public-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#make_public"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="make_public-197"><a href="#make_public-197"><span class="linenos">197</span></a><span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="make_public-198"><a href="#make_public-198"><span class="linenos">198</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
-</span><span id="make_public-199"><a href="#make_public-199"><span class="linenos">199</span></a>
-</span><span id="make_public-200"><a href="#make_public-200"><span class="linenos">200</span></a><span class="sd">    #### :params:</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="make_public-199"><a href="#make_public-199"><span class="linenos">199</span></a><span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="make_public-200"><a href="#make_public-200"><span class="linenos">200</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
 </span><span id="make_public-201"><a href="#make_public-201"><span class="linenos">201</span></a>
-</span><span id="make_public-202"><a href="#make_public-202"><span class="linenos">202</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="make_public-202"><a href="#make_public-202"><span class="linenos">202</span></a><span class="sd">    #### :params:</span>
 </span><span id="make_public-203"><a href="#make_public-203"><span class="linenos">203</span></a>
-</span><span id="make_public-204"><a href="#make_public-204"><span class="linenos">204</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="make_public-205"><a href="#make_public-205"><span class="linenos">205</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility public&quot;</span><span class="p">)</span>
+</span><span id="make_public-204"><a href="#make_public-204"><span class="linenos">204</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="make_public-205"><a href="#make_public-205"><span class="linenos">205</span></a>
+</span><span id="make_public-206"><a href="#make_public-206"><span class="linenos">206</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="make_public-207"><a href="#make_public-207"><span class="linenos">207</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility public&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be installed and configured) to set the repo's visibility to public.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1082,23 +1084,23 @@
         <span class="def">def</span>
         <span class="name">delete_remote</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="delete_remote-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#delete_remote"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_remote-208"><a href="#delete_remote-208"><span class="linenos">208</span></a><span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="delete_remote-209"><a href="#delete_remote-209"><span class="linenos">209</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
-</span><span id="delete_remote-210"><a href="#delete_remote-210"><span class="linenos">210</span></a>
-</span><span id="delete_remote-211"><a href="#delete_remote-211"><span class="linenos">211</span></a><span class="sd">    #### :params:</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_remote-210"><a href="#delete_remote-210"><span class="linenos">210</span></a><span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="delete_remote-211"><a href="#delete_remote-211"><span class="linenos">211</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
 </span><span id="delete_remote-212"><a href="#delete_remote-212"><span class="linenos">212</span></a>
-</span><span id="delete_remote-213"><a href="#delete_remote-213"><span class="linenos">213</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="delete_remote-213"><a href="#delete_remote-213"><span class="linenos">213</span></a><span class="sd">    #### :params:</span>
 </span><span id="delete_remote-214"><a href="#delete_remote-214"><span class="linenos">214</span></a>
-</span><span id="delete_remote-215"><a href="#delete_remote-215"><span class="linenos">215</span></a><span class="sd">    `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
-</span><span id="delete_remote-216"><a href="#delete_remote-216"><span class="linenos">216</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo delete </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --yes&quot;</span><span class="p">)</span>
+</span><span id="delete_remote-215"><a href="#delete_remote-215"><span class="linenos">215</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="delete_remote-216"><a href="#delete_remote-216"><span class="linenos">216</span></a>
+</span><span id="delete_remote-217"><a href="#delete_remote-217"><span class="linenos">217</span></a><span class="sd">    `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
+</span><span id="delete_remote-218"><a href="#delete_remote-218"><span class="linenos">218</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo delete </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --yes&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</p>
 
 <h4 id="params">:params:</h4>
```

#### html2text {}

```diff
@@ -33,520 +33,522 @@
     * delete_remote
 built_with_pdoc[pdoc_logo]
 
 ****** gitbetter.git ******
 ⁰ View Source
 __1import os
 __2
-__3
-__4def execute(command: str) -> int:
-__5    """Execute git command.
-__6
-__7    Equivalent to `os.system(f"git {command}")`
+__3from pathier import Pathier
+__4
+__5
+__6def execute(command: str) -> int:
+__7    """Execute git command.
 __8
-__9    Returns the output of the `os.system` call."""
-_10    return os.system(f"git {command}")
-_11
-_12
-_13def new_repo():
-_14    """>>> git init -b main"""
-_15    execute("init -b main")
-_16
-_17
-_18def loggy():
-_19    """Equivalent to `git log --oneline --name-only --abbrev-commit --
+__9    Equivalent to `os.system(f"git {command}")`
+_10
+_11    Returns the output of the `os.system` call."""
+_12    return os.system(f"git {command}")
+_13
+_14
+_15def new_repo():
+_16    """>>> git init -b main"""
+_17    execute("init -b main")
+_18
+_19
+_20def loggy():
+_21    """Equivalent to `git log --oneline --name-only --abbrev-commit --
 graph`."""
-_20    execute("log --oneline --name-only --abbrev-commit --graph")
-_21
-_22
-_23def status():
-_24    """Execute `git status`."""
-_25    execute("status")
-_26
-_27
-_28# ======================================Staging/
+_22    execute("log --oneline --name-only --abbrev-commit --graph")
+_23
+_24
+_25def status():
+_26    """Execute `git status`."""
+_27    execute("status")
+_28
+_29
+_30# ======================================Staging/
 Committing======================================
-_29def commit(args: str):
-_30    """>>> git commit {args}"""
-_31    execute(f"commit {args}")
-_32
-_33
-_34def add(files: list[str] | None = None):
-_35    """Stage a list of files.
-_36
-_37    If no files are given (`files=None`), all files will be staged."""
-_38    if not files:
-_39        execute("add .")
-_40    else:
-_41        execute(f'add {" ".join(files)}')
-_42
-_43
-_44def commit_files(files: list[str], message: str):
-_45    """Stage and commit a list of files with commit message `message`."""
-_46    add(files)
-_47    commit(f'-m "{message}"')
-_48
-_49
-_50def initcommit():
-_51    """Equivalent to
-_52    >>> git add .
-_53    >>> git commit -m "Initial commit" """
-_54    add()
-_55    commit('-m "Initial commit"')
-_56
-_57
-_58def amend(files: list[str] | None = None):
-_59    """Stage and commit changes to the previous commit.
-_60
-_61    If `files` is `None`, all files will be staged.
+_31def commit(args: str):
+_32    """>>> git commit {args}"""
+_33    execute(f"commit {args}")
+_34
+_35
+_36def add(files: list[str] | None = None):
+_37    """Stage a list of files.
+_38
+_39    If no files are given (`files=None`), all files will be staged."""
+_40    if not files:
+_41        execute("add .")
+_42    else:
+_43        execute(f'add {" ".join(files)}')
+_44
+_45
+_46def commit_files(files: list[str], message: str):
+_47    """Stage and commit a list of files with commit message `message`."""
+_48    add(files)
+_49    commit(f'-m "{message}"')
+_50
+_51
+_52def initcommit():
+_53    """Equivalent to
+_54    >>> git add .
+_55    >>> git commit -m "Initial commit" """
+_56    add()
+_57    commit('-m "Initial commit"')
+_58
+_59
+_60def amend(files: list[str] | None = None):
+_61    """Stage and commit changes to the previous commit.
 _62
-_63    Equivalent to:
-_64    >>> git add {files}
-_65    >>> git commit --amend --no-edit
-_66    """
-_67    add(files)
-_68    commit("--amend --no-edit")
-_69
-_70
-_71def tag(id_: str):
-_72    """Tag the current commit with `id_`.
-_73
-_74    Equivalent to `git tag {id_}`."""
-_75    execute(f"tag {id_}")
-_76
-_77
-_78# ==========================================Push/
+_63    If `files` is `None`, all files will be staged.
+_64
+_65    Equivalent to:
+_66    >>> git add {files}
+_67    >>> git commit --amend --no-edit
+_68    """
+_69    add(files)
+_70    commit("--amend --no-edit")
+_71
+_72
+_73def tag(id_: str):
+_74    """Tag the current commit with `id_`.
+_75
+_76    Equivalent to `git tag {id_}`."""
+_77    execute(f"tag {id_}")
+_78
+_79
+_80# ==========================================Push/
 Pull==========================================
-_79def add_remote_url(url: str, name: str = "origin"):
-_80    """Add remote url to repo."""
-_81    execute(f"remote add {name} {url}")
-_82
-_83
-_84def push(args: str = ""):
-_85    """Equivalent to `git push {args}`."""
-_86    execute(f"push {args}")
-_87
-_88
-_89def pull(args: str = ""):
-_90    """Equivalent to `git pull {args}`."""
-_91    execute(f"pull {args}")
-_92
-_93
-_94def push_new_branch(branch: str):
-_95    """Push a new branch to origin with tracking.
-_96
-_97    Equivalent to `git push -u origin {branch}`."""
-_98    push(f"-u origin {branch}")
-_99
-100
-101def pull_branch(branch: str):
-102    """Pull `branch` from origin."""
-103    pull(f"origin {branch}")
-104
-105
-106# ============================================Checkout/
+_81def add_remote_url(url: str, name: str = "origin"):
+_82    """Add remote url to repo."""
+_83    execute(f"remote add {name} {url}")
+_84
+_85
+_86def push(args: str = ""):
+_87    """Equivalent to `git push {args}`."""
+_88    execute(f"push {args}")
+_89
+_90
+_91def pull(args: str = ""):
+_92    """Equivalent to `git pull {args}`."""
+_93    execute(f"pull {args}")
+_94
+_95
+_96def push_new_branch(branch: str):
+_97    """Push a new branch to origin with tracking.
+_98
+_99    Equivalent to `git push -u origin {branch}`."""
+100    push(f"-u origin {branch}")
+101
+102
+103def pull_branch(branch: str):
+104    """Pull `branch` from origin."""
+105    pull(f"origin {branch}")
+106
+107
+108# ============================================Checkout/
 Branches============================================
-107def branch(args: str):
-108    """Equivalent to `git branch {args}`."""
-109    execute(f"branch {args}")
-110
-111
-112def list_branches():
-113    """Print a list of branches."""
-114    branch("-vva")
-115
-116
-117def checkout(args: str):
-118    """Equivalent to `git checkout {args}`."""
-119    execute(f"checkout {args}")
-120
-121
-122def switch_branch(branch_name: str):
-123    """Switch to the branch specified by `branch_name`.
-124
-125    Equivalent to `git checkout {branch_name}`."""
-126    checkout(branch_name)
-127
-128
-129def create_new_branch(branch_name: str):
-130    """Create and switch to a new branch named with `branch_name`.
-131
-132    Equivalent to `git checkout -b {branch_name} --track`."""
-133    checkout(f"-b {branch_name} --track")
-134
-135
-136def delete_branch(branch_name: str, local_only: bool = True):
-137    """Delete `branch_name` from repo.
-138
-139    #### :params:
+109def branch(args: str):
+110    """Equivalent to `git branch {args}`."""
+111    execute(f"branch {args}")
+112
+113
+114def list_branches():
+115    """Print a list of branches."""
+116    branch("-vva")
+117
+118
+119def checkout(args: str):
+120    """Equivalent to `git checkout {args}`."""
+121    execute(f"checkout {args}")
+122
+123
+124def switch_branch(branch_name: str):
+125    """Switch to the branch specified by `branch_name`.
+126
+127    Equivalent to `git checkout {branch_name}`."""
+128    checkout(branch_name)
+129
+130
+131def create_new_branch(branch_name: str):
+132    """Create and switch to a new branch named with `branch_name`.
+133
+134    Equivalent to `git checkout -b {branch_name} --track`."""
+135    checkout(f"-b {branch_name} --track")
+136
+137
+138def delete_branch(branch_name: str, local_only: bool = True):
+139    """Delete `branch_name` from repo.
 140
-141    `local_only`: Only delete the local copy of `branch`, otherwise also
+141    #### :params:
+142
+143    `local_only`: Only delete the local copy of `branch`, otherwise also
 delete the remote branch on origin and remote-tracking branch."""
-142    branch(f"--delete {branch_name}")
-143    if not local_only:
-144        push(f"origin --delete {branch_name}")
-145
-146
-147def undo():
-148    """Undo uncommitted changes.
-149
-150    Equivalent to `git checkout .`."""
-151    checkout(".")
-152
-153
-154def merge(branch_name: str):
-155    """Merge branch `branch_name` with currently active branch."""
-156    execute(f"merge {branch_name}")
-157
-158
-159# ===============================Requires GitHub CLI to be installed and
-configured===============================
+144    branch(f"--delete {branch_name}")
+145    if not local_only:
+146        push(f"origin --delete {branch_name}")
+147
+148
+149def undo():
+150    """Undo uncommitted changes.
+151
+152    Equivalent to `git checkout .`."""
+153    checkout(".")
+154
+155
+156def merge(branch_name: str):
+157    """Merge branch `branch_name` with currently active branch."""
+158    execute(f"merge {branch_name}")
+159
 160
-161
-162def create_remote(name: str, public: bool = False):
-163    """Uses GitHub CLI (must be installed and configured) to create a remote
+161# ===============================Requires GitHub CLI to be installed and
+configured===============================
+162
+163
+164def create_remote(name: str, public: bool = False):
+165    """Uses GitHub CLI (must be installed and configured) to create a remote
 GitHub repo.
-164
-165    #### :params:
 166
-167    `name`: The name for the repo.
+167    #### :params:
 168
-169    `public`: Set to `True` to create the repo as public, otherwise it'll be
+169    `name`: The name for the repo.
+170
+171    `public`: Set to `True` to create the repo as public, otherwise it'll be
 created as private."""
-170    visibility = "--public" if public else "--private"
-171    os.system(f"gh repo create {name} {visibility}")
-172
-173
-174def create_remote_from_cwd(public: bool = False):
-175    """Use GitHub CLI (must be installed and configured) to create a remote
+172    visibility = "--public" if public else "--private"
+173    os.system(f"gh repo create {name} {visibility}")
+174
+175
+176def create_remote_from_cwd(public: bool = False):
+177    """Use GitHub CLI (must be installed and configured) to create a remote
 GitHub repo from
-176    the current working directory repo and add its url as this repo's remote
+178    the current working directory repo and add its url as this repo's remote
 origin.
-177
-178    #### :params:
 179
-180    `public`: Create the GitHub repo as a public repo, default is to create
+180    #### :params:
+181
+182    `public`: Create the GitHub repo as a public repo, default is to create
 it as private."""
-181    visibility = "public" if public else "private"
-182    os.system(f"gh repo create --source=. --remote=upstream --{visibility}")
-183
-184
-185def make_private(owner: str, name: str):
-186    """Uses GitHub CLI (must be installed and configured) to set the repo's
+183    visibility = "public" if public else "private"
+184    os.system(f"gh repo create --source . --{visibility} --push")
+185
+186
+187def make_private(owner: str, name: str):
+188    """Uses GitHub CLI (must be installed and configured) to set the repo's
 visibility to private.
-187
-188    #### :params:
 189
-190    `owner`: The repo owner.
+190    #### :params:
 191
-192    `name`: The name of the repo to edit."""
-193    os.system(f"gh repo edit {owner}/{name} --visibility private")
-194
-195
-196def make_public(owner: str, name: str):
-197    """Uses GitHub CLI (must be installed and configured) to set the repo's
+192    `owner`: The repo owner.
+193
+194    `name`: The name of the repo to edit."""
+195    os.system(f"gh repo edit {owner}/{name} --visibility private")
+196
+197
+198def make_public(owner: str, name: str):
+199    """Uses GitHub CLI (must be installed and configured) to set the repo's
 visibility to public.
-198
-199    #### :params:
 200
-201    `owner`: The repo owner.
+201    #### :params:
 202
-203    `name`: The name of the repo to edit."""
-204    os.system(f"gh repo edit {owner}/{name} --visibility public")
-205
-206
-207def delete_remote(owner: str, name: str):
-208    """Uses GitHub CLI (must be isntalled and configured) to delete the
+203    `owner`: The repo owner.
+204
+205    `name`: The name of the repo to edit."""
+206    os.system(f"gh repo edit {owner}/{name} --visibility public")
+207
+208
+209def delete_remote(owner: str, name: str):
+210    """Uses GitHub CLI (must be isntalled and configured) to delete the
 remote for this repo.
-209
-210    #### :params:
 211
-212    `owner`: The repo owner.
+212    #### :params:
 213
-214    `name`: The name of the remote repo to delete."""
-215    os.system(f"gh repo delete {owner}/{name} --yes")
+214    `owner`: The repo owner.
+215
+216    `name`: The name of the remote repo to delete."""
+217    os.system(f"gh repo delete {owner}/{name} --yes")
   ⁰
 def execute(command: str) -> int: View Source
-_5def execute(command: str) -> int:
-_6    """Execute git command.
-_7
-_8    Equivalent to `os.system(f"git {command}")`
+_7def execute(command: str) -> int:
+_8    """Execute git command.
 _9
-10    Returns the output of the `os.system` call."""
-11    return os.system(f"git {command}")
+10    Equivalent to `os.system(f"git {command}")`
+11
+12    Returns the output of the `os.system` call."""
+13    return os.system(f"git {command}")
 Execute git command.
 Equivalent to os.system(f"git {command}")
 Returns the output of the os.system call.
   ⁰
 def new_repo(): View Source
-14def new_repo():
-15    """>>> git init -b main"""
-16    execute("init -b main")
+16def new_repo():
+17    """>>> git init -b main"""
+18    execute("init -b main")
 >>> git init -b main
   ⁰
 def loggy(): View Source
-19def loggy():
-20    """Equivalent to `git log --oneline --name-only --abbrev-commit --
+21def loggy():
+22    """Equivalent to `git log --oneline --name-only --abbrev-commit --
 graph`."""
-21    execute("log --oneline --name-only --abbrev-commit --graph")
+23    execute("log --oneline --name-only --abbrev-commit --graph")
 Equivalent to git log --oneline --name-only --abbrev-commit --graph.
   ⁰
 def status(): View Source
-24def status():
-25    """Execute `git status`."""
-26    execute("status")
+26def status():
+27    """Execute `git status`."""
+28    execute("status")
 Execute git status.
   ⁰
 def commit(args: str): View Source
-30def commit(args: str):
-31    """>>> git commit {args}"""
-32    execute(f"commit {args}")
+32def commit(args: str):
+33    """>>> git commit {args}"""
+34    execute(f"commit {args}")
 >>> git commit {args}
   ⁰
 def add(files: list[str] | None = None): View Source
-35def add(files: list[str] | None = None):
-36    """Stage a list of files.
-37
-38    If no files are given (`files=None`), all files will be staged."""
-39    if not files:
-40        execute("add .")
-41    else:
-42        execute(f'add {" ".join(files)}')
+37def add(files: list[str] | None = None):
+38    """Stage a list of files.
+39
+40    If no files are given (`files=None`), all files will be staged."""
+41    if not files:
+42        execute("add .")
+43    else:
+44        execute(f'add {" ".join(files)}')
 Stage a list of files.
 If no files are given (files=None), all files will be staged.
   ⁰
 def commit_files(files: list[str], message: str): View Source
-45def commit_files(files: list[str], message: str):
-46    """Stage and commit a list of files with commit message `message`."""
-47    add(files)
-48    commit(f'-m "{message}"')
+47def commit_files(files: list[str], message: str):
+48    """Stage and commit a list of files with commit message `message`."""
+49    add(files)
+50    commit(f'-m "{message}"')
 Stage and commit a list of files with commit message message.
   ⁰
 def initcommit(): View Source
-51def initcommit():
-52    """Equivalent to
-53    >>> git add .
-54    >>> git commit -m "Initial commit" """
-55    add()
-56    commit('-m "Initial commit"')
+53def initcommit():
+54    """Equivalent to
+55    >>> git add .
+56    >>> git commit -m "Initial commit" """
+57    add()
+58    commit('-m "Initial commit"')
 Equivalent to
 >>> git add .
 >>> git commit -m "Initial commit"
   ⁰
 def amend(files: list[str] | None = None): View Source
-59def amend(files: list[str] | None = None):
-60    """Stage and commit changes to the previous commit.
-61
-62    If `files` is `None`, all files will be staged.
+61def amend(files: list[str] | None = None):
+62    """Stage and commit changes to the previous commit.
 63
-64    Equivalent to:
-65    >>> git add {files}
-66    >>> git commit --amend --no-edit
-67    """
-68    add(files)
-69    commit("--amend --no-edit")
+64    If `files` is `None`, all files will be staged.
+65
+66    Equivalent to:
+67    >>> git add {files}
+68    >>> git commit --amend --no-edit
+69    """
+70    add(files)
+71    commit("--amend --no-edit")
 Stage and commit changes to the previous commit.
 If files is None, all files will be staged.
 Equivalent to:
 >>> git add {files}
 >>> git commit --amend --no-edit
   ⁰
 def tag(id_: str): View Source
-72def tag(id_: str):
-73    """Tag the current commit with `id_`.
-74
-75    Equivalent to `git tag {id_}`."""
-76    execute(f"tag {id_}")
+74def tag(id_: str):
+75    """Tag the current commit with `id_`.
+76
+77    Equivalent to `git tag {id_}`."""
+78    execute(f"tag {id_}")
 Tag the current commit with id_.
 Equivalent to git tag {id_}.
   ⁰
 def add_remote_url(url: str, name: str = 'origin'): View Source
-80def add_remote_url(url: str, name: str = "origin"):
-81    """Add remote url to repo."""
-82    execute(f"remote add {name} {url}")
+82def add_remote_url(url: str, name: str = "origin"):
+83    """Add remote url to repo."""
+84    execute(f"remote add {name} {url}")
 Add remote url to repo.
   ⁰
 def push(args: str = ''): View Source
-85def push(args: str = ""):
-86    """Equivalent to `git push {args}`."""
-87    execute(f"push {args}")
+87def push(args: str = ""):
+88    """Equivalent to `git push {args}`."""
+89    execute(f"push {args}")
 Equivalent to git push {args}.
   ⁰
 def pull(args: str = ''): View Source
-90def pull(args: str = ""):
-91    """Equivalent to `git pull {args}`."""
-92    execute(f"pull {args}")
+92def pull(args: str = ""):
+93    """Equivalent to `git pull {args}`."""
+94    execute(f"pull {args}")
 Equivalent to git pull {args}.
   ⁰
 def push_new_branch(branch: str): View Source
-95def push_new_branch(branch: str):
-96    """Push a new branch to origin with tracking.
-97
-98    Equivalent to `git push -u origin {branch}`."""
-99    push(f"-u origin {branch}")
+_97def push_new_branch(branch: str):
+_98    """Push a new branch to origin with tracking.
+_99
+100    Equivalent to `git push -u origin {branch}`."""
+101    push(f"-u origin {branch}")
 Push a new branch to origin with tracking.
 Equivalent to git push -u origin {branch}.
   ⁰
 def pull_branch(branch: str): View Source
-102def pull_branch(branch: str):
-103    """Pull `branch` from origin."""
-104    pull(f"origin {branch}")
+104def pull_branch(branch: str):
+105    """Pull `branch` from origin."""
+106    pull(f"origin {branch}")
 Pull branch from origin.
   ⁰
 def branch(args: str): View Source
-108def branch(args: str):
-109    """Equivalent to `git branch {args}`."""
-110    execute(f"branch {args}")
+110def branch(args: str):
+111    """Equivalent to `git branch {args}`."""
+112    execute(f"branch {args}")
 Equivalent to git branch {args}.
   ⁰
 def list_branches(): View Source
-113def list_branches():
-114    """Print a list of branches."""
-115    branch("-vva")
+115def list_branches():
+116    """Print a list of branches."""
+117    branch("-vva")
 Print a list of branches.
   ⁰
 def checkout(args: str): View Source
-118def checkout(args: str):
-119    """Equivalent to `git checkout {args}`."""
-120    execute(f"checkout {args}")
+120def checkout(args: str):
+121    """Equivalent to `git checkout {args}`."""
+122    execute(f"checkout {args}")
 Equivalent to git checkout {args}.
   ⁰
 def switch_branch(branch_name: str): View Source
-123def switch_branch(branch_name: str):
-124    """Switch to the branch specified by `branch_name`.
-125
-126    Equivalent to `git checkout {branch_name}`."""
-127    checkout(branch_name)
+125def switch_branch(branch_name: str):
+126    """Switch to the branch specified by `branch_name`.
+127
+128    Equivalent to `git checkout {branch_name}`."""
+129    checkout(branch_name)
 Switch to the branch specified by branch_name.
 Equivalent to git checkout {branch_name}.
   ⁰
 def create_new_branch(branch_name: str): View Source
-130def create_new_branch(branch_name: str):
-131    """Create and switch to a new branch named with `branch_name`.
-132
-133    Equivalent to `git checkout -b {branch_name} --track`."""
-134    checkout(f"-b {branch_name} --track")
+132def create_new_branch(branch_name: str):
+133    """Create and switch to a new branch named with `branch_name`.
+134
+135    Equivalent to `git checkout -b {branch_name} --track`."""
+136    checkout(f"-b {branch_name} --track")
 Create and switch to a new branch named with branch_name.
 Equivalent to git checkout -b {branch_name} --track.
   ⁰
 def delete_branch(branch_name: str, local_only: bool = True): View Source
-137def delete_branch(branch_name: str, local_only: bool = True):
-138    """Delete `branch_name` from repo.
-139
-140    #### :params:
+139def delete_branch(branch_name: str, local_only: bool = True):
+140    """Delete `branch_name` from repo.
 141
-142    `local_only`: Only delete the local copy of `branch`, otherwise also
+142    #### :params:
+143
+144    `local_only`: Only delete the local copy of `branch`, otherwise also
 delete the remote branch on origin and remote-tracking branch."""
-143    branch(f"--delete {branch_name}")
-144    if not local_only:
-145        push(f"origin --delete {branch_name}")
+145    branch(f"--delete {branch_name}")
+146    if not local_only:
+147        push(f"origin --delete {branch_name}")
 Delete branch_name from repo.
 *** :params: ***
 local_only: Only delete the local copy of branch, otherwise also delete the
 remote branch on origin and remote-tracking branch.
   ⁰
 def undo(): View Source
-148def undo():
-149    """Undo uncommitted changes.
-150
-151    Equivalent to `git checkout .`."""
-152    checkout(".")
+150def undo():
+151    """Undo uncommitted changes.
+152
+153    Equivalent to `git checkout .`."""
+154    checkout(".")
 Undo uncommitted changes.
 Equivalent to git checkout ..
   ⁰
 def merge(branch_name: str): View Source
-155def merge(branch_name: str):
-156    """Merge branch `branch_name` with currently active branch."""
-157    execute(f"merge {branch_name}")
+157def merge(branch_name: str):
+158    """Merge branch `branch_name` with currently active branch."""
+159    execute(f"merge {branch_name}")
 Merge branch branch_name with currently active branch.
   ⁰
 def create_remote(name: str, public: bool = False): View Source
-163def create_remote(name: str, public: bool = False):
-164    """Uses GitHub CLI (must be installed and configured) to create a remote
+165def create_remote(name: str, public: bool = False):
+166    """Uses GitHub CLI (must be installed and configured) to create a remote
 GitHub repo.
-165
-166    #### :params:
 167
-168    `name`: The name for the repo.
+168    #### :params:
 169
-170    `public`: Set to `True` to create the repo as public, otherwise it'll be
+170    `name`: The name for the repo.
+171
+172    `public`: Set to `True` to create the repo as public, otherwise it'll be
 created as private."""
-171    visibility = "--public" if public else "--private"
-172    os.system(f"gh repo create {name} {visibility}")
+173    visibility = "--public" if public else "--private"
+174    os.system(f"gh repo create {name} {visibility}")
 Uses GitHub CLI (must be installed and configured) to create a remote GitHub
 repo.
 *** :params: ***
 name: The name for the repo.
 public: Set to True to create the repo as public, otherwise it'll be created as
 private.
   ⁰
 def create_remote_from_cwd(public: bool = False): View Source
-175def create_remote_from_cwd(public: bool = False):
-176    """Use GitHub CLI (must be installed and configured) to create a remote
+177def create_remote_from_cwd(public: bool = False):
+178    """Use GitHub CLI (must be installed and configured) to create a remote
 GitHub repo from
-177    the current working directory repo and add its url as this repo's remote
+179    the current working directory repo and add its url as this repo's remote
 origin.
-178
-179    #### :params:
 180
-181    `public`: Create the GitHub repo as a public repo, default is to create
+181    #### :params:
+182
+183    `public`: Create the GitHub repo as a public repo, default is to create
 it as private."""
-182    visibility = "public" if public else "private"
-183    os.system(f"gh repo create --source=. --remote=upstream --{visibility}")
+184    visibility = "public" if public else "private"
+185    os.system(f"gh repo create --source . --{visibility} --push")
 Use GitHub CLI (must be installed and configured) to create a remote GitHub
 repo from the current working directory repo and add its url as this repo's
 remote origin.
 *** :params: ***
 public: Create the GitHub repo as a public repo, default is to create it as
 private.
   ⁰
 def make_private(owner: str, name: str): View Source
-186def make_private(owner: str, name: str):
-187    """Uses GitHub CLI (must be installed and configured) to set the repo's
+188def make_private(owner: str, name: str):
+189    """Uses GitHub CLI (must be installed and configured) to set the repo's
 visibility to private.
-188
-189    #### :params:
 190
-191    `owner`: The repo owner.
+191    #### :params:
 192
-193    `name`: The name of the repo to edit."""
-194    os.system(f"gh repo edit {owner}/{name} --visibility private")
+193    `owner`: The repo owner.
+194
+195    `name`: The name of the repo to edit."""
+196    os.system(f"gh repo edit {owner}/{name} --visibility private")
 Uses GitHub CLI (must be installed and configured) to set the repo's visibility
 to private.
 *** :params: ***
 owner: The repo owner.
 name: The name of the repo to edit.
   ⁰
 def make_public(owner: str, name: str): View Source
-197def make_public(owner: str, name: str):
-198    """Uses GitHub CLI (must be installed and configured) to set the repo's
+199def make_public(owner: str, name: str):
+200    """Uses GitHub CLI (must be installed and configured) to set the repo's
 visibility to public.
-199
-200    #### :params:
 201
-202    `owner`: The repo owner.
+202    #### :params:
 203
-204    `name`: The name of the repo to edit."""
-205    os.system(f"gh repo edit {owner}/{name} --visibility public")
+204    `owner`: The repo owner.
+205
+206    `name`: The name of the repo to edit."""
+207    os.system(f"gh repo edit {owner}/{name} --visibility public")
 Uses GitHub CLI (must be installed and configured) to set the repo's visibility
 to public.
 *** :params: ***
 owner: The repo owner.
 name: The name of the repo to edit.
   ⁰
 def delete_remote(owner: str, name: str): View Source
-208def delete_remote(owner: str, name: str):
-209    """Uses GitHub CLI (must be isntalled and configured) to delete the
+210def delete_remote(owner: str, name: str):
+211    """Uses GitHub CLI (must be isntalled and configured) to delete the
 remote for this repo.
-210
-211    #### :params:
 212
-213    `owner`: The repo owner.
+213    #### :params:
 214
-215    `name`: The name of the remote repo to delete."""
-216    os.system(f"gh repo delete {owner}/{name} --yes")
+215    `owner`: The repo owner.
+216
+217    `name`: The name of the remote repo to delete."""
+218    os.system(f"gh repo delete {owner}/{name} --yes")
 Uses GitHub CLI (must be isntalled and configured) to delete the remote for
 this repo.
 *** :params: ***
 owner: The repo owner.
 name: The name of the remote repo to delete.
```

### Comparing `gitbetter-0.5.1/docs/gitbetter/gitbetter.html` & `gitbetter-0.5.2/docs/gitbetter/gitbetter.html`

 * *Files identical despite different names*

### Comparing `gitbetter-0.5.1/src/gitbetter/git.py` & `gitbetter-0.5.2/src/gitbetter/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 
+from pathier import Pathier
+
 
 def execute(command: str) -> int:
     """Execute git command.
 
     Equivalent to `os.system(f"git {command}")`
 
     Returns the output of the `os.system` call."""
@@ -175,15 +177,15 @@
     """Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from
     the current working directory repo and add its url as this repo's remote origin.
 
     #### :params:
 
     `public`: Create the GitHub repo as a public repo, default is to create it as private."""
     visibility = "public" if public else "private"
-    os.system(f"gh repo create --source=. --remote=upstream --{visibility}")
+    os.system(f"gh repo create --source . --{visibility} --push")
 
 
 def make_private(owner: str, name: str):
     """Uses GitHub CLI (must be installed and configured) to set the repo's visibility to private.
 
     #### :params:
```

### Comparing `gitbetter-0.5.1/src/gitbetter/gitbetter.py` & `gitbetter-0.5.2/src/gitbetter/gitbetter.py`

 * *Files identical despite different names*

### Comparing `gitbetter-0.5.1/LICENSE.txt` & `gitbetter-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitbetter-0.5.1/README.md` & `gitbetter-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `gitbetter-0.5.1/pyproject.toml` & `gitbetter-0.5.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6769 7462 6574 7465 7222 0d0a 6465   "gitbetter"..de
 00000070: 7363 7269 7074 696f 6e20 3d20 2243 7573  scription = "Cus
 00000080: 746f 6d20 6769 7420 7368 656c 6c20 746f  tom git shell to
 00000090: 2074 7970 6520 6c65 7373 2061 6e64 2063   type less and c
 000000a0: 6f6d 6d69 7420 6d6f 7265 2e22 0d0a 7665  ommit more."..ve
-000000b0: 7273 696f 6e20 3d20 2230 2e35 2e31 220d  rsion = "0.5.1".
+000000b0: 7273 696f 6e20 3d20 2230 2e35 2e32 220d  rsion = "0.5.2".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 6172  endencies = ["ar
 000000f0: 6773 6865 6c6c 222c 2022 7061 7468 6965  gshell", "pathie
 00000100: 7222 2c20 2270 7974 6573 7422 5d0d 0a72  r", "pytest"]..r
 00000110: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
 00000120: 6d64 220d 0a6b 6579 776f 7264 7320 3d20  md"..keywords =
```

### Comparing `gitbetter-0.5.1/PKG-INFO` & `gitbetter-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitbetter
-Version: 0.5.1
+Version: 0.5.2
 Summary: Custom git shell to type less and commit more.
 Project-URL: Homepage, https://github.com/matt-manes/gitbetter
 Project-URL: Documentation, https://github.com/matt-manes/gitbetter/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gitbetter/tree/main/src/gitbetter
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,commit,git,shell,terminal
```

