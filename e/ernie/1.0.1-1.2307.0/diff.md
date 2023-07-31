# Comparing `tmp/ernie-1.0.1-py3-none-any.whl.zip` & `tmp/ernie-1.2307.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 18052 bytes, number of entries: 17
--rw-r--r--  2.0 unx     1054 b- defN 21-Dec-24 15:49 ernie/__init__.py
--rw-r--r--  2.0 unx     2011 b- defN 21-Dec-24 15:49 ernie/aggregation_strategies.py
--rw-r--r--  2.0 unx    13304 b- defN 21-Dec-24 15:49 ernie/ernie.py
--rw-r--r--  2.0 unx     2823 b- defN 21-Dec-24 15:49 ernie/helper.py
--rw-r--r--  2.0 unx     1704 b- defN 21-Dec-24 15:49 ernie/models.py
--rw-r--r--  2.0 unx     4260 b- defN 21-Dec-24 15:49 ernie/split_strategies.py
--rw-r--r--  2.0 unx       87 b- defN 21-Dec-24 15:49 test/__init__.py
--rw-r--r--  2.0 unx     1414 b- defN 21-Dec-24 15:49 test/dump_load.py
--rw-r--r--  2.0 unx      772 b- defN 21-Dec-24 15:49 test/load_csv.py
--rw-r--r--  2.0 unx      936 b- defN 21-Dec-24 15:49 test/load_model.py
--rw-r--r--  2.0 unx      713 b- defN 21-Dec-24 15:49 test/predict.py
--rw-r--r--  2.0 unx    18120 b- defN 21-Dec-24 15:49 test/split_aggregate.py
--rw-r--r--  2.0 unx    11358 b- defN 21-Dec-24 16:05 ernie-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1043 b- defN 21-Dec-24 16:05 ernie-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Dec-24 16:05 ernie-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 21-Dec-24 16:05 ernie-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1280 b- defN 21-Dec-24 16:05 ernie-1.0.1.dist-info/RECORD
-17 files, 60982 bytes uncompressed, 15996 bytes compressed:  73.8%
+Zip file size: 18111 bytes, number of entries: 17
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Jul-31 18:23 ernie/__init__.py
+-rw-rw-r--  2.0 unx     1934 b- defN 23-Jul-31 18:23 ernie/aggregation_strategies.py
+-rw-rw-r--  2.0 unx    13127 b- defN 23-Jul-31 18:23 ernie/ernie.py
+-rw-rw-r--  2.0 unx     2912 b- defN 23-Jul-31 18:23 ernie/helper.py
+-rw-rw-r--  2.0 unx     1758 b- defN 23-Jul-31 18:23 ernie/models.py
+-rw-rw-r--  2.0 unx     4314 b- defN 23-Jul-31 18:23 ernie/split_strategies.py
+-rw-rw-r--  2.0 unx       87 b- defN 23-Jul-31 18:24 test/__init__.py
+-rw-rw-r--  2.0 unx     1414 b- defN 23-Jul-31 18:24 test/dump_load.py
+-rw-rw-r--  2.0 unx      775 b- defN 23-Jul-31 18:24 test/load_csv.py
+-rw-rw-r--  2.0 unx      973 b- defN 23-Jul-31 18:24 test/load_model.py
+-rw-rw-r--  2.0 unx      714 b- defN 23-Jul-31 18:25 test/predict.py
+-rw-rw-r--  2.0 unx    18131 b- defN 23-Jul-31 18:26 test/split_aggregate.py
+-rw-rw-r--  2.0 unx    11358 b- defN 23-Jul-31 18:28 ernie-1.2307.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1016 b- defN 23-Jul-31 18:28 ernie-1.2307.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-31 18:28 ernie-1.2307.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jul-31 18:28 ernie-1.2307.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1295 b- defN 23-Jul-31 18:28 ernie-1.2307.0.dist-info/RECORD
+17 files, 60972 bytes uncompressed, 16025 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: test/predict.py
 Comment: 
 
 Filename: test/split_aggregate.py
 Comment: 
 
-Filename: ernie-1.0.1.dist-info/LICENSE
+Filename: ernie-1.2307.0.dist-info/LICENSE
 Comment: 
 
-Filename: ernie-1.0.1.dist-info/METADATA
+Filename: ernie-1.2307.0.dist-info/METADATA
 Comment: 
 
-Filename: ernie-1.0.1.dist-info/WHEEL
+Filename: ernie-1.2307.0.dist-info/WHEEL
 Comment: 
 
-Filename: ernie-1.0.1.dist-info/top_level.txt
+Filename: ernie-1.2307.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ernie-1.0.1.dist-info/RECORD
+Filename: ernie-1.2307.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ernie/__init__.py

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from .ernie import *  # noqa: F401, F403
 from tensorflow.python.client import device_lib
 import logging
 
-__version__ = '1.0.1'
+__version__ = '1.2307.0'
 
 logging.getLogger().setLevel(logging.WARNING)
 logging.getLogger("transformers.tokenization_utils").setLevel(logging.ERROR)
 logging.basicConfig(
     format='%(asctime)-15s [%(levelname)s] %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S'
 )
 
 
 def _get_cpu_name():
     import cpuinfo
     cpu_info = cpuinfo.get_cpu_info()
-    cpu_name = f"{cpu_info['brand']}, {cpu_info['count']} vCores"
+    cpu_name = f"{cpu_info['brand_raw']}, {cpu_info['count']} vCores"
     return cpu_name
 
 
 def _get_gpu_name():
     gpu_name = \
         device_lib\
         .list_local_devices()[3]\
