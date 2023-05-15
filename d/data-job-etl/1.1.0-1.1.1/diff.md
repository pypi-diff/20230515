# Comparing `tmp/data_job_etl-1.1.0-py3-none-any.whl.zip` & `tmp/data_job_etl-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,28 @@
-Zip file size: 171607 bytes, number of entries: 18
+Zip file size: 212293 bytes, number of entries: 26
+-rw-r--r--  2.0 unx     4480 b- defN 80-Jan-01 00:00 data_job_etl/.ipynb_checkpoints/rank-checkpoint.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 data_job_etl/__init__.py
--rw-r--r--  2.0 unx     1959 b- defN 80-Jan-01 00:00 data_job_etl/config/definitions.py
+-rw-r--r--  2.0 unx    75536 b- defN 80-Jan-01 00:00 data_job_etl/analysis.ipynb
+-rw-r--r--  2.0 unx     3487 b- defN 80-Jan-01 00:00 data_job_etl/build_technos.py
+-rw-r--r--  2.0 unx      371 b- defN 80-Jan-01 00:00 data_job_etl/config/definitions.py
 -rw-r--r--  2.0 unx      486 b- defN 80-Jan-01 00:00 data_job_etl/config/etl_logger.py
--rw-r--r--  2.0 unx     1836 b- defN 80-Jan-01 00:00 data_job_etl/config/postgres_schema.py
+-rw-r--r--  2.0 unx     2300 b- defN 80-Jan-01 00:00 data_job_etl/config/postgres_schema.py
+-rw-r--r--  2.0 unx      518 b- defN 80-Jan-01 00:00 data_job_etl/credentials.json
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 data_job_etl/data/__init__.py
 -rw-r--r--  2.0 unx   799758 b- defN 80-Jan-01 00:00 data_job_etl/data/mad2023.json
--rw-r--r--  2.0 unx     1147 b- defN 80-Jan-01 00:00 data_job_etl/etl.py
--rw-r--r--  2.0 unx      492 b- defN 80-Jan-01 00:00 data_job_etl/extract/extract.py
--rw-r--r--  2.0 unx      239 b- defN 80-Jan-01 00:00 data_job_etl/file.log
+-rw-r--r--  2.0 unx     1363 b- defN 80-Jan-01 00:00 data_job_etl/etl.py
+-rw-r--r--  2.0 unx      418 b- defN 80-Jan-01 00:00 data_job_etl/extract/extract.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 data_job_etl/file.log
 -rw-r--r--  2.0 unx      380 b- defN 80-Jan-01 00:00 data_job_etl/load/create_tables.py
--rw-r--r--  2.0 unx     4094 b- defN 80-Jan-01 00:00 data_job_etl/load/load.py
--rw-r--r--  2.0 unx     3390 b- defN 80-Jan-01 00:00 data_job_etl/transform/.ipynb_checkpoints/process-checkpoint.py
--rw-r--r--  2.0 unx     1589 b- defN 80-Jan-01 00:00 data_job_etl/transform/preprocess.py
--rw-r--r--  2.0 unx     2151 b- defN 80-Jan-01 00:00 data_job_etl/transform/process.py
--rw-r--r--  2.0 unx     2529 b- defN 80-Jan-01 00:00 data_job_etl/transform/summarise.py
--rw-r--r--  2.0 unx      466 b- defN 80-Jan-01 00:00 data_job_etl-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 data_job_etl-1.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1552 b- defN 16-Jan-01 00:00 data_job_etl-1.1.0.dist-info/RECORD
-18 files, 822156 bytes uncompressed, 169035 bytes compressed:  79.4%
+-rw-r--r--  2.0 unx     4661 b- defN 80-Jan-01 00:00 data_job_etl/load/load.py
+-rw-r--r--  2.0 unx     5979 b- defN 80-Jan-01 00:00 data_job_etl/message.py
+-rw-r--r--  2.0 unx     4480 b- defN 80-Jan-01 00:00 data_job_etl/rank.py
+-rw-r--r--  2.0 unx     3040 b- defN 80-Jan-01 00:00 data_job_etl/recommendation_system.py
+-rw-r--r--  2.0 unx     2547 b- defN 80-Jan-01 00:00 data_job_etl/summarise.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 data_job_etl/transform/file.log
+-rw-r--r--  2.0 unx     1965 b- defN 80-Jan-01 00:00 data_job_etl/transform/preprocess.py
+-rw-r--r--  2.0 unx     2254 b- defN 80-Jan-01 00:00 data_job_etl/transform/process.py
+-rw-r--r--  2.0 unx     1641 b- defN 80-Jan-01 00:00 data_job_etl/update_table.py
+-rw-r--r--  2.0 unx      465 b- defN 80-Jan-01 00:00 data_job_etl-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 data_job_etl-1.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2203 b- defN 16-Jan-01 00:00 data_job_etl-1.1.1.dist-info/RECORD
+26 files, 918420 bytes uncompressed, 208711 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -1,19 +1,31 @@
+Filename: data_job_etl/.ipynb_checkpoints/rank-checkpoint.py
+Comment: 
+
 Filename: data_job_etl/__init__.py
 Comment: 
 
