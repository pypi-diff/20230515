# Comparing `tmp/kmerator-0.7.5b0.tar.gz` & `tmp/kmerator-0.7.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmerator-0.7.5b0.tar", last modified: Mon Apr 17 07:50:29 2023, max compression
+gzip compressed data, was "kmerator-0.7.6b0.tar", last modified: Mon May 15 08:37:12 2023, max compression
```

## Comparing `kmerator-0.7.5b0.tar` & `kmerator-0.7.6b0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-04-17 07:50:29.755334 kmerator-0.7.5b0/
--rw-r--r--   0 benoit    (1017) bio2m     (1010)      182 2023-04-17 07:20:43.000000 kmerator-0.7.5b0/MANIFEST.in
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13140 2023-04-17 07:50:29.751207 kmerator-0.7.5b0/PKG-INFO
--rw-r--r--   0 benoit    (1017) bio2m     (1010)    11313 2023-03-07 12:59:57.000000 kmerator-0.7.5b0/README.md
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-04-17 07:50:29.649519 kmerator-0.7.5b0/kmerator/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      115 2023-04-17 07:49:13.000000 kmerator-0.7.5b0/kmerator/__init__.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)      249 2023-02-16 14:55:54.000000 kmerator-0.7.5b0/kmerator/color.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     2715 2023-02-17 12:04:30.000000 kmerator-0.7.5b0/kmerator/config.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    19214 2023-03-07 18:13:30.000000 kmerator-0.7.5b0/kmerator/dataset.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      289 2023-02-13 12:52:30.000000 kmerator-0.7.5b0/kmerator/exit.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     1554 2023-04-17 07:50:09.000000 kmerator-0.7.5b0/kmerator/info.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    11900 2023-03-07 20:09:49.000000 kmerator-0.7.5b0/kmerator/kmerator.py
--rw-r--r--   0 benoit    (1017) bio2m     (1010)    16721 2023-04-12 13:23:33.000000 kmerator-0.7.5b0/kmerator/kmerize.py
--rw-r--r--   0 benoit    (1017) bio2m     (1010)      757 2023-02-16 14:24:06.000000 kmerator-0.7.5b0/kmerator/longest_transcript.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    10602 2023-02-28 11:49:15.000000 kmerator-0.7.5b0/kmerator/mk_geneinfo.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     8671 2023-02-20 09:09:59.000000 kmerator-0.7.5b0/kmerator/mk_transcriptome.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    11852 2023-03-07 12:30:07.000000 kmerator-0.7.5b0/kmerator/options.py
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-04-17 07:50:29.735819 kmerator-0.7.5b0/kmerator.egg-info/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13140 2023-04-17 07:50:29.000000 kmerator-0.7.5b0/kmerator.egg-info/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      481 2023-04-17 07:50:29.000000 kmerator-0.7.5b0/kmerator.egg-info/SOURCES.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-04-17 07:50:29.000000 kmerator-0.7.5b0/kmerator.egg-info/dependency_links.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2023-04-17 07:50:29.000000 kmerator-0.7.5b0/kmerator.egg-info/entry_points.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       18 2023-04-17 07:50:29.000000 kmerator-0.7.5b0/kmerator.egg-info/requires.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        9 2023-04-17 07:50:29.000000 kmerator-0.7.5b0/kmerator.egg-info/top_level.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2023-04-17 07:50:29.758051 kmerator-0.7.5b0/setup.cfg
--rw-r--r--   0 benoit    (1017) bio2m     (1010)     1008 2023-02-28 16:14:06.000000 kmerator-0.7.5b0/setup.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-15 08:37:12.664667 kmerator-0.7.6b0/
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)      182 2023-04-17 07:20:43.000000 kmerator-0.7.6b0/MANIFEST.in
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13261 2023-05-15 08:37:12.660238 kmerator-0.7.6b0/PKG-INFO
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)    11434 2023-05-10 16:09:57.000000 kmerator-0.7.6b0/README.md
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-15 08:37:12.516152 kmerator-0.7.6b0/kmerator/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      115 2023-04-17 07:49:13.000000 kmerator-0.7.6b0/kmerator/__init__.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)      249 2023-02-16 14:55:54.000000 kmerator-0.7.6b0/kmerator/color.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     2715 2023-02-17 12:04:30.000000 kmerator-0.7.6b0/kmerator/config.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    19218 2023-05-10 10:26:54.000000 kmerator-0.7.6b0/kmerator/dataset.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      289 2023-02-13 12:52:30.000000 kmerator-0.7.6b0/kmerator/exit.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     1554 2023-05-11 09:37:25.000000 kmerator-0.7.6b0/kmerator/info.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    11900 2023-03-07 20:09:49.000000 kmerator-0.7.6b0/kmerator/kmerator.py
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)    16939 2023-05-11 10:39:13.000000 kmerator-0.7.6b0/kmerator/kmerize.py
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)      757 2023-02-16 14:24:06.000000 kmerator-0.7.6b0/kmerator/longest_transcript.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    10602 2023-02-28 11:49:15.000000 kmerator-0.7.6b0/kmerator/mk_geneinfo.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     8671 2023-02-20 09:09:59.000000 kmerator-0.7.6b0/kmerator/mk_transcriptome.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    11953 2023-05-10 16:30:50.000000 kmerator-0.7.6b0/kmerator/options.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-15 08:37:12.611082 kmerator-0.7.6b0/kmerator.egg-info/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13261 2023-05-15 08:37:11.000000 kmerator-0.7.6b0/kmerator.egg-info/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      481 2023-05-15 08:37:12.000000 kmerator-0.7.6b0/kmerator.egg-info/SOURCES.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-05-15 08:37:11.000000 kmerator-0.7.6b0/kmerator.egg-info/dependency_links.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2023-05-15 08:37:11.000000 kmerator-0.7.6b0/kmerator.egg-info/entry_points.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       18 2023-05-15 08:37:12.000000 kmerator-0.7.6b0/kmerator.egg-info/requires.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        9 2023-05-15 08:37:12.000000 kmerator-0.7.6b0/kmerator.egg-info/top_level.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2023-05-15 08:37:12.667327 kmerator-0.7.6b0/setup.cfg
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)     1008 2023-02-28 16:14:06.000000 kmerator-0.7.6b0/setup.py
```

### Comparing `kmerator-0.7.5b0/PKG-INFO` & `kmerator-0.7.6b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerator
-Version: 0.7.5b0
+Version: 0.7.6b0
 Summary: Find specific gene or transcript kmers. And more.
 Home-page: https://github.com/Transipedia/kmerator
 Author: Sébastien RIQUIER, IRMB, Montpellier
 Author-email: sebastien.riquier@ucd.ie
 License: GPLv3
 Description: # Kmerator
         
