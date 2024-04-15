# Comparing `tmp/nn_wrapper-1.0.4.tar.gz` & `tmp/nn_wrapper-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nn_wrapper-1.0.4.tar", max compression
+gzip compressed data, was "nn_wrapper-1.0.5.tar", max compression
```

## Comparing `nn_wrapper-1.0.4.tar` & `nn_wrapper-1.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2024-04-12 21:11:26.168898 nn_wrapper-1.0.4/LICENSE
--rw-r--r--   0        0        0       42 2024-04-13 23:05:07.771474 nn_wrapper-1.0.4/NetworkWrapper/__init__.py
--rw-r--r--   0        0        0    33458 2024-04-14 12:35:40.302050 nn_wrapper-1.0.4/NetworkWrapper/NetworkWrapper.py
--rw-r--r--   0        0        0      850 2024-04-14 12:33:54.256031 nn_wrapper-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    10313 2024-04-13 23:13:37.978982 nn_wrapper-1.0.4/README.md
--rw-r--r--   0        0        0    11100 1970-01-01 00:00:00.000000 nn_wrapper-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-12 21:11:26.168898 nn_wrapper-1.0.5/LICENSE
+-rw-r--r--   0        0        0       42 2024-04-15 21:21:29.348407 nn_wrapper-1.0.5/NetworkWrapper/__init__.py
+-rw-r--r--   0        0        0    33565 2024-04-15 21:58:13.132032 nn_wrapper-1.0.5/NetworkWrapper/NetworkWrapper.py
+-rw-r--r--   0        0        0      850 2024-04-15 22:01:19.894772 nn_wrapper-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    10313 2024-04-13 23:13:37.978982 nn_wrapper-1.0.5/README.md
+-rw-r--r--   0        0        0    11100 1970-01-01 00:00:00.000000 nn_wrapper-1.0.5/PKG-INFO
```

### Comparing `nn_wrapper-1.0.4/LICENSE` & `nn_wrapper-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nn_wrapper-1.0.4/NetworkWrapper/NetworkWrapper.py` & `nn_wrapper-1.0.5/NetworkWrapper/NetworkWrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,22 +250,21 @@
                                          desc='Fit epoch', ncols=750 if self._colab_view else 75):
             inputs = inputs.float().to(self._device)
             if self._requires_label_encoder:
                 labels = self._label_encoder.transform(labels)
             labels = torch.tensor(labels, dtype=torch.int64).to(self._device)
 
             outputs = self.model(inputs)
-            loss = self.criterion(outputs, labels)
+            loss = self.criterion(outputs, labels).mean()  # .mean() на случай, если у нас сегментация, у которой loss - это вектор
             self.optimizer.zero_grad()
             loss.backward()  # расчитать (вычислить) градиенты, не обновить
             self.optimizer.step()
 
             preds = torch.argmax(outputs, 1)  # выбираем класс с наибольшей вероятностью для каждого объекта батча
-            running_loss += loss.item() * inputs.size(
-                0)  # По умолчанию считается средний loss по батчу. Переводим его в суммарный loss, чтобы потом посчитать средний loss уже по эпохе
+            running_loss += loss.item() * inputs.size(0)  # По умолчанию считается средний loss по батчу. Переводим его в суммарный loss, чтобы потом посчитать средний loss уже по эпохе
             running_corrects += torch.sum(preds == labels.data)
             processed_data += inputs.size(0)
 
         train_loss = running_loss / processed_data
         train_acc = running_corrects.cpu().numpy() / processed_data
         return train_loss, train_acc
```

### Comparing `nn_wrapper-1.0.4/pyproject.toml` & `nn_wrapper-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nn-wrapper"
-version = "1.0.4"
+version = "1.0.5"
 description = "A wrapper class for neural networks that makes working with them easier."
 authors = ["JohnConnor123 <ivan.eudokimoff2014@gmail.com>"]
 readme = "README.md"
 packages = [{include = "NetworkWrapper"}]
 repository = "https://github.com/JohnConnor123/NetworkWrapper"
 
 # poetry config pypi-token.testpypi <API-token>
```

### Comparing `nn_wrapper-1.0.4/README.md` & `nn_wrapper-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nn_wrapper-1.0.4/PKG-INFO` & `nn_wrapper-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nn-wrapper
-Version: 1.0.4
+Version: 1.0.5
 Summary: A wrapper class for neural networks that makes working with them easier.
 Home-page: https://github.com/JohnConnor123/NetworkWrapper
 Author: JohnConnor123
 Author-email: ivan.eudokimoff2014@gmail.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

