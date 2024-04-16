# Comparing `tmp/dbis-tm-0.0.12.tar.gz` & `tmp/dbis_tm-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-tm-0.0.12.tar", last modified: Fri Mar  8 12:14:35 2024, max compression
+gzip compressed data, was "dbis_tm-1.0.0.tar", last modified: Tue Apr 16 11:31:06 2024, max compression
```

## Comparing `dbis-tm-0.0.12.tar` & `dbis_tm-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 12:14:35.955283 dbis-tm-0.0.12/
--rw-r--r--   0 root         (0) root         (0)      705 2024-03-08 12:14:35.951283 dbis-tm-0.0.12/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      809 2024-03-08 12:03:38.000000 dbis-tm-0.0.12/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-08 12:14:35.955283 dbis-tm-0.0.12/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 12:14:35.951283 dbis-tm-0.0.12/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 12:14:35.951283 dbis-tm-0.0.12/src/dbis_tm/
--rw-rw-rw-   0 root         (0) root         (0)    34418 2024-03-08 12:03:38.000000 dbis-tm-0.0.12/src/dbis_tm/Generate.py
--rw-rw-rw-   0 root         (0) root         (0)     7466 2024-03-08 12:03:38.000000 dbis-tm-0.0.12/src/dbis_tm/Generate_Tasks.py
--rw-rw-rw-   0 root         (0) root         (0)    24525 2024-03-08 12:03:38.000000 dbis-tm-0.0.12/src/dbis_tm/Solution_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    12064 2024-03-01 08:34:51.000000 dbis-tm-0.0.12/src/dbis_tm/TM.py
--rw-rw-rw-   0 root         (0) root         (0)    13410 2024-03-08 12:03:38.000000 dbis-tm-0.0.12/src/dbis_tm/TMCheck.py
--rw-rw-rw-   0 root         (0) root         (0)    24777 2024-03-08 12:03:38.000000 dbis-tm-0.0.12/src/dbis_tm/TMSolver.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-03-08 12:03:38.000000 dbis-tm-0.0.12/src/dbis_tm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 12:14:35.951283 dbis-tm-0.0.12/src/dbis_tm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      705 2024-03-08 12:14:35.000000 dbis-tm-0.0.12/src/dbis_tm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-03-08 12:14:35.000000 dbis-tm-0.0.12/src/dbis_tm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 12:14:35.000000 dbis-tm-0.0.12/src/dbis_tm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       93 2024-03-08 12:14:35.000000 dbis-tm-0.0.12/src/dbis_tm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-08 12:14:35.000000 dbis-tm-0.0.12/src/dbis_tm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 12:14:35.951283 dbis-tm-0.0.12/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5177 2024-03-08 12:03:38.000000 dbis-tm-0.0.12/tests/test_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     6692 2024-03-08 12:03:38.000000 dbis-tm-0.0.12/tests/test_perfomance.py
--rw-rw-rw-   0 root         (0) root         (0)    14903 2024-03-08 12:03:38.000000 dbis-tm-0.0.12/tests/test_ub10Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)    35889 2024-03-08 12:03:38.000000 dbis-tm-0.0.12/tests/test_ub10TM.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 11:31:06.948412 dbis_tm-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)      704 2024-04-16 11:31:06.948412 dbis_tm-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      808 2024-04-16 11:15:29.000000 dbis_tm-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 11:31:06.948412 dbis_tm-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 11:31:06.948412 dbis_tm-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 11:31:06.948412 dbis_tm-1.0.0/src/dbis_tm/
+-rw-rw-rw-   0 root         (0) root         (0)    40325 2024-04-14 14:39:41.000000 dbis_tm-1.0.0/src/dbis_tm/Generate.py
+-rw-rw-rw-   0 root         (0) root         (0)     7399 2024-04-09 10:37:55.000000 dbis_tm-1.0.0/src/dbis_tm/Generate_Tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)    24508 2024-04-09 10:37:55.000000 dbis_tm-1.0.0/src/dbis_tm/Solution_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    12780 2024-04-09 12:17:44.000000 dbis_tm-1.0.0/src/dbis_tm/TM.py
+-rw-rw-rw-   0 root         (0) root         (0)    13595 2024-04-09 10:42:22.000000 dbis_tm-1.0.0/src/dbis_tm/TMCheck.py
+-rw-rw-rw-   0 root         (0) root         (0)    25050 2024-04-09 10:42:22.000000 dbis_tm-1.0.0/src/dbis_tm/TMSolver.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-03-08 12:03:38.000000 dbis_tm-1.0.0/src/dbis_tm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 11:31:06.948412 dbis_tm-1.0.0/src/dbis_tm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      704 2024-04-16 11:31:06.000000 dbis_tm-1.0.0/src/dbis_tm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-16 11:31:06.000000 dbis_tm-1.0.0/src/dbis_tm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 11:31:06.000000 dbis_tm-1.0.0/src/dbis_tm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2024-04-16 11:31:06.000000 dbis_tm-1.0.0/src/dbis_tm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 11:31:06.000000 dbis_tm-1.0.0/src/dbis_tm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 11:31:06.948412 dbis_tm-1.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5181 2024-04-09 10:53:52.000000 dbis_tm-1.0.0/tests/test_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     6708 2024-04-09 10:53:52.000000 dbis_tm-1.0.0/tests/test_perfomance.py
+-rw-rw-rw-   0 root         (0) root         (0)    15382 2024-04-09 10:53:52.000000 dbis_tm-1.0.0/tests/test_ub10Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)    36807 2024-04-09 12:17:44.000000 dbis_tm-1.0.0/tests/test_ub10TM.py
```

### Comparing `dbis-tm-0.0.12/PKG-INFO` & `dbis_tm-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-tm
-Version: 0.0.12
+Version: 1.0.0
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: DBIS i5 RWTH Aachen <dbis-vl@dbis.rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-tm
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-tm-0.0.12/pyproject.toml` & `dbis_tm-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="dbis-tm"
-version='0.0.12'
+version='1.0.0'
 description="RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 
 authors = [
 	{ name = "DBIS i5 RWTH Aachen", email = "dbis-vl@dbis.rwth-aachen.de" }
 ]
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `dbis-tm-0.0.12/src/dbis_tm/Generate.py` & `dbis_tm-1.0.0/src/dbis_tm/Generate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from dbis_tm import Schedule, OperationType, Operation
 import random, copy
-from dbis_tm.Solution_generator import predict_deadlock
+from src.dbis_tm.Solution_generator import predict_deadlock
 
 
 def generate(
     transactions: int, resources: list[str], deadlock=None, recovery=None
 ) -> tuple[Schedule, str]:
     """Generates a schedule
-    Gets:
+
+    Args:
         - transactions:int
         - resources: [char]
         - either deadlock: Bool
         - or recovery [n,r,a,s]"""
     if isinstance(deadlock, bool) and isinstance(recovery, str):
         raise ValueError("Not allowed to choose deadlock and recovery.")
 
@@ -40,26 +41,39 @@
 
 class Generator:
     """
     Class to handle variables and common functions for the schedule generation.
     """
 
     def __init__(self, transactions: list, resources: list[str]):
+        """
+        Constructor
+
+        Args:
+            transactions(list): number of transactions
+            resources(list[str]): list of resources
+        """
         # initiate schedule
         self.schedule = Schedule([], resources, transactions, dict(), dict())
         # initiate resources
         self.op_choice = [OperationType.READ, OperationType.WRITE]
         # initiate action parts
         self.generated_operation = None
         # initiate lists for random choice, and length
         self.index = random.randrange(transactions * 3, transactions * 5 + 1)
         self.conclude_choice = [1, 0, 0]
         self.close_trans = [False for _ in range(transactions)]
 
     def check_circle(self, transactions: list) -> bool:
+        """
+        Function to check whether the given lists of transactions which are waiting on each other contain a cycle
+
+        Args:
+            transactions(list): lists for all transactions, which trtansaction they are waiting on
+        """
         ignore = []
         i = 0
         while i < len(transactions):
             if (
                 not [op for op in transactions[i] if op not in ignore]
                 and i + 1 not in ignore
             ):
@@ -68,29 +82,36 @@
             i += 1
         ignore = list(set(ignore))
         if len(ignore) == len(transactions):
             return False
         return True
 
     def evaluate_conclude(self, transaction: int) -> bool:
-        """Function to determine the conclusion status"""
+        """
+        Function to determine the conclusion status
+
+        Args:
+            transaction(int): transaction which should be evaluated
+        """
         if self.schedule.op_trans(transaction) == 0 or (
             len(self.schedule.active()) == 1 and self.index > 1
         ):  # if none performed, if not the last action, but only one operation remains
             return False
         elif (
             self.schedule.op_trans(transaction) > self.schedule.tx_count
             or self.close_trans[transaction - 1]
         ):  # if all performed, must be in this position, so one transaction in not forced to performed till the end by more then transactions+1 times
             return True
         else:  # else (between 1-3 actions)
             return bool(random.choice(self.conclude_choice))
 
     def choose_transaction(self) -> int:
-        """Returns the transaction, either randomly ob forced bc no operation is performed yet and threshold is reached."""
+        """
+        Returns the transaction, either randomly ob forced bc no operation is performed yet and threshold is reached.
+        """
         trans = 0
         if self.index == len(self.schedule.active()):
             for u in self.schedule.active():
                 if self.schedule.op_trans(u) != 0:
                     self.close_trans[u - 1] = True
                 else:
                     self.index += 1
@@ -100,24 +121,41 @@
         return trans
 
 
 class GenerateSchedule(Generator):
     """Class which generates a schedule"""
 
     def __init__(self, transactions: list, resources: list[str]) -> Schedule:
+        """
+        Constructor
+
+        Args:
+            transactions(list): number of transactions
+            resources(list[str]): list of resources
+        """
         super().__init__(transactions, resources)
         self.generate_schedule()
 
     def generate_schedule(self) -> Schedule:
+        """
+        Function to generate a schedule
+        """
         while self.index > 0:
             trans = self.choose_transaction()
             self.generate_action(trans, self.evaluate_conclude(trans))
             self.index -= 1
 
     def generate_action(self, transaction: int, conclude: bool):
+        """
+        Function to generate a schedule action r/w/c/a
+
+        Args:
+            transaction(int): the transaction which performs the action
+            conclude(bool): wether to c/a the transaction
+        """
         if conclude:  # add an abort/commit
             if bool(random.choice([0, 1])):
                 self.schedule.aborts[transaction] = self.schedule.next_index()
             else:
                 self.schedule.commits[transaction] = self.schedule.next_index()
         else:  # add an action
             self.schedule.operations.append(
@@ -127,34 +165,53 @@
                     random.choice(self.schedule.resources),
                     self.schedule.next_index(),
                 )
             )
 
 
 class GenerateRecovery(Generator):
-    """Class which generates a Recovery schedule"""
+    """Class which generates a schedule in a recovery class"""
 
     def __init__(
         self, transactions: list, resources: list[str], recovery: str
     ) -> Schedule:
+        """
+        Constructor
+
+        Args:
+            transactions(list): number of transactions
+            resources(list[str]): list of resources
+            recovery(str): type of recovery class the schedule should be in
+        """
         super().__init__(transactions, resources)
         # recovery
         self.recovery = recovery
         self.not_next = False
         self.generate_schedule()
 
     def generate_schedule(self):
+        """
+        Function to generate a schedule in one recovery class
+        """
         while self.index > 0:
             trans = self.choose_transaction()
             self.generate_recovery_action(trans, self.evaluate_conclude(trans))
             if self.generated_operation == 0:
                 continue
             self.index -= 1
 
     def generate_recovery_action(self, transaction: int, conclude: bool):
+        """
+        Function to produce a action for a recovery schedule.
+        Might also fail and do nothing due to randomness.
+
+        Args:
+            transaction(int): transactions chosen (might change of no operation possible)
+            conclude(bool): indicates wether the transaction should be closed (can be denied by the function)
+        """
         prepared = self.any_read_from()
         if (
             len(self.schedule.active()) == 2
             and not self.not_next
             and (self.recovery == "a" or (self.recovery in ["n", "r"] and not prepared))
         ):
             conclude = False
@@ -245,37 +302,54 @@
         if transaction == 0:
             self.generated_operation = 0
         elif self.generated_operation != None:
             self.schedule.operations.append(self.generated_operation)
         return
 
     def not_ready(self) -> bool:
+        """
+        Function which returns wether the computed schedule is not in the next bigger class.
+        """
         return (
             not self.not_next
             and (self.recovery == "a" or not self.any_read_from())
             and (
                 (self.recovery == "n" and self.index <= len(self.schedule.active()) + 1)
                 or (
                     not self.recovery == "n"
                     and self.index == len(self.schedule.active()) + 1
                 )
             )
         )
 
-    def other_writes(self, trans, res) -> list:
-        """Returns last write transactions on res other than from trans"""
+    def other_writes(self, trans: int, res: str) -> list:
+        """
+        Function which returns last write transactions on res other than from transaction
+
+        Args:
+            trans(int): transaction to look at
+            res(str): resource to look at
+        """
         return [
             op
             for op in self.last_write()
             if op.tx_number != trans and op.resource == res
         ]
 
     def choose_op(
-        self, resource, operation, transaction
+        self, resource: str, operation: OperationType, transaction: int
     ) -> list[str, OperationType, int]:
+        """
+        Function which chooses an operation so the schedule is no longer in the next bigger class.
+
+        Args:
+            resource(str): resource to look at
+            operation(OperationType): Operation type to consider
+            transaction(int): transaction to look at
+        """
         if not self.other_writes(transaction, resource) or self.recovery == "n":
             if self.last_write():
                 if (
                     self.recovery == "n"
                     and self.index < len(self.schedule.active()) + 1
                 ):
                     self.index = len(self.schedule.active()) + 1
@@ -319,15 +393,20 @@
                 if j.resource == i and j.op_type == OperationType.WRITE:
                     l_cur_write.append(j)
                     break
         l_cur_write = [x for x in l_cur_write if x.tx_number in self.schedule.active()]
         return l_cur_write
 
     def read_from(self, op1: Operation, op2: Operation) -> bool:
-        """Says wether op1 reads from op2, commits and aborts only till this operation"""
+        """Says wether op1 reads from op2, commits and aborts only till this operation
+
+        Args:
+            op1(Operation): possible read operation
+            op2(Operation): possible write operation
+        """
         if (
             op1.op_type == OperationType.READ
             and op2.op_type == OperationType.WRITE
             and op1.resource == op2.resource
         ):
             if op1.tx_number != op2.tx_number and op1.index > op2.index:
                 for i in self.schedule.operations:
@@ -346,15 +425,19 @@
                         )
                     ):
                         return False
                 return True
         return False
 
     def read_from_trans(self, current_transaction: int) -> list:
-        """Function returning transactions which read from current_transaction"""
+        """Function returning transactions which read from current_transaction
+
+        Args:
+            current_transaction(int): transaction to check
+        """
         reads = []
         open_operations = [
             op
             for op in self.schedule.operations
             if op.tx_number in self.schedule.active()
         ]
         for i in range(len(open_operations)):
@@ -365,15 +448,19 @@
                 for j in range(i, len(open_operations)):
                     if self.read_from(open_operations[j], open_operations[i]):
                         reads.append(open_operations[j].tx_number)
         reads = list(set(reads))
         return reads
 
     def trans_read_from(self, current_transaction: int) -> list:
-        """Function returning transactions which current_transaction reads from"""
+        """Function returning transactions which current_transaction reads from
+
+        Args:
+            current_transaction(int): transaction to check
+        """
         reads = []
         open_operations = [
             op
             for op in self.schedule.operations
             if op.tx_number in self.schedule.active()
         ]
         for i in range(len(open_operations)):
@@ -390,30 +477,39 @@
     def any_read_from(self) -> bool:
         """Returns wether there are any reads performed"""
         for i in range(1, self.schedule.tx_count + 1):
             if self.read_from_trans(i):
                 return True
         return False
 
-    def check_circle_trans(self, current_transaction: int, write: int) -> bool:
-        """Returns True if a circle is produced when executing the current read transaction"""
+    def check_circle_trans(self, current_transaction: int, write: list) -> bool:
+        """Returns True if a circle is produced when executing the current read transaction
+
+        Args:
+            current_transaction(int): transaction to check (read transaction)
+            write(list): all write transaction
+        """
         check_circle_reads = []
         for i in range(1, self.schedule.tx_count + 1):
             if i == current_transaction:
                 check_circle_reads.append(self.read_from_trans(i) + [write])
             else:
                 check_circle_reads.append(self.read_from_trans(i))
         return self.check_circle(check_circle_reads)
 
     def new_transaction(self, current_trans: int, recovery=None) -> int:
         """Returning usable transaction or 0
-        Gets:
-        - (optional) recovery: Bool, in recovery
+
+        Args:
+            current_trans(int): transaction to check
+            (optional) recovery(bool):  in recovery
+
         Returns:
-        - valid transaction or 0"""
+            valid transaction or 0
+        """
         transactions1 = [
             q
             for q in range(1, self.schedule.tx_count + 1)
             if q in self.schedule.active() and self.trans_read_from(q) == []
         ]
         if recovery == "r":
             for t in transactions1:
@@ -429,38 +525,56 @@
 
 class GenerateDeadlock(Generator):
     """Class to generate a schedule with or without a Deadlock."""
 
     def __init__(
         self, transactions: list, resources: list[str], deadlock: bool
     ) -> Schedule:
+        """
+        Constructor
+
+        Args:
+            transactions(list): transactions
+            resources(list(str)):  resources to use
+            deadlock(bool): wether or not a deadlock should occur
+        """
         super().__init__(transactions, resources)
         # deadlock
         self.deadlock = deadlock
         self.deadlock_occurred = False
         self.counter = 0
         self.waiting = False
         self.performed_l = []  # for efficency
         self.generate_schedule()
 
     def generate_schedule(self):
+        """
+        Function to generate a schedule with considerations to deadlocks
+        """
         while self.index > 0:
             trans = self.choose_transaction()
             self.generate_deadlock_action(trans, self.evaluate_conclude(trans))
             if self.generated_operation == 0:
                 continue
             self.index -= 1
 
         if self.deadlock and self.deadlock_occurred and self.schedule.active():
             for i in self.schedule.active():
                 self.generate_deadlock_action(i, True)
 
     def generate_deadlock_action(
         self, transaction: int, conclude: bool
     ) -> tuple[list, list]:
+        """
+        Function to generate an action for a schedule with(out) deadlocks
+
+        Args:
+            transaction(int): transaction to consider (might be changes by the function)
+            conclude(bool):  wether to conclude (might be overwritten by the function)
+        """
         self.performed_l = []
         if self.deadlock and not self.deadlock_occurred:
             if len(self.schedule.active()) == 2 or (
                 len(self.schedule.active()) - 1 == len(self.schedule.resources)
                 and self.waiting
             ):
                 conclude = False
@@ -554,45 +668,61 @@
             self.counter += 1
         elif self.generated_operation != None:
             self.counter = 0
             self.schedule.operations.append(self.generated_operation)
         return
 
     def different_action(self, transaction: int, no_waiting=False) -> list[Operation]:
-        """"""
+        """
+        Function
+
+        Args:
+            transactions(list): transactions
+            resources(list(str)):  resources to use
+            deadlock(bool): wether or not a deadlock should occur
+        """
         dif_act = [
             op for op in self.first_locks(False, []) if op.tx_number != transaction
         ]
         if no_waiting:
             return [
                 op
                 for op in dif_act
                 if op.tx_number not in self.all_trans_waiting_on()
                 and op.tx_number in self.trans_first_lock(False, False)
             ]
         else:
             return dif_act
 
     def res_not_locked(self) -> list[int]:
-        """Returns resources which are not locked yet"""
+        """Returns resources which are not locked yet (no w/r performed on resource by active/waiting transaction)."""
         return [
             res for res in self.schedule.resources if res not in self.res_first_lock()
         ]
 
     def trans_no_lock(self) -> list[int]:
-        """Returns transactions which are not locked yet"""
+        """Returns transactions which are not locked yet
+        - transactions have to be active
+        - transactions have to be waiting on another transaction for some resource
+        """
         return [
             trans
             for trans in self.schedule.active()
             if trans not in self.trans_first_lock(True)
         ]
 
     def trans_first_lock(self, active=False, waiting=False) -> list[int]:
-        """Function returns all transactions which hold a first lock and are active or (if acitve=False(default)) waiting
-        - if waiting: active transactions which are not waiting"""
+        """
+        Function returns all transactions which hold a first lock and are active or waiting
+
+        Args:
+            - active(Bool): optional, only consider active transactions
+            - waiting(Bool): optional, only interesting if active = True:
+                exclude waiting transactions
+        """
         trans_fl = list(set([op.tx_number for op in self.first_locks(False, [])]))
         if active:
             if waiting:
                 return [
                     trans
                     for trans in trans_fl
                     if trans in self.schedule.active() and not self.waiting_on(trans)
@@ -603,48 +733,62 @@
             return [
                 trans
                 for trans in trans_fl
                 if trans in self.schedule.active() or self.waiting_on(trans)
             ]
 
     def res_first_lock(self) -> list[int]:
-        """Function returns resources on which an active trans or the trans is waiting on someone holds a first lock"""
+        """Function returns resources on which an active transaction or the transaction is waiting on someone holds a first lock"""
         return list(
             set(
                 [
                     op.resource
                     for op in self.first_locks(False, [])
                     if op.tx_number in self.schedule.active()
                     or self.waiting_on(op.tx_number)
                 ]
             )
         )
 
     def all_trans_waiting_on(self, circle=False) -> list[int]:
-        """Function which returns all active transactions anyone waits on,
-        - if circle = True: list of lists of all trans who is waiting on who"""
+        """
+        Function which returns all active transactions anyone waits on
+
+        Args:
+            - circle(Bool): optional, return list[lists] instead of all transactions which are waiting on each other
+        """
         waiting = []
         for i in range(1, self.schedule.tx_count + 1):
             if not circle and i not in self.schedule.active():
                 continue
             waiting.append(self.waiting_on(i))
         if circle:
             return waiting
         return list(set([trans for list in waiting for trans in list]))
 
     def waiting_on(self, trans: int) -> list[int]:
-        """Function which returns which transaction the current trans is waiting on"""
+        """Function which returns which transaction the current transaction is waiting on
+
+        Args:
+            - trans(int): transaction to check
+        """
         if self.freed(trans, False, []):
             return []
         waiting = self.perform_waiting(trans, [])
         waiting_indirect = self.indirect_waiting(trans, [])
         return list(set(waiting + waiting_indirect))
 
     def indirect_waiting(self, transaction: int, ignore_trans=[]) -> list:
-        """Function to check which transactions are indirectly waiting on each other"""
+        """
+        Function to check which transactions are indirectly waiting on each other
+
+        Args:
+            - transaction(int): transaction to check (which other transactions it waits on)
+            - ignore_trans(list): optional, transactions to ignore from consideration
+        """
         waiting = []
         altered = False
         for i in [t for t in self.schedule.active() if t != transaction]:
             if (
                 i != self.schedule.operations[-1].tx_number
                 and i not in ignore_trans
                 and [
@@ -660,15 +804,21 @@
         if altered:
             waiting = self.indirect_waiting(transaction, ignore_trans)
         else:
             waiting = self.perform_waiting(transaction, ignore_trans)
         return waiting
 
     def perform_waiting(self, transaction: int, ignore=[]) -> list:
-        """Given the transaction and the locks returns transactions which it is waiting on"""
+        """
+        Given the transaction and the locks returns transactions which it is waiting on
+
+        Args:
+            - transaction(int): transaction to check which other transactions it works on
+            - ignore(list): optional, transaction which are assumed to be concluded in the schedule
+        """
         first_locks = self.first_locks(True, ignore)
         _, unperformed_op = self.performed(ignore)
         waiting = []
         for res in self.schedule.resources:
             if [op for op in unperformed_op if op.tx_number == transaction] and [
                 op for op in unperformed_op if op.tx_number == transaction
             ][
@@ -690,26 +840,37 @@
                 else:  # search for first lock
                     waiting.append(
                         [op for op in first_locks if op.resource == res][0].tx_number
                     )
         return waiting
 
     def circle_deadlock(self, operation=None) -> bool:
-        """Returns True if the schedule contains a deadlock
-        - operation (optional): checks if operation performed deadlock occurs"""
+        """
+        Function to check wether the schedule contains a deadlock.
+        Returns True if the schedule contains a deadlock.
+
+        Args:
+            - operation(Bool): optional, adds the operation to the schedule, and then checks it
+        """
         if operation:
             self.schedule.operations.append(operation)
         waiting_lst = self.all_trans_waiting_on(True)
         if operation:
             self.schedule.operations.pop()
         return self.check_circle(waiting_lst)
 
     def first_locks(self, additional_write=False, add_conclude=[]) -> list:
-        """Returns the first locks on all resources, excluding already performed and freed transactions
-        If optional parameter, include first write locks if available"""
+        """
+        Returns the first locks on all resources, excluding already performed and freed transactions.
+        If optional parameter, include first write locks if available
+
+        Args:
+            - additional_write(Bool): optional, if the first lock is a rl, include the first wl if existing (r1(x) w1(x) include both)
+            - add_conclude(list): optional, assume for those transactions to be committed
+        """
         first_locks = []
         performed, waiting = self.performed(add_conclude)
         for i in self.schedule.operations:
             trans = i.tx_number
             res = i.resource
             if trans in add_conclude and not [
                 op for op in waiting if op.tx_number == trans
@@ -732,15 +893,24 @@
                 and [op for op in performed if op.__same__(i)]
                 and not self.freed(trans, False, add_conclude)
             ):
                 first_locks.append(i)
         return first_locks
 
     def performed(self, add_conclude=[]):
-        """Returns all performed operations up to now and waiting ones"""
+        """
+        Computes which operations from the schedule are performed, and which are waiting
+
+        Args:
+            - add_conclude(list): optional, adds a commit to these schedules
+
+        Return:
+            - list: all performed operations
+            - list: all waiting operations
+        """
         for concl, per in self.performed_l:
             if concl == add_conclude:
                 return per
         all_actions = copy.deepcopy(self.schedule.operations)[:-1]
         terminate = dict()
         for i in self.schedule.commits.keys():
             terminate[self.index_last_op(i)] = i
@@ -766,22 +936,38 @@
             ]
         )
         return [op for op in performed_operations if type(op) == Operation], [
             op for op in wait if type(op) == Operation
         ]
 
     def index_last_op(self, trans: int) -> int:
-        """Function to return the index of the last operation of a transaction, and ignores commits, aborts in the indexing"""
+        """
+        Function to return the index of the last operation of a transaction, and ignores commits, aborts in the indexing
+
+        Args:
+            - trans(int): Transaction to check
+        """
         for ind, i in enumerate(self.schedule.operations, 1):
             if i.tx_number == trans:
                 index = ind
         return max(0, index)
 
     def perform(self, actions: list, locks: list) -> list[list, list, list]:
-        """Function which performs a schedule and returns the executed operations, locks and waiting operations"""
+        """
+        Function which performs a schedule and returns the executed operations, locks and waiting operations
+
+        Args:
+            - actions(list): all operations to check (including a/c)
+            - locks(list): locks set on resources (needed bc it is an recursive function)
+
+        Return:
+            - List: all locks set
+            - List: all waiting operations
+            - List: all performed operations
+        """
         performed_op = []
         waiting = []
         for i in actions:
             if type(i) != int:
                 if not [
                     op
                     for op in locks
@@ -809,15 +995,22 @@
                     for j in performed:
                         performed_op.append(j)
                 else:
                     waiting.append(i)
         return locks, waiting, performed_op
 
     def freed(self, trans: int, test_all_performed=False, ignore=[]) -> bool:
-        """Returns wether a transaction has finished and was able to perform all its operations"""
+        """
+        Returns wether a transaction has finished and was able to perform all its operations
+
+        Args:
+            - trans(int): transaction to check
+            - test_all_performed(bool): optional, to check if all operations of an still active transaction have been performed
+            - ignore(list): optional, other transactions which can be assumed c/a in this process (they dont hold the locks anymore)
+        """
         performed, _ = self.performed(ignore)
         if trans in self.schedule.active() and not test_all_performed:
             return False
         for i in [op for op in self.schedule.operations if op.tx_number == trans]:
             if not [op for op in performed if op.__same__(i)]:
                 return False
         return True
```