```

## ernie/aggregation_strategies.py

```diff
@@ -2,19 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from statistics import mean
 
 
 class AggregationStrategy:
     def __init__(
-        self,
-        method,
-        max_items=None,
-        top_items=True,
-        sorting_class_index=1
+        self, method, max_items=None, top_items=True, sorting_class_index=1
     ):
         self.method = method
         self.max_items = max_items
         self.top_items = top_items
         self.sorting_class_index = sorting_class_index
 
     def aggregate(self, softmax_tuples):
@@ -32,39 +28,30 @@
                 reverse=self.top_items
             )
             if self.max_items < len(softmax_dicts):
                 softmax_dicts = softmax_dicts[:self.max_items]
 
         softmax_list = []
         for key in softmax_dicts[0].keys():
-            softmax_list.append(self.method(
-                [probabilities[key] for probabilities in softmax_dicts]))
+            softmax_list.append(
+                self.method(
+                    [probabilities[key] for probabilities in softmax_dicts]
+                )
+            )
         softmax_tuple = tuple(softmax_list)
         return softmax_tuple
 
 
 class AggregationStrategies:
     Mean = AggregationStrategy(method=mean)
     MeanTopFiveBinaryClassification = AggregationStrategy(
-        method=mean,
-        max_items=5,
-        top_items=True,
-        sorting_class_index=1
+        method=mean, max_items=5, top_items=True, sorting_class_index=1
     )
     MeanTopTenBinaryClassification = AggregationStrategy(
-        method=mean,
-        max_items=10,
-        top_items=True,
-        sorting_class_index=1
+        method=mean, max_items=10, top_items=True, sorting_class_index=1
     )
     MeanTopFifteenBinaryClassification = AggregationStrategy(
-        method=mean,
-        max_items=15,
-        top_items=True,
-        sorting_class_index=1
+        method=mean, max_items=15, top_items=True, sorting_class_index=1
     )
     MeanTopTwentyBinaryClassification = AggregationStrategy(
-        method=mean,
-        max_items=20,
-        top_items=True,
-        sorting_class_index=1
+        method=mean, max_items=20, top_items=True, sorting_class_index=1
     )
```

## ernie/ernie.py

```diff
@@ -19,123 +19,124 @@
     SplitStrategies,
     RegexExpressions
 )
 from .aggregation_strategies import (  # noqa: F401
     AggregationStrategy,
     AggregationStrategies
 )
-from .helper import (
-    get_features,
-    softmax,
-    remove_dir,
-    make_dir,
-    copy_dir
-)
+from .helper import (get_features, softmax, remove_dir, make_dir, copy_dir)
 
 AUTOSAVE_PATH = './ernie-autosave/'
 
 
 def clean_autosave():
     remove_dir(AUTOSAVE_PATH)
 
 
 class SentenceClassifier:
-    def __init__(self,
-                 model_name=Models.BertBaseUncased,
-                 model_path=None,
-                 max_length=64,
-                 labels_no=2,
-                 tokenizer_kwargs=None,
-                 model_kwargs=None):
+    def __init__(
+        self,
+        model_name=Models.BertBaseUncased,
+        model_path=None,
+        max_length=64,
+        labels_no=2,
+        tokenizer_kwargs=None,
+        model_kwargs=None,
+    ):
         self._loaded_data = False
         self._model_path = None
 
         if model_kwargs is None:
             model_kwargs = {}
         model_kwargs['num_labels'] = labels_no
 
         if tokenizer_kwargs is None:
             tokenizer_kwargs = {}
         tokenizer_kwargs['max_len'] = max_length
 
         if model_path is not None:
             self._load_local_model(model_path)
         else:
-            self._load_remote_model(model_name, tokenizer_kwargs, model_kwargs)
+            self._load_remote_model(
+                model_name,
+                tokenizer_kwargs,
+                model_kwargs,
+            )
 
     @property
     def model(self):
         return self._model
 
     @property
     def tokenizer(self):
         return self._tokenizer
 
-    def load_dataset(self,
-                     dataframe=None,
-                     validation_split=0.1,
-                     random_state=None,
-                     stratify=None,
-                     csv_path=None,
-                     read_csv_kwargs=None):
+    def load_dataset(
+        self,
+        dataframe=None,
+        validation_split=0.1,
+        random_state=None,
+        stratify=None,
+        csv_path=None,
+        read_csv_kwargs=None,
+    ):
 
         if dataframe is None and csv_path is None:
             raise ValueError
 
         if csv_path is not None:
             dataframe = pd.read_csv(csv_path, **read_csv_kwargs)
 
         sentences = list(dataframe[dataframe.columns[0]])
         labels = dataframe[dataframe.columns[1]].values
 
         (
-            training_sentences,
-            validation_sentences,
-            training_labels,
+            training_sentences, validation_sentences, training_labels,
             validation_labels
         ) = train_test_split(
             sentences,
             labels,
             test_size=validation_split,
             shuffle=True,
             random_state=random_state,
             stratify=stratify
         )
 
         self._training_features = get_features(
-            self._tokenizer, training_sentences, training_labels)
+            self._tokenizer, training_sentences, training_labels
+        )
 
         self._training_size = len(training_sentences)
 
         self._validation_features = get_features(
-            self._tokenizer,
-            validation_sentences,
-            validation_labels
+            self._tokenizer, validation_sentences, validation_labels
         )
         self._validation_split = len(validation_sentences)
 
         logging.info(f'training_size: {self._training_size}')
         logging.info(f'validation_split: {self._validation_split}')
 
         self._loaded_data = True
 