@@ -49,15 +49,15 @@
         git clone https://github.com/Transipedia/kmerator3.git
         ln -s $PWD/kmerator3/kmerator/kmerator.py /usr/local/bin/kmerator  # or somewhere in your $PATH
         ```
         
         
         ## How to use kmerator
         
-        Before all, remember that kmerator needs a jellyfish index of the genome. You must build it according to the species you are studying.
+        Before all, remember that kmerator needs a jellyfish index of the genome. You must build it according to the species you are studying. You can store and name the index file whatever you want.
         
         ### Configuration file
         
         The arguments to run kmerator are numerous, so to reduce the number of arguments to enter, it is advisable to edit the configuration file with the command :
         
         ```
         kmerator -e
@@ -73,17 +73,17 @@
         	- the list of gene and/or transcripts separated by a space
         	- or a file with the list of genes/transcripts. Separator could by a space, a tab or a newline, and comments are allowed (`#`)
         - you find for specific k-mers of unannotated sequences : use the `--fasta-file` option, followed by a fasta file containing yours requests. In case of you focuses on chimeras, add the `--chimera` option
         
         **Examples:**
         
         ```
-        kmerator -s npm1 brca2 ENST00000255409 ENSG00000159216      # you can mix genes and transcripts
-        kmerator -s genes.txt   									 # you can also use a file with gene list
-        kmerator -f file.fa     									 # give a fasta file fr unannotated sequences
+        kmerator -s npm1 brca2 ENST00000255409 ENSG00000159216    # you can mix genes and transcripts
+        kmerator -s genes.txt                                     # you can also use a file with gene list
+        kmerator -f file.fa                                       # give a fasta file fr unannotated sequences
         ```
         
         **Note** the above commands assume that the configuration file contains at least the `datadir` and `genome` directives, the default species is homo_sapiens and the last available version will be used (if it is not present in datadir, kmerator will propose the construction of a dataset automatically)
         
         
         ### Note the difference between genes and transcripts
         
