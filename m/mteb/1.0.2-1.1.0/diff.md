# Comparing `tmp/mteb-1.0.2.tar.gz` & `tmp/mteb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mteb-1.0.2.tar", last modified: Tue Mar 28 10:26:29 2023, max compression
+gzip compressed data, was "mteb-1.1.0.tar", last modified: Mon Jul 31 08:57:26 2023, max compression
```

## Comparing `mteb-1.0.2.tar` & `mteb-1.1.0.tar`

### file list

```diff
@@ -1,134 +1,149 @@
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.697401 mteb-1.0.2/
--rw-r--r--   0 muennighoff   (501) staff       (20)    11357 2023-03-27 18:13:25.000000 mteb-1.0.2/LICENSE
--rw-r--r--   0 muennighoff   (501) staff       (20)    30488 2023-03-28 10:26:29.697765 mteb-1.0.2/PKG-INFO
--rw-r--r--   0 muennighoff   (501) staff       (20)    29502 2023-03-27 18:13:25.000000 mteb-1.0.2/README.md
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.664274 mteb-1.0.2/mteb/
--rw-r--r--   0 muennighoff   (501) staff       (20)       53 2023-03-28 10:23:54.000000 mteb-1.0.2/mteb/__init__.py
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.668056 mteb-1.0.2/mteb/abstasks/
--rw-r--r--   0 muennighoff   (501) staff       (20)     1890 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/abstasks/AbsTask.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     2144 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/abstasks/AbsTaskBitextMining.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     4740 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/abstasks/AbsTaskClassification.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      771 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/abstasks/AbsTaskClustering.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     1347 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/abstasks/AbsTaskPairClassification.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      820 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/abstasks/AbsTaskReranking.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     7107 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/abstasks/AbsTaskRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     1769 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/abstasks/AbsTaskSTS.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     1982 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/abstasks/AbsTaskSummarization.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     2269 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/abstasks/BeIRTask.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      914 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/abstasks/CrosslingualTask.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      973 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/abstasks/MultilingualTask.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      383 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/abstasks/__init__.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     3955 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/cmd.py
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.668434 mteb-1.0.2/mteb/evaluation/
--rw-r--r--   0 muennighoff   (501) staff       (20)    10644 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/evaluation/MTEB.py
--rw-r--r--   0 muennighoff   (501) staff       (20)       20 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/evaluation/__init__.py
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.671452 mteb-1.0.2/mteb/evaluation/evaluators/
--rw-r--r--   0 muennighoff   (501) staff       (20)     5518 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/evaluation/evaluators/BitextMiningEvaluator.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     8560 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/evaluation/evaluators/ClassificationEvaluator.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     1201 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/evaluation/evaluators/ClusteringEvaluator.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      706 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/evaluation/evaluators/Evaluator.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     7022 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/evaluation/evaluators/PairClassificationEvaluator.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     8374 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/evaluation/evaluators/RerankingEvaluator.py
--rw-r--r--   0 muennighoff   (501) staff       (20)    10438 2023-03-28 10:22:29.000000 mteb-1.0.2/mteb/evaluation/evaluators/RetrievalEvaluator.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     2285 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/evaluation/evaluators/STSEvaluator.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     4548 2023-03-28 10:22:29.000000 mteb-1.0.2/mteb/evaluation/evaluators/SummarizationEvaluator.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      288 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/evaluation/evaluators/__init__.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     1075 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/evaluation/evaluators/utils.py
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.671639 mteb-1.0.2/mteb/tasks/
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.672301 mteb-1.0.2/mteb/tasks/BitextMining/
--rw-r--r--   0 muennighoff   (501) staff       (20)      711 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/BitextMining/BUCCBitextMining.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     2436 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/BitextMining/TatoebaBitextMining.py
--rw-r--r--   0 muennighoff   (501) staff       (20)       67 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/BitextMining/__init__.py
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.674977 mteb-1.0.2/mteb/tasks/Classification/
--rw-r--r--   0 muennighoff   (501) staff       (20)      932 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Classification/AmazonCounterfactualClassification.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      669 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Classification/AmazonPolarityClassification.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      881 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Classification/AmazonReviewsClassification.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      686 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Classification/Banking77Classification.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      915 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Classification/EmotionClassification.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      619 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Classification/ImdbClassification.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      763 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Classification/MTOPDomainClassification.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      763 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Classification/MTOPIntentClassification.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     1473 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Classification/MassiveIntentClassification.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     1479 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Classification/MassiveScenarioClassification.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      960 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Classification/ToxicConversationsClassification.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      756 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Classification/TweetSentimentExtractionClassification.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      517 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Classification/__init__.py
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.677102 mteb-1.0.2/mteb/tasks/Clustering/
--rw-r--r--   0 muennighoff   (501) staff       (20)      779 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Clustering/ArxivClusteringP2P.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      751 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Clustering/ArxivClusteringS2S.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      732 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Clustering/BiorxivClusteringP2P.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      691 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Clustering/BiorxivClusteringS2S.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      732 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Clustering/MedrxivClusteringP2P.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      691 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Clustering/MedrxivClusteringS2S.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      783 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Clustering/RedditClustering.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      791 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Clustering/RedditClusteringP2P.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      822 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Clustering/StackExchangeClustering.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      850 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Clustering/StackExchangeClusteringP2P.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      715 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Clustering/TwentyNewsgroupsClustering.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      402 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Clustering/__init__.py
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.678259 mteb-1.0.2/mteb/tasks/PairClassification/
--rw-r--r--   0 muennighoff   (501) staff       (20)      740 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/PairClassification/SprintDuplicateQuestionsPC.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      717 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/PairClassification/TwitterSemEval2015PC.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      671 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/PairClassification/TwitterURLCorpusPC.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      112 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/PairClassification/__init__.py
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.679686 mteb-1.0.2/mteb/tasks/Reranking/
--rw-r--r--   0 muennighoff   (501) staff       (20)      801 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Reranking/AskUbuntuDupQuestions.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      694 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Reranking/MindSmallReranking.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      656 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Reranking/SciDocsReranking.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      801 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Reranking/StackOverflowDupQuestions.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      144 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Reranking/__init__.py
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.692285 mteb-1.0.2/mteb/tasks/Retrieval/
--rw-r--r--   0 muennighoff   (501) staff       (20)      640 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/ArguAnaRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      694 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackAndroidRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      694 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackEnglishRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      691 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackGamingRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      682 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackGisRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      706 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackMathematicaRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      694 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackPhysicsRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      706 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackProgrammersRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      688 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackStatsRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      682 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackTexRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      685 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackUnixRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      703 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackWebmastersRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      700 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackWordpressRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      774 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/ClimateFEVERRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      692 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/DBPediaRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      804 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/FEVERRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      596 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/FiQA2018Retrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      776 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/HotpotQARetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      691 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/MSMARCORetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      762 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/MSMARCOv2Retrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      653 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/NFCorpusRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      628 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/NQRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      803 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/QuoraRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      755 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/SCIDOCSRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      814 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/SciFactRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      860 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/TRECCOVIDRetrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      644 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/Touche2020Retrieval.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     1001 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/Retrieval/__init__.py
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.696284 mteb-1.0.2/mteb/tasks/STS/
--rw-r--r--   0 muennighoff   (501) staff       (20)      677 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/STS/BiossesSTS.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      646 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/STS/STS12STS.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      643 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/STS/STS13STS.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      675 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/STS/STS14STS.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      638 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/STS/STS15STS.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      638 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/STS/STS16STS.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      796 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/STS/STS17CrosslingualSTS.py
--rw-r--r--   0 muennighoff   (501) staff       (20)     1093 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/STS/STS22CrosslingualSTS.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      724 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/STS/STSBenchmarkSTS.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      683 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/STS/SickrSTS.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      273 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/STS/__init__.py
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.696910 mteb-1.0.2/mteb/tasks/Summarization/
--rw-r--r--   0 muennighoff   (501) staff       (20)      715 2023-03-28 10:22:29.000000 mteb-1.0.2/mteb/tasks/Summarization/SummEvalSummarization.py
--rw-r--r--   0 muennighoff   (501) staff       (20)       57 2023-03-28 10:22:29.000000 mteb-1.0.2/mteb/tasks/Summarization/__init__.py
--rw-r--r--   0 muennighoff   (501) staff       (20)      216 2023-03-27 18:13:25.000000 mteb-1.0.2/mteb/tasks/__init__.py
-drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-03-28 10:26:29.665280 mteb-1.0.2/mteb.egg-info/
--rw-r--r--   0 muennighoff   (501) staff       (20)    30488 2023-03-28 10:26:29.000000 mteb-1.0.2/mteb.egg-info/PKG-INFO
--rw-r--r--   0 muennighoff   (501) staff       (20)     4792 2023-03-28 10:26:29.000000 mteb-1.0.2/mteb.egg-info/SOURCES.txt
--rw-r--r--   0 muennighoff   (501) staff       (20)        1 2023-03-28 10:26:29.000000 mteb-1.0.2/mteb.egg-info/dependency_links.txt
--rw-r--r--   0 muennighoff   (501) staff       (20)       40 2023-03-28 10:26:29.000000 mteb-1.0.2/mteb.egg-info/entry_points.txt
--rw-r--r--   0 muennighoff   (501) staff       (20)      133 2023-03-28 10:26:29.000000 mteb-1.0.2/mteb.egg-info/requires.txt
--rw-r--r--   0 muennighoff   (501) staff       (20)        5 2023-03-28 10:26:29.000000 mteb-1.0.2/mteb.egg-info/top_level.txt
--rw-r--r--   0 muennighoff   (501) staff       (20)      148 2023-03-27 18:13:25.000000 mteb-1.0.2/pyproject.toml
--rw-r--r--   0 muennighoff   (501) staff       (20)      778 2023-03-28 10:26:29.698609 mteb-1.0.2/setup.cfg
--rw-r--r--   0 muennighoff   (501) staff       (20)     3657 2023-03-28 10:24:06.000000 mteb-1.0.2/setup.py
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.970327 mteb-1.1.0/
+-rw-r--r--   0 muennighoff   (501) staff       (20)    11357 2023-07-31 08:55:33.000000 mteb-1.1.0/LICENSE
+-rw-r--r--   0 muennighoff   (501) staff       (20)    70371 2023-07-31 08:57:26.970772 mteb-1.1.0/PKG-INFO
+-rw-r--r--   0 muennighoff   (501) staff       (20)    69385 2023-07-31 08:55:33.000000 mteb-1.1.0/README.md
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.937011 mteb-1.1.0/mteb/
+-rw-r--r--   0 muennighoff   (501) staff       (20)       53 2023-07-31 08:56:26.000000 mteb-1.1.0/mteb/__init__.py
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.940067 mteb-1.1.0/mteb/abstasks/
+-rw-r--r--   0 muennighoff   (501) staff       (20)     1891 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/abstasks/AbsTask.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     2479 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/abstasks/AbsTaskBitextMining.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     4725 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/abstasks/AbsTaskClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      771 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/abstasks/AbsTaskClustering.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     1347 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/abstasks/AbsTaskPairClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      820 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/abstasks/AbsTaskReranking.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     7138 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/abstasks/AbsTaskRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     1769 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/abstasks/AbsTaskSTS.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     1982 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/abstasks/AbsTaskSummarization.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     2240 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/abstasks/BeIRTask.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      913 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/abstasks/CrosslingualTask.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      972 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/abstasks/MultilingualTask.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      383 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/abstasks/__init__.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     3955 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/cmd.py
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.941008 mteb-1.1.0/mteb/evaluation/
+-rw-r--r--   0 muennighoff   (501) staff       (20)    11208 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/evaluation/MTEB.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)       20 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/evaluation/__init__.py
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.950964 mteb-1.1.0/mteb/evaluation/evaluators/
+-rw-r--r--   0 muennighoff   (501) staff       (20)     5517 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/evaluation/evaluators/BitextMiningEvaluator.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     8467 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/evaluation/evaluators/ClassificationEvaluator.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     1215 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/evaluation/evaluators/ClusteringEvaluator.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      708 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/evaluation/evaluators/Evaluator.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     7038 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/evaluation/evaluators/PairClassificationEvaluator.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     8373 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/evaluation/evaluators/RerankingEvaluator.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)    10436 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/evaluation/evaluators/RetrievalEvaluator.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     2300 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/evaluation/evaluators/STSEvaluator.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     4615 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/evaluation/evaluators/SummarizationEvaluator.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      288 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/evaluation/evaluators/__init__.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     1075 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/evaluation/evaluators/utils.py
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.951112 mteb-1.1.0/mteb/tasks/
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.951816 mteb-1.1.0/mteb/tasks/BitextMining/
+-rw-r--r--   0 muennighoff   (501) staff       (20)      711 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/BitextMining/BUCCBitextMining.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     1507 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/BitextMining/BornholmskBitextMining.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     2435 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/BitextMining/TatoebaBitextMining.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      105 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/BitextMining/__init__.py
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.955804 mteb-1.1.0/mteb/tasks/Classification/
+-rw-r--r--   0 muennighoff   (501) staff       (20)      932 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/AmazonCounterfactualClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      669 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/AmazonPolarityClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      880 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/AmazonReviewsClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      796 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/AngryTweetsClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      686 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/Banking77Classification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     1458 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/DKHateClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     2311 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/DalajClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     1412 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/DanishPoliticalCommentsClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      915 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/EmotionClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      619 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/ImdbClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      736 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/LccSentimentClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      762 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/MTOPDomainClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      762 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/MTOPIntentClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     1472 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/MassiveIntentClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     1478 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/MassiveScenarioClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      811 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/NoRecClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     1355 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/NordicLangClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      811 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/NorwegianParliamentClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     5622 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/ScalaClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      808 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/SweRecClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      960 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/ToxicConversationsClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      756 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/TweetSentimentExtractionClassification.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      921 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Classification/__init__.py
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.958217 mteb-1.1.0/mteb/tasks/Clustering/
+-rw-r--r--   0 muennighoff   (501) staff       (20)      779 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/ArxivClusteringP2P.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      751 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/ArxivClusteringS2S.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      732 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/BiorxivClusteringP2P.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      691 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/BiorxivClusteringS2S.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      760 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/BlurbsClusteringP2P.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      753 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/BlurbsClusteringS2S.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      732 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/MedrxivClusteringP2P.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      691 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/MedrxivClusteringS2S.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      783 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/RedditClustering.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      791 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/RedditClusteringP2P.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      822 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/StackExchangeClustering.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      850 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/StackExchangeClusteringP2P.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      728 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/TenKGnadClusteringP2P.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      710 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/TenKGnadClusteringS2S.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      715 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/TwentyNewsgroupsClustering.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      546 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Clustering/__init__.py
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.958747 mteb-1.1.0/mteb/tasks/PairClassification/
+-rw-r--r--   0 muennighoff   (501) staff       (20)      740 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/PairClassification/SprintDuplicateQuestionsPC.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      717 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/PairClassification/TwitterSemEval2015PC.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      671 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/PairClassification/TwitterURLCorpusPC.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      112 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/PairClassification/__init__.py
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.959424 mteb-1.1.0/mteb/tasks/Reranking/
+-rw-r--r--   0 muennighoff   (501) staff       (20)      801 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Reranking/AskUbuntuDupQuestions.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      694 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Reranking/MindSmallReranking.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      656 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Reranking/SciDocsReranking.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      801 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Reranking/StackOverflowDupQuestions.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      144 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Reranking/__init__.py
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.966148 mteb-1.1.0/mteb/tasks/Retrieval/
+-rw-r--r--   0 muennighoff   (501) staff       (20)      640 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/ArguAnaRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      694 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackAndroidRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      694 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackEnglishRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      691 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackGamingRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      682 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackGisRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      706 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackMathematicaRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      694 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackPhysicsRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      706 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackProgrammersRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      688 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackStatsRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      682 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackTexRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      685 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackUnixRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      703 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackWebmastersRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      700 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackWordpressRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      774 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/ClimateFEVERRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      692 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/DBPediaRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      804 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/FEVERRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      596 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/FiQA2018Retrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      776 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/HotpotQARetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      684 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/MSMARCORetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      762 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/MSMARCOv2Retrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      653 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/NFCorpusRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      628 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/NQRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      829 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/QuoraRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      755 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/SCIDOCSRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      814 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/SciFactRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      860 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/TRECCOVIDRetrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      644 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/Touche2020Retrieval.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     1001 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Retrieval/__init__.py
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.969448 mteb-1.1.0/mteb/tasks/STS/
+-rw-r--r--   0 muennighoff   (501) staff       (20)      677 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/STS/BiossesSTS.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      646 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/STS/STS12STS.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      643 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/STS/STS13STS.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      675 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/STS/STS14STS.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      638 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/STS/STS15STS.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      638 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/STS/STS16STS.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      795 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/STS/STS17CrosslingualSTS.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)     1092 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/STS/STS22CrosslingualSTS.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      724 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/STS/STSBenchmarkSTS.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      683 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/STS/SickrSTS.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      273 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/STS/__init__.py
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.970054 mteb-1.1.0/mteb/tasks/Summarization/
+-rw-r--r--   0 muennighoff   (501) staff       (20)      715 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Summarization/SummEvalSummarization.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)       57 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/Summarization/__init__.py
+-rw-r--r--   0 muennighoff   (501) staff       (20)      216 2023-07-31 08:55:33.000000 mteb-1.1.0/mteb/tasks/__init__.py
+drwxr-xr-x   0 muennighoff   (501) staff       (20)        0 2023-07-31 08:57:26.937884 mteb-1.1.0/mteb.egg-info/
+-rw-r--r--   0 muennighoff   (501) staff       (20)    70371 2023-07-31 08:57:26.000000 mteb-1.1.0/mteb.egg-info/PKG-INFO
+-rw-r--r--   0 muennighoff   (501) staff       (20)     5568 2023-07-31 08:57:26.000000 mteb-1.1.0/mteb.egg-info/SOURCES.txt
+-rw-r--r--   0 muennighoff   (501) staff       (20)        1 2023-07-31 08:57:26.000000 mteb-1.1.0/mteb.egg-info/dependency_links.txt
+-rw-r--r--   0 muennighoff   (501) staff       (20)       40 2023-07-31 08:57:26.000000 mteb-1.1.0/mteb.egg-info/entry_points.txt
+-rw-r--r--   0 muennighoff   (501) staff       (20)      133 2023-07-31 08:57:26.000000 mteb-1.1.0/mteb.egg-info/requires.txt
+-rw-r--r--   0 muennighoff   (501) staff       (20)        5 2023-07-31 08:57:26.000000 mteb-1.1.0/mteb.egg-info/top_level.txt
+-rw-r--r--   0 muennighoff   (501) staff       (20)      180 2023-07-31 08:55:33.000000 mteb-1.1.0/pyproject.toml
+-rw-r--r--   0 muennighoff   (501) staff       (20)      778 2023-07-31 08:57:26.972043 mteb-1.1.0/setup.cfg
+-rw-r--r--   0 muennighoff   (501) staff       (20)     3691 2023-07-31 08:55:33.000000 mteb-1.1.0/setup.py
```

### Comparing `mteb-1.0.2/LICENSE` & `mteb-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/abstasks/AbsTask.py` & `mteb-1.1.0/mteb/abstasks/AbsTask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from abc import ABC, abstractmethod
 import random