-    def fine_tune(self,
-                  epochs=4,
-                  learning_rate=2e-5,
-                  epsilon=1e-8,
-                  clipnorm=1.0,
-                  optimizer_function=keras.optimizers.Adam,
-                  optimizer_kwargs=None,
-                  loss_function=keras.losses.SparseCategoricalCrossentropy,
-                  loss_kwargs=None,
-                  accuracy_function=keras.metrics.SparseCategoricalAccuracy,
-                  accuracy_kwargs=None,
-                  training_batch_size=32,
-                  validation_batch_size=64,
-                  **kwargs):
+    def fine_tune(
+        self,
+        epochs=4,
+        learning_rate=2e-5,
+        epsilon=1e-8,
+        clipnorm=1.0,
+        optimizer_function=keras.optimizers.Adam,
+        optimizer_kwargs=None,
+        loss_function=keras.losses.SparseCategoricalCrossentropy,
+        loss_kwargs=None,
+        accuracy_function=keras.metrics.SparseCategoricalAccuracy,
+        accuracy_kwargs=None,
+        training_batch_size=32,
+        validation_batch_size=64,
+        **kwargs,
+    ):
         if not self._loaded_data:
             raise Exception('Data has not been loaded.')
 
         if optimizer_kwargs is None:
             optimizer_kwargs = {
                 'learning_rate': learning_rate,
                 'epsilon': epsilon,
@@ -150,58 +151,65 @@
         if accuracy_kwargs is None:
             accuracy_kwargs = {'name': 'accuracy'}
         accuracy = accuracy_function(**accuracy_kwargs)
 
         self._model.compile(optimizer=optimizer, loss=loss, metrics=[accuracy])
 
         training_features = self._training_features.shuffle(
-            self._training_size).batch(training_batch_size).repeat(-1)
+            self._training_size
+        ).batch(training_batch_size).repeat(-1)
         validation_features = self._validation_features.batch(
-            validation_batch_size)
+            validation_batch_size
+        )
 
         training_steps = self._training_size // training_batch_size
         if training_steps == 0:
             training_steps = self._training_size
         logging.info(f'training_steps: {training_steps}')
 
         validation_steps = self._validation_split // validation_batch_size
         if validation_steps == 0:
             validation_steps = self._validation_split
         logging.info(f'validation_steps: {validation_steps}')
 
         for i in range(epochs):
-            self._model.fit(training_features,
-                            epochs=1,
-                            validation_data=validation_features,
-                            steps_per_epoch=training_steps,
-                            validation_steps=validation_steps,
-                            **kwargs)
+            self._model.fit(
+                training_features,
+                epochs=1,
+                validation_data=validation_features,
+                steps_per_epoch=training_steps,
+                validation_steps=validation_steps,
+                **kwargs
+            )
 
         # The fine-tuned model does not have the same input interface
         # after being exported and loaded again.
         self._reload_model()
 
     def predict_one(
         self,
         text,
         split_strategy=None,
-        aggregation_strategy=None
+        aggregation_strategy=None,
     ):
         return next(
-            self.predict([text],
-                         batch_size=1,
-                         split_strategy=split_strategy,
-                         aggregation_strategy=aggregation_strategy))
+            self.predict(
+                [text],
+                batch_size=1,
+                split_strategy=split_strategy,
+                aggregation_strategy=aggregation_strategy,
+            )
+        )
 
     def predict(
         self,
         texts,
         batch_size=32,
         split_strategy=None,
-        aggregation_strategy=None
+        aggregation_strategy=None,
     ):
         if split_strategy is None:
             yield from self._predict_batch(texts, batch_size)
 
         else:
             if aggregation_strategy is None:
                 aggregation_strategy = AggregationStrategies.Mean
@@ -231,15 +239,19 @@
     def _dump(self, path):
         make_dir(path)
         make_dir(path + '/tokenizer')
         self._model.save_pretrained(path)
         self._tokenizer.save_pretrained(path + '/tokenizer')
         self._config.save_pretrained(path + '/tokenizer')
 
-    def _predict_batch(self, sentences: list, batch_size: int):
+    def _predict_batch(
+        self,
+        sentences: list,
+        batch_size: int,
+    ):
         sentences_number = len(sentences)
         if batch_size > sentences_number:
             batch_size = sentences_number
 
         for i in range(0, sentences_number, batch_size):
             input_ids_list = []
             attention_mask_list = []
@@ -248,96 +260,107 @@
             stop_index = stop_index if stop_index < sentences_number \
                 else sentences_number
 
             for j in range(i, stop_index):
                 features = self._tokenizer.encode_plus(
                     sentences[j],
                     add_special_tokens=True,
-                    max_length=self._tokenizer.max_len
+                    max_length=self._tokenizer.model_max_length,
                 )
                 input_ids, _, attention_mask = (
-                    features['input_ids'],
-                    features['token_type_ids'],
+                    features['input_ids'], features['token_type_ids'],
                     features['attention_mask']
                 )
 
                 input_ids = self._list_to_padded_array(features['input_ids'])
                 attention_mask = self._list_to_padded_array(
-                    features['attention_mask'])
+                    features['attention_mask']
+                )
 
                 input_ids_list.append(input_ids)
                 attention_mask_list.append(attention_mask)
 
             input_dict = {
                 'input_ids': np.array(input_ids_list),
                 'attention_mask': np.array(attention_mask_list)
             }
             logit_predictions = self._model.predict_on_batch(input_dict)
             yield from (
-                [softmax(logit_prediction)
-                 for logit_prediction in logit_predictions[0]]
+                [
+                    softmax(logit_prediction)
+                    for logit_prediction in logit_predictions[0]
+                ]
             )
 
     def _list_to_padded_array(self, items):
         array = np.array(items)
