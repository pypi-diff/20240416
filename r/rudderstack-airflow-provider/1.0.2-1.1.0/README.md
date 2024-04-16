# Comparing `tmp/rudderstack-airflow-provider-1.0.2.tar.gz` & `tmp/rudderstack_airflow_provider-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudderstack-airflow-provider-1.0.2.tar", last modified: Mon Feb 26 12:02:16 2024, max compression
+gzip compressed data, was "rudderstack_airflow_provider-1.1.0.tar", last modified: Tue Apr 16 09:54:22 2024, max compression
```

## Comparing `rudderstack-airflow-provider-1.0.2.tar` & `rudderstack_airflow_provider-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 yeshwanth   (501) staff       (20)        0 2024-02-26 12:02:16.992352 rudderstack-airflow-provider-1.0.2/
--rw-r--r--   0 yeshwanth   (501) staff       (20)     1073 2024-02-21 10:29:54.000000 rudderstack-airflow-provider-1.0.2/LICENSE
--rw-r--r--   0 yeshwanth   (501) staff       (20)     3654 2024-02-26 12:02:16.992074 rudderstack-airflow-provider-1.0.2/PKG-INFO
--rw-r--r--   0 yeshwanth   (501) staff       (20)     2984 2024-02-21 10:29:54.000000 rudderstack-airflow-provider-1.0.2/README.md
--rw-r--r--   0 yeshwanth   (501) staff       (20)      104 2024-02-21 10:29:54.000000 rudderstack-airflow-provider-1.0.2/pyproject.toml
-drwxr-xr-x   0 yeshwanth   (501) staff       (20)        0 2024-02-26 12:02:16.987789 rudderstack-airflow-provider-1.0.2/rudder_airflow_provider/
--rw-r--r--   0 yeshwanth   (501) staff       (20)      213 2024-02-21 10:29:54.000000 rudderstack-airflow-provider-1.0.2/rudder_airflow_provider/__init__.py
-drwxr-xr-x   0 yeshwanth   (501) staff       (20)        0 2024-02-26 12:02:16.988245 rudderstack-airflow-provider-1.0.2/rudder_airflow_provider/hooks/
--rw-r--r--   0 yeshwanth   (501) staff       (20)        0 2023-09-29 08:57:26.000000 rudderstack-airflow-provider-1.0.2/rudder_airflow_provider/hooks/__init__.py
--rw-r--r--   0 yeshwanth   (501) staff       (20)     2831 2024-02-26 11:32:31.000000 rudderstack-airflow-provider-1.0.2/rudder_airflow_provider/hooks/rudderstack.py
-drwxr-xr-x   0 yeshwanth   (501) staff       (20)        0 2024-02-26 12:02:16.989532 rudderstack-airflow-provider-1.0.2/rudder_airflow_provider/operators/
--rw-r--r--   0 yeshwanth   (501) staff       (20)        0 2023-09-29 08:57:26.000000 rudderstack-airflow-provider-1.0.2/rudder_airflow_provider/operators/__init__.py
--rw-r--r--   0 yeshwanth   (501) staff       (20)     1158 2024-02-26 11:32:31.000000 rudderstack-airflow-provider-1.0.2/rudder_airflow_provider/operators/rudderstack.py
--rw-r--r--   0 yeshwanth   (501) staff       (20)       21 2024-02-26 11:59:19.000000 rudderstack-airflow-provider-1.0.2/rudder_airflow_provider/version.py
-drwxr-xr-x   0 yeshwanth   (501) staff       (20)        0 2024-02-26 12:02:16.991383 rudderstack-airflow-provider-1.0.2/rudderstack_airflow_provider.egg-info/
--rw-r--r--   0 yeshwanth   (501) staff       (20)     3654 2024-02-26 12:02:16.000000 rudderstack-airflow-provider-1.0.2/rudderstack_airflow_provider.egg-info/PKG-INFO
--rw-r--r--   0 yeshwanth   (501) staff       (20)      609 2024-02-26 12:02:16.000000 rudderstack-airflow-provider-1.0.2/rudderstack_airflow_provider.egg-info/SOURCES.txt
--rw-r--r--   0 yeshwanth   (501) staff       (20)        1 2024-02-26 12:02:16.000000 rudderstack-airflow-provider-1.0.2/rudderstack_airflow_provider.egg-info/dependency_links.txt
--rw-r--r--   0 yeshwanth   (501) staff       (20)       84 2024-02-26 12:02:16.000000 rudderstack-airflow-provider-1.0.2/rudderstack_airflow_provider.egg-info/entry_points.txt
--rw-r--r--   0 yeshwanth   (501) staff       (20)       22 2024-02-26 12:02:16.000000 rudderstack-airflow-provider-1.0.2/rudderstack_airflow_provider.egg-info/requires.txt
--rw-r--r--   0 yeshwanth   (501) staff       (20)       24 2024-02-26 12:02:16.000000 rudderstack-airflow-provider-1.0.2/rudderstack_airflow_provider.egg-info/top_level.txt
--rw-r--r--   0 yeshwanth   (501) staff       (20)     1001 2024-02-26 12:02:16.993036 rudderstack-airflow-provider-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:54:22.780907 rudderstack_airflow_provider-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-16 09:54:19.000000 rudderstack_airflow_provider-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-04-16 09:54:22.780907 rudderstack_airflow_provider-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-16 09:54:19.000000 rudderstack_airflow_provider-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-16 09:54:19.000000 rudderstack_airflow_provider-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:54:22.776907 rudderstack_airflow_provider-1.1.0/rudder_airflow_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-16 09:54:19.000000 rudderstack_airflow_provider-1.1.0/rudder_airflow_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:54:22.776907 rudderstack_airflow_provider-1.1.0/rudder_airflow_provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:54:19.000000 rudderstack_airflow_provider-1.1.0/rudder_airflow_provider/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-16 09:54:19.000000 rudderstack_airflow_provider-1.1.0/rudder_airflow_provider/hooks/rudderstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:54:22.776907 rudderstack_airflow_provider-1.1.0/rudder_airflow_provider/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:54:19.000000 rudderstack_airflow_provider-1.1.0/rudder_airflow_provider/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-16 09:54:19.000000 rudderstack_airflow_provider-1.1.0/rudder_airflow_provider/operators/rudderstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 09:54:19.000000 rudderstack_airflow_provider-1.1.0/rudder_airflow_provider/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:54:22.780907 rudderstack_airflow_provider-1.1.0/rudderstack_airflow_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-04-16 09:54:22.000000 rudderstack_airflow_provider-1.1.0/rudderstack_airflow_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-16 09:54:22.000000 rudderstack_airflow_provider-1.1.0/rudderstack_airflow_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:54:22.000000 rudderstack_airflow_provider-1.1.0/rudderstack_airflow_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-16 09:54:22.000000 rudderstack_airflow_provider-1.1.0/rudderstack_airflow_provider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 09:54:22.000000 rudderstack_airflow_provider-1.1.0/rudderstack_airflow_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 09:54:22.000000 rudderstack_airflow_provider-1.1.0/rudderstack_airflow_provider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-16 09:54:22.780907 rudderstack_airflow_provider-1.1.0/setup.cfg
```

### Comparing `rudderstack-airflow-provider-1.0.2/LICENSE` & `rudderstack_airflow_provider-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rudderstack-airflow-provider-1.0.2/PKG-INFO` & `rudderstack_airflow_provider-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: rudderstack-airflow-provider
-Version: 1.0.2
-Summary: airflow provider for rudderstack
-License: MIT
-Keywords: rudder,rudderstack,airflow,apache-airflow
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: apache-airflow>=2.5.3
-
 <p align="center">
   <a href="https://rudderstack.com/">
     <img src="https://user-images.githubusercontent.com/59817155/121357083-1c571300-c94f-11eb-8cc7-ce6df13855c9.png">
   </a>
 </p>
 
 <p align="center"><b>The Customer Data Platform for Developers</b></p>
