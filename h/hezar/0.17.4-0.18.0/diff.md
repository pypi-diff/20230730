# Comparing `tmp/hezar-0.17.4.tar.gz` & `tmp/hezar-0.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.17.4.tar", max compression
+gzip compressed data, was "hezar-0.18.0.tar", max compression
```

## Comparing `hezar-0.17.4.tar` & `hezar-0.18.0.tar`

### file list

```diff
@@ -1,84 +1,87 @@
--rw-r--r--   0        0        0     1065 2023-07-29 16:06:12.051299 hezar-0.17.4/LICENSE
--rw-r--r--   0        0        0     4309 2023-07-29 16:06:12.051299 hezar-0.17.4/README.md
--rw-r--r--   0        0        0      261 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/__init__.py
--rw-r--r--   0        0        0     5384 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/builders.py
--rw-r--r--   0        0        0    11117 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/configs.py
--rw-r--r--   0        0        0     2068 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/data/__init__.py
--rw-r--r--   0        0        0     6333 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/data/data_collators.py
--rw-r--r--   0        0        0      223 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1709 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4502 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3627 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0       26 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4124 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      141 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     1184 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/metrics/f1.py
--rw-r--r--   0        0        0      983 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/metrics/metric.py
--rw-r--r--   0        0        0     1295 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/metrics/recall.py
--rw-r--r--   0        0        0     2090 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0      282 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1604 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1676 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1634 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0    11656 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/model.py
--rw-r--r--   0        0        0       67 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     3971 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0        0 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0      240 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     3530 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     3666 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     3809 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/models/text_summarization/__init__.py
--rw-r--r--   0        0        0      118 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0     3603 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/preprocessors/normalizer.py
--rw-r--r--   0        0        0     3333 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0      231 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4556 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5045 2023-07-29 16:06:12.055299 hezar-0.17.4/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0    19353 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4132 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     8674 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/registry.py
--rw-r--r--   0        0        0      143 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/trainers/__init__.py
--rw-r--r--   0        0        0       63 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/trainers/sequence_labeling/__init__.py
--rw-r--r--   0        0        0     2538 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
--rw-r--r--   0        0        0       67 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/trainers/text_classification/__init__.py
--rw-r--r--   0        0        0     2177 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/trainers/text_classification/text_classification_trainer.py
--rw-r--r--   0        0        0    17300 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1626 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      161 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/utils/__init__.py
--rw-r--r--   0        0        0      611 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/utils/common_utils.py
--rw-r--r--   0        0        0      482 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     5614 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/utils/core_utils.py
--rw-r--r--   0        0        0     3660 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/utils/logging.py
--rw-r--r--   0        0        0        0 2023-07-29 16:06:12.059299 hezar-0.17.4/hezar/utils/model_utils.py
--rw-r--r--   0        0        0     1648 2023-07-29 16:06:12.059299 hezar-0.17.4/pyproject.toml
--rw-r--r--   0        0        0     6791 1970-01-01 00:00:00.000000 hezar-0.17.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-30 08:30:20.049396 hezar-0.18.0/LICENSE
+-rw-r--r--   0        0        0     4309 2023-07-30 08:30:20.049396 hezar-0.18.0/README.md
+-rw-r--r--   0        0        0      261 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/__init__.py
+-rw-r--r--   0        0        0     5384 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/builders.py
+-rw-r--r--   0        0        0    11117 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/configs.py
+-rw-r--r--   0        0        0     2068 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6364 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      223 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1709 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4502 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3627 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0       26 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4124 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3122 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3081 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      141 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     1184 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/metrics/f1.py
+-rw-r--r--   0        0        0      983 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     1295 2023-07-30 08:30:20.049396 hezar-0.18.0/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     2090 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0      282 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1604 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1676 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1634 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0    11760 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/model.py
+-rw-r--r--   0        0        0      152 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     3971 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      151 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/sequence_labeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     4124 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
+-rw-r--r--   0        0        0      877 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     3530 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     3666 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     3809 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/models/text_summarization/__init__.py
+-rw-r--r--   0        0        0      142 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0     3603 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/normalizer.py
+-rw-r--r--   0        0        0     3852 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0      231 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4556 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5045 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0    19353 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4132 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8674 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/registry.py
+-rw-r--r--   0        0        0      143 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/trainers/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0     2643 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
+-rw-r--r--   0        0        0       67 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/trainers/text_classification/__init__.py
+-rw-r--r--   0        0        0     2243 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/trainers/text_classification/text_classification_trainer.py
+-rw-r--r--   0        0        0    17687 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1626 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      161 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0      482 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     5614 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/utils/core_utils.py
+-rw-r--r--   0        0        0     3660 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/utils/logging.py
+-rw-r--r--   0        0        0        0 2023-07-30 08:30:20.053396 hezar-0.18.0/hezar/utils/model_utils.py
+-rw-r--r--   0        0        0     1648 2023-07-30 08:30:20.053396 hezar-0.18.0/pyproject.toml
+-rw-r--r--   0        0        0     6791 1970-01-01 00:00:00.000000 hezar-0.18.0/PKG-INFO
```

### Comparing `hezar-0.17.4/LICENSE` & `hezar-0.18.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/README.md` & `hezar-0.18.0/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/builders.py` & `hezar-0.18.0/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/configs.py` & `hezar-0.18.0/hezar/configs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/constants.py` & `hezar-0.18.0/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/data/data_collators.py` & `hezar-0.18.0/hezar/data/data_collators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
 import torch
 
 from ..data.utils import convert_batch_dict_dtype
 from ..preprocessors import Tokenizer
 from ..utils import get_logger
 