+Filename: data_job_etl/analysis.ipynb
+Comment: 
+
+Filename: data_job_etl/build_technos.py
+Comment: 
+
 Filename: data_job_etl/config/definitions.py
 Comment: 
 
 Filename: data_job_etl/config/etl_logger.py
 Comment: 
 
 Filename: data_job_etl/config/postgres_schema.py
 Comment: 
 
+Filename: data_job_etl/credentials.json
+Comment: 
+
 Filename: data_job_etl/data/__init__.py
 Comment: 
 
 Filename: data_job_etl/data/mad2023.json
 Comment: 
 
 Filename: data_job_etl/etl.py
@@ -27,29 +39,41 @@
 
 Filename: data_job_etl/load/create_tables.py
 Comment: 
 
 Filename: data_job_etl/load/load.py
 Comment: 
 
-Filename: data_job_etl/transform/.ipynb_checkpoints/process-checkpoint.py
+Filename: data_job_etl/message.py
+Comment: 
+
+Filename: data_job_etl/rank.py
+Comment: 
+
+Filename: data_job_etl/recommendation_system.py
+Comment: 
+
+Filename: data_job_etl/summarise.py
+Comment: 
+
+Filename: data_job_etl/transform/file.log
 Comment: 
 
 Filename: data_job_etl/transform/preprocess.py
 Comment: 
 
 Filename: data_job_etl/transform/process.py
 Comment: 
 
-Filename: data_job_etl/transform/summarise.py
+Filename: data_job_etl/update_table.py
 Comment: 
 
-Filename: data_job_etl-1.1.0.dist-info/METADATA
+Filename: data_job_etl-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: data_job_etl-1.1.0.dist-info/WHEEL
+Filename: data_job_etl-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: data_job_etl-1.1.0.dist-info/RECORD
+Filename: data_job_etl-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## data_job_etl/config/definitions.py