-        padded_array = np.zeros(self._tokenizer.max_len, dtype=np.int)
+        padded_array = np.zeros(self._tokenizer.model_max_length, dtype=np.int)
         padded_array[:array.shape[0]] = array
         return padded_array
 
     def _get_temporary_path(self, name=''):
         return f'{AUTOSAVE_PATH}{name}/{int(round(time.time() * 1000))}'
 
     def _reload_model(self):
         self._model_path = self._get_temporary_path(
-            name=self._get_model_family())
+            name=self._get_model_family()
+        )
         self._dump(self._model_path)
         self._load_local_model(self._model_path)
 
     def _load_local_model(self, model_path):
         try:
             self._tokenizer = AutoTokenizer.from_pretrained(
-                model_path + '/tokenizer')
+                model_path + '/tokenizer'
+            )
             self._config = AutoConfig.from_pretrained(
-                model_path + '/tokenizer')
+                model_path + '/tokenizer'
+            )
 
         # Old models didn't use to have a tokenizer folder
         except OSError:
             self._tokenizer = AutoTokenizer.from_pretrained(model_path)
             self._config = AutoConfig.from_pretrained(model_path)
         self._model = TFAutoModelForSequenceClassification.from_pretrained(
-            model_path,
-            from_pt=False
+            model_path, from_pt=False
         )
 
     def _get_model_family(self):
         model_family = ''.join(self._model.name[2:].split('_')[:2])
         return model_family
 
-    def _load_remote_model(self, model_name, tokenizer_kwargs, model_kwargs):
+    def _load_remote_model(
+        self,
+        model_name,
+        tokenizer_kwargs,
+        model_kwargs,
+    ):
         do_lower_case = False
         if 'uncased' in model_name.lower():
             do_lower_case = True
         tokenizer_kwargs.update({'do_lower_case': do_lower_case})
 
         self._tokenizer = AutoTokenizer.from_pretrained(
-            model_name, **tokenizer_kwargs)
+            model_name,
+            **tokenizer_kwargs,
+        )
         self._config = AutoConfig.from_pretrained(model_name)
 
         temporary_path = self._get_temporary_path()
         make_dir(temporary_path)
 
         # TensorFlow model
         try:
             self._model = TFAutoModelForSequenceClassification.from_pretrained(
                 model_name,
-                from_pt=False
+                from_pt=False,
             )
 
         # PyTorch model
-        except TypeError:
+        except OSError:
             try:
                 self._model = \
                     TFAutoModelForSequenceClassification.from_pretrained(
                         model_name,
                         from_pt=True
                     )
 
@@ -364,34 +387,28 @@
                 break
 
         if clean_last_layer:
             try:
                 getattr(self._model, self._get_model_family()
                         ).save_pretrained(temporary_path)
                 self._model = self._model.__class__.from_pretrained(
-                    temporary_path,
-                    from_pt=False,
-                    **model_kwargs
+                    temporary_path, from_pt=False, **model_kwargs
                 )
 
             # The model is itself the main layer
             except AttributeError:
                 # TensorFlow model
                 try:
                     self._model = self._model.__class__.from_pretrained(
-                        model_name,
-                        from_pt=False,
-                        **model_kwargs
+                        model_name, from_pt=False, **model_kwargs
                     )
 
                 # PyTorch Model
                 except (OSError, TypeError):
                     model = AutoModel.from_pretrained(model_name)
                     model.save_pretrained(temporary_path)
                     self._model = self._model.__class__.from_pretrained(
-                        temporary_path,
-                        from_pt=True,
-                        **model_kwargs
+                        temporary_path, from_pt=True, **model_kwargs
                     )
 
         remove_dir(temporary_path)
         assert self._tokenizer and self._model
```

## ernie/helper.py

```diff
@@ -9,32 +9,34 @@
 
 def get_features(tokenizer, sentences, labels):
     features = []
     for i, sentence in enumerate(sentences):
         inputs = tokenizer.encode_plus(
             sentence,
             add_special_tokens=True,
-            max_length=tokenizer.max_len
+            max_length=tokenizer.model_max_length,
         )
-        input_ids, token_type_ids = \
-            inputs['input_ids'], inputs['token_type_ids']
-        padding_length = tokenizer.max_len - len(input_ids)
+        input_ids, token_type_ids = (
+            inputs['input_ids'],
+            inputs['token_type_ids'],
+        )
+        padding_length = tokenizer.model_max_length - len(input_ids)
 
         if tokenizer.padding_side == 'right':
             attention_mask = [1] * len(input_ids) + [0] * padding_length
             input_ids = input_ids + [tokenizer.pad_token_id] * padding_length
             token_type_ids = token_type_ids + \
                 [tokenizer.pad_token_type_id] * padding_length
         else:
             attention_mask = [0] * padding_length + [1] * len(input_ids)
             input_ids = [tokenizer.pad_token_id] * padding_length + input_ids
             token_type_ids = \
                 [tokenizer.pad_token_type_id] * padding_length + token_type_ids
 