### Comparing `dbis-tm-0.0.12/src/dbis_tm/Generate_Tasks.py` & `dbis_tm-1.0.0/src/dbis_tm/Generate_Tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from Generate import generate
-from dbis_tm.Solution_generator import (
-    Perform_conflictgraph,
-    Perform_scheduling,
-    predict_deadlock,
-)
+from src.dbis_tm.Solution_generator import Perform_conflictgraph, Perform_scheduling
 from dbis_tm import Schedule
 from dbis_tm.TMSolver import Serializability, Recovery
 import random
-from IPython.display import display
 
 
 class Generate_Tasks:
     def __init__(self):
         create = Creating()
         self.task1 = create.create_serialibility()
         self.task2 = create.create_recovery()
```

### Comparing `dbis-tm-0.0.12/src/dbis_tm/Solution_generator.py` & `dbis_tm-1.0.0/src/dbis_tm/Solution_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
     Schedule,
     Operation,
     OperationType,
     ConflictGraph,
     ConflictGraphNode,
 )
 from typing import Union
-from graphviz import Digraph
 import copy
 
 
 class Perform_scheduling:
     """
     I am a class which performs the schedulers.
 
@@ -568,15 +567,15 @@
     if is_deadlock != "":
         return True
     return False
 
 
 class Perform_conflictgraph:
     @classmethod
-    def compute_conflict_quantity(cls, schedule: Union[Schedule, str]) -> list:
+    def compute_conflict_quantity(cls, schedule: Union[Schedule, str]) -> set:
         """
         Method to perform the omputing of the conflict set.
         No check for the corectnes of the schedule included. Please check this before using.
         Takes:
         - A schedule
         Reutrns:
         - The conflict set