```diff
@@ -1,19 +1,10 @@
 import os
-import json
 from pathlib import Path
 
 PROJECT_PATH = Path(os.path.dirname(os.path.abspath(__file__))).parent
 DATA_PATH = os.path.join(PROJECT_PATH, 'elt/transform/data')
 
 JOB_MARKET_DB_PWD = os.environ['JOB_MARKET_DB_PWD']
 JOB_MARKET_DB_USER = os.environ['JOB_MARKET_DB_USER']
 DB_STRING = f"postgresql://{JOB_MARKET_DB_USER}:{JOB_MARKET_DB_PWD}@localhost:5432/job_market"
 
-with open('/Users/donor/PycharmProjects/data-job-etl/data_job_etl/data/mad2023.json', 'r') as f:
-    mad = json.load(f)
-MAD_TECHNOS = [x['name'] for x in mad]
-OTHER_TECHNOS = {'DataBuildTool', 'MxNet', 'Hadoop', 'Beam', 'BigQuery', 'Pig', 'DataStudio', 'Redshift', 'Shell', 'Gitlab', 'data vault', 'Ceph', 'Airflow', 'GCP', 'IAM', 'k8s', 'Numpy', 'MAPR', 'Node', 'Athena', 'Unix', 'NiFi', 'Mongo', 'NoSQL', 'Unix Shell', 'Azure', 'Go', 'Golang', 'Perl', 'EC2', 'EMR', 'SPAR', 'Jenkins', 'Git', 'C/C\\+\\+', 'airflow', 'CloudSQL', 'Ruby', 'Redshift Spectrum', 'Glue', 'Postgres', 'Salt', 'python', 'nodejs', 'Go lang', 'Qlikview', 's3', 'Protobuf', 'MapReduce', 'Google Cloud', 'Elasticsearch', 'Spark', 'Celery', 'Pagerduty', 'mlflow', 'React', 'C\\+\\+', 'Tensorflow', 'Stitch DataGraphQL', 'Django', 'HDFS', 'Matillion WTL', 'SQL server', 'Istio', 'Dataflow', 'Codecov', 'UNIX', 'Typescript', 'DynamoDB', 'Vitess', 'Cassandra', 'HTTP', 'VizQL', 'C#', 'S3', 'SQL', 'Akka', 'MS-SQL', 'Stackdriver', 'Quicksilver', 'Github', 'dbt', 'DAX', 'StitchData', 'HBase', 'Microsoft SSIS', 'AWS S3', 'K8S', 'Java', 'SparkSQL', 'Kubeflow', 'ElasticSearch', '(No)SQL', 'Kinesis', 'Bigtable', 'CockroachDB', 'Scipy', 'Bash', 'git', 'Scikit Learn', 'Google Cloud Platform', 'Synapse', 'AWS', 'Spanner', 'H20', 'Javascript', 'LAMP', 'SQL Server', 'Py torch', 'PHP', 'PowerBI', 'gRPC', 'SAP', 'Neo4J', 'Cloud SQL', 'Reddis', 'Linux', 'SageMaker', 'dataiku', 'PQL', 'GCS', 'CircleCI', 'Kimball'}
-PRETTY_TECHNOS = OTHER_TECHNOS.union(MAD_TECHNOS)
-TECHNOS = {w.lower() for w in PRETTY_TECHNOS}
-
-
```

## data_job_etl/config/postgres_schema.py

```diff
@@ -1,9 +1,9 @@
 from numpy.random._generator import Sequence
-from sqlalchemy import Column, Integer, String, Date, Boolean, ForeignKey, inspect, Table
+from sqlalchemy import Column, Integer, Float, String, Date, Boolean, ForeignKey, inspect, Table
 from sqlalchemy.orm import relationship
 from sqlalchemy.dialects import postgresql
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 import pandas as pd
 
@@ -19,14 +19,17 @@
     company = Column(String(100), nullable=False)
     industry = Column(String(100))
     location = Column(String(100))
     remote = Column(String(100))
     type = Column(String(20))
     created_at = Column(Date)
     text = Column(String)
+    size = Column(String)
+    education = Column(String)
+    experience = Column(String)
 
 
 class ProcessedJob(Base):
     __tablename__ = 'processed_jobs'
 
     id = Column(Integer, primary_key=True)
     url = Column(String(500), nullable=False, unique=True)
@@ -36,14 +39,17 @@
     remote = Column(String(150))
     location = Column(String(150))
     industry = Column(String(150))
     type = Column(String(150))
     created_at = Column(Date)
     text = Column(String)
     summary = Column(String)
+    size = Column(String)
+    education = Column(String)
+    experience = Column(String)
 
 
 class PivottedJob(Base):
     __tablename__ = 'pivotted_jobs'
 
     id = Column(Integer, primary_key=True)
     raw_id = Column(Integer)
@@ -52,7 +58,18 @@
     company = Column(String(150), nullable=False)
     technos = Column(String(500))
     remote = Column(String(150))
     location = Column(String(150))
     industry = Column(String(150))
     type = Column(String(150))
     created_at = Column(Date)
+    size = Column(String)
+    education = Column(String)
+    experience = Column(String)
+
+
+class RankedJob(Base):
+    __tablename__ = 'ranked_jobs'
+    job_id = Column(Integer, primary_key=True)
+    rank = Column(Float)
+    remote_num = Column(Float)
+    exp_num = Column(Float)
```

## data_job_etl/etl.py