-
 __all__ = [
     "TextPaddingDataCollator",
     "SequenceLabelingDataCollator",
 ]
 
 logger = get_logger(__name__)
 
@@ -28,20 +27,20 @@
          have this value as length.
         return_tensors: Specifies the dtype of the returning tensors in the batch. Defaults to `pt(torch.Tensor)`, but
          can also be `np` or `list`.
 
     """
 
     def __init__(
-        self,
-        tokenizer: Tokenizer,
-        padding_type: str = "longest",
-        padding_side: str = "right",
-        max_length: int = None,
-        return_tensors: str = "pt",
+            self,
+            tokenizer: Tokenizer,
+            padding_type: str = "longest",
+            padding_side: str = "right",
+            max_length: int = None,
+            return_tensors: str = "pt",
     ):
         self.tokenizer = tokenizer
         self.padding_type = padding_type
         self.padding_side = padding_side
         self.max_length = max_length
         self.return_tensors = return_tensors
 
@@ -140,15 +139,15 @@
 
     def __call__(self, encoded_batch):
         label_name = "label" if "label" in encoded_batch[0].keys() else "labels"
         labels = [feature[label_name] for feature in encoded_batch] if label_name in encoded_batch[0].keys() else None
         self.tokenizer.config.padding_direction = self.padding_side
         batch = self.tokenizer.pad_encoded_batch(
             encoded_batch,
-            padding=self.padding_type,
+            padding=self.padding_type,  # noqa
             max_length=self.max_length,
             # Conversion to tensors will fail if we have labels as they are not of the same length yet.
             return_tensors="pt" if labels is None else None,
         )
 
         if labels is None:
             return batch
```

### Comparing `hezar-0.17.4/hezar/data/datasets/dataset.py` & `hezar-0.18.0/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.18.0/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.18.0/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/data/utils/data_utils.py` & `hezar-0.18.0/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/embeddings/embedding.py` & `hezar-0.18.0/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/embeddings/fasttext.py` & `hezar-0.18.0/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/embeddings/word2vec.py` & `hezar-0.18.0/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/metrics/f1.py` & `hezar-0.18.0/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/metrics/metric.py` & `hezar-0.18.0/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/metrics/recall.py` & `hezar-0.18.0/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/metrics/seqeval.py` & `hezar-0.18.0/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.18.0/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.18.0/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.18.0/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.18.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.18.0/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.18.0/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/models/model.py` & `hezar-0.18.0/hezar/models/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import torch
 from huggingface_hub import create_repo, hf_hub_download, upload_file
 from torch import nn
 
 from ..builders import build_model
 from ..configs import ModelConfig
 from ..constants import DEFAULT_MODEL_CONFIG_FILE, DEFAULT_MODEL_FILE, HEZAR_CACHE_DIR
-from ..preprocessors import Preprocessor
+from ..preprocessors import Preprocessor, PreprocessorsContainer
 from ..utils import get_logger
 
 
 __all__ = [
     "Model",
     "ModelConfig",
 ]
@@ -222,16 +222,15 @@
             filename=config_filename,
             repo_type="model",
             commit_message=commit_message,
         )
         # upload preprocessor(s)
         if push_preprocessor:
             if self.preprocessor is not None:
-                for p in self.preprocessor.values():
-                    p.push_to_hub(repo_id)
+                self.preprocessor.push_to_hub(repo_id, commit_message=commit_message, private=private)
         # upload model file
         upload_file(
             path_or_fileobj=model_save_path,
             path_in_repo=filename,
             repo_id=repo_id,
             commit_message=commit_message,
         )
@@ -310,15 +309,17 @@
     @property
     def preprocessor(self):
         return self._preprocessor
 
     @preprocessor.setter
     def preprocessor(self, value):
         if isinstance(value, Preprocessor):
-            preprocessor = OrderedDict()
+            preprocessor = PreprocessorsContainer()
             preprocessor[value.config.name] = value
-        elif isinstance(value, (dict, OrderedDict)):
-            preprocessor = OrderedDict(**value)
+        elif isinstance(value, Mapping):
+            preprocessor = PreprocessorsContainer(**value)
+        elif value is None:
+            preprocessor = None
         else:
-            raise ValueError(f"Preprocessor value must be a `Preprocessor` or a dict of `Preprocessor` objects "
+            raise ValueError(f"Preprocessor value must be a `Preprocessor` or a mapping of `Preprocessor` objects "
                              f"not `{type(value)}`!")
         self._preprocessor = preprocessor
```

### Comparing `hezar-0.17.4/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.18.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.18.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.18.0/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.18.0/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.18.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.18.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.18.0/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.18.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/preprocessors/normalizer.py` & `hezar-0.18.0/hezar/preprocessors/normalizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/preprocessors/preprocessor.py` & `hezar-0.18.0/hezar/preprocessors/preprocessor.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,15 +30,21 @@
             **kwargs: Extra keyword arguments depending on the preprocessor
         """
         raise NotImplementedError
 
     def save(self, path, **kwargs):
         raise NotImplementedError
 