@@ -91,18 +91,18 @@
         - When you are looking for a **transcript**, kmerator only keeps the kmer found in the transcript, and only in that transcript. If isoforms completely cover the transcript, no kmer will be kept.
         
         ### Datasets
         
         To work, kmerator needs a jellyfish index of the genome, a jellyfish index of the transcriptome and various files. You will have to make the jellyfish genome index manually. Instead, kmerator builds the jellyfish transcriptome index and the files it needs, which we call datasets. There is one dataset per species and per transcriptome version. When kemrator does not find (in datadir) the requested transcriptome release (by default, the latest available on Ensembl), it offers to automatically build the dataset in question. In addition, dataset management options are available:
         
         ```
-        kmerator -l				# list local datasets
-        kmerator -u				# find last release on Ensembl, and build dataset if not present
-        kmerator --mk-dataset	# build dataset according to -r <release> and -S <specie> arguments
-        kmerator --rm-dataset	# delete dataset according to -r <release> and -S <specie> arguments
+        kmerator -l            # list local datasets
+        kmerator -u            # find last release on Ensembl, and build dataset if not present
+        kmerator --mk-dataset  # build dataset according to -r <release> and -S <specie> arguments
+        kmerator --rm-dataset  # delete dataset according to -r <release> and -S <specie> arguments
         ```
         
         
         ## All arguments
         
         ```
         optional arguments:
```

### Comparing `kmerator-0.7.5b0/README.md` & `kmerator-0.7.6b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 git clone https://github.com/Transipedia/kmerator3.git
 ln -s $PWD/kmerator3/kmerator/kmerator.py /usr/local/bin/kmerator  # or somewhere in your $PATH
 ```
 
 
 ## How to use kmerator
 
-Before all, remember that kmerator needs a jellyfish index of the genome. You must build it according to the species you are studying.
+Before all, remember that kmerator needs a jellyfish index of the genome. You must build it according to the species you are studying. You can store and name the index file whatever you want.
 
 ### Configuration file
 
 The arguments to run kmerator are numerous, so to reduce the number of arguments to enter, it is advisable to edit the configuration file with the command :
 
 ```
 kmerator -e
@@ -65,17 +65,17 @@
 	- the list of gene and/or transcripts separated by a space
 	- or a file with the list of genes/transcripts. Separator could by a space, a tab or a newline, and comments are allowed (`#`)
 - you find for specific k-mers of unannotated sequences : use the `--fasta-file` option, followed by a fasta file containing yours requests. In case of you focuses on chimeras, add the `--chimera` option
 
 **Examples:**
 
 ```
-kmerator -s npm1 brca2 ENST00000255409 ENSG00000159216      # you can mix genes and transcripts
-kmerator -s genes.txt   									 # you can also use a file with gene list
-kmerator -f file.fa     									 # give a fasta file fr unannotated sequences
+kmerator -s npm1 brca2 ENST00000255409 ENSG00000159216    # you can mix genes and transcripts
+kmerator -s genes.txt                                     # you can also use a file with gene list
+kmerator -f file.fa                                       # give a fasta file fr unannotated sequences
 ```
 
 **Note** the above commands assume that the configuration file contains at least the `datadir` and `genome` directives, the default species is homo_sapiens and the last available version will be used (if it is not present in datadir, kmerator will propose the construction of a dataset automatically)
 
 
 ### Note the difference between genes and transcripts
 