```diff
@@ -5,16 +5,24 @@
 from data_job_etl.transform.preprocess import Preprocessor
 from data_job_etl.transform.process import Processor
 from data_job_etl.load.load import Loader
 
 
 def extract():
     extractor = Extractor()
-    raw_jobs = extractor.extract_table('raw_jobs')
-    return raw_jobs
+    new_raw_query = """
+        SELECT *
+        FROM raw_jobs
+        WHERE created_at = (
+            SELECT created_at
+            FROM raw_jobs
+            ORDER BY created_at DESC limit 1);
+    """
+    new_raw_jobs = extractor.extract_query(new_raw_query)
+    return new_raw_jobs
 
 
 def transform(raw_jobs):
     preprocessor = Preprocessor(raw_jobs)
     preprocessor.preprocess()
     preprocessed_jobs = preprocessor.jobs
 
@@ -23,15 +31,15 @@
     pivotted_jobs = processor.pivot_technos(processed_jobs)
     return processed_jobs, pivotted_jobs
 
 
 def load(processed_jobs, pivotted_jobs):
     loader = Loader()
     loader.load_processed(processed_jobs)
-    loader.load_pivotted(pivotted_jobs)
+    # loader.load_pivotted(pivotted_jobs)
 
 
 def main():
     try:
         raw_jobs = extract()
         processed_jobs, pivotted_jobs = transform(raw_jobs)
         load(processed_jobs, pivotted_jobs)
```

## data_job_etl/extract/extract.py

```diff
@@ -3,19 +3,17 @@
 
 from data_job_etl.config.definitions import DB_STRING
 
 
 class Extractor:
 
     def __init__(self):
-        self.engine = None
+        self.engine = create_engine(DB_STRING)
 
     def extract_table(self, table):
-        self.engine = create_engine(DB_STRING)
         jobs = pd.read_sql(table, self.engine)
         return jobs
 
     def extract_query(self, query):
-        self.engine = create_engine(DB_STRING)
         jobs = pd.read_sql_query(query, self.engine)
         return jobs
```

## data_job_etl/file.log

```diff
@@ -1,15 +0,0 @@
-00000000: 3230 3233 2d30 332d 3239 2031 353a 3036  2023-03-29 15:06
-00000010: 3a35 352c 3237 3420 2d20 636f 6e66 6967  :55,274 - config
-00000020: 2e65 746c 5f6c 6f67 6765 7220 2d20 4552  .etl_logger - ER
-00000030: 524f 5220 2d20 5468 6973 2069 7320 616e  ROR - This is an
-00000040: 2065 7272 6f72 0a32 3032 332d 3033 2d32   error.2023-03-2
-00000050: 3920 3137 3a31 313a 3031 2c31 3839 202d  9 17:11:01,189 -
-00000060: 2064 6174 615f 6a6f 625f 6574 6c2e 636f   data_job_etl.co
-00000070: 6e66 6967 2e65 746c 5f6c 6f67 6765 7220  nfig.etl_logger 
-00000080: 2d20 4552 524f 5220 2d20 5468 6973 2069  - ERROR - This i
-00000090: 7320 616e 2065 7272 6f72 0a32 3032 332d  s an error.2023-
-000000a0: 3033 2d33 3120 3136 3a35 333a 3337 2c31  03-31 16:53:37,1
-000000b0: 3832 202d 2064 6174 615f 6a6f 625f 6574  82 - data_job_et
-000000c0: 6c2e 636f 6e66 6967 2e65 746c 5f6c 6f67  l.config.etl_log
-000000d0: 6765 7220 2d20 4552 524f 5220 2d20 5468  ger - ERROR - Th
-000000e0: 6973 2069 7320 616e 2065 7272 6f72 0a    is is an error.
```

## data_job_etl/load/load.py

```diff
@@ -41,26 +41,32 @@
             stack = processed.loc[i, 'stack']
             remote = processed.loc[i, 'remote']
             location = processed.loc[i, 'location']
             industry = processed.loc[i, 'industry']
             _type = processed.loc[i, 'type']
             created_at = processed.loc[i, 'created_at']
             text = processed.loc[i, 'text']
+            size = processed.loc[i, 'size']
+            experience = processed.loc[i, 'experience']
+            education = processed.loc[i, 'education']
 
             job = ProcessedJob(id=_id,
                                url=url,
                                title=title,
                                company=company,
                                stack=stack,
                                remote=remote,
                                location=location,
                                industry=industry,
                                type=_type,
                                created_at=created_at,
-                               text=text)
+                               text=text,
+                               size=size,
+                               experience=experience,
+                               education=education)
 
             with self.engine.connect() as connection:
                 with self.db_session(bind=connection) as session:
                     session.begin()
                     try:
                         session.merge(job)
                         session.commit()
@@ -80,26 +86,31 @@
             company = pivotted.loc[i, 'company']
             technos = pivotted.loc[i, 'technos']
             remote = pivotted.loc[i, 'remote']
             location = pivotted.loc[i, 'location']
             industry = pivotted.loc[i, 'industry']
             _type = pivotted.loc[i, 'type']
             created_at = pivotted.loc[i, 'created_at']
+            size = pivotted.loc[i, 'size']
+            experience = pivotted.loc[i, 'experience']
+            education = pivotted.loc[i, 'education']
 
             job = PivottedJob(raw_id=raw_id,
                               url=url,
                               title=title,
                               company=company,
                               technos=technos,
                               remote=remote,
                               location=location,
                               industry=industry,
                               type=_type,
-                              created_at=created_at
-                              )
+                              created_at=created_at,
+                              size=size,
+                              experience=experience,
+                              education=education)
 
             with self.engine.connect() as connection:
                 with self.db_session(bind=connection) as session:
                     session.begin()
                     try:
                         session.merge(job)
                         session.commit()
```