-        assert tokenizer.max_len \
+        assert tokenizer.model_max_length \
             == len(attention_mask) \
             == len(input_ids) \
             == len(token_type_ids)
 
         feature = {
             'input_ids': input_ids,
             'attention_mask': attention_mask,
@@ -53,19 +55,21 @@
                     'token_type_ids': feature['token_type_ids'],
                 },
                 feature['label'],
             )
 
     dataset = data.Dataset.from_generator(
         gen,
-        ({
-            'input_ids': int32,
-            'attention_mask': int32,
-            'token_type_ids': int32
-        }, int64),
+        (
+            {
+                'input_ids': int32,
+                'attention_mask': int32,
+                'token_type_ids': int32
+            }, int64
+        ),
         (
             {
                 'input_ids': TensorShape([None]),
                 'attention_mask': TensorShape([None]),
                 'token_type_ids': TensorShape([None]),
             },
             TensorShape([]),
```

## ernie/models.py

```diff
@@ -25,27 +25,32 @@
     AlbertBaseCased2 = 'albert-base-v2'
     AlbertLargeCased2 = 'albert-large-v2'
     AlbertXLargeCased2 = 'albert-xlarge-v2'
     AlbertXXLargeCased2 = 'albert-xxlarge-v2'
 
 
 class ModelsByFamily:
-    Bert = set([Models.BertBaseUncased, Models.BertBaseCased,
-               Models.BertLargeUncased, Models.BertLargeCased])
+    Bert = set(
+        [
+            Models.BertBaseUncased, Models.BertBaseCased,
+            Models.BertLargeUncased, Models.BertLargeCased
+        ]
+    )
     Roberta = set([Models.RobertaBaseCased, Models.RobertaLargeCased])
     XLNet = set([Models.XLNetBaseCased, Models.XLNetLargeCased])
-    DistilBert = set([Models.DistilBertBaseUncased,
-                     Models.DistilBertBaseMultilingualCased])
-    Albert = set([
-        Models.AlbertBaseCased,
-        Models.AlbertLargeCased,
-        Models.AlbertXLargeCased,
-        Models.AlbertXXLargeCased,
-        Models.AlbertBaseCased2,
-        Models.AlbertLargeCased2,
-        Models.AlbertXLargeCased2,
-        Models.AlbertXXLargeCased2
-    ])
-    Supported = set([
-        getattr(Models, model_type) for model_type
-        in filter(lambda x: x[:2] != '__', Models.__dict__.keys())
-    ])
+    DistilBert = set(
+        [Models.DistilBertBaseUncased, Models.DistilBertBaseMultilingualCased]
+    )
+    Albert = set(
+        [
+            Models.AlbertBaseCased, Models.AlbertLargeCased,
+            Models.AlbertXLargeCased, Models.AlbertXXLargeCased,
+            Models.AlbertBaseCased2, Models.AlbertLargeCased2,
+            Models.AlbertXLargeCased2, Models.AlbertXXLargeCased2
+        ]
+    )
+    Supported = set(
+        [
+            getattr(Models, model_type) for model_type in
+            filter(lambda x: x[:2] != '__', Models.__dict__.keys())
+        ]
+    )
```

## ernie/split_strategies.py

```diff
@@ -46,15 +46,15 @@
             split_patterns = self.split_patterns
 
         def len_in_tokens(text_):
             no_tokens = len(tokenizer.encode(text_, add_special_tokens=False))
             return no_tokens
 
         no_special_tokens = len(tokenizer.encode('', add_special_tokens=True))
-        max_tokens = tokenizer.max_len - no_special_tokens
+        max_tokens = tokenizer.model_max_length - no_special_tokens
 
         if self.remove_patterns is not None:
             for remove_pattern in self.remove_patterns:
                 text = re.sub(remove_pattern, '', text).strip()
 
         if len_in_tokens(text) <= max_tokens:
             return [text]
@@ -63,15 +63,16 @@
         splits = map(lambda x: x.strip(), re.findall(split_patterns[0], text))
 
         aggregated_splits = ''
         for split in splits:
             if len_in_tokens(split) > max_tokens:
                 if len(split_patterns) > 1:
                     sub_splits = self.split(
-                        split, tokenizer, split_patterns[1:])
+                        split, tokenizer, split_patterns[1:]
+                    )
                     selected_splits.extend(sub_splits)
                 else:
                     selected_splits.append(split)
 
             else:
                 if not self.group_splits:
                     selected_splits.append(split)
@@ -90,36 +91,36 @@
         remove_too_short_groups = len(selected_splits) > 1 \
             and self.group_splits \
             and self.remove_too_short_groups
 
         if not remove_too_short_groups:
             final_splits = selected_splits
         else:
-            final_splits = []
-            min_length = tokenizer.max_len / 2
+            final_splits
+            min_length = tokenizer.model_max_length / 2
             for split in selected_splits:
                 if len_in_tokens(split) >= min_length:
                     final_splits.append(split)
 
         return final_splits
 
 
 class SplitStrategies:
-    SentencesWithoutUrls = SplitStrategy(split_patterns=[
-        RegexExpressions.split_by_dot,
-        RegexExpressions.split_by_semicolon,
-        RegexExpressions.split_by_colon,
-        RegexExpressions.split_by_comma
-    ],
+    SentencesWithoutUrls = SplitStrategy(
+        split_patterns=[
+            RegexExpressions.split_by_dot, RegexExpressions.split_by_semicolon,
+            RegexExpressions.split_by_colon, RegexExpressions.split_by_comma
+        ],
         remove_patterns=[RegexExpressions.url, RegexExpressions.domain],
         remove_too_short_groups=False,
-        group_splits=False)
+        group_splits=False
+    )
 
-    GroupedSentencesWithoutUrls = SplitStrategy(split_patterns=[
-        RegexExpressions.split_by_dot,
-        RegexExpressions.split_by_semicolon,
-        RegexExpressions.split_by_colon,
-        RegexExpressions.split_by_comma
-    ],
+    GroupedSentencesWithoutUrls = SplitStrategy(
+        split_patterns=[
+            RegexExpressions.split_by_dot, RegexExpressions.split_by_semicolon,
+            RegexExpressions.split_by_colon, RegexExpressions.split_by_comma
+        ],
         remove_patterns=[RegexExpressions.url, RegexExpressions.domain],
         remove_too_short_groups=True,
-        group_splits=True)
+        group_splits=True
+    )
```

## test/load_csv.py

```diff
@@ -5,26 +5,26 @@
 from ernie import SentenceClassifier, Models
 
 
 class TestLoadCsv(unittest.TestCase):
     classifier = SentenceClassifier(
         model_name=Models.BertBaseUncased,
         max_length=128,
-        labels_no=2
+        labels_no=2,
     )
     classifier.load_dataset(
         validation_split=0.2,
         csv_path="example.csv",
-        read_csv_kwargs={"header": None}
+        read_csv_kwargs={"header": None},
     )
     classifier.fine_tune(
         epochs=4,
         learning_rate=2e-5,
         training_batch_size=32,
-        validation_batch_size=64
+        validation_batch_size=64,
     )
 
     def test_predict(self):
         text = "Oh, that's great!"
         prediction = self.classifier.predict_one(text)
         self.assertEqual(len(prediction), 2)
```

## test/load_model.py

```diff
@@ -6,23 +6,30 @@
 from ernie import SentenceClassifier, Models  # noqa: F401
 
 
 class TestLoadModel(unittest.TestCase):
     tuples = [
         ("This is a negative sentence. Everything was wrong today.", 0),
         ("This is a positive example. I'm very happy today.", 1),
-        ("This is a neutral sentence. That's normal.", 2)
+        ("This is a neutral sentence. That's normal.", 2),
     ]
     df = pd.DataFrame(tuples)
 
     classifier = SentenceClassifier(
-        model_name='xlm-roberta-large', max_length=128, labels_no=3)
+        model_name='xlm-roberta-large',
+        max_length=128,
+        labels_no=3,
+    )
     classifier.load_dataset(df, validation_split=0.2)