@@ -47,14 +29,19 @@
 
 ```bash
 pip install rudderstack-airflow-provider
 ```
 
 ## Usage
 
+### RudderstackOperator
+
+> [!NOTE]  
+> Use [RudderstackRETLOperator](#rudderstackretloperator) for reverse ETL connections
+
 A simple DAG for triggering syncs for a RudderStack source:
 
 ```python
 with DAG(
     'rudderstack-sample',
     default_args=default_args,
     description='A simple tutorial DAG',
@@ -68,27 +55,62 @@
         task_id='<any-task-id>',
         connection_id='rudderstack_conn'
     )
 ```
 
 For the complete code, refer to this [example](https://github.com/rudderlabs/rudder-airflow-provider/blob/main/examples/sample_dag.py).
 
-### Operator Parameters
+#### Operator Parameters
 
 | Parameter | Description | Type | Default |
-| :--- |:--- | :--- | :--- |
+| :--- |:--- | :--- | :--- 
 | `source_id` | Valid RudderStack source ID | String | `None` |
 | `task_id` | A unique task ID within a DAG | String | `None` |
 | `wait_for_completion` | If `True`, the task will wait for sync to complete. | Boolean | `False` |
 | `connection_id` | The Airflow connection to use for connecting to the Rudderstack API. | String | `rudderstack_default` |
 
 The RudderStack operator also supports all the parameters supported by the [Airflow base operator](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/models/baseoperator/index.html).
 
 For details on how to run the DAG in Airflow, refer to the [documentation](https://www.rudderstack.com/docs/reverse-etl/features/airflow-provider/#running-the-dag).
 
+### RudderstackRETLOperator
+
+Trigger syncs for RETL connections
+
+```python
+with DAG('rudderstack-sample',
+    default_args=default_args,
+    description='A simple tutorial DAG',
+    schedule_interval=timedelta(days=1),
+    start_date=datetime(2021, 1, 1),
+    catchup=False,
+    tags=['rs']) as dag:
+    rs_operator = RudderstackRETLOperator(
+        retl_connection_id='2aiDQzMqP6LNuUokWstmaubcZOP',
+        task_id='retl-test-sync',
+        connection_id='rudder_yeshwanth_dev',
+        sync_type='full',
+        wait_for_completion=True
+    )
+```
+
+#### Operator parameters
+
+| Parameter | Description | Type | Default |
+| :--- |:--- | :--- | :--- 
+| `retl_connection_id` | Valid RudderStack RETL connection ID | String (templatable) | `None` |
+| `task_id` | A unique task ID within a DAG | String | `None` |
+| `wait_for_completion` | If `True`, the task will wait for sync to complete. | Boolean | `False` |
+| `connection_id` | The Airflow connection to use for connecting to the Rudderstack API. | String | `rudderstack_default` |
+|`sync_type`| Type of sync to trigger | `incremental` or `full` (templatable) | `incremental`|
+
+
+For details on how to run the DAG in Airflow, refer to the [documentation](https://www.rudderstack.com/docs/reverse-etl/features/airflow-provider/#running-the-dag).
+
+
 ## Contribute
 
 We would love to see you contribute to this project. Get more information on how to contribute [here](CONTRIBUTING.md).
 
 ## License
 
 The RudderStack Airflow Provider is released under the [MIT License](LICENSE).
```

#### html2text {}

```diff
@@ -1,44 +1,54 @@
-Metadata-Version: 2.1 Name: rudderstack-airflow-provider Version: 1.0.2
-Summary: airflow provider for rudderstack License: MIT Keywords:
-rudder,rudderstack,airflow,apache-airflow Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: apache-airflow>=2.5.3
  _[_h_t_t_p_s_:_/_/_u_s_e_r_-_i_m_a_g_e_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_5_9_8_1_7_1_5_5_/_1_2_1_3_5_7_0_8_3_-_1_c_5_7_1_3_0_0_-_c_9_4_f_-
                           _1_1_e_b_-_8_c_c_7_-_c_e_6_d_f_1_3_8_5_5_c_9_._p_n_g_]
                    TThhee CCuussttoommeerr DDaattaa PPllaattffoorrmm ffoorr DDeevveellooppeerrss
                   _WW_ee_bb_ss_ii_tt_ee ?Â?· _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ?Â?· _SS_ll_aa_cc_kk_ _CC_oo_mm_mm_uu_nn_ii_tt_yy
 --- # RudderStack Airflow Provider The [RudderStack](https://rudderstack.com)
 Airflow Provider lets you programmatically schedule and trigger your [Reverse
 ETL](https://www.rudderstack.com/docs/reverse-etl) syncs from outside
 RudderStack and integrate them with your existing Airflow workflows. | For more
 information on using the Airflow Provider utility, refer to the [documentation]
 (https://www.rudderstack.com/docs/reverse-etl/features/airflow-provider/). | |
 :---------| ## Installation ```bash pip install rudderstack-airflow-provider
-``` ## Usage A simple DAG for triggering syncs for a RudderStack source:
-```python with DAG( 'rudderstack-sample', default_args=default_args,
-description='A simple tutorial DAG', schedule_interval=timedelta(days=1),
-start_date=datetime(2021, 1, 1), catchup=False, tags=['rs'] ) as dag:
-rs_operator = RudderstackOperator( source_id='', task_id='',
-connection_id='rudderstack_conn' ) ``` For the complete code, refer to this
-[example](https://github.com/rudderlabs/rudder-airflow-provider/blob/main/
-examples/sample_dag.py). ### Operator Parameters | Parameter | Description |
-Type | Default | | :--- |:--- | :--- | :--- | | `source_id` | Valid RudderStack
-source ID | String | `None` | | `task_id` | A unique task ID within a DAG |
-String | `None` | | `wait_for_completion` | If `True`, the task will wait for
-sync to complete. | Boolean | `False` | | `connection_id` | The Airflow
-connection to use for connecting to the Rudderstack API. | String |
-`rudderstack_default` | The RudderStack operator also supports all the
-parameters supported by the [Airflow base operator](https://airflow.apache.org/
-docs/apache-airflow/stable/_api/airflow/models/baseoperator/index.html). For
-details on how to run the DAG in Airflow, refer to the [documentation](https://
-www.rudderstack.com/docs/reverse-etl/features/airflow-provider/#running-the-
-dag). ## Contribute We would love to see you contribute to this project. Get
-more information on how to contribute [here](CONTRIBUTING.md). ## License The
-RudderStack Airflow Provider is released under the [MIT License](LICENSE). ##
-Contact Us For more information or queries on this feature, you can [contact
-us](mailto:%20docs@rudderstack.com) or start a conversation in our [Slack]
-(https://rudderstack.com/join-rudderstack-slack-community) community.
+``` ## Usage ### RudderstackOperator > [!NOTE] > Use [RudderstackRETLOperator]
+(#rudderstackretloperator) for reverse ETL connections A simple DAG for
+triggering syncs for a RudderStack source: ```python with DAG( 'rudderstack-
+sample', default_args=default_args, description='A simple tutorial DAG',
+schedule_interval=timedelta(days=1), start_date=datetime(2021, 1, 1),
+catchup=False, tags=['rs'] ) as dag: rs_operator = RudderstackOperator
+( source_id='', task_id='', connection_id='rudderstack_conn' ) ``` For the
+complete code, refer to this [example](https://github.com/rudderlabs/rudder-
+airflow-provider/blob/main/examples/sample_dag.py). #### Operator Parameters |
+Parameter | Description | Type | Default | | :--- |:--- | :--- | :--- |
+`source_id` | Valid RudderStack source ID | String | `None` | | `task_id` | A
+unique task ID within a DAG | String | `None` | | `wait_for_completion` | If
+`True`, the task will wait for sync to complete. | Boolean | `False` | |
+`connection_id` | The Airflow connection to use for connecting to the
+Rudderstack API. | String | `rudderstack_default` | The RudderStack operator
+also supports all the parameters supported by the [Airflow base operator]
+(https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/models/
+baseoperator/index.html). For details on how to run the DAG in Airflow, refer
+to the [documentation](https://www.rudderstack.com/docs/reverse-etl/features/
+airflow-provider/#running-the-dag). ### RudderstackRETLOperator Trigger syncs
+for RETL connections ```python with DAG('rudderstack-sample',
+default_args=default_args, description='A simple tutorial DAG',
+schedule_interval=timedelta(days=1), start_date=datetime(2021, 1, 1),
+catchup=False, tags=['rs']) as dag: rs_operator = RudderstackRETLOperator
+( retl_connection_id='2aiDQzMqP6LNuUokWstmaubcZOP', task_id='retl-test-sync',
+connection_id='rudder_yeshwanth_dev', sync_type='full',
+wait_for_completion=True ) ``` #### Operator parameters | Parameter |
+Description | Type | Default | | :--- |:--- | :--- | :--- |
+`retl_connection_id` | Valid RudderStack RETL connection ID | String
+(templatable) | `None` | | `task_id` | A unique task ID within a DAG | String |
+`None` | | `wait_for_completion` | If `True`, the task will wait for sync to
+complete. | Boolean | `False` | | `connection_id` | The Airflow connection to
+use for connecting to the Rudderstack API. | String | `rudderstack_default` |
+|`sync_type`| Type of sync to trigger | `incremental` or `full` (templatable) |
+`incremental`| For details on how to run the DAG in Airflow, refer to the
+[documentation](https://www.rudderstack.com/docs/reverse-etl/features/airflow-
+provider/#running-the-dag). ## Contribute We would love to see you contribute
+to this project. Get more information on how to contribute [here]
+(CONTRIBUTING.md). ## License The RudderStack Airflow Provider is released
+under the [MIT License](LICENSE). ## Contact Us For more information or queries
+on this feature, you can [contact us](mailto:%20docs@rudderstack.com) or start
+a conversation in our [Slack](https://rudderstack.com/join-rudderstack-slack-
+community) community.
```

### Comparing `rudderstack-airflow-provider-1.0.2/rudderstack_airflow_provider.egg-info/PKG-INFO` & `rudderstack_airflow_provider-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: rudderstack-airflow-provider
-Version: 1.0.2
+Version: 1.1.0
 Summary: airflow provider for rudderstack
 License: MIT
 Keywords: rudder,rudderstack,airflow,apache-airflow
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apache-airflow>=2.5.3
+Requires-Dist: apache-airflow-providers-http>=4.2.0
+Requires-Dist: requests>=2.28.2
 
 <p align="center">
   <a href="https://rudderstack.com/">
     <img src="https://user-images.githubusercontent.com/59817155/121357083-1c571300-c94f-11eb-8cc7-ce6df13855c9.png">
   </a>
 </p>
 
@@ -47,14 +49,19 @@
 
 ```bash
 pip install rudderstack-airflow-provider
 ```
 
 ## Usage
 
+### RudderstackOperator
+
+> [!NOTE]  
+> Use [RudderstackRETLOperator](#rudderstackretloperator) for reverse ETL connections
+
 A simple DAG for triggering syncs for a RudderStack source:
 
 ```python
 with DAG(
     'rudderstack-sample',
     default_args=default_args,
     description='A simple tutorial DAG',
@@ -68,27 +75,62 @@
         task_id='<any-task-id>',
         connection_id='rudderstack_conn'
     )
 ```
 
 For the complete code, refer to this [example](https://github.com/rudderlabs/rudder-airflow-provider/blob/main/examples/sample_dag.py).
 
-### Operator Parameters
+#### Operator Parameters
 
 | Parameter | Description | Type | Default |
-| :--- |:--- | :--- | :--- |
+| :--- |:--- | :--- | :--- 
 | `source_id` | Valid RudderStack source ID | String | `None` |
 | `task_id` | A unique task ID within a DAG | String | `None` |
 | `wait_for_completion` | If `True`, the task will wait for sync to complete. | Boolean | `False` |
 | `connection_id` | The Airflow connection to use for connecting to the Rudderstack API. | String | `rudderstack_default` |
 
 The RudderStack operator also supports all the parameters supported by the [Airflow base operator](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/models/baseoperator/index.html).
 
 For details on how to run the DAG in Airflow, refer to the [documentation](https://www.rudderstack.com/docs/reverse-etl/features/airflow-provider/#running-the-dag).
 
+### RudderstackRETLOperator
+
+Trigger syncs for RETL connections
+
+```python
+with DAG('rudderstack-sample',
+    default_args=default_args,
+    description='A simple tutorial DAG',
+    schedule_interval=timedelta(days=1),
+    start_date=datetime(2021, 1, 1),
+    catchup=False,
+    tags=['rs']) as dag:
+    rs_operator = RudderstackRETLOperator(
+        retl_connection_id='2aiDQzMqP6LNuUokWstmaubcZOP',
+        task_id='retl-test-sync',
+        connection_id='rudder_yeshwanth_dev',
+        sync_type='full',
+        wait_for_completion=True
+    )
+```
+
+#### Operator parameters
+
+| Parameter | Description | Type | Default |
+| :--- |:--- | :--- | :--- 
+| `retl_connection_id` | Valid RudderStack RETL connection ID | String (templatable) | `None` |
+| `task_id` | A unique task ID within a DAG | String | `None` |
+| `wait_for_completion` | If `True`, the task will wait for sync to complete. | Boolean | `False` |
+| `connection_id` | The Airflow connection to use for connecting to the Rudderstack API. | String | `rudderstack_default` |
+|`sync_type`| Type of sync to trigger | `incremental` or `full` (templatable) | `incremental`|
+
+
+For details on how to run the DAG in Airflow, refer to the [documentation](https://www.rudderstack.com/docs/reverse-etl/features/airflow-provider/#running-the-dag).
+
+
 ## Contribute
 
 We would love to see you contribute to this project. Get more information on how to contribute [here](CONTRIBUTING.md).
 
 ## License
 
 The RudderStack Airflow Provider is released under the [MIT License](LICENSE).
```

#### html2text {}

```diff
@@ -1,44 +1,65 @@
-Metadata-Version: 2.1 Name: rudderstack-airflow-provider Version: 1.0.2
+Metadata-Version: 2.1 Name: rudderstack-airflow-provider Version: 1.1.0
 Summary: airflow provider for rudderstack License: MIT Keywords:
 rudder,rudderstack,airflow,apache-airflow Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: apache-airflow>=2.5.3
+Requires-Dist: apache-airflow-providers-http>=4.2.0 Requires-Dist:
+requests>=2.28.2
  _[_h_t_t_p_s_:_/_/_u_s_e_r_-_i_m_a_g_e_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_5_9_8_1_7_1_5_5_/_1_2_1_3_5_7_0_8_3_-_1_c_5_7_1_3_0_0_-_c_9_4_f_-
                           _1_1_e_b_-_8_c_c_7_-_c_e_6_d_f_1_3_8_5_5_c_9_._p_n_g_]
                    TThhee CCuussttoommeerr DDaattaa PPllaattffoorrmm ffoorr DDeevveellooppeerrss
                   _WW_ee_bb_ss_ii_tt_ee ?Â?· _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ?Â?· _SS_ll_aa_cc_kk_ _CC_oo_mm_mm_uu_nn_ii_tt_yy
 --- # RudderStack Airflow Provider The [RudderStack](https://rudderstack.com)
 Airflow Provider lets you programmatically schedule and trigger your [Reverse
 ETL](https://www.rudderstack.com/docs/reverse-etl) syncs from outside
 RudderStack and integrate them with your existing Airflow workflows. | For more
 information on using the Airflow Provider utility, refer to the [documentation]
 (https://www.rudderstack.com/docs/reverse-etl/features/airflow-provider/). | |
 :---------| ## Installation ```bash pip install rudderstack-airflow-provider
-``` ## Usage A simple DAG for triggering syncs for a RudderStack source:
-```python with DAG( 'rudderstack-sample', default_args=default_args,
-description='A simple tutorial DAG', schedule_interval=timedelta(days=1),
-start_date=datetime(2021, 1, 1), catchup=False, tags=['rs'] ) as dag:
-rs_operator = RudderstackOperator( source_id='', task_id='',
-connection_id='rudderstack_conn' ) ``` For the complete code, refer to this
-[example](https://github.com/rudderlabs/rudder-airflow-provider/blob/main/
-examples/sample_dag.py). ### Operator Parameters | Parameter | Description |
-Type | Default | | :--- |:--- | :--- | :--- | | `source_id` | Valid RudderStack
-source ID | String | `None` | | `task_id` | A unique task ID within a DAG |
-String | `None` | | `wait_for_completion` | If `True`, the task will wait for
-sync to complete. | Boolean | `False` | | `connection_id` | The Airflow
-connection to use for connecting to the Rudderstack API. | String |
-`rudderstack_default` | The RudderStack operator also supports all the
-parameters supported by the [Airflow base operator](https://airflow.apache.org/
-docs/apache-airflow/stable/_api/airflow/models/baseoperator/index.html). For
-details on how to run the DAG in Airflow, refer to the [documentation](https://
-www.rudderstack.com/docs/reverse-etl/features/airflow-provider/#running-the-
-dag). ## Contribute We would love to see you contribute to this project. Get
-more information on how to contribute [here](CONTRIBUTING.md). ## License The
-RudderStack Airflow Provider is released under the [MIT License](LICENSE). ##
-Contact Us For more information or queries on this feature, you can [contact
-us](mailto:%20docs@rudderstack.com) or start a conversation in our [Slack]
-(https://rudderstack.com/join-rudderstack-slack-community) community.
+``` ## Usage ### RudderstackOperator > [!NOTE] > Use [RudderstackRETLOperator]
+(#rudderstackretloperator) for reverse ETL connections A simple DAG for
+triggering syncs for a RudderStack source: ```python with DAG( 'rudderstack-
+sample', default_args=default_args, description='A simple tutorial DAG',
+schedule_interval=timedelta(days=1), start_date=datetime(2021, 1, 1),
+catchup=False, tags=['rs'] ) as dag: rs_operator = RudderstackOperator
+( source_id='', task_id='', connection_id='rudderstack_conn' ) ``` For the
+complete code, refer to this [example](https://github.com/rudderlabs/rudder-
+airflow-provider/blob/main/examples/sample_dag.py). #### Operator Parameters |
+Parameter | Description | Type | Default | | :--- |:--- | :--- | :--- |
+`source_id` | Valid RudderStack source ID | String | `None` | | `task_id` | A
+unique task ID within a DAG | String | `None` | | `wait_for_completion` | If
+`True`, the task will wait for sync to complete. | Boolean | `False` | |
+`connection_id` | The Airflow connection to use for connecting to the
+Rudderstack API. | String | `rudderstack_default` | The RudderStack operator
+also supports all the parameters supported by the [Airflow base operator]
+(https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/models/
+baseoperator/index.html). For details on how to run the DAG in Airflow, refer
+to the [documentation](https://www.rudderstack.com/docs/reverse-etl/features/
+airflow-provider/#running-the-dag). ### RudderstackRETLOperator Trigger syncs
+for RETL connections ```python with DAG('rudderstack-sample',
+default_args=default_args, description='A simple tutorial DAG',
+schedule_interval=timedelta(days=1), start_date=datetime(2021, 1, 1),
+catchup=False, tags=['rs']) as dag: rs_operator = RudderstackRETLOperator
+( retl_connection_id='2aiDQzMqP6LNuUokWstmaubcZOP', task_id='retl-test-sync',
+connection_id='rudder_yeshwanth_dev', sync_type='full',
+wait_for_completion=True ) ``` #### Operator parameters | Parameter |
+Description | Type | Default | | :--- |:--- | :--- | :--- |
+`retl_connection_id` | Valid RudderStack RETL connection ID | String
+(templatable) | `None` | | `task_id` | A unique task ID within a DAG | String |
+`None` | | `wait_for_completion` | If `True`, the task will wait for sync to
+complete. | Boolean | `False` | | `connection_id` | The Airflow connection to
+use for connecting to the Rudderstack API. | String | `rudderstack_default` |
+|`sync_type`| Type of sync to trigger | `incremental` or `full` (templatable) |
+`incremental`| For details on how to run the DAG in Airflow, refer to the
+[documentation](https://www.rudderstack.com/docs/reverse-etl/features/airflow-
+provider/#running-the-dag). ## Contribute We would love to see you contribute
+to this project. Get more information on how to contribute [here]
+(CONTRIBUTING.md). ## License The RudderStack Airflow Provider is released
+under the [MIT License](LICENSE). ## Contact Us For more information or queries
+on this feature, you can [contact us](mailto:%20docs@rudderstack.com) or start
+a conversation in our [Slack](https://rudderstack.com/join-rudderstack-slack-
+community) community.
```

### Comparing `rudderstack-airflow-provider-1.0.2/rudderstack_airflow_provider.egg-info/SOURCES.txt` & `rudderstack_airflow_provider-1.1.0/rudderstack_airflow_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rudderstack-airflow-provider-1.0.2/setup.cfg` & `rudderstack_airflow_provider-1.1.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 	apache-airflow
 
 [options]
 python_requires > = 3.6
 packages = find:
 install_requires = 
 	apache-airflow >= 2.5.3
+	apache-airflow-providers-http >= 4.2.0
+	requests >= 2.28.2
 
 [options.packages.find]
 exclude = *test*
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=rudder_airflow_provider:get_provider_info
```