## data_job_etl/transform/preprocess.py

```diff
@@ -9,14 +9,15 @@
         self.jobs = jobs
 
     def preprocess(self):
         self.cast_types(self.jobs)
         self.add_missing_value(self.jobs)
         self.jobs['title'] = self.jobs['title'].apply(lambda x: self.process_title(x))
         self.jobs['text'] = self.jobs['text'].apply(lambda x: self.process_text(x))
+        self.jobs['remote'] = self.jobs['remote'].apply(lambda x: self.process_remote(x))
         self.jobs.reset_index(inplace=True, drop=True)
 
     @staticmethod
     def cast_types(jobs):
         jobs = jobs.convert_dtypes()
         jobs['id'] = jobs['id'].values.astype(int)
         jobs['created_at'] = pd.to_datetime(jobs['created_at'])
@@ -45,7 +46,18 @@
 
     @staticmethod
     def process_text(text):
         text = text.replace(u'\xa0', u' ')  # \xa0 (non-breaking space in Latin1 ISO 8859-1)
         text = re.sub(r'\s\s\s+', ' ', text)
         text = re.sub(r'\s\s+', ' ', text)
         return text.strip()
+
+    @staticmethod
+    def process_remote(original):
+        if 'partiel' in original:
+            return 'partiel'
+        elif 'ponctuel' in original:
+            return 'ponctuel'
+        elif 'total' in original:
+            return 'total'
+        else:
+            return original
```

## data_job_etl/transform/process.py

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import re
 
-from data_job_etl.config.definitions import TECHNOS
+from data_job_etl.build_technos import TechnoBuilder
 
 
 class Processor:
 
     def process_technos(self, jobs):
         """
         Add columns to a dataframe with technology names from a text.
@@ -30,17 +30,18 @@
         return jobs
 
     @staticmethod
     def extract_technos(text):
         """
         Identify and extract list of technology names.
         """
+        technos = TechnoBuilder().build_all_technos()
         words = re.split(r'\W+', text)
-        technos = {w for w in words if w.lower() in TECHNOS}
-        return list(technos)
+        technos_in_text = {w for w in words if w in technos}
+        return list(set(technos_in_text))
 
     @staticmethod
     def expand_stack(jobs):
         """
         Expand the stack column in as many columns as there are elements.
         """
         technos = pd.DataFrame(jobs['stack'].to_list())
@@ -49,15 +50,15 @@
 
     @staticmethod
     def melt_technos(jobs):
         """ 
         Melt dataframe to have one technology per row (for usage in Tableau). 
         """
         unpivotted_columns = ['id', 'url', 'title', 'company', 'location', 'type', 'industry', 'remote', 'created_at',
-                              'text', 'stack']
+                              'text', 'stack', 'size', 'education', 'experience']
         jobs = pd.melt(jobs, id_vars=unpivotted_columns).sort_values(by=['company', 'created_at', 'title'])
         jobs.reset_index(drop=True, inplace=True)
         return jobs
 
     @staticmethod
     def clean_pivot(jobs):
         """
```

## Comparing `data_job_etl/transform/summarise.py` & `data_job_etl/summarise.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,73 +3,71 @@
 from datetime import date
 from sqlalchemy.exc import SQLAlchemyError
 
 from data_job_etl.extract.extract import Extractor
 from data_job_etl.config.postgres_schema import ProcessedJob
 from data_job_etl.load.load import Loader
 