-    def push_to_hub(self, hub_path):
+    def push_to_hub(
+        self,
+        repo_id,
+        subfolder=None,
+        commit_message=None,
+        private=None,
+    ):
         raise NotImplementedError
 
     @classmethod
     def load(
         cls,
         hub_or_local_path,
         subfolder: str = None,
@@ -60,15 +66,15 @@
             **kwargs: Extra kwargs
 
         Returns:
             A Preprocessor subclass or a dict of Preprocessor subclass instances
         """
         subfolder = subfolder or cls.preprocessor_subfolder
         preprocessor_files = list_repo_files(hub_or_local_path, subfolder=subfolder)
-        preprocessors = OrderedDict()
+        preprocessors = PreprocessorsContainer()
         for f in preprocessor_files:
             if f.endswith(".yaml"):
                 if os.path.isdir(hub_or_local_path):
                     config_file = os.path.join(hub_or_local_path, subfolder, f)
                 else:
                     config_file = hf_hub_download(
                         hub_or_local_path,
@@ -84,7 +90,23 @@
                     preprocessors[name] = preprocessor
                 else:
                     raise ValueError(f"The config file `{config_file}` does not have the property `name`!")
         if len(preprocessors) == 1 and not force_return_dict:
             return list(preprocessors.values())[0]
 
         return preprocessors
+
+
+class PreprocessorsContainer(OrderedDict):
+    """
+    A class to hold the preprocessors by their name
+    """
+
+    def push_to_hub(
+        self,
+        repo_id,
+        subfolder=None,
+        commit_message=None,
+        private=None,
+    ):
+        for name, preprocessor in self.items():
+            preprocessor.push_to_hub(repo_id, subfolder=subfolder, commit_message=commit_message, private=private)
```

### Comparing `hezar-0.17.4/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.18.0/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.18.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.18.0/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.18.0/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/registry.py` & `hezar-0.18.0/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py` & `hezar-0.18.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from typing import Callable
+
 import numpy as np
 import torch
 
+from ..trainer import Trainer
 from ...configs import TrainerConfig
 from ...constants import MetricType
 from ...data.datasets import Dataset
 from ...models import Model
 from ...utils import get_logger
-from ..trainer import Trainer
-
 
 logger = get_logger(__name__)
 
 
 class SequenceLabelingTrainer(Trainer):
     """
     A trainer for all text classification models
@@ -30,24 +31,26 @@
 
     def __init__(
         self,
         model: Model = None,
         config: TrainerConfig = None,
         train_dataset: Dataset = None,
         eval_dataset: Dataset = None,
-        data_collator=None,
+        data_collator: Callable = None,
+        preprocessor=None,
         optimizer: torch.optim.Optimizer = None,
         lr_scheduler=None,
     ):
         super().__init__(
             model=model,
             config=config,
             train_dataset=train_dataset,
             eval_dataset=eval_dataset,
             data_collator=data_collator,
+            preprocessor=preprocessor,
             optimizer=optimizer,
             lr_scheduler=lr_scheduler,
         )
         self.criterion = torch.nn.CrossEntropyLoss()
 
     def compute_loss(self, logits, labels, **kwargs) -> torch.Tensor:
         loss = self.criterion(logits.view(-1, self.model.config.num_labels), labels.view(-1))
@@ -67,8 +70,7 @@
             for prediction, label in zip(predictions, labels)
         ]
 
         results = {}
         for metric_name, metric in self.metrics.items():
             results[metric_name] = metric.compute(true_predictions, true_labels)["f1"]
         return results