@@ -613,28 +612,28 @@
                         ):  # no conflict if both are read operations
                             continue
                         conflict_list_dup.append([i, j])
         # discard duplicates
         conflict_list = []
         [conflict_list.append(x) for x in conflict_list_dup if x not in conflict_list]
         # compute string
-        conflict = []
+        conflict = set()
         for [k, l] in conflict_list:
             str1 = k.op_type.value + str(k.tx_number) + "(" + k.resource + ")"
             str2 = l.op_type.value + str(l.tx_number) + "(" + l.resource + ")"
             conflict_tuple = (str1, str2)
-            conflict.append(conflict_tuple)
-            # [("w_3(y)", "w_1(y)"), ("w_1(y)", "r_3(y)"), ("w_1(z)", "w_3(z)"), ("w_1(x)", "r_3(x)")]
+            conflict.add(conflict_tuple)
+            # {("w_3(y)", "w_1(y)"), ("w_1(y)", "r_3(y)"), ("w_1(z)", "w_3(z)"), ("w_1(x)", "r_3(x)")}
         return conflict
 
     @classmethod
-    def compute_conflictgraph(cls, conflict_list: dict) -> ConflictGraph:
+    def compute_conflictgraph(cls, conflict_list: dict, name="") -> ConflictGraph:
         knots = []
         for i in range(1, len(conflict_list) + 1):
             knots.append(ConflictGraphNode(i))