@@ -83,18 +83,18 @@
 - When you are looking for a **transcript**, kmerator only keeps the kmer found in the transcript, and only in that transcript. If isoforms completely cover the transcript, no kmer will be kept.
 
 ### Datasets
 
 To work, kmerator needs a jellyfish index of the genome, a jellyfish index of the transcriptome and various files. You will have to make the jellyfish genome index manually. Instead, kmerator builds the jellyfish transcriptome index and the files it needs, which we call datasets. There is one dataset per species and per transcriptome version. When kemrator does not find (in datadir) the requested transcriptome release (by default, the latest available on Ensembl), it offers to automatically build the dataset in question. In addition, dataset management options are available:
 
 ```
-kmerator -l				# list local datasets
-kmerator -u				# find last release on Ensembl, and build dataset if not present
-kmerator --mk-dataset	# build dataset according to -r <release> and -S <specie> arguments
-kmerator --rm-dataset	# delete dataset according to -r <release> and -S <specie> arguments
+kmerator -l            # list local datasets
+kmerator -u            # find last release on Ensembl, and build dataset if not present
+kmerator --mk-dataset  # build dataset according to -r <release> and -S <specie> arguments
+kmerator --rm-dataset  # delete dataset according to -r <release> and -S <specie> arguments
 ```
 
 
 ## All arguments
 
 ```
 optional arguments:
```

### Comparing `kmerator-0.7.5b0/kmerator/config.py` & `kmerator-0.7.6b0/kmerator/config.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.5b0/kmerator/dataset.py` & `kmerator-0.7.6b0/kmerator/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
             try:
                 file = file.split('.')
                 specie = file[0]
                 release = file[2]
                 item = f"{file[3]}.{file[4]}"
                 releases.setdefault(specie, {}).setdefault(release, []).append(item)
             except IndexError:
-                print(f"{DEBUG} Error: {'.'.join(file)!r} improperly formated.{ENDCOL}")
+                print(f"{DEBUG} Comment: {'.'.join(file)!r} is not a Dataset file.{ENDCOL}")
 
         ### classify the releases (complete or incomplete)
         releases_ok = {}
         releases_ko = {}
         for specie in releases:
             for release in releases[specie]:
                 if all(map(lambda v: v in releases[specie][release], attended )):
```

### Comparing `kmerator-0.7.5b0/kmerator/info.py` & `kmerator-0.7.6b0/kmerator/info.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Genral informations on to the program.
 """
 
 APPNAME = "kmerator"
 SHORTDESC = "Find specific gene or transcript kmers. And more."
 LICENCE = "GPL3"
-VERSION = "0.7.5-beta"
+VERSION = "0.7.6-beta"
 AUTHOR = 'Sébastien RIQUIER, IRMB, Montpellier'
 AUTHOR_EMAIL = "sebastien.riquier@ucd.ie"
 CONTIBUTORS = [
     'Chloe BESSIERE chloe.bessiere@inserm.fr>'
     'Benoit GUIBERT <benoit.guibert@inserm.fr>',
 ]
 DOC = f"""
```

### Comparing `kmerator-0.7.5b0/kmerator/kmerator.py` & `kmerator-0.7.6b0/kmerator/kmerator.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.5b0/kmerator/kmerize.py` & `kmerator-0.7.6b0/kmerator/kmerize.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,19 +102,22 @@
 
 
     def jellyfish(self, seq_file, jf_file):
         """
         From sequence, compute jellyfish againt the genome/transcriptome and convert results as dict ()
         """
         if self.args['debug']: print(f"{YELLOW}start jellyfish on {os.path.basename(seq_file)} against {os.path.basename(jf_file)}{ENDCOL}")
-        cmd = (f"jellyfish query -s '{seq_file}' {jf_file}")
+        cmd = f"jellyfish query -s '{seq_file}' {jf_file}"
         try:
