# Comparing `tmp/cduv-0.1.tar.gz` & `tmp/cduv-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cduv-0.1.tar", last modified: Mon May 15 05:25:38 2023, max compression
+gzip compressed data, was "cduv-0.2.tar", last modified: Mon May 15 05:36:06 2023, max compression
```

## Comparing `cduv-0.1.tar` & `cduv-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 dm19       (501) staff       (20)        0 2023-05-15 05:25:38.247951 cduv-0.1/
--rw-r--r--   0 dm19       (501) staff       (20)      144 2023-05-15 05:25:38.247786 cduv-0.1/PKG-INFO
-drwxr-xr-x   0 dm19       (501) staff       (20)        0 2023-05-15 05:25:38.246802 cduv-0.1/cduv/
--rw-r--r--   0 dm19       (501) staff       (20)    29319 2023-05-15 05:05:05.000000 cduv-0.1/cduv/__init__.py
-drwxr-xr-x   0 dm19       (501) staff       (20)        0 2023-05-15 05:25:38.247597 cduv-0.1/cduv.egg-info/
--rw-r--r--   0 dm19       (501) staff       (20)      144 2023-05-15 05:25:38.000000 cduv-0.1/cduv.egg-info/PKG-INFO
--rw-r--r--   0 dm19       (501) staff       (20)      137 2023-05-15 05:25:38.000000 cduv-0.1/cduv.egg-info/SOURCES.txt
--rw-r--r--   0 dm19       (501) staff       (20)        1 2023-05-15 05:25:38.000000 cduv-0.1/cduv.egg-info/dependency_links.txt
--rw-r--r--   0 dm19       (501) staff       (20)        5 2023-05-15 05:25:38.000000 cduv-0.1/cduv.egg-info/top_level.txt
--rw-r--r--   0 dm19       (501) staff       (20)       38 2023-05-15 05:25:38.247999 cduv-0.1/setup.cfg
--rw-r--r--   0 dm19       (501) staff       (20)      175 2023-05-15 05:25:30.000000 cduv-0.1/setup.py
+drwxr-xr-x   0 dm19       (501) staff       (20)        0 2023-05-15 05:36:06.451005 cduv-0.2/
+-rw-r--r--   0 dm19       (501) staff       (20)      144 2023-05-15 05:36:06.450846 cduv-0.2/PKG-INFO
+drwxr-xr-x   0 dm19       (501) staff       (20)        0 2023-05-15 05:36:06.449797 cduv-0.2/cduv/
+-rw-r--r--   0 dm19       (501) staff       (20)    26800 2023-05-15 05:34:20.000000 cduv-0.2/cduv/__init__.py
+drwxr-xr-x   0 dm19       (501) staff       (20)        0 2023-05-15 05:36:06.450658 cduv-0.2/cduv.egg-info/
+-rw-r--r--   0 dm19       (501) staff       (20)      144 2023-05-15 05:36:06.000000 cduv-0.2/cduv.egg-info/PKG-INFO
+-rw-r--r--   0 dm19       (501) staff       (20)      137 2023-05-15 05:36:06.000000 cduv-0.2/cduv.egg-info/SOURCES.txt
+-rw-r--r--   0 dm19       (501) staff       (20)        1 2023-05-15 05:36:06.000000 cduv-0.2/cduv.egg-info/dependency_links.txt
+-rw-r--r--   0 dm19       (501) staff       (20)        5 2023-05-15 05:36:06.000000 cduv-0.2/cduv.egg-info/top_level.txt
+-rw-r--r--   0 dm19       (501) staff       (20)       38 2023-05-15 05:36:06.451058 cduv-0.2/setup.cfg
+-rw-r--r--   0 dm19       (501) staff       (20)      175 2023-05-15 05:35:43.000000 cduv-0.2/setup.py
```

### Comparing `cduv-0.1/cduv/__init__.py` & `cduv-0.2/cduv/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -792,177 +792,14 @@
 
 	if action:
 		print(f'{stack: <15}'+"|"+f'{inp: <15}'+"|"+f'Rejected')
 		break"""
     return s
 
 
-def leadandtrail8():
-    s = """#include<iostream>
-#include<conio.h>
-#include<stdio.h>
-#include<string.h>
-#include<stdlib.h>
-using namespace std;
-
-int vars,terms,i,j,k,m,rep,cont,temp=-1;
-char var[10],term[10],lead[10][10],trail[10][10];
-struct grammar
-{	
-	int prodno;
-	char lhs,rhs[20][20];
-}gram[50];
-void get()
-{
-	cout<<"\nLEADING AND TRAILING\n";
-	cout<<"\nEnter the no. of variables : ";
-	cin>>vars;
-	cout<<"\nEnter the variables : \n";
-	for(i=0;i<vars;i++)
-	{
-		cin>>gram[i].lhs;
-		var[i]=gram[i].lhs;
-	}
-	cout<<"\nEnter the no. of terminals : ";
-	cin>>terms;
-	cout<<"\nEnter the terminals : ";
-	for(j=0;j<terms;j++)
-		cin>>term[j];
-	cout<<"\nPRODUCTION DETAILS\n";
-	for(i=0;i<vars;i++)
-	{
-		cout<<"\nEnter the no. of production of "<<gram[i].lhs<<":";
-		cin>>gram[i].prodno;
-		for(j=0;j<gram[i].prodno;j++)
-		{
-			cout<<gram[i].lhs<<"->";
-			cin>>gram[i].rhs[j];
-		}
-	}
-}
-void leading()
-{
-	for(i=0;i<vars;i++)
-	{
-		for(j=0;j<gram[i].prodno;j++)
-		{
-			for(k=0;k<terms;k++)
-			{
-				if(gram[i].rhs[j][0]==term[k])
-					lead[i][k]=1;
-				else
-				{
-					if(gram[i].rhs[j][1]==term[k])
-						lead[i][k]=1;
-				}
-			}
-		}
-	}
-	for(rep=0;rep<vars;rep++)
-	{
-		for(i=0;i<vars;i++)
-		{
-			for(j=0;j<gram[i].prodno;j++)
-			{
-				for(m=1;m<vars;m++)
-				{
-					if(gram[i].rhs[j][0]==var[m])
-					{
-						temp=m;
-						goto out;
-					}
-				}
-				out:
-				for(k=0;k<terms;k++)
-				{
-					if(lead[temp][k]==1)
-						lead[i][k]=1;
-				}
-			}
-		}
-	}
-}
-void trailing()
-{
-	for(i=0;i<vars;i++)
-	{
-		for(j=0;j<gram[i].prodno;j++)
-		{
-			cont=0;
-			while(gram[i].rhs[j][cont]!='\x0')
-				cont++;
-			for(k=0;k<terms;k++)
-			{
-				if(gram[i].rhs[j][cont-1]==term[k])
-					trail[i][k]=1;
-				else
-				{
-					if(gram[i].rhs[j][cont-2]==term[k])
-						trail[i][k]=1;
-				}
-			}
-		}
-	}
-	for(rep=0;rep<vars;rep++)
-	{
-		for(i=0;i<vars;i++)
-		{
-			for(j=0;j<gram[i].prodno;j++)
-			{
-				cont=0;
-				while(gram[i].rhs[j][cont]!='\x0')
-					cont++;
-				for(m=1;m<vars;m++)
-				{
-					if(gram[i].rhs[j][cont-1]==var[m])
-						temp=m;
-				}
-				for(k=0;k<terms;k++)
-				{
-					if(trail[temp][k]==1)
-						trail[i][k]=1;
-				}
-			}
-		}
-	}
-}
-void display()
-{
-	for(i=0;i<vars;i++)
-	{
-		cout<<"\nLEADING("<<gram[i].lhs<<") = ";
-		for(j=0;j<terms;j++)
-		{
-			if(lead[i][j]==1)
-				cout<<term[j]<<",";
-		}
-	}
-	cout<<endl;
-	for(i=0;i<vars;i++)
-	{
-		cout<<"\nTRAILING("<<gram[i].lhs<<") = ";
-		for(j=0;j<terms;j++)
-		{
-			if(trail[i][j]==1)
-				cout<<term[j]<<",";
-		}
-	}
-}
-int main()
-{
-
-	get();
-	leading();
-	trailing();
-	display();
-
-}"""
-    return s
-
-
 def lroitems9():
     s = """#include<iostream>
 #include<conio.h>
 #include<string.h>
 
 using namespace std;
```