-openai.api_key = os.getenv('OPENAI_API_KEY')
-
 
 class Summariser:
     """
     Pipeline taking a text as input and summarising it in a new column.
     """
+
     def __init__(self):
         self.loader = Loader()
         self.extractor = Extractor()
 
     def summarise(self):
-        # Extract table to summarise
         processed_jobs = self.extract_processed_jobs()
-
-        for i in range(len(processed_jobs)):
-            # Prompt gpt-3.5-turbo
-            summary = self.request_gpt(processed_jobs['text'][i])
-
-            # Select new fields to update table
-            _id = processed_jobs['id'][i]
-            job = ProcessedJob(id=_id,
-                               summary=summary)
-
-            # Update id and summary in database
-            with self.loader.engine.connect() as connection:
-                with self.loader.db_session(bind=connection) as session:
-                    session.begin()
-                    try:
-                        session.merge(job)
-                        session.commit()
-                    except SQLAlchemyError as e:
-                        error = str(e.__dict__['orig'])
-                        print('An exception occurred:\n', error)
-                        session.rollback()
+        self.load_summary(processed_jobs)
 
     def extract_processed_jobs(self):
         # Restrict to relevant data engineer jobs
         query = 'SELECT id, text ' \
                 'FROM processed_jobs ' \
                 "WHERE title ~* '.*(data|analytics|devops|cloud).*(engineer|ingénieur).*|.*(engineer|ingénieur).*(data|données|big data|bigdata)|.*etl.*' " \
                 'AND summary is null ' \
                 'ORDER BY created_at DESC;'
         processed_jobs = self.extractor.extract_query(query)
         return processed_jobs
 
     @staticmethod
     def request_gpt(text):
+        api_key = os.getenv('OPENAI_API_KEY')
+        openai.api_key = api_key
         response = openai.ChatCompletion.create(
             model="gpt-3.5-turbo",
             messages=[
                 {"role": "user",
                  "content": f"Please provide a summary for this job description in less than 50 "
                             f"words and by emphasizing on the skills: {text}"}
             ]
         )
         summary = response.choices[0].message.content
         return summary
 
+    def load_summary(self, processed_jobs):
+        for i in range(len(processed_jobs)):
+            # Prompt gpt-3.5-turbo
+            summary = self.request_gpt(processed_jobs['text'][i])
 
-def main():
-    Summariser().summarise()
+            # Select new fields to update table
+            _id = processed_jobs['id'][i]
+            job = ProcessedJob(id=_id,
+                               summary=summary)
+
+            # Update id and summary in database
+        with self.loader.engine.connect() as connection:
+            with self.loader.db_session(bind=connection) as session:
+                session.begin()
+                try:
+                    session.merge(job)
+                    session.commit()
+                except SQLAlchemyError as e:
+                    error = str(e.__dict__['orig'])
+                    print('An exception occurred:\n', error)
+                    session.rollback()
 
 
 if __name__ == '__main__':
-    main()
+    Summariser().summarise()
```

## Comparing `data_job_etl-1.1.0.dist-info/RECORD` & `data_job_etl-1.1.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,26 @@
+data_job_etl/.ipynb_checkpoints/rank-checkpoint.py,sha256=opyH6EnTLpLUs-166yN71uiCu4Yklp4yzGJb5_MiNUI,4480
 data_job_etl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-data_job_etl/config/definitions.py,sha256=NCLf4c0h-XN1wetr7XaUiNacBKwKyeIfwiWJzjs_bZ4,1959
+data_job_etl/analysis.ipynb,sha256=70AjHmGw0SkS-6cyvsw3uVY6s0ZqNvKTMb1Nh3NVMzU,75536
+data_job_etl/build_technos.py,sha256=kfIvA3c1_nzuYj6ssb68TwnrgRYI4FVXvOGLZi-_93s,3487
+data_job_etl/config/definitions.py,sha256=1ZrAqDFV2uvn4FtYlem2hQYx14v_4EJMVuCYUG3f52w,371
 data_job_etl/config/etl_logger.py,sha256=1BE7eKhdw37uAxSWDu0IJYmDJhY8lZ2iwjzJ0hNZ8_4,486