-            result = subprocess.run(cmd, shell=True, check=True, capture_output=True).stdout.decode().rstrip().split('\n')
-        except subprocess.CalledProcessError:
-            sys.exit(f"{RED}Error: an error occured in jellyfish query command:\n  {cmd}{ENDCOL}")
+            # ~ result = subprocess.run(cmd, shell=True, check=True, capture_output=True).stdout.decode().rstrip().split('\n')
+            result = subprocess.check_output(cmd, shell=True, text=True, stderr=subprocess.STDOUT).rstrip('\n').split('\n')
+        except subprocess.CalledProcessError as err:
+            sys.exit(f"{ERROR}Error: executing jellyfish:\n"
+                     f"  {ERROR}command: {ENDCOL}{cmd}\n"
+                     f"  {ERROR}returned: {ENDCOL}{err.output}")
         result_dict = dict([ (b[0], int(b[1])) for b in [a.split() for a in result]])
         return result_dict
 
 
     def get_specific_kmers(self, item, kmercounts_transcriptome_dict, kmercounts_genome_dict):
         '''
         Keep only specific kmers, according to the arguments
```

### Comparing `kmerator-0.7.5b0/kmerator/longest_transcript.py` & `kmerator-0.7.6b0/kmerator/longest_transcript.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.5b0/kmerator/mk_geneinfo.py` & `kmerator-0.7.6b0/kmerator/mk_geneinfo.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.5b0/kmerator/mk_transcriptome.py` & `kmerator-0.7.6b0/kmerator/mk_transcriptome.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.5b0/kmerator/options.py` & `kmerator-0.7.6b0/kmerator/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                         )
     parser.add_argument('-t', '--thread',
                         type=int,
                         help="run n process simultaneously (default: 1)",
                         default=1,
                         )
     parser.add_argument('--tmpdir',
-                        help="directory to temporary file (default: /tmp/kmerator_<random>",
+                        help="directory to temporary file (default: /tmp/kmerator_<random>)",
                         default=None,
                         )
     parser.add_argument('-D', '--debug',
                         action='store_true',
                         help="Show more details while Kmerator is running.",
                         )
     parser.add_argument('--keep',
@@ -225,31 +225,31 @@
         ### Define genes/transcripts provided when they are in a file
         if len(args.selection) == 1 and os.path.isfile(args.selection[0]):
             with open(args.selection[0]) as fh:
                 args.selection = []
                 for line in fh:
                     args.selection += line.split('#')[0].split()
     ### --genome - check jellifish genome
-    if not args.genome[-3:] == '.jf':
-        sys.exit(f"{ERROR}Error: file not a jellyfish index ({args.genome.name!r}).{ENDCOL}")
+    # ~ if not args.genome[-3:] == '.jf':
+        # ~ sys.exit(f"{ERROR}Error: file not a jellyfish index ({args.genome!r}).{ENDCOL}")
     ### --chimera level works only with --fasta-file option
     if args.chimera and not args.fasta_file:
         sys.exit(f"{ERROR}Error: '--chimera' needs '--fasta-file' option.{ENDCOL}")
     ### temporary directory
     if not args.keep:
         if not args.tmpdir:
             args.tmpdir = tempfile.mkdtemp(prefix="kmerator_")
-        elif not os.isdir(args.tmpdir):
+        elif not os.path.isdir(args.tmpdir):
             sys.exit(f"{ERROR}Error: temporary directory not found ({args.tmpdir}).{ENDCOL}")
+        else:
+            args.tmpdir = tempfile.mkdtemp(prefix="kmerator_", dir=args.tmpdir)
     else:
         args.tmpdir = args.output
 
 
-
-
 '''
 def is_transcriptome_ensembl_file(first_row):
     """Checks if the line matches the Ensembl transcriptome file format"""
     line = first_row.split()
     try:
         if (not line[6].startswith('gene_symbol:') or
             not line[0].startswith('>ENST') or
```

### Comparing `kmerator-0.7.5b0/kmerator.egg-info/PKG-INFO` & `kmerator-0.7.6b0/kmerator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerator
-Version: 0.7.5b0
+Version: 0.7.6b0
 Summary: Find specific gene or transcript kmers. And more.
 Home-page: https://github.com/Transipedia/kmerator
 Author: Sébastien RIQUIER, IRMB, Montpellier
 Author-email: sebastien.riquier@ucd.ie
 License: GPLv3
 Description: # Kmerator
         
@@ -49,15 +49,15 @@
         git clone https://github.com/Transipedia/kmerator3.git
         ln -s $PWD/kmerator3/kmerator/kmerator.py /usr/local/bin/kmerator  # or somewhere in your $PATH
         ```
         
         
         ## How to use kmerator
         
-        Before all, remember that kmerator needs a jellyfish index of the genome. You must build it according to the species you are studying.
+        Before all, remember that kmerator needs a jellyfish index of the genome. You must build it according to the species you are studying. You can store and name the index file whatever you want.
         
         ### Configuration file
         
         The arguments to run kmerator are numerous, so to reduce the number of arguments to enter, it is advisable to edit the configuration file with the command :
         
         ```
         kmerator -e
@@ -73,17 +73,17 @@
         	- the list of gene and/or transcripts separated by a space
         	- or a file with the list of genes/transcripts. Separator could by a space, a tab or a newline, and comments are allowed (`#`)
         - you find for specific k-mers of unannotated sequences : use the `--fasta-file` option, followed by a fasta file containing yours requests. In case of you focuses on chimeras, add the `--chimera` option
         
         **Examples:**
         
         ```
-        kmerator -s npm1 brca2 ENST00000255409 ENSG00000159216      # you can mix genes and transcripts
-        kmerator -s genes.txt   									 # you can also use a file with gene list
-        kmerator -f file.fa     									 # give a fasta file fr unannotated sequences
+        kmerator -s npm1 brca2 ENST00000255409 ENSG00000159216    # you can mix genes and transcripts
+        kmerator -s genes.txt                                     # you can also use a file with gene list
+        kmerator -f file.fa                                       # give a fasta file fr unannotated sequences
         ```
         
         **Note** the above commands assume that the configuration file contains at least the `datadir` and `genome` directives, the default species is homo_sapiens and the last available version will be used (if it is not present in datadir, kmerator will propose the construction of a dataset automatically)
         
         
         ### Note the difference between genes and transcripts
         
@@ -91,18 +91,18 @@
         - When you are looking for a **transcript**, kmerator only keeps the kmer found in the transcript, and only in that transcript. If isoforms completely cover the transcript, no kmer will be kept.
         
         ### Datasets
         
         To work, kmerator needs a jellyfish index of the genome, a jellyfish index of the transcriptome and various files. You will have to make the jellyfish genome index manually. Instead, kmerator builds the jellyfish transcriptome index and the files it needs, which we call datasets. There is one dataset per species and per transcriptome version. When kemrator does not find (in datadir) the requested transcriptome release (by default, the latest available on Ensembl), it offers to automatically build the dataset in question. In addition, dataset management options are available:
         
         ```
-        kmerator -l				# list local datasets
-        kmerator -u				# find last release on Ensembl, and build dataset if not present
-        kmerator --mk-dataset	# build dataset according to -r <release> and -S <specie> arguments
-        kmerator --rm-dataset	# delete dataset according to -r <release> and -S <specie> arguments
+        kmerator -l            # list local datasets
+        kmerator -u            # find last release on Ensembl, and build dataset if not present
+        kmerator --mk-dataset  # build dataset according to -r <release> and -S <specie> arguments
+        kmerator --rm-dataset  # delete dataset according to -r <release> and -S <specie> arguments
         ```
         
         
         ## All arguments
         
         ```
         optional arguments:
```

### Comparing `kmerator-0.7.5b0/setup.py` & `kmerator-0.7.6b0/setup.py`

 * *Files identical despite different names*