-    classifier.fine_tune(epochs=4, learning_rate=2e-5,
-                         training_batch_size=32, validation_batch_size=64)
+    classifier.fine_tune(
+        epochs=4,
+        learning_rate=2e-5,
+        training_batch_size=32,
+        validation_batch_size=64,
+    )
 
     def test_predict(self):
         text = "Oh, that's great!"
         prediction = self.classifier.predict_one(text)
         self.assertEqual(len(prediction), 3)
```

## test/predict.py

```diff
@@ -5,15 +5,15 @@
 from ernie import SentenceClassifier, Models
 
 
 class TestPredict(unittest.TestCase):
     classifier = SentenceClassifier(
         model_name=Models.BertBaseUncased,
         max_length=128,
-        labels_no=2
+        labels_no=2,
     )
 
     def test_batch_predict(self):
         sentences_no = 50
         predictions = list(self.classifier.predict(
             ["this is a test " * 100] * sentences_no)
         )
```

## test/split_aggregate.py

```diff
@@ -3,15 +3,15 @@
 
 import unittest
 from ernie import (
     SentenceClassifier,
     Models,
     AggregationStrategy,
     SplitStrategy,
-    RegexExpressions
+    RegexExpressions,
 )
 from statistics import mean
 import logging
 
 
 def round_float_two_decimals(number):
     return int((number * 1000 + 1) / 10) / 100
@@ -62,15 +62,15 @@
 
     def test_split_groups(self):
         splitter = SplitStrategy(
             split_patterns=[
                 RegexExpressions.split_by_dot,
                 RegexExpressions.split_by_semicolon,
                 RegexExpressions.split_by_colon,
-                RegexExpressions.split_by_comma
+                RegexExpressions.split_by_comma,
             ],
             remove_patterns=[RegexExpressions.url, RegexExpressions.domain],
             remove_too_short_groups=False,
             group_splits=True
         )
 
         # 256 tokens + 2 special tokens => no action (single sentence)