-
```

### Comparing `hezar-0.17.4/hezar/trainers/text_classification/text_classification_trainer.py` & `hezar-0.18.0/hezar/trainers/text_classification/text_classification_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,23 +39,25 @@
     def __init__(
         self,
         model: Model = None,
         config: TrainerConfig = None,
         train_dataset: Dataset = None,
         eval_dataset: Dataset = None,
         data_collator=None,
+        preprocessor=None,
         optimizer: torch.optim.Optimizer = None,
         lr_scheduler=None,
     ):
         super().__init__(
             model=model,
             config=config,
             train_dataset=train_dataset,
             eval_dataset=eval_dataset,
             data_collator=data_collator,
+            preprocessor=preprocessor,
             optimizer=optimizer,
             lr_scheduler=lr_scheduler,
         )
         self.criterion = torch.nn.CrossEntropyLoss(ignore_index=-100)
 
     def compute_loss(self, logits, labels, **kwargs) -> torch.Tensor:
         loss = self.criterion(logits, labels)
```

### Comparing `hezar-0.17.4/hezar/trainers/trainer.py` & `hezar-0.18.0/hezar/trainers/trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import os
 import random
-from typing import Any, Dict, Tuple
+from typing import Any, Dict, Tuple, Union, Callable
 
 import numpy as np
 import torch
 from huggingface_hub import create_repo, hf_hub_download
 from torch.utils.data import DataLoader
 from torch.utils.tensorboard import SummaryWriter
 from tqdm import tqdm
 
+from .trainer_utils import MetricsTracker
 from ..builders import build_metric
 from ..configs import LRSchedulerConfig, MetricConfig, OptimizerConfig, TrainerConfig
 from ..constants import (
     DEFAULT_DATASET_CONFIG_FILE,
     DEFAULT_TRAINER_CONFIG_FILE,
     DEFAULT_TRAINER_SUBFOLDER,
     HEZAR_CACHE_DIR,
     TQDM_BAR_FORMAT,
 )
 from ..data.datasets import Dataset
 from ..models import Model
+from ..preprocessors import Preprocessor, PreprocessorsContainer
 from ..utils import get_logger