-data_job_etl/config/postgres_schema.py,sha256=9ddtL1q2TLTWL6-8o2w4U2GcywluKhyPb_H50MZ5av4,1836
+data_job_etl/config/postgres_schema.py,sha256=IiBBuLrwSsGrZq7o4joFfmTuUAm4TGFW612sCKOHAIk,2300
+data_job_etl/credentials.json,sha256=l9Os9iRXhIFYA5dyN3hIwwLXw50HhrrSFHaApx1PaxI,518
 data_job_etl/data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 data_job_etl/data/mad2023.json,sha256=xEOg0W-CB2XswC-gp1dX4y6_hls-HiAXgRTSOfttU_A,799758
-data_job_etl/etl.py,sha256=bHBoj7m-IB0Mj_aryrVxd4wRj1Iu18WHwkr3F3dwlIY,1147
-data_job_etl/extract/extract.py,sha256=Nh68ilP5E_uN2ySKABthnPjo0htGYL1i9y9QY0C-nwk,492
-data_job_etl/file.log,sha256=QTLp1vRzTKOrKC4xWRHvewQf82KYADpEW52nhp7mXbc,239
+data_job_etl/etl.py,sha256=XLATUe1psRm9j3fWYBxL0-jwC7eOOvcIY-B04T2qCCo,1363
+data_job_etl/extract/extract.py,sha256=KZ2Vtye9N6xzLzAOxx-DeljrWobCvLHF4bSqDYtA_Cs,418
+data_job_etl/file.log,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 data_job_etl/load/create_tables.py,sha256=InZHxc-rU0W-1mLmgU9Ul7b5w7CkSI4aoW84tQNx-OU,380
-data_job_etl/load/load.py,sha256=vYsPfs4uJDoq3bx6_RRGDzHUUtKYnrq-O2UfaTFkTz0,4094
-data_job_etl/transform/.ipynb_checkpoints/process-checkpoint.py,sha256=swirnfkgiSbJ8tdUE4tplXrt7lBiiOFeT5r-5bQMDnQ,3390
-data_job_etl/transform/preprocess.py,sha256=F1R5bDC2zyEvbcr88oCREQ4lQAmH_dVnuuJ7CLRILk8,1589
-data_job_etl/transform/process.py,sha256=lsey09QCZ9LlKp8vcy9DIexnZoGKdWzxHzw2dpPdEo0,2151
-data_job_etl/transform/summarise.py,sha256=nBa37y__xnw9yRIESI_Vk08Fx9cTLAwQX-3hQxAFwl4,2529
-data_job_etl-1.1.0.dist-info/METADATA,sha256=McNh0OCBG7i_Tq2nC38UJDa766v8p896CDXyKa9KlVI,466
-data_job_etl-1.1.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-data_job_etl-1.1.0.dist-info/RECORD,,
+data_job_etl/load/load.py,sha256=CzogYxoKwlh4TX0sYa1i-oVciMl-q2OWCyPmi0EGG98,4661
+data_job_etl/message.py,sha256=8nHJ7Lrh7IHZ0sPZ5Ge6TNP4pJIheOrJz8F9bxUq4_Y,5979
+data_job_etl/rank.py,sha256=opyH6EnTLpLUs-166yN71uiCu4Yklp4yzGJb5_MiNUI,4480
+data_job_etl/recommendation_system.py,sha256=-TWysP-GoVNrZf1HrA3xLugnmmzbCawMznb0GJelm2U,3040
+data_job_etl/summarise.py,sha256=-CwLg-gTooiRHwCFBlLytwRuM9T1wqwWCq4P7ZQ9_Ok,2547
+data_job_etl/transform/file.log,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+data_job_etl/transform/preprocess.py,sha256=S8cW6C7z2nBCcOQxxCqF4TEkDg6JpUEXgxf-VW3XHbE,1965
+data_job_etl/transform/process.py,sha256=xgL0CWAVwJN4kSECexOI4odt7HWWyk90943Uzcv8B7I,2254
+data_job_etl/update_table.py,sha256=9maWu5wjwXFseMbs5B6yfS6_CygBRW7DzJtKzo_jSIA,1641
+data_job_etl-1.1.1.dist-info/METADATA,sha256=iPaF6D09SeYcK_r8ueFqqTTJ9-hq6wQKpYP0M3Gg4Jw,465
+data_job_etl-1.1.1.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+data_job_etl-1.1.1.dist-info/RECORD,,
```