@@ -81,51 +81,51 @@
         sentences = splitter.split(sentence, self.classifier.tokenizer)
         self.assertEqual(sentences, expected_sentences)
 
         # 128 tokens + 2 special tokens => 2 tokens exceeded in second group
         sentence = "0. 1. 2. 3. 4. 5. 6. 7. 8. 9. 10. 11. 12. 13. 14. 15. 16. 17. 18. 19. 20. 21. 22. 23. 24. 25. 26. 27. 28. 29. 30. 31. 32. 33. 34. 35. 36. 37. 38. 39. 40. 41. 42. 43. 44. 45. 46. 47. 48. 49. 50. 51. 52. 53. 54. 55. 56. 57. 58. 59. 60. 61. 62. 63."  # noqa: E501
         expected_sentences = [
             "0. 1. 2. 3. 4. 5. 6. 7. 8. 9. 10. 11. 12. 13. 14. 15. 16. 17. 18. 19. 20. 21. 22. 23. 24. 25. 26. 27. 28. 29. 30. 31. 32. 33. 34. 35. 36. 37. 38. 39. 40. 41. 42. 43. 44. 45. 46. 47. 48. 49. 50. 51. 52. 53. 54. 55. 56. 57. 58. 59. 60. 61. 62.",  # noqa: E501
-            "63."
+            "63.",
         ]
         sentences = splitter.split(sentence, self.classifier.tokenizer)
         self.assertEqual(sentences, expected_sentences)
 
         # 128 tokens + 2 special tokens => 2 tokens exceeded in second group
         sentence = "0; 1; 2; 3; 4; 5; 6; 7; 8; 9; 10; 11; 12; 13; 14; 15; 16; 17; 18; 19; 20; 21; 22; 23; 24; 25; 26; 27; 28; 29; 30; 31; 32; 33; 34; 35; 36; 37; 38; 39; 40; 41; 42; 43; 44; 45; 46; 47; 48; 49; 50; 51; 52; 53; 54; 55; 56; 57; 58; 59; 60; 61; 62; 63;"  # noqa: E501
         expected_sentences = [
             "0; 1; 2; 3; 4; 5; 6; 7; 8; 9; 10; 11; 12; 13; 14; 15; 16; 17; 18; 19; 20; 21; 22; 23; 24; 25; 26; 27; 28; 29; 30; 31; 32; 33; 34; 35; 36; 37; 38; 39; 40; 41; 42; 43; 44; 45; 46; 47; 48; 49; 50; 51; 52; 53; 54; 55; 56; 57; 58; 59; 60; 61; 62;",  # noqa: E501
-            "63;"
+            "63;",
         ]
         sentences = splitter.split(sentence, self.classifier.tokenizer)
         self.assertEqual(sentences, expected_sentences)
 
         # 128 tokens + 2 special tokens => 2 tokens exceeded in second group
         sentence = "0: 1: 2: 3: 4: 5: 6: 7: 8: 9: 10: 11: 12: 13: 14: 15: 16: 17: 18: 19: 20: 21: 22: 23: 24: 25: 26: 27: 28: 29: 30: 31: 32: 33: 34: 35: 36: 37: 38: 39: 40: 41: 42: 43: 44: 45: 46: 47: 48: 49: 50: 51: 52: 53: 54: 55: 56: 57: 58: 59: 60: 61: 62: 63: "  # noqa: E501
         expected_sentences = [
             "0: 1: 2: 3: 4: 5: 6: 7: 8: 9: 10: 11: 12: 13: 14: 15: 16: 17: 18: 19: 20: 21: 22: 23: 24: 25: 26: 27: 28: 29: 30: 31: 32: 33: 34: 35: 36: 37: 38: 39: 40: 41: 42: 43: 44: 45: 46: 47: 48: 49: 50: 51: 52: 53: 54: 55: 56: 57: 58: 59: 60: 61: 62:",  # noqa: E501
-            "63:"
+            "63:",
         ]
         sentences = splitter.split(sentence, self.classifier.tokenizer)
         self.assertEqual(sentences, expected_sentences)
 
         # 128 tokens + 2 special tokens => 2 tokens exceeded in second group
         sentence = "0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, "  # noqa: E501
         expected_sentences = [
             "0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62,",  # noqa: E501
-            "63,"
+            "63,",
         ]
         sentences = splitter.split(sentence, self.classifier.tokenizer)
         self.assertEqual(sentences, expected_sentences)
 
         # 128 tokens + 2 special tokens => two groups splitted by the comma
         sentence = "0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63, 64 65 66 67 68 69 70 71 72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95 96 97 98 99 100 101 102 103 104 105 106 107 108 109 110 111 112 113 114 115 116 117 118 119 120 121 122 123 124 125 126 127"  # noqa: E501
         expected_sentences = [
             "0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63,",  # noqa: E501
-            "64 65 66 67 68 69 70 71 72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95 96 97 98 99 100 101 102 103 104 105 106 107 108 109 110 111 112 113 114 115 116 117 118 119 120 121 122 123 124 125 126 127"  # noqa: E501
+            "64 65 66 67 68 69 70 71 72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95 96 97 98 99 100 101 102 103 104 105 106 107 108 109 110 111 112 113 114 115 116 117 118 119 120 121 122 123 124 125 126 127",  # noqa: E501
         ]
         sentences = splitter.split(sentence, self.classifier.tokenizer)
         self.assertEqual(sentences, expected_sentences)
 
         # 128 tokens + 2 special tokens =>
         # two groups splitted by the period and not by the comma
         sentence = "0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15. 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63, 64 65 66 67 68 69 70 71 72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95 96 97 98 99 100 101 102 103 104 105 106 107 108 109 110 111 112 113 114 115 116 117 118 119 120 121 122 123 124 125 126 127"  # noqa: E501
@@ -142,15 +142,15 @@
                 RegexExpressions.split_by_dot,
                 RegexExpressions.split_by_semicolon,
                 RegexExpressions.split_by_colon,
                 RegexExpressions.split_by_comma
             ],
             remove_patterns=[RegexExpressions.url, RegexExpressions.domain],
             remove_too_short_groups=False,