-        graph = ConflictGraph()
+        graph = ConflictGraph(name)
         print("test:", conflict_list)
         for i in conflict_list.keys():
             if conflict_list[i] != set():
                 for k in conflict_list[i]:
                     graph.add_edge(knots[i - 1], knots[k - 1])
         return graph
```

### Comparing `dbis-tm-0.0.12/src/dbis_tm/TM.py` & `dbis_tm-1.0.0/src/dbis_tm/TM.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,15 +102,14 @@
     I am a container for
         a list of operations,
         a set of resources,
         a map of aborts and commits,
         and a count of transactions
     """
 
-    # aborts: key:value (transaction: index)
     def __init__(
         self,
         operations: list[Operation],
         resources: set[str],
         tx_count: int,
         aborts: dict,
         commits: dict,
@@ -196,15 +195,14 @@
         schedule_str = Schedule.sanitize(schedule_str)
 
         parsed_schedule = Schedule([], set(), 0, {}, {})
         tx = set()
         index = 0
         i = 0
         while i < len(schedule_str):
-            start = i
             curr_char = schedule_str[i].lower()
             next_char = schedule_str[i + 1].lower()
 
             if curr_char + next_char in OperationType:
                 operation_type = OperationType(curr_char + next_char)
                 index += 1
                 i += 2
@@ -309,70 +307,94 @@
         Checks whether the two  given schedules do have the same operations.
 
         Gets:
             schedule: 'original' schedule (without locks and unlocks)
             schedule_mod: modified schedule (with locks and unlocks)
 
         Returns:
-            True if those schedules are the same
-            False otherwise
+           bool: True if no problems
+        """
+
+        problems = Schedule.check_operations_same(schedule, mod_schedule)
+        return len(problems) == 0
+
+    @classmethod
+    def check_operations_same(
+        cls, schedule: Union[Schedule, str], mod_schedule: Union[Schedule, str]
+    ) -> list:
+        """
+        Checks whether the two  given schedules do have the same operations.
+
+        Gets:
+            schedule: 'original' schedule (without locks and unlocks)
+            schedule_mod: modified schedule (with locks and unlocks)
+
+        Returns:
+           list of problems
         """
         if isinstance(schedule, str):
             schedule = Schedule.parse_schedule(schedule)
             assert not schedule[1]
             schedule = schedule[0]
         if isinstance(mod_schedule, str):
             mod_schedule = Schedule.parse_schedule(mod_schedule)
             assert not mod_schedule[1]
             mod_schedule = mod_schedule[0]
-
+        problems = []
         org_operations = list(
             filter(
                 lambda op: op.op_type in [OperationType.READ, OperationType.WRITE],
                 mod_schedule.operations,
             )
         )
         for x in org_operations:
             if x in schedule.operations:
                 continue
             else:
-                return False
+                problems.append(x)
         for y in schedule.operations:
             if y in org_operations:
                 continue
             else:
-                return False
+                problems.append(y)
         for i in range(1, schedule.tx_count + 1):
             trans_op_mod = list(
                 filter(
                     lambda op: op.op_type in [OperationType.READ, OperationType.WRITE]
                     and op.tx_number == i,
                     mod_schedule.operations,
                 )
             )
             trans_op_org = list(
                 filter(lambda op: op.tx_number == i, schedule.operations)
             )
             if not (trans_op_mod == trans_op_org):
-                return False
-        return True
+                problems.append(f"{trans_op_mod} != {trans_op_org} at {i}")
+        return problems
 
 
 class ConflictGraph:
     """
     a conflict graph
     """
 
-    def __init__(self):
+    def __init__(self, labelPostfix=""):
+        """
+        constructor
+
+        Args:
+            labelPostfix(str): the postfix for the label to be used
+        """
         self.nodes = set()
         self.edges = set()