+from abc import ABC, abstractmethod
 
 import datasets
 import numpy as np
 import torch
 
+
 class AbsTask(ABC):
     def __init__(self, seed=42, **kwargs):
         self.dataset = None
         self.data_loaded = False
         self.is_multilingual = False
         self.is_crosslingual = False
         self.save_suffix = kwargs.get("save_suffix", "")
 
         self.seed = seed
         random.seed(self.seed)
         np.random.seed(self.seed)
         torch.manual_seed(self.seed)
         torch.cuda.manual_seed_all(self.seed)
 
-
     def load_data(self, **kwargs):
         """
         Load dataset from HuggingFace hub
         """
         if self.data_loaded:
             return
 
         # TODO: add split argument
         self.dataset = datasets.load_dataset(
-            self.description["hf_hub_name"], 
-            revision=self.description.get("revision", None)
+            self.description["hf_hub_name"], revision=self.description.get("revision", None)
         )
         self.data_loaded = True
 
+    @property
     @abstractmethod
     def description(self):
         """
         Returns a description of the task. Should contain the following fields:
         name: Name of the task (usually equal to the class name. Should be a valid name for a path on disc)
         description: Longer description & references for the task
         type: Of the set: [sts]
```

### Comparing `mteb-1.0.2/mteb/abstasks/AbsTaskBitextMining.py` & `mteb-1.1.0/mteb/abstasks/AbsTaskBitextMining.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,13 +41,20 @@
             gold = data_split["gold"]
             if len(gold) == 1:
                 gold = gold[0]
             # MTEB currently only loads GOLD labels for BUCC, which is 1-indexed
             # If a 2nd 0-indexed dataset is added, it'd be cleaner to update BUCC on the Hub to be 0-indexed
             gold = [(i - 1, j - 1) for (i, j) in gold]
             assert all(
-                [(i>0) and (j>0) for i,j in gold]
+                [(i > 0) and (j > 0) for i, j in gold]
             ), "Found negative gold indices. This may be caused by MTEB expecting 1-indexed gold labels."
 
         evaluator = BitextMiningEvaluator(sentence1, sentence2, gold, **kwargs)
         metrics = evaluator(model)
+        self._add_main_score(metrics)
         return metrics
+
+    def _add_main_score(self, scores):
+        if self.description["main_score"] in scores:
+            scores["main_score"] = scores[self.description["main_score"]]
+        else:
+            print(f"WARNING: main score {self.description['main_score']} not found in scores {scores.keys()}")
```

### Comparing `mteb-1.0.2/mteb/abstasks/AbsTaskClassification.py` & `mteb-1.1.0/mteb/abstasks/AbsTaskClassification.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-from collections import defaultdict
 import logging
+from collections import defaultdict
 
 import numpy as np
 
 from ..evaluation.evaluators import (
     kNNClassificationEvaluator,
     kNNClassificationEvaluatorPytorch,
     logRegClassificationEvaluator,
 )
 from .AbsTask import AbsTask
 
-
 logger = logging.getLogger(__name__)
 
 
 class AbsTaskClassification(AbsTask):
     """
     Abstract class for kNN classification tasks
     The similarity is computed between pairs and the results are ranked. Average precision
     is computed to measure how well the methods can be used for classification. #TODO:
     """
 
-    def __init__(
-        self, method="logReg", n_experiments=None, samples_per_label=None, k=3, batch_size=32, **kwargs
-    ):
+    def __init__(self, method="logReg", n_experiments=None, samples_per_label=None, k=3, batch_size=32, **kwargs):
         super().__init__(**kwargs)
         self.batch_size = batch_size
         self.method = method
 
         # Bootstrap parameters
         self.n_experiments = n_experiments if n_experiments is not None else self.description.get("n_experiments", 10)
         self.samples_per_label = (
```

### Comparing `mteb-1.0.2/mteb/abstasks/AbsTaskClustering.py` & `mteb-1.1.0/mteb/abstasks/AbsTaskClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/abstasks/AbsTaskPairClassification.py` & `mteb-1.1.0/mteb/abstasks/AbsTaskPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/abstasks/AbsTaskReranking.py` & `mteb-1.1.0/mteb/abstasks/AbsTaskReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/abstasks/AbsTaskRetrieval.py` & `mteb-1.1.0/mteb/abstasks/AbsTaskRetrieval.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import logging
 from time import time
 from typing import Dict, List
 
 import torch.multiprocessing as mp
-
 from sentence_transformers import SentenceTransformer
 
 from .AbsTask import AbsTask
 
-
 logger = logging.getLogger(__name__)
 
 DRES_METHODS = ["encode_queries", "encode_corpus"]
-DRPES_METHODS = ["start_multi_process_pool", "stop_multi_process_pool", "encode_queries", "encode_corpus", "encode_corpus_parallel"]
+DRPES_METHODS = [
+    "start_multi_process_pool",
+    "stop_multi_process_pool",
+    "encode_queries",
+    "encode_corpus",
+    "encode_corpus_parallel",
+]
 
 
 class AbsTaskRetrieval(AbsTask):
     """
     Abstract class for re-ranking experiments.
     Child-classes must implement the following properties:
     self.corpus = Dict[id, Dict[str, str]] #id => dict with document datas like title and text