-from .trainer_utils import MetricsTracker
-
 
 logger = get_logger(__name__)
 
 optimizers = {
     "adam": torch.optim.Adam,
     "adamw": torch.optim.AdamW,
     "sgd": torch.optim.SGD,
@@ -43,14 +43,15 @@
 
     Args:
         model ([`Model`] or `torch.nn.Module`): The main model to train and evaluate
         config (TrainerConfig): Training configuration and parameters
         train_dataset (Dataset): Train dataset
         eval_dataset (Dataset): Evaluation dataset
         data_collator: Collate function, usually included in the dataset object itself
+        preprocessor: Preprocessor object(s)
         optimizer (optim.Optimizer): Model optimizer
         lr_scheduler: Optional learning-rate scheduler
 
     """
 
     trainer_subfolder = DEFAULT_TRAINER_SUBFOLDER
     trainer_config_file = DEFAULT_TRAINER_CONFIG_FILE
@@ -59,30 +60,31 @@
 
     def __init__(
         self,
         model: Model = None,
         config: TrainerConfig = None,
         train_dataset: Dataset = None,
         eval_dataset: Dataset = None,
-        data_collator=None,
+        data_collator: Callable = None,
+        preprocessor: Union[Preprocessor, PreprocessorsContainer] = None,
         optimizer: torch.optim.Optimizer = None,
         lr_scheduler=None,
-        compute_metrics=None,
         **kwargs,
     ):
 
         self.config = config
 
         self.device, self.device_type = self._prepare_device_and_type()
         self.autocast_dtype = torch.bfloat16 if self.device_type == "cpu" else torch.float16
         self.scaler = torch.cuda.amp.GradScaler(enabled=self.config.use_amp and self.device_type == "cuda")
 
         self._set_seed(self.config.seed)
 
         self.model = self._prepare_model(model)
+        self.model.preprocessor = preprocessor
 
         self.train_dataset = train_dataset
         self.eval_dataset = eval_dataset
         self.data_collator = data_collator or self.train_dataset.data_collator
         self.train_dataloader, self.eval_dataloader = self._prepare_dataloaders()
 
         self.optimizer, self.lr_scheduler = self._prepare_optimizers(optimizer, lr_scheduler)
@@ -115,15 +117,15 @@
         hub_path = self.config.init_weights_from
         if hub_path is not None:
             local_path = hf_hub_download(hub_path, filename=model.model_filename, cache_dir=HEZAR_CACHE_DIR)
             model.load_state_dict(torch.load(local_path, map_location="cpu"))
         model.to(self.device)
         return model
 
-    def _prepare_dataloaders(self):
+    def _prepare_dataloaders(self) -> Tuple[DataLoader, Union[DataLoader, None]]:
         """
         Set up data loaders (train/eval) and return them.
 
         Returns:
              A tuple of train and eval dataloaders
         """
         if self.train_dataset is not None:
@@ -143,15 +145,16 @@
                 batch_size=self.config.batch_size,
                 collate_fn=self.data_collator,
                 num_workers=self.config.num_dataloader_workers,
                 drop_last=True,
                 shuffle=True,
             )
         else:
-            logger.warning("Cannot create eval dataloader because `eval_dataset` is not given to the Trainer!")
+            logger.warning("Cannot create eval dataloader because `eval_dataset` is not given to the Trainer! "
+                           "Setting eval_dataloader to None...")
             eval_dataloader = None
 
         return train_dataloader, eval_dataloader
 
     def _prepare_optimizers(self, optimizer: torch.optim.Optimizer = None, lr_scheduler=None):
         """
         Set up the optimizer and lr scheduler if they're not already given
@@ -193,15 +196,15 @@
                 metrics_dict[metric] = build_metric(metric)
             elif isinstance(metric, MetricConfig):
                 metrics_dict[metric.name] = build_metric(metric.name, config=metric)
             else:
                 raise ValueError(f"Invalid metric type `{type(metric)}`! Available metrics: {self.AVAILABLE_METRICS}")
         return metrics_dict
 
-    def prepare_input_batch(self, input_batch):
+    def prepare_input_batch(self, input_batch) -> Dict[str, torch.Tensor]:
         """
         Every operation required to prepare the inputs for model forward like moving to device, permutations, etc.
         Args:
             input_batch: Raw input batch from the dataloader
 
         Returns:
             The proper input batch required by model forward
@@ -245,15 +248,15 @@
             labels: Ground truth labels
 
         Returns:
             The loss tensor
         """
         raise NotImplementedError
 
-    def compute_metrics(self, predictions, labels, **kwargs):
+    def compute_metrics(self, predictions, labels, **kwargs) -> Dict[str, float]:
         """
         Compute metric values on the predictions and labels
 
         Args:
             predictions: A list of all predictions
             labels: A list of all labels
```

### Comparing `hezar-0.17.4/hezar/trainers/trainer_utils.py` & `hezar-0.18.0/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/utils/common_utils.py` & `hezar-0.18.0/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/utils/core_utils.py` & `hezar-0.18.0/hezar/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/hezar/utils/hub_utils.py` & `hezar-0.18.0/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.17.4/pyproject.toml` & `hezar-0.18.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.17.4"
+version = "0.18.0"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.17.4/PKG-INFO` & `hezar-0.18.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.17.4
+Version: 0.18.0
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
```