+        cglabel = f"Konfliktgraph {labelPostfix}"
         self.digraph = Digraph(
-            "ConflictGraph",
-            "generated by DBIS VL UB 10 TM.ConflictGraph",
-            graph_attr={"label": "Conflict Graph"},
+            "Konfliktgraph",
+            "generiert von DBIS VL UB 8 TM.ConflictGraph",
+            graph_attr={"label": cglabel},
         )
 
     def isEmpty(self):
         return len(self.nodes) == 0
 
     def __eq__(self, obj):
         return (
```

### Comparing `dbis-tm-0.0.12/src/dbis_tm/TMCheck.py` & `dbis_tm-1.0.0/src/dbis_tm/TMCheck.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 @author: Lara
 @author: Marc
 @author: wf
 
 """
 import re
 from dbis_tm import Schedule
-from dbis_tm.TMSolver import Scheduling, Recovery, Serializability
-from dbis_tm.Solution_generator import Perform_conflictgraph
+from src.dbis_tm.TMSolver import Scheduling, Recovery, Serializability
+from src.dbis_tm.Solution_generator import Perform_conflictgraph
 from typing import Union
 from excmanager.scorer import Scorer, SetScorer
 
 
 class ScheduleCheck:
     """
     check the schedule
@@ -23,15 +23,15 @@
     def check(cls, index, schedule, result) -> str:
         """
         check the given schedule against the given result
         """
         msg = None
         s_parsed, s_problem = Schedule.parse_schedule(schedule)
         result_parsed, result_problem = Schedule.parse_schedule(result)
-        problems = Scheduling.check_operations_same(s_parsed, result_parsed)
+        problems = Schedule.check_operations_same(s_parsed, result_parsed)
         if not len(problems) == 0:
             msg = f"schedule_{index} enthält unterschiedliche oder nicht alle Operationen aus s{index}"
         return msg
 
     @classmethod
     def feedback(cls, msg: str, positive: bool):
         """
@@ -55,28 +55,29 @@
         Returns:
             True if no errors occur
         """
         sameProblemCount = 0
         problems = Schedule.is_operations_same(original, schedule)
         if not problems:
             self.feedback(
-                f"schedule has not the same operations as the original.", False
+                f"Der schedule hat nicht die selben Operationen wie der originale Schedule",
+                False,
             )
             sameProblemCount += 1
         else:
-            self.feedback("schedule covers all operations", True)
+            self.feedback("Schedule behinhaltet alle Operationen.", True)
 
         s_parsed, error_parse = Schedule.parse_schedule(schedule_str)
         if error_parse:
             ScheduleCheck.feedback(
-                f"Could not parse schedule due to '{error_parse}'", False
+                f"Das parsen war nicht möglich wegen '{error_parse}'", False
             )
             sameProblemCount += 1
         else:
-            ScheduleCheck.feedback("parse schedule ok", True)
+            ScheduleCheck.feedback("Parsing des Schedules war erfolgreich.", True)
         return sameProblemCount == 0
 
 
 class SyntaxCheck:
     """
     I am an interface for checking the syntax of inputs.
     You should not construct me because I am a stateless interface that merely provides static functions.
@@ -106,25 +107,27 @@
         if schedule == "":
             msg = "Leerer Schedule kann keine Lösung sein"
         if p_count > 1:
             msg = f"Schedule '{schedule}' hat keine korrekte Syntax"
         return msg
 
     @classmethod
-    def check_conf_set_syntax(cls, conf_set: list[tuple[str, str]]) -> str:
+    def check_conf_set_syntax(cls, conf_set: set[tuple[str, str]]) -> str:
         """
         Check syntax of strings in tuple that denotes conflicting operations.
 
         Returns:
             None if input is formatted according to pattern
             or an error message in case a tuple is formatted incorrectly
         """
         tuple_pattern = "[rw][1-3][(][a-z][)]|[rw]_[1-3][(][a-z][)]"
-        if not isinstance(conf_set, list):
-            return f"{conf_set} ist keine Liste"
+        if conf_set == {}:
+            pass
+        elif not isinstance(conf_set, set):
+            return f"{conf_set} ist kein Set"
         for t in conf_set:
             if not len(t) == 2:
                 return f"Das Tupel {t} von {conf_set} ist kein Paar"
             for s in sorted(list(t)):
                 if not re.match(tuple_pattern, s):
                     return f"Das Tupel {t} von {conf_set} hat keine korrekte Syntax"
         return None
@@ -176,15 +179,15 @@
         Returns:
             points
         """
         original_p, original_error = Schedule.parse_schedule(original)
         schedule_p, schedule_error = Schedule.parse_schedule(schedule)
         checkSame = ScheduleCheck.check_same(original_p, schedule_p, schedule)
         if checkSame:
-            check = f"checking '{check_scheduling}' of schedule '{schedule}'"
+            check = f"Prüfe '{check_scheduling}' von Schedule '{schedule}'"
             errors = self.check_schedule(schedule_p, check_scheduling)
             if errors:
                 for error in errors:
                     # just for feedback
                     self.addScore(max_points, check, problem=f"'{error}'")
             else:
                 self.addScore(max_points, check, problem=None)
@@ -192,37 +195,50 @@
 
 
 class ConflictSetScorer:
     """
     scorer for conflict sets
     """
 
-    def removeBlanks(self, result):
+    def removeBlanksandUnderscores(self, result):
         """
         remove blanks and underscores
         """
         resultNoBlanks = {
             (str1.replace(" ", ""), str2.replace(" ", "")) for (str1, str2) in result
         }
         resultNoBlanks = {
             (str1.replace("_", ""), str2.replace("_", "")) for (str1, str2) in result
         }
         return resultNoBlanks
 
-    def score_conflictSet(self, result1, result2, schedule1, schedule2, max_points):
+    def score_conflictSet(
+        self,
+        result1,
+        result2,
+        schedule1: Union[Schedule, set],
+        schedule2: Union[Schedule, set],
+        max_points,
+    ):
         """
         score the given result sets against the given solutions
         """
-        result1 = self.removeBlanks(result1)
-        solution1 = Perform_conflictgraph.compute_conflict_quantity(schedule1)
+        result1 = self.removeBlanksandUnderscores(result1)
+        result2 = self.removeBlanksandUnderscores(result2)
+        if type(schedule1) == set:
+            solution1 = self.removeBlanksandUnderscores(schedule1)
+        else:
+            solution1 = Perform_conflictgraph.compute_conflict_quantity(schedule1)
+        if type(schedule1) == set:
+            solution2 = self.removeBlanksandUnderscores(schedule2)
+        else:
+            solution2 = Perform_conflictgraph.compute_conflict_quantity(schedule2)
         setScorer1 = SetScorer()
-        setScorer1.evaluate_set(result1, solution1, max_points=max_points / 2)
-        result2 = self.removeBlanks(result2)
-        solution2 = Perform_conflictgraph.compute_conflict_quantity(schedule2)
         setScorer2 = SetScorer()
+        setScorer1.evaluate_set(result1, solution1, max_points=max_points / 2)
         setScorer2.evaluate_set(result2, solution2, max_points=max_points / 2)
         score = setScorer1.score + setScorer2.score
         return round(score, 2)
 
 
 class ConflictSerializationScorer(Scorer):
     """
@@ -237,26 +253,28 @@
         """
         points_seri = 0.5
         points_graph = max_points - points_seri
         if points_graph <= 0:
             points_seri = max_points / 2
             points_graph = max_points / 2
         serializable = Serializability.is_serializable(schedule)
-        cgsolution = Perform_conflictgraph.compute_conflictgraph(serializable[1])
+        cgsolution = Perform_conflictgraph.compute_conflictgraph(serializable[1], name)
 
-        serializableCheck = f"check that your result for serializable of {name} {serializableResult} = correct solution serializable {serializable[0]}"
+        serializableCheck = f"Prüfe das Ihre Lösung für die Serialisierung von {name} {serializableResult} = Korrekte Lösung der Serialisierung {serializable[0]}"
         serializableProblem = None
         if serializableResult != serializable[0]:
             serializableProblem = ""
         self.addScore(points_seri, serializableCheck, serializableProblem)
         expectedGraph = str(cgsolution.digraph)
-        conflictGraphCheck = f"check that conflictGraph is '''{expectedGraph}'''"
+        conflictGraphCheck = (
+            f"Prüfe ob der Konfliktgraph folgender ist'''{expectedGraph}'''"
+        )
         conflictGraphProblem = None
         if cgresult != cgsolution:
-            conflictGraphProblem = f"{str(cgresult.digraph)} is different"
+            conflictGraphProblem = f"{str(cgresult.digraph)} ist unterschiedlich"
         self.addScore(points_graph, conflictGraphCheck, conflictGraphProblem)
         return self.score
 
 
 class RecoveryScorer(Scorer):
     """
     a scorer for recovery
@@ -305,46 +323,35 @@
             proofClassSolution(set): the set which proves to be in the class
         """
         negativeProof = False
         problem = None
         proofClass = self.removeBlanksAndUnderScores(proofClass)
         # positive Proof
         if isClassSolution:
-            check = f"{name} is {proofName} with expected proof {proofClassSolution}"
-            # check sets:
-            errors1 = []
-            errors2 = []
-            for i in proofClassSolution:
-                if i not in proofClass:
-                    errors1.append(i)
-            for j in proofClass:
-                if j not in proofClassSolution:
-                    errors2.append(j)
-            if isClassSolution == isClass and len(errors1) == 0 == len(errors2):
+            check = f"{name} ist {proofName} mit erwartetem Beweis {proofClassSolution}"
+            if isClassSolution == isClass and proofClass == proofClassSolution:
                 pass
             else:
-                problem = f"Missing tuples: {errors1},wrong tuples: {errors2}"
+                problem = f"{proofClass}"
             self.addScore(self.points_per_class, check, problem)
         else:
-            check = (
-                f"{name} is not {proofName} with expected proof {proofClassSolution}"
-            )
+            check = f"{name} ist nicht {proofName} mit erwartetem Beweis {proofClassSolution}"
             if isClassSolution == isClass:
                 # get first element of set
                 if len(proofClassSolution) == 0 and len(proofClass) == 0:
                     negativeProof = True
                 else:
                     if len(proofClass) > 0:
                         proofClassItem = tuple(proofClass)[0]
                         negativeProof = (
                             len(proofClass) > 0 and proofClassItem in proofClassSolution
                         )
             if not negativeProof:
                 problem = (
-                    f"your proof {self.setString(proofClass)} is not the expected one"
+                    f"Ihr Beweis {self.setString(proofClass)} ist nicht der erwartete"
                 )
             self.addScore(self.points_per_class, check, problem)
         return negativeProof
 
     def score_recovery(
         self, name: str, schedule: Union[Schedule, str], result, max_score
     ) -> int:
```

### Comparing `dbis-tm-0.0.12/src/dbis_tm/TMSolver.py` & `dbis_tm-1.0.0/src/dbis_tm/TMSolver.py`

 * *Files 5% similar despite different names*

```diff
@@ -343,19 +343,19 @@
                     t
                     for t in locks_compatibility
                     if t.tx_number != i.tx_number and t.resource == i.resource
                 ]
                 # check wether both write
                 if [t for t in conflict if t.op_type == OperationType.WRITE_LOCK]:
                     errors.append(
-                        f"L4: write-lock incompatible with any-lock(s) {i, conflict}"
+                        f"L4: Schreibsperre inkompatibel mit allen andeden Sperren {i, conflict}"
                     )
                 elif conflict and i.op_type == OperationType.WRITE_LOCK:
                     errors.append(
-                        f"L4: write-lock incompatible with read-lock(s) {i, conflict}"
+                        f"L4: Schreibsperre inkompatibel mit Lesesperren {i, conflict}"
                     )
                 else:
                     locks_compatibility.append(i)
             elif (
                 i.op_type == OperationType.READ_UNLOCK
                 or i.op_type == OperationType.WRITE_UNLOCK
             ):
@@ -407,36 +407,38 @@
                     current_op == OperationType.WRITE_LOCK
                     or current_op == OperationType.READ_LOCK
                 ):
                     if representation not in locks_set:
                         locks_set.append(representation)
                         missed_locks.append(representation)
                     else:
-                        errors.append(f"--Double lock: {j}")
+                        errors.append(f"L1/L2: Doppelte Sperre: {j}")
                 elif (
                     current_op == OperationType.WRITE
                     or current_op == OperationType.READ
                 ):
                     if representation not in locks_set:
-                        errors.append(f"--Not locked before using: {j}")
+                        errors.append(f"L2: Nicht gesperrt vor Ausführung: {j}")
                 elif (
                     current_op == OperationType.WRITE_UNLOCK
                     or current_op == OperationType.READ_UNLOCK
                 ):
                     if all_locked:  # all locked?
                         if representation in locks_set:  # already locked?
                             locks_set.remove(representation)
                             missed_locks.remove(representation)
                         else:
-                            errors.append(f"--Not locked before unlocking: {j}")
+                            errors.append(f"L3: Nicht gesperrt vor entsperren: {j}")
                     else:
-                        errors.append(f"2PL: Unlocking before all locks set: {j}")
+                        errors.append(
+                            f"2PL: Entsperren bevor alle anderen Sperren gesetzt sind: {j}"
+                        )
                         missed_locks.remove(representation)
         if missed_locks:
-            errors.append(f"--Not all locks removed: {missed_locks}")
+            errors.append(f"L1: Nicht alle Sperren aufgehoben: {missed_locks}")
         is2PL = not errors
         return is2PL, errors
 
     @classmethod
     def is_C2PL(cls, schedule: Union[Schedule, str]) -> tuple[bool, list[str]]:
         """
         Check whether `schedule` s satisfies conservative 2-phase-locking, i.e., whether the following holds:
@@ -477,15 +479,17 @@
                 locks += [
                     op
                     for op in tx_ops
                     if op.op_type in [OperationType.READ_LOCK, OperationType.WRITE_LOCK]
                     and tx_ops.index(op) > index_first_op
                 ]
         if locks:
-            return False, [f"Lock {locks} was acquired after first r/w operation"]
+            return False, [
+                f"C2PL: Sperren {locks} wurden nach der ersten r/w Operation gesetzt"
+            ]
         return True, []
 
     @classmethod
     def is_S2PL(cls, schedule: Union[Schedule, str]) -> tuple[bool, list[str]]:
         """
         Check whether `schedule` s satisfies strict 2-phase-locking, i.e., whether the following holds:
             satisfies 2-phase-locking && all write locks of a transaction are held until its last operation
@@ -529,18 +533,20 @@
             if final_unlocks[0].index != index_last_op + 1:
                 late_unlocks += [i]
             # have to check wether
             # unlocks after locking all immediately performed
             elif len(final_unlocks) + index_last_op != final_unlocks[-1].index:
                 late_unlocks += [i]
         if early_unlocks:
-            errors += [f"Unlock {early_unlocks} was done before last r/w operation"]
+            errors += [
+                f"S2PL: {early_unlocks} wurden vor der letzten r/w Operation entsperrt"
+            ]
         if late_unlocks:
             errors += [
-                f"Unlocks were not performed immediately after last r/w operation,{late_unlocks}"
+                f"S2PL: Entsperren von {late_unlocks} ist nicht direkt nach der letzten r/w Operation erfolgt"
             ]
         if errors:
             return False, errors
         return True, []
 
     @classmethod
     def is_SS2PL(cls, schedule: Union[Schedule, str]) -> tuple[bool, list[str]]:
@@ -598,14 +604,16 @@
                 index_last_op
                 + len([op for op in tx_unlocks if op.index > index_last_op])
                 != tx_unlocks[-1].index
             ):
                 late_unlocks.append(i)
         if late_unlocks:
             errors.append(
-                f"Unlocks were not performed immediately after last r/w operation,{late_unlocks}"
+                f"SS2PL: Entsperren von {late_unlocks} ist nicht direkt nach der letzten r/w Operation erfolgt"
             )
         if early_unlocks:
-            errors.append(f"Unlock {early_unlocks} was done before last r/w operation")
+            errors.append(
+                f"SS2PL: {early_unlocks} wurde vor der letzten r/w Operation entsperrt"
+            )
         if errors:
             return False, errors
         return True, []
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dbis-tm-0.0.12/src/dbis_tm.egg-info/PKG-INFO` & `dbis_tm-1.0.0/src/dbis_tm.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-tm
-Version: 0.0.12
+Version: 1.0.0
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: DBIS i5 RWTH Aachen <dbis-vl@dbis.rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-tm
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-tm-0.0.12/tests/test_generator.py` & `dbis_tm-1.0.0/tests/test_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dbis_tm import Schedule
 from dbis_tm.TMSolver import Recovery
 from dbis_tm.Generate import generate
-from dbis_tm.Solution_generator import predict_deadlock
+from src.dbis_tm.Solution_generator import predict_deadlock
 from unittest import TestCase
 import random
 
 
 class TestGenerator(TestCase):
     def valid_schedule(self, schedule: Schedule, transactions, resources):
         """Helper function to assert wether the schedule is valid."""
```

### Comparing `dbis-tm-0.0.12/tests/test_perfomance.py` & `dbis_tm-1.0.0/tests/test_perfomance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dbis_tm import Schedule, OperationType, Operation
 from dbis_tm.TMSolver import Scheduling