@@ -28,15 +32,15 @@
         super().__init__(**kwargs)
 
     @staticmethod
     def is_dres_compatible(model, is_parallel=True):
         methods = DRPES_METHODS if is_parallel else DRES_METHODS
         for method in methods:
             op = getattr(model, method, None)
-            if not(callable(op)):
+            if not (callable(op)):
                 return False
         return True
 
     def evaluate(
         self,
         model,
         split="test",
@@ -54,18 +58,20 @@
         if not self.data_loaded:
             self.load_data()
 
         corpus, queries, relevant_docs = self.corpus[split], self.queries[split], self.relevant_docs[split]
 
         try:
             raise ImportError("MTEB is temporarily incompatible with HFDataLoader")
-            
+
             if self.description["beir_name"].startswith("cqadupstack"):
                 raise ImportError("CQADupstack is incompatible with latest BEIR")
-            from beir.retrieval.search.dense import DenseRetrievalParallelExactSearch as DRPES
+            from beir.retrieval.search.dense import (
+                DenseRetrievalParallelExactSearch as DRPES,
+            )
 
             model = model if self.is_dres_compatible(model, is_parallel=True) else DRESModel(model)
 
             model = DRPES(
                 model,
                 batch_size=batch_size,
                 target_devices=target_devices,
@@ -76,15 +82,15 @@
             if target_devices is not None:
                 logger.warning(
                     "DenseRetrievalParallelExactSearch could not be imported from beir. Using DenseRetrievalExactSearch instead."
                 )
                 logger.warning("The parameter target_devices is ignored.")
 
             from beir.retrieval.search.dense import DenseRetrievalExactSearch as DRES
-            
+
             model = model if self.is_dres_compatible(model, is_parallel=False) else DRESModel(model)
 
             model = DRES(
                 model,
                 batch_size=batch_size,
                 corpus_chunk_size=corpus_chunk_size if corpus_chunk_size is not None else 50000,
                 **kwargs,
```

### Comparing `mteb-1.0.2/mteb/abstasks/AbsTaskSTS.py` & `mteb-1.1.0/mteb/abstasks/AbsTaskSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/abstasks/AbsTaskSummarization.py` & `mteb-1.1.0/mteb/abstasks/AbsTaskSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/abstasks/BeIRTask.py` & `mteb-1.1.0/mteb/abstasks/BeIRTask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+
 import datasets
 
 from .AbsTask import AbsTask
 
 
 class BeIRTask(AbsTask):
     def __init__(self, **kwargs):
@@ -16,15 +17,15 @@
             from beir import util
         except ImportError:
             raise Exception("Retrieval tasks require beir package. Please install it with `pip install mteb[beir]`")
 
         USE_BEIR_DEVELOPMENT = False
         try:
             raise ImportError("MTEB is temporarily incompatible with HFDataLoader")
-                              
+
             if self.description["beir_name"].startswith("cqadupstack"):
                 raise ImportError("CQADupstack is incompatible with latest BEIR")
             from beir.datasets.data_loader_hf import HFDataLoader as BeirDataLoader
 
             USE_BEIR_DEVELOPMENT = True
         except ImportError:
             from beir.datasets.data_loader import GenericDataLoader as BeirDataLoader
```

### Comparing `mteb-1.0.2/mteb/abstasks/CrosslingualTask.py` & `mteb-1.1.0/mteb/abstasks/CrosslingualTask.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,12 +19,12 @@
         Load dataset from HuggingFace hub
         """
         if self.data_loaded:
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
-                self.description["hf_hub_name"], 
+                self.description["hf_hub_name"],
                 lang,
                 revision=self.description.get("revision", None),
             )
         self.data_loaded = True
```

### Comparing `mteb-1.0.2/mteb/abstasks/MultilingualTask.py` & `mteb-1.1.0/mteb/abstasks/MultilingualTask.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,12 +19,12 @@
         Load dataset from HuggingFace hub
         """
         if self.data_loaded:
             return
         self.dataset = {}
         for lang in self.langs:
             self.dataset[lang] = datasets.load_dataset(
-                self.description["hf_hub_name"], 
+                self.description["hf_hub_name"],
                 lang,
                 revision=self.description.get("revision", None),
             )
         self.data_loaded = True
```

### Comparing `mteb-1.0.2/mteb/cmd.py` & `mteb-1.1.0/mteb/cmd.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
        --verbosity 3
 """
 
 
 import argparse
 import logging
 
-from mteb import MTEB
 from sentence_transformers import SentenceTransformer
 
+from mteb import MTEB
 
 logging.basicConfig(level=logging.WARNING)
 logger = logging.getLogger(__name__)
 
 
 def main():
     parser = argparse.ArgumentParser()
```

### Comparing `mteb-1.0.2/mteb/evaluation/MTEB.py` & `mteb-1.1.0/mteb/evaluation/MTEB.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 import traceback
 from datetime import datetime
 from time import time
 
 import datasets
 from rich.console import Console
 
+from .. import __version__
 from ..abstasks import *
 from ..tasks import *
-from .. import __version__
-
 
 logger = logging.getLogger(__name__)
 
 
 class MTEB:
     def __init__(
         self,
@@ -52,17 +51,15 @@
         """
         self._task_types = task_types
         self._task_categories = task_categories
         self._version = version
         self._task_langs = task_langs if task_langs is not None else []
         if type(self._task_langs) is str:
             self._task_langs = [self._task_langs]
-        self._task_langs.extend(
-            [f"{x}-{y}" for x in self._task_langs for y in self._task_langs]
-        )  # add all possible pairs
+        self._extend_lang_pairs()  # add all possible pairs
 
         self._tasks = tasks
 
         self.err_logs_path = err_logs_path if err_logs_path is not None else "error_logs.txt"
 
         self.select_tasks(**kwargs)
 
@@ -74,14 +71,26 @@
     def available_task_types(self):
         return set([x.description["type"] for x in self.tasks_cls])
 
     @property
     def available_task_categories(self):
         return set([x.description["category"] for x in self.tasks_cls])
 
+    def _extend_lang_pairs(self):
+        # add all possible language pairs
+        langs = set(self._task_langs)
+        for x in langs:
+            if "-" not in x:
+                for y in langs:
+                    if "-" not in y:
+                        pair = f"{x}-{y}"
+                        if pair not in langs:
+                            self._task_langs.append(pair)
+        return
+
     def _display_tasks(self, task_list, name=None):
         console = Console()
         if name:
             console.rule(f"[bold]{name}\n", style="grey15")
         for task_type in self.available_task_types:
             current_type_tasks = list(filter(lambda x: x.description["type"] == task_type, task_list))
             if len(current_type_tasks) == 0:
@@ -111,15 +120,15 @@
         """
         Get all tasks available in the MTEB.
         """
         instance = cls()
         instance._display_tasks(instance.tasks_cls, name="MTEB tasks")
 
     def print_selected_tasks(self):
-        """ Print the selected tasks. """
+        """Print the selected tasks."""
         self._display_tasks(self.tasks, name="Selected tasks")
 
     def select_tasks(self, **kwargs):
         """
         Select the tasks to be evaluated.
         """
         # Get all existing tasks
@@ -134,16 +143,16 @@
         # If `task_list` is specified, select list of tasks
         if self._tasks is not None:
             self.tasks = list(filter(lambda x: (x.description["name"] in self._tasks), self.tasks_cls))
             if len(self.tasks) != len(self._tasks):
                 tasks_known = set([x.description["name"] for x in self.tasks_cls])
                 tasks_unknown = set(x for x in self._tasks if isinstance(x, str)) - tasks_known
                 if tasks_unknown:
-                    unknown_str, known_str = ','.join(sorted(list(tasks_unknown))), ','.join(sorted(list(tasks_known)))
-                    logger.warn(f"WARNING: Unknown tasks: {unknown_str}. Known tasks: {known_str}.")
+                    unknown_str, known_str = ",".join(sorted(list(tasks_unknown))), ",".join(sorted(list(tasks_known)))
+                    logger.warning(f"WARNING: Unknown tasks: {unknown_str}. Known tasks: {known_str}.")
             # add task if subclass of mteb.tasks
             self.tasks.extend([x for x in self._tasks if isinstance(x, AbsTask)])
             return
 
         # Otherwise use filters to select tasks
         filtered_tasks = filter(
             lambda x: (self._task_types is None) or (x.description["type"] in self._task_types), self.tasks_cls
@@ -153,16 +162,15 @@
             filtered_tasks,
         )
         filtered_tasks = filter(
             lambda x: (self._version is None) or (x.description["version"] >= self._version), filtered_tasks
         )
         # keep only tasks with at least one language in the filter
         filtered_tasks = filter(
-            lambda x: (not(self._task_langs))
-            or (len(set(x.description["eval_langs"]) & set(self._task_langs)) > 0),
+            lambda x: (not (self._task_langs)) or (len(set(x.description["eval_langs"]) & set(self._task_langs)) > 0),
             filtered_tasks,
         )
 
         # Get final list of tasks
         self.tasks = list(filtered_tasks)
 
     def load_tasks_data(self):
@@ -170,30 +178,40 @@
         Load datasets for the selected tasks.
         """
         logger.info(f"\n\n## Loading datasets for {len(self.tasks)} tasks")
         for task in self.tasks:
             logger.info(f"\n# Loading dataset for {task.description['name']}")
             task.load_data()
 
-
-    def run(self, model, verbosity=1, output_folder="results/result", eval_splits=None, overwrite_results=False, **kwargs):
+    def run(
+        self,
+        model,
+        verbosity=1,
+        output_folder="results/result",
+        eval_splits=None,
+        overwrite_results=False,
+        raise_error: bool = True,
+        **kwargs
+    ):
         """
         Run the evaluation pipeline on the selected tasks.
 
         Parameters
         ----------
         model:
             Model to be used for evaluation
         verbosity: int
             Verbosity level. Default is 1.
             0: print tasks tqdm progress bar
             1: print tasks tqdm progress bar and scores
             2: print everything (including datasets loading)
         output_folder: str
             Folder where the results will be saved
+        raise_error: bool
+            Whether to raise an error if an exception occurs during evaluation.
         :return: Returns a dictionary of task names and corresponding metrics results.
         """
         # Set logging
         if verbosity < 2:
             datasets.logging.set_verbosity(40)
             datasets.logging.disable_progress_bar()
 
@@ -209,30 +227,30 @@
             task = self.tasks[0]
             logger.info(f"\n\n********************** Evaluating {task.description['name']} **********************")
 
             # skip evaluation if results folder exists and overwrite_results is False
             if output_folder is not None:
                 save_path = os.path.join(output_folder, f"{task.description['name']}{task.save_suffix}.json")
                 if os.path.exists(save_path) and overwrite_results is False:
-                    logger.warn(f"WARNING: {task.description['name']} results already exists. Skipping.")
+                    logger.warning(f"WARNING: {task.description['name']} results already exists. Skipping.")
                     del self.tasks[0]
                     continue
 
             try:
                 task_eval_splits = eval_splits if eval_splits is not None else task.description.get("eval_splits", [])
 
                 # load data
                 logger.info(f"Loading dataset for {task.description['name']}")
                 task.load_data(eval_splits=task_eval_splits)
 
                 # run evaluation
                 task_results = {
-                    "mteb_version": __version__, 
+                    "mteb_version": __version__,
                     "dataset_revision": task.description.get("revision", None),
-                    "mteb_dataset_name": task.description['name'],
+                    "mteb_dataset_name": task.description["name"],
                 }
                 for split in task_eval_splits:
                     tick = time()
                     results = task.evaluate(model, split, **kwargs)
                     tock = time()
                     logger.info(f"Evaluation for {task.description['name']} on {split} took {tock - tick:.2f} seconds")
                     results["evaluation_time"] = round(tock - tick, 2)
@@ -241,18 +259,20 @@
                         logger.info(f"Scores: {results}")
 
                 # save results
                 if output_folder is not None:
                     with open(save_path, "w") as f_out:
                         json.dump(task_results, f_out, indent=2, sort_keys=True)
 
-                evaluation_results[task.description['name']] = task_results
+                evaluation_results[task.description["name"]] = task_results
 
             except Exception as e:
                 logger.error(f"Error while evaluating {task.description['name']}: {e}")
+                if raise_error:
+                    raise e
                 logger.error(f"Please check all the error logs at: {self.err_logs_path}")
                 with open(self.err_logs_path, "a") as f_out:
                     f_out.write(f"{datetime.now()} >>> {task.description['name']}\n")
                     f_out.write(traceback.format_exc())
                     f_out.write("\n\n")
 
             # empty memory
```

### Comparing `mteb-1.0.2/mteb/evaluation/evaluators/BitextMiningEvaluator.py` & `mteb-1.1.0/mteb/evaluation/evaluators/BitextMiningEvaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import numpy as np
 import torch
 from sklearn.metrics import accuracy_score, f1_score, precision_score, recall_score
 
 from .Evaluator import Evaluator
 from .utils import cos_sim
 
-
 logger = logging.getLogger(__name__)
 
 
 class BitextMiningEvaluator(Evaluator):
     def __init__(self, sentences1, sentences2, gold, batch_size=32, limit=None, **kwargs):
         super().__init__(**kwargs)
         self.gold = gold
```

### Comparing `mteb-1.0.2/mteb/evaluation/evaluators/ClassificationEvaluator.py` & `mteb-1.1.0/mteb/evaluation/evaluators/ClassificationEvaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,19 @@
 from sklearn.linear_model import LogisticRegression
 from sklearn.metrics import accuracy_score, average_precision_score, f1_score
 from sklearn.neighbors import KNeighborsClassifier
 from torch import Tensor
 
 from .Evaluator import Evaluator
 
-
 logger = logging.getLogger(__name__)
 
 
 class kNNClassificationEvaluator(Evaluator):
-    def __init__(
-        self, sentences_train, y_train, sentences_test, y_test, k=1, batch_size=32, limit=None, **kwargs
-    ):
+    def __init__(self, sentences_train, y_train, sentences_test, y_test, k=1, batch_size=32, limit=None, **kwargs):
         super().__init__(**kwargs)
         if limit is not None:
             sentences_train = sentences_train[:limit]
             y_train = y_train[:limit]
             sentences_test = sentences_test[:limit]
             y_test = y_test[:limit]
         self.sentences_train = sentences_train
@@ -62,17 +59,15 @@
         scores["f1"] = max_f1
         if len(np.unique(self.y_train)) == 2:
             scores["ap"] = max_ap
         return scores, test_cache
 
 
 class kNNClassificationEvaluatorPytorch(Evaluator):
-    def __init__(
-        self, sentences_train, y_train, sentences_test, y_test, k=1, batch_size=32, limit=None, **kwargs
-    ):
+    def __init__(self, sentences_train, y_train, sentences_test, y_test, k=1, batch_size=32, limit=None, **kwargs):
         super().__init__(**kwargs)
         if limit is not None:
             sentences_train = sentences_train[:limit]
             y_train = y_train[:limit]
             sentences_test = sentences_test[:limit]
             y_test = y_test[:limit]
 
@@ -184,23 +179,15 @@
             b = b.unsqueeze(0)
 
         return torch.mm(a, b.transpose(0, 1))
 
 
 class logRegClassificationEvaluator(Evaluator):
     def __init__(
-        self,
-        sentences_train,
-        y_train,
-        sentences_test,
-        y_test,
-        max_iter=100,
-        batch_size=32,
-        limit=None,
-        **kwargs
+        self, sentences_train, y_train, sentences_test, y_test, max_iter=100, batch_size=32, limit=None, **kwargs
     ):
         super().__init__(**kwargs)
         if limit is not None:
             sentences_train = sentences_train[:limit]
             y_train = y_train[:limit]
             sentences_test = sentences_test[:limit]
             y_test = y_test[:limit]
```

### Comparing `mteb-1.0.2/mteb/evaluation/evaluators/ClusteringEvaluator.py` & `mteb-1.1.0/mteb/evaluation/evaluators/ClusteringEvaluator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 
 import numpy as np
 import sklearn
 import sklearn.cluster
 
-
 logger = logging.getLogger(__name__)
 
 from .Evaluator import Evaluator
 
 
 class ClusteringEvaluator(Evaluator):
     def __init__(self, sentences, labels, clustering_batch_size=500, limit=None, **kwargs):
@@ -22,15 +21,15 @@
 
     def __call__(self, model):
         logger.info(f"Encoding {len(self.sentences)} sentences...")
         corpus_embeddings = np.asarray(model.encode(self.sentences))
 
         logger.info("Fitting Mini-Batch K-Means model...")
         clustering_model = sklearn.cluster.MiniBatchKMeans(
-            n_clusters=len(set(self.labels)), batch_size=self.clustering_batch_size
+            n_clusters=len(set(self.labels)), batch_size=self.clustering_batch_size, n_init="auto"
         )
         clustering_model.fit(corpus_embeddings)
         cluster_assignment = clustering_model.labels_
 
         logger.info("Evaluating...")
         v_measure = sklearn.metrics.cluster.v_measure_score(self.labels, cluster_assignment)
```

### Comparing `mteb-1.0.2/mteb/evaluation/evaluators/Evaluator.py` & `mteb-1.1.0/mteb/evaluation/evaluators/Evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from abc import ABC, abstractmethod
 import random
+from abc import ABC, abstractmethod
 
 import numpy as np
 import torch
 
+
 class Evaluator(ABC):
     """
     Base class for all evaluators
     Extend this class and implement __call__ for custom evaluators.
     """
+
     def __init__(self, seed=42, **kwargs):
         self.seed = seed
         random.seed(self.seed)
         np.random.seed(self.seed)
         torch.manual_seed(self.seed)
         torch.cuda.manual_seed_all(self.seed)
```

### Comparing `mteb-1.0.2/mteb/evaluation/evaluators/PairClassificationEvaluator.py` & `mteb-1.1.0/mteb/evaluation/evaluators/PairClassificationEvaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import logging
 
 import numpy as np
 from sklearn.metrics import average_precision_score
-from sklearn.metrics.pairwise import paired_cosine_distances, paired_euclidean_distances, paired_manhattan_distances
+from sklearn.metrics.pairwise import (
+    paired_cosine_distances,
+    paired_euclidean_distances,
+    paired_manhattan_distances,
+)
 
 from .Evaluator import Evaluator
 
-
 logger = logging.getLogger(__name__)
 
 
 class PairClassificationEvaluator(Evaluator):
     """
     Evaluate a model based on the similarity of the embeddings by calculating the accuracy of identifying similar and
     dissimilar sentences.
```

### Comparing `mteb-1.0.2/mteb/evaluation/evaluators/RerankingEvaluator.py` & `mteb-1.1.0/mteb/evaluation/evaluators/RerankingEvaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import torch
 import tqdm
 from sklearn.metrics import average_precision_score
 
 from .Evaluator import Evaluator
 from .utils import cos_sim
 
-
 logger = logging.getLogger(__name__)
 
 
 class RerankingEvaluator(Evaluator):
     """
     This class evaluates a SentenceTransformer model for the task of re-ranking.
     Given a query and a list of documents, it computes the score [query, doc_i] for all possible
```

### Comparing `mteb-1.0.2/mteb/evaluation/evaluators/RetrievalEvaluator.py` & `mteb-1.1.0/mteb/evaluation/evaluators/RetrievalEvaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import numpy as np
 import torch
 from tqdm import trange
 
 from .Evaluator import Evaluator
 from .utils import cos_sim, dot_score
 
-
 logger = logging.getLogger(__name__)
 
 
 class RetrievalEvaluator(Evaluator):
     """
     This class evaluates an Information Retrieval (IR) setting.
     Given a set of queries and a large corpus set. It will retrieve for each query the top-k most similar document. It measures
@@ -110,15 +109,14 @@
         for corpus_start_idx in trange(
             0,
             len(self.corpus),
             self.corpus_chunk_size,
             desc="Corpus Chunks",
             disable=not self.show_progress_bar,
         ):
-
             # Encode chunk of corpus
             if corpus_embeddings is None:
                 corpus_end_idx = min(corpus_start_idx + self.corpus_chunk_size, len(self.corpus))
                 sub_corpus_embeddings = corpus_model.encode(
                     self.corpus[corpus_start_idx:corpus_end_idx],
                     show_progress_bar=False,
                     batch_size=self.batch_size,
```

### Comparing `mteb-1.0.2/mteb/evaluation/evaluators/STSEvaluator.py` & `mteb-1.1.0/mteb/evaluation/evaluators/STSEvaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 
 import numpy as np
-from sklearn.metrics.pairwise import paired_cosine_distances, paired_euclidean_distances, paired_manhattan_distances
-
 from scipy.stats import pearsonr, spearmanr
-
+from sklearn.metrics.pairwise import (
+    paired_cosine_distances,
+    paired_euclidean_distances,
+    paired_manhattan_distances,
+)
 
 logger = logging.getLogger(__name__)
 
 from .Evaluator import Evaluator
 
 
 class STSEvaluator(Evaluator):
```

### Comparing `mteb-1.0.2/mteb/evaluation/evaluators/SummarizationEvaluator.py` & `mteb-1.1.0/mteb/evaluation/evaluators/SummarizationEvaluator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import logging
 
 import numpy as np
 import torch
 import tqdm
-
 from scipy.stats import pearsonr, spearmanr
 
 from .utils import cos_sim, dot_score
 
-
 logger = logging.getLogger(__name__)
 
 from .Evaluator import Evaluator
 
 
 class SummarizationEvaluator(Evaluator):
     def __init__(
-        self, 
-        human_summaries=None, 
-        machine_summaries=None, 
-        texts=None, 
-        gold_scores=None, 
-        limit=None, 
-        batch_size=32, 
+        self,
+        human_summaries=None,
+        machine_summaries=None,
+        texts=None,
+        gold_scores=None,
+        limit=None,
+        batch_size=32,
         **kwargs
     ):
         # human_summaries shape: (None, num_human_summaries)
         # machine_summaries shape: (None, num_machine_summaries)
         # gold scores shape: (None, num_machine_summaries)
         # texts: (None,)
         super().__init__(**kwargs)
@@ -38,15 +36,14 @@
         self.human_summaries = human_summaries
         self.machine_summaries = machine_summaries
         self.texts = texts
         self.gold_scores = gold_scores
         self.batch_size = batch_size
 
     def __call__(self, model):
-
         cosine_spearman_scores = []
         cosine_pearson_scores = []
         dot_spearman_scores = []
         dot_pearson_scores = []
 
         # Get the human & machine summaries for the text in one go for all
         human_lens = [len(human_summaries) for human_summaries in self.human_summaries]
@@ -64,33 +61,38 @@
         )
 
         # Split the embeddings into the original human & machine summaries
         embs_human_summaries_all = np.split(embs_human_summaries_all, np.cumsum(human_lens)[:-1])
         embs_machine_summaries_all = np.split(embs_machine_summaries_all, np.cumsum(machine_lens)[:-1])
 
         for i, (embs_human_summaries, embs_machine_summaries) in tqdm.tqdm(
-            enumerate(zip(embs_human_summaries_all, embs_machine_summaries_all)), 
-            desc="Scoring", total=len(self.human_summaries)
+            enumerate(zip(embs_human_summaries_all, embs_machine_summaries_all)),
+            desc="Scoring",
+            total=len(self.human_summaries),
         ):
             cosine_pred_scores = []  # Predicted quality score for a summary
             dot_pred_scores = []  # Predicted quality score for a summary
             human_scores = []  # Human score for a summary
             for emb_machine_summary, human_eval_score in zip(
                 embs_machine_summaries, self.gold_scores[i]
-            ): # Iterate through all machine summaries + scores for a single sample
+            ):  # Iterate through all machine summaries + scores for a single sample
                 cosine_scores = cos_sim(emb_machine_summary, embs_human_summaries)
                 dot_scores = dot_score(emb_machine_summary, embs_human_summaries)
 
                 cosine_max_score = torch.max(cosine_scores).item()
                 cosine_pred_scores.append(cosine_max_score)
                 dot_max_score = torch.max(dot_scores).item()
                 dot_pred_scores.append(dot_max_score)
                 human_scores.append(human_eval_score)
 
-            if (len(set(human_scores)) == 1) or (len(set(dot_pred_scores)) == 1) or (len(set(cosine_pred_scores)) == 1):
+            if (
+                (len(set(human_scores)) == 1)
+                or (len(set(dot_pred_scores)) == 1)
+                or (len(set(cosine_pred_scores)) == 1)
+            ):
                 logger.info(f"Skipping sample {i} due to equal scores")
                 continue
 
             cosine_spearman_scores.append(spearmanr(human_scores, cosine_pred_scores))
             cosine_pearson_scores.append(pearsonr(human_scores, cosine_pred_scores))
             dot_spearman_scores.append(spearmanr(human_scores, dot_pred_scores))
             dot_pearson_scores.append(pearsonr(human_scores, dot_pred_scores))
```

### Comparing `mteb-1.0.2/mteb/evaluation/evaluators/utils.py` & `mteb-1.1.0/mteb/evaluation/evaluators/utils.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/BitextMining/BUCCBitextMining.py` & `mteb-1.1.0/mteb/tasks/BitextMining/BUCCBitextMining.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from ...abstasks import AbsTaskBitextMining, CrosslingualTask
 
-
 _LANGUAGES = ["de-en", "fr-en", "ru-en", "zh-en"]
 
 
 class BUCCBitextMining(AbsTaskBitextMining, CrosslingualTask):
     @property
     def description(self):
         return {
@@ -13,9 +12,9 @@
             "description": "BUCC bitext mining dataset",
             "reference": "https://comparable.limsi.fr/bucc2018/bucc2018-task.html",
             "type": "BitextMining",
             "category": "s2s",
             "eval_splits": ["test"],
             "eval_langs": _LANGUAGES,
             "main_score": "f1",
-            "revision": "d51519689f32196a32af33b075a01d0e7c51e252"
+            "revision": "d51519689f32196a32af33b075a01d0e7c51e252",
         }
```

### Comparing `mteb-1.0.2/mteb/tasks/BitextMining/TatoebaBitextMining.py` & `mteb-1.1.0/mteb/tasks/BitextMining/TatoebaBitextMining.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from ...abstasks import AbsTaskBitextMining, CrosslingualTask
 
-
 _LANGUAGES = [
     "sqi-eng",
     "fry-eng",
     "kur-eng",
     "tur-eng",
     "deu-eng",
     "nld-eng",
```

### Comparing `mteb-1.0.2/mteb/tasks/Classification/AmazonCounterfactualClassification.py` & `mteb-1.1.0/mteb/tasks/Classification/AmazonCounterfactualClassification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from ...abstasks import AbsTaskClassification, MultilingualTask
 
-
 _LANGUAGES = ["en", "de", "en-ext", "ja"]
 
 
 class AmazonCounterfactualClassification(MultilingualTask, AbsTaskClassification):
     @property
     def description(self):
         return {
@@ -17,9 +16,9 @@
             "category": "s2s",
             "type": "Classification",
             "eval_splits": ["validation", "test"],
             "eval_langs": _LANGUAGES,
             "main_score": "accuracy",
             "n_experiments": 10,
             "samples_per_label": 32,
-            "revision": "e8379541af4e31359cca9fbcf4b00f2671dba205"
+            "revision": "e8379541af4e31359cca9fbcf4b00f2671dba205",
         }
```

### Comparing `mteb-1.0.2/mteb/tasks/Classification/AmazonPolarityClassification.py` & `mteb-1.1.0/mteb/tasks/Classification/AmazonPolarityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Classification/AmazonReviewsClassification.py` & `mteb-1.1.0/mteb/tasks/Classification/AmazonReviewsClassification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from ...abstasks import AbsTaskClassification, MultilingualTask
 
-
 _LANGUAGES = ["en", "de", "es", "fr", "ja", "zh"]
 
 
 class AmazonReviewsClassification(MultilingualTask, AbsTaskClassification):
     @property
     def description(self):
         return {
```

### Comparing `mteb-1.0.2/mteb/tasks/Classification/Banking77Classification.py` & `mteb-1.1.0/mteb/tasks/Classification/Banking77Classification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Classification/EmotionClassification.py` & `mteb-1.1.0/mteb/tasks/Classification/EmotionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Classification/ImdbClassification.py` & `mteb-1.1.0/mteb/tasks/Classification/ImdbClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Classification/MTOPDomainClassification.py` & `mteb-1.1.0/mteb/tasks/Classification/MTOPDomainClassification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from ...abstasks import AbsTaskClassification, MultilingualTask
 
-
 _LANGUAGES = ["en", "de", "es", "fr", "hi", "th"]
 
 
 class MTOPDomainClassification(MultilingualTask, AbsTaskClassification):
     @property
     def description(self):
         return {
```

### Comparing `mteb-1.0.2/mteb/tasks/Classification/MTOPIntentClassification.py` & `mteb-1.1.0/mteb/tasks/Classification/MTOPIntentClassification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from ...abstasks import AbsTaskClassification, MultilingualTask
 
-
 _LANGUAGES = ["en", "de", "es", "fr", "hi", "th"]
 
 
 class MTOPIntentClassification(MultilingualTask, AbsTaskClassification):
     @property
     def description(self):
         return {
```

### Comparing `mteb-1.0.2/mteb/tasks/Classification/MassiveIntentClassification.py` & `mteb-1.1.0/mteb/tasks/Classification/MassiveIntentClassification.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from ...abstasks import AbsTaskClassification, MultilingualTask
 
-
 _LANGUAGES = [
     "af",
     "am",
     "ar",
     "az",
     "bn",
     "cy",
```

### Comparing `mteb-1.0.2/mteb/tasks/Classification/MassiveScenarioClassification.py` & `mteb-1.1.0/mteb/tasks/Classification/MassiveScenarioClassification.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from ...abstasks import AbsTaskClassification, MultilingualTask
 
-
 _LANGUAGES = [
     "af",
     "am",
     "ar",
     "az",
     "bn",
     "cy",
```

### Comparing `mteb-1.0.2/mteb/tasks/Classification/ToxicConversationsClassification.py` & `mteb-1.1.0/mteb/tasks/Classification/ToxicConversationsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Classification/TweetSentimentExtractionClassification.py` & `mteb-1.1.0/mteb/tasks/Classification/TweetSentimentExtractionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Classification/__init__.py` & `mteb-1.1.0/mteb/tasks/Classification/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,24 @@
+
+
 from .AmazonCounterfactualClassification import *
 from .AmazonPolarityClassification import *
 from .AmazonReviewsClassification import *
+from .AngryTweetsClassification import *
 from .Banking77Classification import *
+from .DalajClassification import *
+from .DanishPoliticalCommentsClassification import *
+from .DKHateClassification import *
 from .EmotionClassification import *
 from .ImdbClassification import *
+from .LccSentimentClassification import *
 from .MassiveIntentClassification import *
 from .MassiveScenarioClassification import *
 from .MTOPDomainClassification import *
 from .MTOPIntentClassification import *
+from .NoRecClassification import *
+from .NordicLangClassification import *
+from .NorwegianParliamentClassification import *
+from .ScalaClassification import *
+from .SweRecClassification import *
 from .ToxicConversationsClassification import *
 from .TweetSentimentExtractionClassification import *
```

### Comparing `mteb-1.0.2/mteb/tasks/Clustering/ArxivClusteringP2P.py` & `mteb-1.1.0/mteb/tasks/Clustering/ArxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Clustering/ArxivClusteringS2S.py` & `mteb-1.1.0/mteb/tasks/Clustering/ArxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Clustering/BiorxivClusteringP2P.py` & `mteb-1.1.0/mteb/tasks/Clustering/BiorxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Clustering/BiorxivClusteringS2S.py` & `mteb-1.1.0/mteb/tasks/Clustering/BiorxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Clustering/MedrxivClusteringP2P.py` & `mteb-1.1.0/mteb/tasks/Clustering/MedrxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Clustering/MedrxivClusteringS2S.py` & `mteb-1.1.0/mteb/tasks/Clustering/MedrxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Clustering/RedditClustering.py` & `mteb-1.1.0/mteb/tasks/Clustering/RedditClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Clustering/RedditClusteringP2P.py` & `mteb-1.1.0/mteb/tasks/Clustering/RedditClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Clustering/StackExchangeClustering.py` & `mteb-1.1.0/mteb/tasks/Clustering/StackExchangeClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Clustering/StackExchangeClusteringP2P.py` & `mteb-1.1.0/mteb/tasks/Clustering/StackExchangeClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Clustering/TwentyNewsgroupsClustering.py` & `mteb-1.1.0/mteb/tasks/Clustering/TwentyNewsgroupsClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/PairClassification/SprintDuplicateQuestionsPC.py` & `mteb-1.1.0/mteb/tasks/PairClassification/SprintDuplicateQuestionsPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/PairClassification/TwitterSemEval2015PC.py` & `mteb-1.1.0/mteb/tasks/PairClassification/TwitterSemEval2015PC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/PairClassification/TwitterURLCorpusPC.py` & `mteb-1.1.0/mteb/tasks/PairClassification/TwitterURLCorpusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Reranking/AskUbuntuDupQuestions.py` & `mteb-1.1.0/mteb/tasks/Reranking/AskUbuntuDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Reranking/MindSmallReranking.py` & `mteb-1.1.0/mteb/tasks/Reranking/MindSmallReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Reranking/SciDocsReranking.py` & `mteb-1.1.0/mteb/tasks/Reranking/SciDocsReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Reranking/StackOverflowDupQuestions.py` & `mteb-1.1.0/mteb/tasks/Reranking/StackOverflowDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/ArguAnaRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/ArguAnaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackAndroidRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackAndroidRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackEnglishRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackEnglishRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackGamingRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackGamingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackGisRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackGisRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackMathematicaRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackMathematicaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackPhysicsRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackPhysicsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackProgrammersRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackProgrammersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackStatsRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackStatsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackTexRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackTexRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackUnixRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackUnixRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackWebmastersRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackWebmastersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/CQADupstackWordpressRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/CQADupstackWordpressRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/ClimateFEVERRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/ClimateFEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/DBPediaRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/DBPediaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/FEVERRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/FEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/FiQA2018Retrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/FiQA2018Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/HotpotQARetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/HotpotQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/MSMARCORetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/MSMARCORetrieval.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,11 +8,11 @@
         return {
             "name": "MSMARCO",
             "beir_name": "msmarco",
             "description": "MS MARCO is a collection of datasets focused on deep learning in search",
             "reference": "https://microsoft.github.io/msmarco/",
             "type": "Retrieval",
             "category": "s2p",
-            "eval_splits": ["validation", "test"], # "dev" if not using latest BEIR i.e. not HFDataLoader
+            "eval_splits": ["dev", "test"],  # "validation" if using latest BEIR i.e. HFDataLoader
             "eval_langs": ["en"],
             "main_score": "ndcg_at_10",
         }
```

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/MSMARCOv2Retrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/MSMARCOv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/NFCorpusRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/NFCorpusRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/NQRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/NQRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/QuoraRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/Touche2020Retrieval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from ...abstasks.AbsTaskRetrieval import AbsTaskRetrieval
 from ...abstasks.BeIRTask import BeIRTask
 
 
-class QuoraRetrieval(AbsTaskRetrieval, BeIRTask):
+class Touche2020(AbsTaskRetrieval, BeIRTask):
     @property
     def description(self):
         return {
-            "name": "QuoraRetrieval",
-            "beir_name": "quora",
-            "description": (
-                "QuoraRetrieval is based on questions that are marked as duplicates on the Quora platform. Given a"
-                " question, find other (duplicate) questions."
-            ),
-            "reference": "https://quoradata.quora.com/First-Quora-Dataset-Release-Question-Pairs",
+            "name": "Touche2020",
+            "beir_name": "webis-touche2020",
+            "description": "Touché Task 1: Argument Retrieval for Controversial Questions",
+            "reference": "https://webis.de/events/touche-20/shared-task-1.html",
             "type": "Retrieval",
-            "category": "s2s",
-            "eval_splits": ["validation", "test"],
+            "category": "s2p",
+            "eval_splits": ["test"],
             "eval_langs": ["en"],
             "main_score": "ndcg_at_10",
         }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/SCIDOCSRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/SCIDOCSRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/SciFactRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/SciFactRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/TRECCOVIDRetrieval.py` & `mteb-1.1.0/mteb/tasks/Retrieval/TRECCOVIDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Retrieval/__init__.py` & `mteb-1.1.0/mteb/tasks/Retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/STS/BiossesSTS.py` & `mteb-1.1.0/mteb/tasks/STS/BiossesSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/STS/STS12STS.py` & `mteb-1.1.0/mteb/tasks/STS/STS12STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/STS/STS13STS.py` & `mteb-1.1.0/mteb/tasks/STS/STS13STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/STS/STS14STS.py` & `mteb-1.1.0/mteb/tasks/STS/STS14STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/STS/STS15STS.py` & `mteb-1.1.0/mteb/tasks/STS/STS15STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/STS/STS16STS.py` & `mteb-1.1.0/mteb/tasks/STS/STS16STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/STS/STS17CrosslingualSTS.py` & `mteb-1.1.0/mteb/tasks/STS/STS17CrosslingualSTS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from ...abstasks import AbsTaskSTS, CrosslingualTask
 
-
 _LANGUAGES = ["ko-ko", "ar-ar", "en-ar", "en-de", "en-en", "en-tr", "es-en", "es-es", "fr-en", "it-en", "nl-en"]
 
 
 class STS17Crosslingual(AbsTaskSTS, CrosslingualTask):
     @property
     def description(self):
         return {
```

### Comparing `mteb-1.0.2/mteb/tasks/STS/STS22CrosslingualSTS.py` & `mteb-1.1.0/mteb/tasks/STS/STS22CrosslingualSTS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from ...abstasks import AbsTaskSTS, CrosslingualTask
 
-
 _LANGUAGES = {
     "en": "en",
     "de": "de",
     "es": "es",
     "pl": "pl",
     "tr": "tr",
     "ar": "ar",
```

### Comparing `mteb-1.0.2/mteb/tasks/STS/STSBenchmarkSTS.py` & `mteb-1.1.0/mteb/tasks/STS/STSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/STS/SickrSTS.py` & `mteb-1.1.0/mteb/tasks/STS/SickrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb/tasks/Summarization/SummEvalSummarization.py` & `mteb-1.1.0/mteb/tasks/Summarization/SummEvalSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/mteb.egg-info/SOURCES.txt` & `mteb-1.1.0/mteb.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -35,39 +35,54 @@
 mteb/evaluation/evaluators/RetrievalEvaluator.py
 mteb/evaluation/evaluators/STSEvaluator.py
 mteb/evaluation/evaluators/SummarizationEvaluator.py
 mteb/evaluation/evaluators/__init__.py
 mteb/evaluation/evaluators/utils.py
 mteb/tasks/__init__.py
 mteb/tasks/BitextMining/BUCCBitextMining.py
+mteb/tasks/BitextMining/BornholmskBitextMining.py
 mteb/tasks/BitextMining/TatoebaBitextMining.py
 mteb/tasks/BitextMining/__init__.py
 mteb/tasks/Classification/AmazonCounterfactualClassification.py
 mteb/tasks/Classification/AmazonPolarityClassification.py
 mteb/tasks/Classification/AmazonReviewsClassification.py
+mteb/tasks/Classification/AngryTweetsClassification.py
 mteb/tasks/Classification/Banking77Classification.py
+mteb/tasks/Classification/DKHateClassification.py
+mteb/tasks/Classification/DalajClassification.py
+mteb/tasks/Classification/DanishPoliticalCommentsClassification.py
 mteb/tasks/Classification/EmotionClassification.py
 mteb/tasks/Classification/ImdbClassification.py
+mteb/tasks/Classification/LccSentimentClassification.py
 mteb/tasks/Classification/MTOPDomainClassification.py
 mteb/tasks/Classification/MTOPIntentClassification.py
 mteb/tasks/Classification/MassiveIntentClassification.py
 mteb/tasks/Classification/MassiveScenarioClassification.py
+mteb/tasks/Classification/NoRecClassification.py
+mteb/tasks/Classification/NordicLangClassification.py
+mteb/tasks/Classification/NorwegianParliamentClassification.py
+mteb/tasks/Classification/ScalaClassification.py
+mteb/tasks/Classification/SweRecClassification.py
 mteb/tasks/Classification/ToxicConversationsClassification.py
 mteb/tasks/Classification/TweetSentimentExtractionClassification.py
 mteb/tasks/Classification/__init__.py
 mteb/tasks/Clustering/ArxivClusteringP2P.py
 mteb/tasks/Clustering/ArxivClusteringS2S.py
 mteb/tasks/Clustering/BiorxivClusteringP2P.py
 mteb/tasks/Clustering/BiorxivClusteringS2S.py
+mteb/tasks/Clustering/BlurbsClusteringP2P.py
+mteb/tasks/Clustering/BlurbsClusteringS2S.py
 mteb/tasks/Clustering/MedrxivClusteringP2P.py
 mteb/tasks/Clustering/MedrxivClusteringS2S.py
 mteb/tasks/Clustering/RedditClustering.py
 mteb/tasks/Clustering/RedditClusteringP2P.py
 mteb/tasks/Clustering/StackExchangeClustering.py
 mteb/tasks/Clustering/StackExchangeClusteringP2P.py
+mteb/tasks/Clustering/TenKGnadClusteringP2P.py
+mteb/tasks/Clustering/TenKGnadClusteringS2S.py
 mteb/tasks/Clustering/TwentyNewsgroupsClustering.py
 mteb/tasks/Clustering/__init__.py
 mteb/tasks/PairClassification/SprintDuplicateQuestionsPC.py
 mteb/tasks/PairClassification/TwitterSemEval2015PC.py
 mteb/tasks/PairClassification/TwitterURLCorpusPC.py
 mteb/tasks/PairClassification/__init__.py
 mteb/tasks/Reranking/AskUbuntuDupQuestions.py
```

### Comparing `mteb-1.0.2/setup.cfg` & `mteb-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mteb-1.0.2/setup.py` & `mteb-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
    VERSION needs to be formatted following the MAJOR.MINOR.PATCH convention
    (we need to follow this convention to be able to retrieve versioned scripts)
 Inspired by: https://github.com/huggingface/datasets/blob/main/setup.py
 To create the package for pypi.
 0. Prerequisites:
    - Dependencies:
      - twine: "pip install twine"
+     - wheel: "pip install wheel"
    - Create an account in (and join the 'datasets' project):
      - PyPI: https://pypi.org/
      - Test PyPI: https://test.pypi.org/
 1. Change the version in:
    - mteb/__init__.py
    - setup.py
 2. Commit these changes: "git commit -m 'Release: VERSION'"
@@ -46,15 +47,15 @@
 
 extras = {}
 extras["beir"] = ["beir"]
 
 
 setup(
     name="mteb",
-    version="1.0.2",
+    version="1.1.0",
     description="Massive Text Embedding Benchmark",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords="deep learning, text embeddings, benchmark",
     license="Apache",
     author="MTEB Contributors (https://github.com/embeddings-benchmark/mteb/graphs/contributors)",
     author_email="niklas@huggingface.co, nouamane@huggingface.co, info@nils-reimers.de",
```