-            group_splits=False
+            group_splits=False,
         )
 
         # 128 tokens + 2 special tokens =>
         # two sentences splitted by the period and not by the comma
         sentence = "0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15. 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63, 64 65 66 67 68 69 70 71 72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95 96 97 98 99 100 101 102 103 104 105 106 107 108 109 110 111 112 113 114 115 116 117 118 119 120 121 122 123 124 125 126 127"  # noqa: E501
         expected_sentences = [
             "0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15.",
@@ -171,39 +171,39 @@
 
         # 256 tokens + 2 special tokens =>
         # three sentences: split first with the period, then with the comma
         sentence = "0 1 2 3 4 5 6, 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71 72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95 96 97 98 99 100 101 102 103 104 105 106 107 108 109 110 111 112 113 114 115 116 117 118 119 120 121 122 123 124 125 126 127. 128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157 158 159 160 161 162 163 164 165 166 167 168 169 170 171 172 173 174 175 176 177 178 179 180 181 182 183 184 185 186 187 188 189 190 191 192 193 194 195 196 197 198 199 200 201 202 203 204 205 206 207 208 209 210 211 212 213 214 215 216 217 218 219 220 221 222 223 224 225 226 227 228 229 230 231 232 233 234 235 236 237 238 239 240 241 242 243 244 245 246 247 248 249 250 251 252 253 254 255"  # noqa: E501
         expected_sentences = [
             "0 1 2 3 4 5 6,",
             "7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71 72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95 96 97 98 99 100 101 102 103 104 105 106 107 108 109 110 111 112 113 114 115 116 117 118 119 120 121 122 123 124 125 126 127.",  # noqa: E501
-            "128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157 158 159 160 161 162 163 164 165 166 167 168 169 170 171 172 173 174 175 176 177 178 179 180 181 182 183 184 185 186 187 188 189 190 191 192 193 194 195 196 197 198 199 200 201 202 203 204 205 206 207 208 209 210 211 212 213 214 215 216 217 218 219 220 221 222 223 224 225 226 227 228 229 230 231 232 233 234 235 236 237 238 239 240 241 242 243 244 245 246 247 248 249 250 251 252 253 254 255"  # noqa: E501
+            "128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157 158 159 160 161 162 163 164 165 166 167 168 169 170 171 172 173 174 175 176 177 178 179 180 181 182 183 184 185 186 187 188 189 190 191 192 193 194 195 196 197 198 199 200 201 202 203 204 205 206 207 208 209 210 211 212 213 214 215 216 217 218 219 220 221 222 223 224 225 226 227 228 229 230 231 232 233 234 235 236 237 238 239 240 241 242 243 244 245 246 247 248 249 250 251 252 253 254 255",  # noqa: E501
         ]
         sentences = splitter.split(sentence, self.classifier.tokenizer)
         self.assertEqual(sentences, expected_sentences)
 
     def test_split_groups_remove_too_short(self):
         splitter = SplitStrategy(
             split_patterns=[
                 RegexExpressions.split_by_dot,
                 RegexExpressions.split_by_semicolon,
                 RegexExpressions.split_by_colon,
-                RegexExpressions.split_by_comma
+                RegexExpressions.split_by_comma,
             ],
             remove_patterns=[RegexExpressions.url, RegexExpressions.domain],
             remove_too_short_groups=True,
             group_splits=True
         )
 
         # 256 tokens + 2 special tokens =>
         # three sentences: split first with the period, then with the comma;
         # remove first group
         sentence = "0 1 2 3 4 5 6, 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71 72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95 96 97 98 99 100 101 102 103 104 105 106 107 108 109 110 111 112 113 114 115 116 117 118 119 120 121 122 123 124 125 126 127. 128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157 158 159 160 161 162 163 164 165 166 167 168 169 170 171 172 173 174 175 176 177 178 179 180 181 182 183 184 185 186 187 188 189 190 191 192 193 194 195 196 197 198 199 200 201 202 203 204 205 206 207 208 209 210 211 212 213 214 215 216 217 218 219 220 221 222 223 224 225 226 227 228 229 230 231 232 233 234 235 236 237 238 239 240 241 242 243 244 245 246 247 248 249 250 251 252 253 254 255"  # noqa: E501
         expected_sentences = [
             "7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71 72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95 96 97 98 99 100 101 102 103 104 105 106 107 108 109 110 111 112 113 114 115 116 117 118 119 120 121 122 123 124 125 126 127.",  # noqa: E501
-            "128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157 158 159 160 161 162 163 164 165 166 167 168 169 170 171 172 173 174 175 176 177 178 179 180 181 182 183 184 185 186 187 188 189 190 191 192 193 194 195 196 197 198 199 200 201 202 203 204 205 206 207 208 209 210 211 212 213 214 215 216 217 218 219 220 221 222 223 224 225 226 227 228 229 230 231 232 233 234 235 236 237 238 239 240 241 242 243 244 245 246 247 248 249 250 251 252 253 254 255"  # noqa: E501
+            "128 129 130 131 132 133 134 135 136 137 138 139 140 141 142 143 144 145 146 147 148 149 150 151 152 153 154 155 156 157 158 159 160 161 162 163 164 165 166 167 168 169 170 171 172 173 174 175 176 177 178 179 180 181 182 183 184 185 186 187 188 189 190 191 192 193 194 195 196 197 198 199 200 201 202 203 204 205 206 207 208 209 210 211 212 213 214 215 216 217 218 219 220 221 222 223 224 225 226 227 228 229 230 231 232 233 234 235 236 237 238 239 240 241 242 243 244 245 246 247 248 249 250 251 252 253 254 255",  # noqa: E501
         ]
         sentences = splitter.split(sentence, self.classifier.tokenizer)
         self.assertEqual(sentences, expected_sentences)
 
 
 if __name__ == '__main__':
     unittest.main()
```

## Comparing `ernie-1.0.1.dist-info/LICENSE` & `ernie-1.2307.0.dist-info/LICENSE`

 * *Files identical despite different names*