-from dbis_tm.Solution_generator import Perform_scheduling, Perform_conflictgraph
+from src.dbis_tm.Solution_generator import Perform_scheduling, Perform_conflictgraph
 from unittest import TestCase
 
 
 class TestPerformer(TestCase):
     test_cases_scheduling = [
         (0, "w_1(z) w_3(y) r_1(x) r_3(z) r_2(y) w_2(z) w_3(x) c_1 c_2 c_3", "", ""),
         (1, "r_1(x) w_3(z) r_2(x) r_1(z) r_3(y) w_1(z) w_2(y) c_1 c_2 c_3", "", ""),
@@ -141,23 +141,23 @@
                 self.assertTrue(Operation.__eq__(k, l))
 
     def test_compute_conflictset(self):
         # A tuple denotes: (schedule, conflictset)
         conflict_schedules = [
             (
                 "w1(x)r2(y)r1(x)r2(x)c1w2(x)c2",
-                [("w1(x)", "r2(x)"), ("w1(x)", "w2(x)"), ("r1(x)", "w2(x)")],
+                {("w1(x)", "r2(x)"), ("w1(x)", "w2(x)"), ("r1(x)", "w2(x)")},
             ),
-            ("w1(x)r2(y)r1(x)r2(x)c1w2(x)a2", []),
-            ("w1(x)r2(y)r1(x)r2(x)a1w2(x)c2", []),
-            ("w1(x)r2(y)r1(x)r2(x)a1w2(x)a2", []),
-            ("w1(a) w3(c) r2(a) a2 r1(c) r3(a) a1 a3", []),
+            ("w1(x)r2(y)r1(x)r2(x)c1w2(x)a2", set()),
+            ("w1(x)r2(y)r1(x)r2(x)a1w2(x)c2", set()),
+            ("w1(x)r2(y)r1(x)r2(x)a1w2(x)a2", set()),
+            ("w1(a) w3(c) r2(a) a2 r1(c) r3(a) a1 a3", set()),
             (
                 "w1(a) w3(c) r2(a) c2 r1(c) r3(a) c1 c3",
-                [("w1(a)", "r2(a)"), ("w1(a)", "r3(a)"), ("w3(c)", "r1(c)")],
+                {("w1(a)", "r2(a)"), ("w1(a)", "r3(a)"), ("w3(c)", "r1(c)")},
             ),
         ]
         for schedule, cset in conflict_schedules:
             solution = Perform_conflictgraph.compute_conflict_quantity(
                 Schedule.parse_schedule(schedule)[0]
             )
             self.assertEqual(
```

### Comparing `dbis-tm-0.0.12/tests/test_ub10Scorer.py` & `dbis_tm-1.0.0/tests/test_ub10Scorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ 
 Created on 2022-07-16
 
 @author: wf
 """
-from dbis_tm.TMCheck import (
+from src.dbis_tm.TMCheck import (
     ConflictSetScorer,
     ConflictSerializationScorer,
     RecoveryScorer,
     ScheduleScorer,
 )
 from dbis_tm import ConflictGraph, ConflictGraphNode
 from tests.scheduletest import ScheduleTest
@@ -40,20 +40,36 @@
                     ("w_3(y)", "r_1(y)"),
                     ("w_3(y)", "w_2(y)"),
                     ("r_1(y)", "w_2(y)"),
                 },
                 "expected": 4.0,
             }
         ]
-        solution1 = "w2(x) r2(x) w1(z) r1(x) w3(y) a3 w2(z) c1 c2 "  # {("w_2(x)", "r_1(x)"), ("w_1(z)", "w_2(z)")}
-        solution2 = "r2(x) w3(x) w1(y) r2(y) w2(y) w3(y) w3(z) w1(z) w2(z) r1(y) w2(y)"
-        # {("r_2(x)", "w_3(x)"),- ("w_1(y)", "r_2(y)"), ("w_1(y)", "w_2(y)"), ("w_1(y)", "w_3(y)"),- ("w_3(z)", "w_1(z)"), ("w_3(z)", "w_2(z)"), ("r_2(y)", "w_3(y)"),
-        #  ("w_2(y)", "w_3(y)"), ("w_2(y)", "r_1(y)"), ("w_1(z)", "w_2(z)"), ("w_3(y)", "r_1(y)"), ("w_3(y)", "w_2(y)"), ("r_1(y)", "w_2(y)")}
+        solution1 = {
+            ("w_2(x)", "r_1(x)"),
+            ("w_1(z)", "w_2(z)"),
+        }  # "w2(x) r2(x) w1(z) r1(x) w3(y) a3 w2(z) c1 c2 "
+        solution2 = {
+            ("r_2(x)", "w_3(x)"),
+            ("w_1(y)", "r_2(y)"),
+            ("w_1(y)", "w_2(y)"),
+            ("w_1(y)", "w_3(y)"),
+            ("w_3(z)", "w_1(z)"),
+            ("w_3(z)", "w_2(z)"),
+            ("r_2(y)", "w_3(y)"),
+            ("w_2(y)", "w_3(y)"),
+            ("w_2(y)", "r_1(y)"),
+            ("w_1(z)", "w_2(z)"),
+            ("w_3(y)", "r_1(y)"),
+            ("w_3(y)", "w_2(y)"),
+            ("r_1(y)", "w_2(y)"),
+        }
+        # "r2(x) w3(x) w1(y) r2(y) w2(y) w3(y) w3(z) w1(z) w2(z) r1(y) w2(y)"
         max_points = 4
-        debug = True
+        debug = False
         for i, example in enumerate(examples):
             result1 = example["result1"]
             result2 = example["result2"]
             expected = example["expected"]
             css = ConflictSetScorer()
             score = css.score_conflictSet(
                 result1, result2, solution1, solution2, max_points
@@ -82,14 +98,18 @@
 
         graph2 = ConflictGraph()
         graph2.add_edge(t1, t3)
         graph2.add_edge(t3, t1)
 
         conf_g3 = ConflictGraph()
         conf_g3.add_edge(t1, t2)
+
+        conf_g4 = ConflictGraph("s5")
+        conf_g4.add_edge(t1, t3)
+        conf_g4.add_edge(t3, t1)
         examples = [
             {
                 "name": "s3",
                 "result": graph1,
                 "serializable": False,
                 "schedule": schedule1,
                 "expected": 1.5,
@@ -104,28 +124,34 @@
             {
                 "name": "s4",
                 "result": graph2,
                 "schedule": schedule2,
                 "serializable": False,
                 "expected": 1.5,
             },
+            {
+                "name": "s5",
+                "result": conf_g4,
+                "schedule": schedule2,
+                "serializable": False,
+                "expected": 1.5,
+            },
         ]
         debug = False
         for i, example in enumerate(examples):
             name = example["name"]
             result = example["result"]
             schedule = example["schedule"]
             expected = example["expected"]
             serializableResult = example["serializable"]
 
             css = ConflictSerializationScorer()
             score = css.score_conflictSerialization(
                 name, result, serializableResult, schedule, 1.5
             )
-            print(score)
             if debug:
                 print(f"{i+1} score: {score} expected: {expected}")
             self.assertEqual(expected, score)
 
     def testRecoveryScorer(self):
         """
         test the recovery scorer
```

### Comparing `dbis-tm-0.0.12/tests/test_ub10TM.py` & `dbis_tm-1.0.0/tests/test_ub10TM.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Created 2022-05
 
 @author: Lara
 @author: Marc
 @author: Wolfgang
 """
 from dbis_tm import Schedule, ConflictGraph, ConflictGraphNode
-from dbis_tm.TMSolver import Recovery, Scheduling, Serializability
-from dbis_tm.TMCheck import SyntaxCheck, ScheduleCheck
+from src.dbis_tm.TMSolver import Recovery, Scheduling, Serializability
+from src.dbis_tm.TMCheck import SyntaxCheck
 from tests.scheduletest import ScheduleTest
 
 
 class TestTM(ScheduleTest):
     """
     tests and playground
     for https://git.rwth-aachen.de/i5/teaching/dbis-digi-2022/-/issues/35
@@ -495,187 +495,212 @@
         ),
     ]
 
     # A tuple denotes: (schedule, (is_2PL,[errors]), (is_C2PL,[errors]), (is_S2PL,[errors]), (is_SS2PL,[errors]))
     scheduling_tests = [
         (
             "r1(y)rl1(y)ru1(y)",  # l1 broken
-            (False, ["--Not locked before using: r1(y)"]),
-            (False, ["--Not locked before using: r1(y)"]),
-            (False, ["--Not locked before using: r1(y)"]),
-            (False, ["--Not locked before using: r1(y)"]),
+            (False, ["L2: Nicht gesperrt vor Ausführung: r1(y)"]),
+            (False, ["L2: Nicht gesperrt vor Ausführung: r1(y)"]),
+            (False, ["L2: Nicht gesperrt vor Ausführung: r1(y)"]),
+            (False, ["L2: Nicht gesperrt vor Ausführung: r1(y)"]),
         ),
         (
             "rl1(y)ru1(y)r1(y)",  # l1 broken
-            (False, ["--Not locked before using: r1(y)"]),
-            (False, ["--Not locked before using: r1(y)"]),
-            (False, ["--Not locked before using: r1(y)"]),
-            (False, ["--Not locked before using: r1(y)"]),
+            (False, ["L2: Nicht gesperrt vor Ausführung: r1(y)"]),
+            (False, ["L2: Nicht gesperrt vor Ausführung: r1(y)"]),
+            (False, ["L2: Nicht gesperrt vor Ausführung: r1(y)"]),
+            (False, ["L2: Nicht gesperrt vor Ausführung: r1(y)"]),
         ),
         (
             "wl1(x)w1(x)r1(y)wu1(x)",  # l2 broken
-            (False, ["--Not locked before using: r1(y)"]),
-            (False, ["--Not locked before using: r1(y)"]),
-            (False, ["--Not locked before using: r1(y)"]),
-            (False, ["--Not locked before using: r1(y)"]),
+            (False, ["L2: Nicht gesperrt vor Ausführung: r1(y)"]),
+            (False, ["L2: Nicht gesperrt vor Ausführung: r1(y)"]),
+            (False, ["L2: Nicht gesperrt vor Ausführung: r1(y)"]),
+            (False, ["L2: Nicht gesperrt vor Ausführung: r1(y)"]),
         ),
         (
             "wl1(x)rl1(y)w1(x)r1(y)ru1(y)ru1(y)wu1(x)",  # l3 broken
-            (False, ["--Not locked before unlocking: ru1(y)"]),
-            (False, ["--Not locked before unlocking: ru1(y)"]),
-            (False, ["--Not locked before unlocking: ru1(y)"]),
-            (False, ["--Not locked before unlocking: ru1(y)"]),
+            (False, ["L3: Nicht gesperrt vor entsperren: ru1(y)"]),
+            (False, ["L3: Nicht gesperrt vor entsperren: ru1(y)"]),
+            (False, ["L3: Nicht gesperrt vor entsperren: ru1(y)"]),
+            (False, ["L3: Nicht gesperrt vor entsperren: ru1(y)"]),
         ),
         (
             "wl1(x)rl1(y)w1(x)r1(y)ru1(y)ru1(z)wu1(x)",  # l3 broken
-            (False, ["--Not locked before unlocking: ru1(z)"]),
-            (False, ["--Not locked before unlocking: ru1(z)"]),
-            (False, ["--Not locked before unlocking: ru1(z)"]),
-            (False, ["--Not locked before unlocking: ru1(z)"]),
+            (False, ["L3: Nicht gesperrt vor entsperren: ru1(z)"]),
+            (False, ["L3: Nicht gesperrt vor entsperren: ru1(z)"]),
+            (False, ["L3: Nicht gesperrt vor entsperren: ru1(z)"]),
+            (False, ["L3: Nicht gesperrt vor entsperren: ru1(z)"]),
         ),
         (
             "wl1(x)rl2(x)r2(x)ru2(x)w1(x)wu1(x)",  # l4 broken
             (
                 False,
-                ["L4: write-lock incompatible with any-lock(s) (rl2(x), [wl1(x)])"],
+                [
+                    "L4: Schreibsperre inkompatibel mit allen andeden Sperren (rl2(x), [wl1(x)])"
+                ],
             ),
             (
                 False,
-                ["L4: write-lock incompatible with any-lock(s) (rl2(x), [wl1(x)])"],
+                [
+                    "L4: Schreibsperre inkompatibel mit allen andeden Sperren (rl2(x), [wl1(x)])"
+                ],
             ),
             (
                 False,
-                ["L4: write-lock incompatible with any-lock(s) (rl2(x), [wl1(x)])"],
+                [
+                    "L4: Schreibsperre inkompatibel mit allen andeden Sperren (rl2(x), [wl1(x)])"
+                ],
             ),
             (
                 False,
-                ["L4: write-lock incompatible with any-lock(s) (rl2(x), [wl1(x)])"],
+                [
+                    "L4: Schreibsperre inkompatibel mit allen andeden Sperren (rl2(x), [wl1(x)])"
+                ],
             ),
         ),
         (
             "rl1(x)wl2(x)r1(x)ru1(x)w2(x)wu2(x)",  # l4 broken
             (
                 False,
-                ["L4: write-lock incompatible with read-lock(s) (wl2(x), [rl1(x)])"],
+                ["L4: Schreibsperre inkompatibel mit Lesesperren (wl2(x), [rl1(x)])"],
             ),
             (
                 False,
-                ["L4: write-lock incompatible with read-lock(s) (wl2(x), [rl1(x)])"],
+                ["L4: Schreibsperre inkompatibel mit Lesesperren (wl2(x), [rl1(x)])"],
             ),
             (
                 False,
-                ["L4: write-lock incompatible with read-lock(s) (wl2(x), [rl1(x)])"],
+                ["L4: Schreibsperre inkompatibel mit Lesesperren (wl2(x), [rl1(x)])"],
             ),
             (
                 False,
-                ["L4: write-lock incompatible with read-lock(s) (wl2(x), [rl1(x)])"],
+                ["L4: Schreibsperre inkompatibel mit Lesesperren (wl2(x), [rl1(x)])"],
             ),
         ),
         (
             "wl1(x)w1(x)r2(e)wu1(x)rl1(y)r1(y)ru1(y)",  # 2PL verletzt
             (
                 False,
                 [
-                    "2PL: Unlocking before all locks set: wu1(x)",
-                    "--Not locked before using: r2(e)",
+                    "2PL: Entsperren bevor alle anderen Sperren gesetzt sind: wu1(x)",
+                    "L2: Nicht gesperrt vor Ausführung: r2(e)",
                 ],
             ),
             (
                 False,
                 [
-                    "2PL: Unlocking before all locks set: wu1(x)",
-                    "--Not locked before using: r2(e)",
+                    "2PL: Entsperren bevor alle anderen Sperren gesetzt sind: wu1(x)",
+                    "L2: Nicht gesperrt vor Ausführung: r2(e)",
                 ],
             ),
             (
                 False,
                 [
-                    "2PL: Unlocking before all locks set: wu1(x)",
-                    "--Not locked before using: r2(e)",
+                    "2PL: Entsperren bevor alle anderen Sperren gesetzt sind: wu1(x)",
+                    "L2: Nicht gesperrt vor Ausführung: r2(e)",
                 ],
             ),
             (
                 False,
                 [
-                    "2PL: Unlocking before all locks set: wu1(x)",
-                    "--Not locked before using: r2(e)",
+                    "2PL: Entsperren bevor alle anderen Sperren gesetzt sind: wu1(x)",
+                    "L2: Nicht gesperrt vor Ausführung: r2(e)",
                 ],
             ),
         ),
         (
             "rl2(y)r2(y)wl3(x)w3(x)wl1(z)w1(z)",
-            (False, ["--Not all locks removed: ['r2y', 'w3x', 'w1z']"]),
-            (False, ["--Not all locks removed: ['r2y', 'w3x', 'w1z']"]),
-            (False, ["--Not all locks removed: ['r2y', 'w3x', 'w1z']"]),
-            (False, ["--Not all locks removed: ['r2y', 'w3x', 'w1z']"]),
+            (False, ["L1: Nicht alle Sperren aufgehoben: ['r2y', 'w3x', 'w1z']"]),
+            (False, ["L1: Nicht alle Sperren aufgehoben: ['r2y', 'w3x', 'w1z']"]),
+            (False, ["L1: Nicht alle Sperren aufgehoben: ['r2y', 'w3x', 'w1z']"]),
+            (False, ["L1: Nicht alle Sperren aufgehoben: ['r2y', 'w3x', 'w1z']"]),
         ),
         (
             "rl2(e)wl1(x)w1(x)r2(e)rl1(y)r1(y)ru1(y)wu1(x)ru2(e)",
             (True, []),
-            (False, ["Lock [rl1(y)] was acquired after first r/w operation"]),
             (
                 False,
-                ["Unlocks were not performed immediately after last r/w operation,[2]"],
+                ["C2PL: Sperren [rl1(y)] wurden nach der ersten r/w Operation gesetzt"],
+            ),
+            (
+                False,
+                [
+                    "S2PL: Entsperren von [2] ist nicht direkt nach der letzten r/w Operation erfolgt"
+                ],
             ),
             (
                 False,
-                ["Unlocks were not performed immediately after last r/w operation,[2]"],
+                [
+                    "SS2PL: Entsperren von [2] ist nicht direkt nach der letzten r/w Operation erfolgt"
+                ],
             ),
         ),
         (
             "rl1(x)r1(x)wl3(z)w3(z)rl2(x)r2(x)rl3(y)r3(y)wu3(z)ru3(y)"
             "c3rl1(z)r1(z)wl1(z)ru1(x)ru1(z)w1(z)wu1(z)c1wl2(y)ru2(x)"
             "w2(y)wu2(y)c2",
             (True, []),
             (
                 False,
                 [
-                    "Lock [rl1(z), wl1(z), wl2(y), rl3(y)] was acquired after first r/w operation"
+                    "C2PL: Sperren [rl1(z), wl1(z), wl2(y), rl3(y)] wurden nach der ersten r/w Operation gesetzt"
                 ],
             ),
             (True, []),
             (
                 False,
-                ["Unlock [ru1(x), ru1(z), ru2(x)] was done before last r/w operation"],
+                [
+                    "SS2PL: [ru1(x), ru1(z), ru2(x)] wurde vor der letzten r/w Operation entsperrt"
+                ],
             ),
         ),
         (
             "wl1(x)rl1(y)w1(x)wu1(x)r1(y)ru1(y)",
             (True, []),
             (True, []),
-            (False, ["Unlock [wu1(x)] was done before last r/w operation"]),
-            (False, ["Unlock [wu1(x)] was done before last r/w operation"]),
+            (False, ["S2PL: [wu1(x)] wurden vor der letzten r/w Operation entsperrt"]),
+            (False, ["SS2PL: [wu1(x)] wurde vor der letzten r/w Operation entsperrt"]),
         ),
         (
             "wl1(z)rl1(x)w1(z)wu1(z)r1(x)ru1(x)c1wl3(y)rl3(z)wl3(x)"
             "w3(y)wu3(y)r3(z)ru3(z)rl2(y)wl2(z)r2(y)ru2(y)w2(z)wu2(z)"
             "c2w3(x)wu3(x)c3",
             (True, []),
             (True, []),
-            (False, ["Unlock [wu1(z), wu3(y)] was done before last r/w operation"]),
             (
                 False,
                 [
-                    "Unlock [wu1(z), ru2(y), wu3(y), ru3(z)] was done before last r/w operation"
+                    "S2PL: [wu1(z), wu3(y)] wurden vor der letzten r/w Operation entsperrt"
+                ],
+            ),
+            (
+                False,
+                [
+                    "SS2PL: [wu1(z), ru2(y), wu3(y), ru3(z)] wurde vor der letzten r/w Operation entsperrt"
                 ],
             ),
         ),
         (
             "wl1(x)w1(x)rl1(y)r1(y)ru1(y)wu1(x)",
             (True, []),
-            (False, ["Lock [rl1(y)] was acquired after first r/w operation"]),
+            (
+                False,
+                ["C2PL: Sperren [rl1(y)] wurden nach der ersten r/w Operation gesetzt"],
+            ),
             (True, []),
             (True, []),
         ),
         (
             "wl1(x)rl1(y)r1(y)ru1(y)w1(x)wu1(x)",
             (True, []),
             (True, []),
             (True, []),
-            (False, ["Unlock [ru1(y)] was done before last r/w operation"]),
+            (False, ["SS2PL: [ru1(y)] wurde vor der letzten r/w Operation entsperrt"]),
         ),
         (
             "wl1(x)rl1(y)w1(x)r1(y)ru1(y)wu1(x)",
             (True, []),
             (True, []),
             (True, []),
             (True, []),
@@ -925,61 +950,61 @@
         self.assertTrue(g_1.isEmpty())
         gvMarkup = g_1.get_graphviz_graph()
         debug = False
         if debug:
             print(gvMarkup)
         self.assertTrue(
             """{
-	graph [label="Conflict Graph"]
+	graph [label="Konfliktgraph "]
 }"""
             in str(gvMarkup)
         )
         g_1.add_edge(t1, t2)
         gvMarkup = g_1.get_graphviz_graph()
         if debug:
             print(gvMarkup)
         self.assertTrue("t1 -> t2" in str(gvMarkup))
 
     def testConfSyntaxCheck(self):
         """
         test the SyntaxCheck functionality for Conflicts
         """
-        s1_conf = [("w_2(x)", "r_1(x)"), ("w_1(z)", "w_2(z)")]
-        s2_conf = [
+        s1_conf = {("w_2(x)", "r_1(x)"), ("w_1(z)", "w_2(z)")}
+        s2_conf = {
             ("r_2(x)", "w_3(x)"),
             ("w_1(y)", "r_2(y)"),
             ("w_1(y)", "w_2(y)"),
             ("w_1(y)", "w_3(y)"),
             ("w_3(z)", "w_1(z)"),
             ("w_3(z)", "w_2(z)"),
             ("r_2(y)", "w_3(y)"),
             ("w_2(y)", "w_3(y)"),
             ("w_2(y)", "r_1(y)"),
             ("w_1(z)", "w_2(z)"),
             ("w_3(y)", "r_1(y)"),
             ("w_3(y)", "w_2(y)"),
             ("r_1(y)", "w_2(y)"),
-        ]
-        conf_err1 = {}
-        conf_err2 = []
+        }
+        conf_err1 = []
+        conf_err2 = {}
         conf_err3 = "Garbage"
-        conf_err4 = [("a"), ("b", "c", "e")]
-        conf_err5 = [("a_3(x)", "b")]
+        conf_err4 = {("a"), ("b", "c", "e")}
+        conf_err5 = {("a_3(x)", "b")}
         debug = False
         expectedList = [
             None,
             None,
-            "{} ist keine Liste",
+            "[] ist kein Set",
             None,
-            "Garbage ist keine Liste",
+            "Garbage ist kein Set",
             (
-                "Das Tupel ('b', 'c', 'e') von [('b', 'c', 'e'), 'a'] ist kein Paar",
-                "Das Tupel a von ['a', ('b', 'c', 'e')] ist kein Paar",
+                "Das Tupel ('b', 'c', 'e') von {('b', 'c', 'e'), 'a'} ist kein Paar",
+                "Das Tupel a von {'a', ('b', 'c', 'e')} ist kein Paar",
             ),
-            "Das Tupel ('a_3(x)', 'b') von [('a_3(x)', 'b')] hat keine korrekte Syntax",
+            "Das Tupel ('a_3(x)', 'b') von {('a_3(x)', 'b')} hat keine korrekte Syntax",
         ]
         for i, conf in enumerate(
             [s1_conf, s2_conf, conf_err1, conf_err2, conf_err3, conf_err4, conf_err5]
         ):
             msg = SyntaxCheck.check_conf_set_syntax(conf)
             if debug:
                 print(f"{i}:{msg}", "test")
```

