# Comparing `tmp/aniemore-1.1.1.tar.gz` & `tmp/aniemore-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aniemore-1.1.1.tar", max compression
+gzip compressed data, was "aniemore-1.2.0.tar", max compression
```

## Comparing `aniemore-1.1.1.tar` & `aniemore-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-02-19 15:39:16.440064 aniemore-1.1.1/aniemore/__init__.py
--rw-r--r--   0        0        0        0 2023-03-09 00:36:38.168893 aniemore-1.1.1/aniemore/custom/__init__.py
--rw-r--r--   0        0        0    19229 2023-04-15 10:55:25.882627 aniemore-1.1.1/aniemore/custom/models.py
--rw-r--r--   0        0        0      587 2023-04-13 19:34:20.236375 aniemore-1.1.1/aniemore/datasets.py
--rw-r--r--   0        0        0     4507 2023-04-14 23:20:44.281921 aniemore-1.1.1/aniemore/models.py
--rw-r--r--   0        0        0        0 2023-03-09 00:36:38.169894 aniemore-1.1.1/aniemore/recognizers/__init__.py
--rw-r--r--   0        0        0     9924 2023-04-15 01:26:46.065774 aniemore-1.1.1/aniemore/recognizers/multimodal.py
--rw-r--r--   0        0        0     5641 2023-04-13 23:41:12.889330 aniemore-1.1.1/aniemore/recognizers/text.py
--rw-r--r--   0        0        0     3981 2023-04-13 23:56:25.137542 aniemore-1.1.1/aniemore/recognizers/voice.py
--rw-r--r--   0        0        0        0 2023-02-19 15:39:16.444744 aniemore-1.1.1/aniemore/utils/__init__.py
--rw-r--r--   0        0        0    15860 2023-04-13 21:22:28.319429 aniemore-1.1.1/aniemore/utils/classes.py
--rw-r--r--   0        0        0     3104 2023-04-12 13:02:56.273113 aniemore-1.1.1/aniemore/utils/speech2text.py
--rw-r--r--   0        0        0     1125 2023-02-19 15:39:16.439561 aniemore-1.1.1/LICENSE
--rw-r--r--   0        0        0     2303 2023-04-22 09:56:21.195121 aniemore-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    11294 2023-04-14 10:29:39.799959 aniemore-1.1.1/README.md
--rw-r--r--   0        0        0    13402 1970-01-01 00:00:00.000000 aniemore-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-19 15:39:16.440064 aniemore-1.2.0/aniemore/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-09 00:36:38.168893 aniemore-1.2.0/aniemore/custom/__init__.py
+-rw-r--r--   0        0        0    28010 2023-05-11 01:32:48.849285 aniemore-1.2.0/aniemore/custom/models.py
+-rw-r--r--   0        0        0      587 2023-04-13 19:34:20.236375 aniemore-1.2.0/aniemore/datasets.py
+-rw-r--r--   0        0        0     4729 2023-05-11 01:32:48.849285 aniemore-1.2.0/aniemore/models.py
+-rw-r--r--   0        0        0        0 2023-03-09 00:36:38.169894 aniemore-1.2.0/aniemore/recognizers/__init__.py
+-rw-r--r--   0        0        0     9924 2023-04-15 01:26:46.065774 aniemore-1.2.0/aniemore/recognizers/multimodal.py
+-rw-r--r--   0        0        0     5641 2023-04-13 23:41:12.889330 aniemore-1.2.0/aniemore/recognizers/text.py
+-rw-r--r--   0        0        0     3981 2023-04-13 23:56:25.137542 aniemore-1.2.0/aniemore/recognizers/voice.py
+-rw-r--r--   0        0        0        0 2023-02-19 15:39:16.444744 aniemore-1.2.0/aniemore/utils/__init__.py
+-rw-r--r--   0        0        0    15860 2023-04-13 21:22:28.319429 aniemore-1.2.0/aniemore/utils/classes.py
+-rw-r--r--   0        0        0     3104 2023-04-12 13:02:56.273113 aniemore-1.2.0/aniemore/utils/speech2text.py
+-rw-r--r--   0        0        0     1125 2023-02-19 15:39:16.439561 aniemore-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2303 2023-05-11 01:32:48.850285 aniemore-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11671 2023-05-11 01:32:48.848285 aniemore-1.2.0/README.md
+-rw-r--r--   0        0        0    13775 1970-01-01 00:00:00.000000 aniemore-1.2.0/PKG-INFO
```

### Comparing `aniemore-1.1.1/aniemore/custom/models.py` & `aniemore-1.2.0/aniemore/custom/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -287,16 +287,15 @@
         return SpeechModelOutput(
             loss=loss,
             logits=logits
         )
 
 
 class Wav2Vec2ForVoiceClassification(BaseModelForVoiceBaseClassification):  # noqa
-    """
-    Wav2Vec2ForVoiceClassification is a model for voice classification task
+    """Wav2Vec2ForVoiceClassification is a model for voice classification task
      (e.g. speech command, voice activity detection, etc.)
 
     Args:
         config (Wav2Vec2Config): config
         num_labels (int): number of labels
 
     Attributes:
@@ -307,16 +306,15 @@
     def __init__(self, config, num_labels):
         super().__init__(config, num_labels)
         self.wav2vec2 = Wav2Vec2ForSequenceClassification(config)
         self.init_weights()
 
 
 class WavLMForVoiceClassification(BaseModelForVoiceBaseClassification):  # noqa
-    """
-    WavLMForVoiceClassification is a model for voice classification task
+    """WavLMForVoiceClassification is a model for voice classification task
      (e.g. speech command, voice activity detection, etc.)
 
     Args:
         config (WavLMConfig): config
         num_labels (int): number of labels
 
     Attributes:
@@ -327,16 +325,15 @@
     def __init__(self, config, num_labels):
         super().__init__(config, num_labels)
         self.wavlm = WavLMForSequenceClassification(config)
         self.init_weights()
 
 
 class UniSpeechSatForVoiceClassification(BaseModelForVoiceBaseClassification):  # noqa
-    """
-    UniSpeechSatForVoiceClassification is a model for voice classification task
+    """UniSpeechSatForVoiceClassification is a model for voice classification task
      (e.g. speech command, voice activity detection, etc.)
 
     Args:
         config (UniSpeechSatConfig): config
         num_labels (int): number of labels
 
     Attributes:
@@ -347,16 +344,15 @@
     def __init__(self, config, num_labels):
         super().__init__(config, num_labels)
         self.unispeech_sat = UniSpeechSatForSequenceClassification(config)
         self.init_weights()
 
 
 class HubertForVoiceClassification(BaseModelForVoiceBaseClassification):  # noqa
-    """
-    HubertForVoiceClassification is a model for voice classification task
+    """HubertForVoiceClassification is a model for voice classification task
      (e.g. speech command, voice activity detection, etc.)
 
     Args:
         config (HubertConfig): config
         num_labels (int): number of labels
 
     Attributes:
@@ -367,16 +363,15 @@
     def __init__(self, config, num_labels):
         super().__init__(config, num_labels)
         self.hubert = HubertForSequenceClassification(config)
         self.init_weights()
 
 
 class Wav2Vec2BertForSequenceClassification(BaseMultiModalForSequenceBaseClassification):  # noqa
-    """
-    Wav2Vec2BertForSequenceClassification is a model for sequence classification task
+    """Wav2Vec2BertForSequenceClassification is a model for sequence classification task
      (e.g. sentiment analysis, text classification, etc.)
 
     Args:
         config (Wav2Vec2BertConfig): config
 
     Attributes:
         config (Wav2Vec2BertConfig): config
@@ -395,16 +390,15 @@
         self.classifier = torch.nn.Linear(
             self.audio_config.hidden_size + self.text_config.hidden_size, self.num_labels
         )
         self.init_weights()
 
 
 class WavLMBertForSequenceClassification(BaseMultiModalForSequenceBaseClassification):  # noqa
-    """
-    WavLMBertForSequenceClassification is a model for sequence classification task
+    """WavLMBertForSequenceClassification is a model for sequence classification task
      (e.g. sentiment analysis, text classification, etc.)
 
     Args:
         config (WavLMBertConfig): config
 
     Attributes:
         config (WavLMBertConfig): config
@@ -423,16 +417,15 @@
         self.classifier = torch.nn.Linear(
             self.audio_config.hidden_size + self.text_config.hidden_size, self.num_labels
         )
         self.init_weights()
 
 
 class FineTuneWav2Vec2BertForSequenceClassification(BaseMultiModalForSequenceBaseClassification):  # noqa
-    """
-    FineTuneWav2Vec2BertForSequenceClassification is a model for sequence classification task
+    """FineTuneWav2Vec2BertForSequenceClassification is a model for sequence classification task
      (e.g. sentiment analysis, text classification, etc.) for fine-tuning
 
     Args:
         config (Wav2Vec2BertConfig): config
 
     Attributes:
         config (Wav2Vec2BertConfig): config
@@ -451,16 +444,15 @@
         self.classifier = torch.nn.Linear(
             self.audio_config.hidden_size + self.text_config.hidden_size, self.num_labels
         )
         self.init_weights()
 
 
 class FineTuneWavLMBertForSequenceClassification(BaseMultiModalForSequenceBaseClassification):  # noqa
-    """
-    FineTuneWavLMBertForSequenceClassification is a model for sequence classification task
+    """FineTuneWavLMBertForSequenceClassification is a model for sequence classification task
      (e.g. sentiment analysis, text classification, etc.) for fine-tuning
 
     Args:
         config (WavLMBertConfig): config
 
     Attributes:
         config (WavLMBertConfig): config
@@ -476,7 +468,209 @@
         self.text_config = BertConfig.from_dict(self.config.BertModel)
         self.audio_model = WavLMModel.from_pretrained(self.audio_config._name_or_path, config=self.audio_config)
         self.text_model = BertModel.from_pretrained(self.text_config._name_or_path, config=self.text_config)
         self.classifier = torch.nn.Linear(
             self.audio_config.hidden_size + self.text_config.hidden_size, self.num_labels
         )
         self.init_weights()
+
+
+class FusionModuleQ(torch.nn.Module):
+    """FusionModuleQ is a fusion module for the query
+    https://arxiv.org/abs/2302.13661
+    https://arxiv.org/abs/2207.04697
+
+    Args:
+        audio_dim (int): audio dimension
+        text_dim (int): text dimension
+        num_heads (int): number of heads
+    """
+    def __init__(self, audio_dim, text_dim, num_heads):
+        super().__init__()
+
+        # pick the lowest dimension of the two modalities
+        self.dimension = min(audio_dim, text_dim)
+
+        # attention modules
+        self.a_self_attention = torch.nn.MultiheadAttention(self.dimension, num_heads=num_heads)
+        self.t_self_attention = torch.nn.MultiheadAttention(self.dimension, num_heads=num_heads)
+
+        # layer norm
+        self.audio_norm = torch.nn.LayerNorm(self.dimension)
+        self.text_norm = torch.nn.LayerNorm(self.dimension)
+
+    def forward(self, audio_output, text_output):
+        """Forward pass
+
+        Args:
+            audio_output (torch.Tensor): audio output
+            text_output (torch.Tensor): text output
+
+        Returns:
+            torch.Tensor: audio output of the fusion module
+        """
+        # Multihead cross attention (dims ARE switched)
+        audio_attn, _ = self.a_self_attention(audio_output, text_output, text_output)
+        text_attn, _ = self.t_self_attention(text_output, audio_output, audio_output)
+
+        # Add & Norm with dropout
+        audio_add = self.audio_norm(audio_output + audio_attn)
+        text_add = self.text_norm(text_output + text_attn)
+
+        return audio_add, text_add
+
+
+class AudioTextFusionModelForSequenceClassificaion(BaseMultiModalForSequenceBaseClassification):  # noqa
+    def __init__(self, config):
+        """
+        Args:
+            config (MultiModalConfig): config
+        Attributes:
+            audio_projector (Union[torch.nn.Linear, None]): Projection layer for audio embeds
+            text_projector (Union[torch.nn.Linear, None]): Projection layer for text embeds
+            audio_avg_pool (Union[torch.nn.AvgPool1d, None]): Audio average pool (out from fusion block)
+            text_avg_pool (Union[torch.nn.AvgPool1d, None]): Text average pool (out from fusion block)
+        """
+        super().__init__(config)
+        self.audio_projector: Union[torch.nn.Linear, None] = None
+        self.text_projector: Union[torch.nn.Linear, None] = None
+        self.audio_avg_pool: Union[torch.nn.AvgPool1d, None] = None
+        self.text_avg_pool: Union[torch.nn.AvgPool1d, None] = None
+
+
+class WavLMBertFusionForSequenceClassification(AudioTextFusionModelForSequenceClassificaion):  # noqa
+    """
+    WavLMBertForSequenceClassification is a model for sequence classification task
+     (e.g. sentiment analysis, text classification, etc.) for fine-tuning
+    Args:
+        config (WavLMBertConfig): config
+    Attributes:
+        config (WavLMBertConfig): config
+        audio_config (WavLMConfig): wavlm config
+        text_config (BertConfig): bert config
+        audio_model (WavLMModel): wavlm model
+        text_model (BertModel): bert model
+        fusion_module_{i} (FusionModuleQ): Fusion Module Q
+        audio_projector (Union[torch.nn.Linear, None]): Projection layer for audio embeds
+        text_projector (Union[torch.nn.Linear, None]): Projection layer for text embeds
+        audio_avg_pool (Union[torch.nn.AvgPool1d, None]): Audio average pool (out from fusion block)
+        text_avg_pool (Union[torch.nn.AvgPool1d, None]): Text average pool (out from fusion block)
+        classifier (torch.nn.Linear): classifier
+    """
+
+    def __init__(self, config, finetune=False):
+        super().__init__(config)
+        self.audio_config = WavLMConfig.from_dict(self.config.WavLMModel)
+        self.text_config = BertConfig.from_dict(self.config.BertModel)
+
+        if not finetune:
+            self.audio_model = WavLMModel(self.audio_config)
+            self.text_model = BertModel(self.text_config)
+
+        else:
+            self.audio_model = WavLMModel.from_pretrained(self.audio_config._name_or_path, config=self.audio_config)
+            self.text_model = BertModel.from_pretrained(self.text_config._name_or_path, config=self.text_config)
+
+        # fusion module with V3 strategy (one projection on entry, no projection in continuous)
+        for i in range(self.config.num_fusion_layers):
+            setattr(self, f"fusion_module_{i + 1}", FusionModuleQ(
+                self.audio_config.hidden_size, self.text_config.hidden_size, self.config.num_heads
+            ))
+
+        self.audio_projector = torch.nn.Linear(self.audio_config.hidden_size, self.text_config.hidden_size)
+        self.text_projector = torch.nn.Linear(self.text_config.hidden_size, self.text_config.hidden_size)
+
+        # Avg Pool
+        self.audio_avg_pool = torch.nn.AvgPool1d(self.config.kernel_size)
+        self.text_avg_pool = torch.nn.AvgPool1d(self.config.kernel_size)
+
+        # output dimensions of wav2vec2 and bert are 768 and 1024 respectively
+        cls_dim = min(self.audio_config.hidden_size, self.text_config.hidden_size)
+        self.classifier = torch.nn.Linear(
+            (cls_dim * 2) // self.config.kernel_size, self.config.num_labels
+        )
+
+        self.init_weights()
+
+    def forward(
+            self,
+            input_ids=None,
+            input_values=None,
+            text_attention_mask=None,
+            audio_attention_mask=None,
+            token_type_ids=None,
+            position_ids=None,
+            head_mask=None,
+            inputs_embeds=None,
+            labels=None,
+            output_attentions=None,
+            output_hidden_states=None,
+            return_dict=True,
+    ):
+        """Forward method for multimodal model for sequence classification task (e.g. text + audio)
+        Args:
+            input_ids (torch.LongTensor, optional): input ids. Defaults to None.
+            input_values (torch.FloatTensor, optional): input values. Defaults to None.
+            text_attention_mask (torch.LongTensor, optional): text attention mask. Defaults to None.
+            audio_attention_mask (torch.LongTensor, optional): audio attention mask. Defaults to None.
+            token_type_ids (torch.LongTensor, optional): token type ids. Defaults to None.
+            position_ids (torch.LongTensor, optional): position ids. Defaults to None.
+            head_mask (torch.FloatTensor, optional): head mask. Defaults to None.
+            inputs_embeds (torch.FloatTensor, optional): inputs embeds. Defaults to None.
+            labels (torch.LongTensor, optional): labels. Defaults to None.
+            output_attentions (bool, optional): output attentions. Defaults to None.
+            output_hidden_states (bool, optional): output hidden states. Defaults to None.
+            return_dict (bool, optional): return dict. Defaults to True.
+        Returns:
+            torch.FloatTensor: logits
+        """
+        audio_output = self.audio_model(
+            input_values=input_values,
+            attention_mask=audio_attention_mask,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            return_dict=return_dict
+        )
+        text_output = self.text_model(
+            input_ids=input_ids,
+            attention_mask=text_attention_mask,
+            token_type_ids=token_type_ids,
+            position_ids=position_ids,
+            head_mask=head_mask,
+            inputs_embeds=inputs_embeds,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            return_dict=return_dict,
+        )
+
+        # Mean pooling
+        audio_avg = self.merged_strategy(audio_output.last_hidden_state, mode=self.config.pooling_mode)
+
+        # Projection
+        audio_proj = self.audio_projector(audio_avg)
+        text_proj = self.text_projector(text_output.pooler_output)
+
+        audio_mha, text_mha = None, None
+
+        for i in range(self.config.num_fusion_layers):
+            fusion_module = getattr(self, f"fusion_module_{i + 1}")
+
+            if i == 0:
+                audio_mha, text_mha = fusion_module(audio_proj, text_proj)
+            else:
+                audio_mha, text_mha = fusion_module(audio_mha, text_mha)
+
+        audio_avg = self.audio_avg_pool(audio_mha)
+        text_avg = self.text_avg_pool(text_mha)
+
+        fusion_output = torch.concat((audio_avg, text_avg), dim=1)
+
+        logits = self.classifier(fusion_output)
+        loss = None
+
+        if labels is not None:
+            loss = self.compute_loss(logits, labels)
+
+        return SpeechModelOutput(
+            loss=loss,
+            logits=logits
+        )
```

### Comparing `aniemore-1.1.1/aniemore/datasets.py` & `aniemore-1.2.0/aniemore/datasets.py`

 * *Files identical despite different names*

### Comparing `aniemore-1.1.1/aniemore/models.py` & `aniemore-1.2.0/aniemore/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     AutoModelForSequenceClassification,
     BertForSequenceClassification,
     PreTrainedModel
 )
 
 from aniemore.custom.models import (
     Wav2Vec2BertForSequenceClassification,
-    WavLMBertForSequenceClassification
+    WavLMBertForSequenceClassification, WavLMBertFusionForSequenceClassification
 )
 
 
 class Model(NamedTuple):
     """
     NamedTuple класс, используемый для более удобного доступа к информации о модели
 
@@ -91,7 +91,12 @@
             Wav2Vec2BertForSequenceClassification, 'aniemore/wav2vec2-bert-tiny2-s-emotion-russian-resd')
         Wav2Vec2BertBase = Model(
             Wav2Vec2BertForSequenceClassification, 'aniemore/wav2vec2-bert-base-s-emotion-russian-resd')
         WavLMBertTiny = Model(
             WavLMBertForSequenceClassification, 'aniemore/wavlm-bert-tiny2-s-emotion-russian-resd')
         WavLMBertBase = Model(
             WavLMBertForSequenceClassification, 'aniemore/wavlm-bert-base-s-emotion-russian-resd')
+
+        # Fusion Version
+        WavLMBertFusion = Model(
+            WavLMBertFusionForSequenceClassification, 'aniemore/wavlm-bert-fusion-s-emotion-russian-resd'
+        )
```

### Comparing `aniemore-1.1.1/aniemore/recognizers/multimodal.py` & `aniemore-1.2.0/aniemore/recognizers/multimodal.py`

 * *Files identical despite different names*

### Comparing `aniemore-1.1.1/aniemore/recognizers/text.py` & `aniemore-1.2.0/aniemore/recognizers/text.py`

 * *Files identical despite different names*

### Comparing `aniemore-1.1.1/aniemore/recognizers/voice.py` & `aniemore-1.2.0/aniemore/recognizers/voice.py`

 * *Files identical despite different names*

### Comparing `aniemore-1.1.1/aniemore/utils/classes.py` & `aniemore-1.2.0/aniemore/utils/classes.py`

 * *Files identical despite different names*

### Comparing `aniemore-1.1.1/aniemore/utils/speech2text.py` & `aniemore-1.2.0/aniemore/utils/speech2text.py`

 * *Files identical despite different names*

### Comparing `aniemore-1.1.1/LICENSE` & `aniemore-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aniemore-1.1.1/pyproject.toml` & `aniemore-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aniemore"
-version = "1.1.1"
+version = "1.2.0"
 authors = [
     "Ilya Lubenets <lii291001@gmail.com>",
     "Nikita Davidchuk <ar4ikov228@gmail.com>",
     "Artem Amentes <artem@socialcode.ru>",
 ]
 maintainers = [
     "Ilya Lubenets <lii291001@gmail.com>",
```

### Comparing `aniemore-1.1.1/README.md` & `aniemore-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,53 +37,57 @@
 | RESD           | 7 эмоций, 4 часа аудиозаписей диалогов **студийное качество**               |
 | RESD_Annotated | RESD + speech-to-text аннотации                                             |
 | REPV           | 2000 голосовых сообщений (.ogg), 200 актеров, 2 нейтральные фразы, 5 эмоций |
 | REPV-S         | 140 голосовых сообщений (.ogg) "Привет, как дела?" с разными эмоциями       |
 
 Вы можете использовать готовые предобученные модели из библиотеки: 
 
-| Модель                                                                                                                            | Точность |
-|-----------------------------------------------------------------------------------------------------------------------------------|----------|
-| Голосовые модели                                                                                                                  |          |
-| [**wav2vec2-xlsr-53-russian-emotion-recognition**](https://huggingface.co/Aniemore/wav2vec2-xlsr-53-russian-emotion-recognition)  | 73%      |
-| [**wav2vec2-emotion-russian-resd**](https://huggingface.co/Aniemore/wav2vec2-emotion-russian-resd)                                | 75%      |
-| [**wavlm-emotion-russian-resd**](https://huggingface.co/Aniemore/wavlm-emotion-russian-resd)                                      | 82%      |
-| [**hubert-emotion-russian-resd**](https://huggingface.co/Aniemore/hubert-emotion-russian-resd)                                    | 75%      |
-| [**unispeech-sat-emotion-russian-resd Copied**](https://huggingface.co/Aniemore/unispeech-sat-emotion-russian-resd)               | 72%      |
-| Текстовые модели                                                                                                                  |          |
-| [**rubert-base-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-base-emotion-russian-cedr-m7)                    | 74%      |
-| [**rubert-tiny2-russian-emotion-detection**](https://huggingface.co/Aniemore/rubert-tiny2-russian-emotion-detection)              | 85%      |
-| [**rubert-large-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-large-emotion-russian-cedr-m7)                  | 76%      |
-| [**rubert-tiny-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-tiny-emotion-russian-cedr-m7)                    | 72%      |
+| Модель                                                                                                                           | Точность |
+|----------------------------------------------------------------------------------------------------------------------------------|----------|
+| Голосовые модели                                                                                                                 |          |
+| [**wav2vec2-xlsr-53-russian-emotion-recognition**](https://huggingface.co/Aniemore/wav2vec2-xlsr-53-russian-emotion-recognition) | 73%      |
+| [**wav2vec2-emotion-russian-resd**](https://huggingface.co/Aniemore/wav2vec2-emotion-russian-resd)                               | 75%      |
+| [**wavlm-emotion-russian-resd**](https://huggingface.co/Aniemore/wavlm-emotion-russian-resd)                                     | 82%      |
+| [**hubert-emotion-russian-resd**](https://huggingface.co/Aniemore/hubert-emotion-russian-resd)                                   | 75%      |
+| [**unispeech-sat-emotion-russian-resd Copied**](https://huggingface.co/Aniemore/unispeech-sat-emotion-russian-resd)              | 72%      |
+| [**wavlm-bert-base**](Aniemore/wavlm-bert-base-s-emotion-russian-resd)                                                           | 81%      |
+| [**wavlm-bert-fusion**](https://huggingface.co/Aniemore/wavlm-bert-fusion-s-emotion-russian-resd)                                | 83%      |
+| Текстовые модели                                                                                                                 |          |
+| [**rubert-base-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-base-emotion-russian-cedr-m7)                   | 74%      |
+| [**rubert-tiny2-russian-emotion-detection**](https://huggingface.co/Aniemore/rubert-tiny2-russian-emotion-detection)             | 85%      |
+| [**rubert-large-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-large-emotion-russian-cedr-m7)                 | 76%      |
+| [**rubert-tiny-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-tiny-emotion-russian-cedr-m7)                   | 72%      |
 
 #### Показатели моделей в разрезе эмоций
 ![показатели моделей.jpg](images/model_sota.jpg)
 
 
 ## <a name="Install"></a>	Установка
 ```shell
 pip install aniemore
 ```
 ## <a name="Install"></a>	Минимальные требования к оборудованию
 
-| Архитектура              | ЦПУ      | ОЗУ   | SSD   |
-|--------------------------|----------|-------|-------|
-| **Wave2Vec2**            | 2 ядра   | 8 ГБ  | 40 ГБ |
-| **WaveLM**               | 2 ядра   | 8 ГБ  | 40 ГБ |
-| **Hubert**               | 2 ядра   | 8 ГБ  | 40 ГБ |
-| **UniSpeechSAT**         | 2 ядра   | 8 ГБ  | 40 ГБ |
-| **Bert_Tiny/Bert_Tiny2** | 2 ядра   | 4 ГБ  | 40 ГБ |
-| **Bert_Base**            | 2 ядра   | 4 ГБ  | 40 ГБ |
-| **Bert_Large**           | 2 ядра   | 8 ГБ  | 40 ГБ |
-| **Whisper Tiny**         | 2 ядра   | 4 ГБ  | 40 ГБ |
-| **Whisper Base**         | 2 ядра   | 4 ГБ  | 40 ГБ |
-| **Whisper Small**        | 2 ядра   | 4 ГБ  | 40 ГБ |
-| **Whisper Medium**       | 2 ядра   | 8 ГБ  | 40 ГБ |
-| **Whisper Large**        | 2 ядра   | 16 ГБ | 40 ГБ |
-| **TextEnhancer**         | 2 ядра   | 4 ГБ  | 40 ГБ |
+| Архитектура              | ЦПУ    | ОЗУ   | SSD   |
+|--------------------------|--------|-------|-------|
+| **Wave2Vec2**            | 2 ядра | 8 ГБ  | 40 ГБ |
+| **WaveLM**               | 2 ядра | 8 ГБ  | 40 ГБ |
+| **Hubert**               | 2 ядра | 8 ГБ  | 40 ГБ |
+| **UniSpeechSAT**         | 2 ядра | 8 ГБ  | 40 ГБ |
+| **Bert_Tiny/Bert_Tiny2** | 2 ядра | 4 ГБ  | 40 ГБ |
+| **Bert_Base**            | 2 ядра | 4 ГБ  | 40 ГБ |
+| **Bert_Large**           | 2 ядра | 8 ГБ  | 40 ГБ |
+| **WavLM Bert Base**      | 2 ядра | 16 ГБ | 40 ГБ |
+| **WavLM Bert Fusion**    | 2 ядра | 16 ГБ | 40 ГБ |
+| **Whisper Tiny**         | 2 ядра | 4 ГБ  | 40 ГБ |
+| **Whisper Base**         | 2 ядра | 4 ГБ  | 40 ГБ |
+| **Whisper Small**        | 2 ядра | 4 ГБ  | 40 ГБ |
+| **Whisper Medium**       | 2 ядра | 8 ГБ  | 40 ГБ |
+| **Whisper Large**        | 2 ядра | 16 ГБ | 40 ГБ |
+| **TextEnhancer**         | 2 ядра | 4 ГБ  | 40 ГБ |
 <hr>
 
 ### Пример использования
 
 Ниже приведены простые примеры использования библиотеки. Для более детальных примеров, в том числе **загрузка cобственной модели** - смотрите сделанный для этого *Google Colab*
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_W2ngr_ShrLdTLVTBP3XF176JW1zdChl)
@@ -115,15 +119,15 @@
 
 ```python
 import torch
 from aniemore.recognizers.multimodal import VoiceTextRecognizer
 from aniemore.utils.speech2text import SmallSpeech2Text
 from aniemore.models import HuggingFaceModel
 
-model = HuggingFaceModel.MultiModal.WavLMBertBase
+model = HuggingFaceModel.MultiModal.WavLMBertFusion
 s2t_model = SmallSpeech2Text()
 
 text = SmallSpeech2Text.recognize('/content/ваш-звуковой-файл.wav').text
 device = 'cuda' if torch.cuda.is_available() else 'cpu'
 
 vtr = VoiceTextRecognizer(model=model, device=device)
 vtr.recognize(('/content/ваш-звуковой-файл.wav', text), return_single_label=True)
@@ -132,15 +136,15 @@
 
 ```python
 import torch
 from aniemore.recognizers.multimodal import MultiModalRecognizer
 from aniemore.utils.speech2text import SmallSpeech2Text
 from aniemore.models import HuggingFaceModel
 
-model = HuggingFaceModel.MultiModal.WavLMBertBase
+model = HuggingFaceModel.MultiModal.WavLMBertFusion
 device = 'cuda' if torch.cuda.is_available() else 'cpu'
 mr = MultiModalRecognizer(model=model, s2t_model=SmallSpeech2Text(), device=device)
 mr.recognize('/content/ваш-звуковой-файл.wav', return_single_label=True)
 ```
 <hr>
 
 ## Доп. ссылки
```

### Comparing `aniemore-1.1.1/PKG-INFO` & `aniemore-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aniemore
-Version: 1.1.1
+Version: 1.2.0
 Summary: Aniemore (Artem Nikita Ilya EMOtion REcognition) is a library for emotion recognition in voice and text for russian language.
 License: MIT
 Author: Ilya Lubenets
 Author-email: lii291001@gmail.com
 Maintainer: Ilya Lubenets
 Maintainer-email: lii291001@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -85,53 +85,57 @@
 | RESD           | 7 эмоций, 4 часа аудиозаписей диалогов **студийное качество**               |
 | RESD_Annotated | RESD + speech-to-text аннотации                                             |
 | REPV           | 2000 голосовых сообщений (.ogg), 200 актеров, 2 нейтральные фразы, 5 эмоций |
 | REPV-S         | 140 голосовых сообщений (.ogg) "Привет, как дела?" с разными эмоциями       |
 
 Вы можете использовать готовые предобученные модели из библиотеки: 
 
-| Модель                                                                                                                            | Точность |
-|-----------------------------------------------------------------------------------------------------------------------------------|----------|
-| Голосовые модели                                                                                                                  |          |
-| [**wav2vec2-xlsr-53-russian-emotion-recognition**](https://huggingface.co/Aniemore/wav2vec2-xlsr-53-russian-emotion-recognition)  | 73%      |
-| [**wav2vec2-emotion-russian-resd**](https://huggingface.co/Aniemore/wav2vec2-emotion-russian-resd)                                | 75%      |
-| [**wavlm-emotion-russian-resd**](https://huggingface.co/Aniemore/wavlm-emotion-russian-resd)                                      | 82%      |
-| [**hubert-emotion-russian-resd**](https://huggingface.co/Aniemore/hubert-emotion-russian-resd)                                    | 75%      |
-| [**unispeech-sat-emotion-russian-resd Copied**](https://huggingface.co/Aniemore/unispeech-sat-emotion-russian-resd)               | 72%      |
-| Текстовые модели                                                                                                                  |          |
-| [**rubert-base-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-base-emotion-russian-cedr-m7)                    | 74%      |
-| [**rubert-tiny2-russian-emotion-detection**](https://huggingface.co/Aniemore/rubert-tiny2-russian-emotion-detection)              | 85%      |
-| [**rubert-large-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-large-emotion-russian-cedr-m7)                  | 76%      |
-| [**rubert-tiny-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-tiny-emotion-russian-cedr-m7)                    | 72%      |
+| Модель                                                                                                                           | Точность |
+|----------------------------------------------------------------------------------------------------------------------------------|----------|
+| Голосовые модели                                                                                                                 |          |
+| [**wav2vec2-xlsr-53-russian-emotion-recognition**](https://huggingface.co/Aniemore/wav2vec2-xlsr-53-russian-emotion-recognition) | 73%      |
+| [**wav2vec2-emotion-russian-resd**](https://huggingface.co/Aniemore/wav2vec2-emotion-russian-resd)                               | 75%      |
+| [**wavlm-emotion-russian-resd**](https://huggingface.co/Aniemore/wavlm-emotion-russian-resd)                                     | 82%      |
+| [**hubert-emotion-russian-resd**](https://huggingface.co/Aniemore/hubert-emotion-russian-resd)                                   | 75%      |
+| [**unispeech-sat-emotion-russian-resd Copied**](https://huggingface.co/Aniemore/unispeech-sat-emotion-russian-resd)              | 72%      |
+| [**wavlm-bert-base**](Aniemore/wavlm-bert-base-s-emotion-russian-resd)                                                           | 81%      |
+| [**wavlm-bert-fusion**](https://huggingface.co/Aniemore/wavlm-bert-fusion-s-emotion-russian-resd)                                | 83%      |
+| Текстовые модели                                                                                                                 |          |
+| [**rubert-base-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-base-emotion-russian-cedr-m7)                   | 74%      |
+| [**rubert-tiny2-russian-emotion-detection**](https://huggingface.co/Aniemore/rubert-tiny2-russian-emotion-detection)             | 85%      |
+| [**rubert-large-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-large-emotion-russian-cedr-m7)                 | 76%      |
+| [**rubert-tiny-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-tiny-emotion-russian-cedr-m7)                   | 72%      |
 
 #### Показатели моделей в разрезе эмоций
 ![показатели моделей.jpg](images/model_sota.jpg)
 
 
 ## <a name="Install"></a>	Установка
 ```shell
 pip install aniemore
 ```
 ## <a name="Install"></a>	Минимальные требования к оборудованию
 
-| Архитектура              | ЦПУ      | ОЗУ   | SSD   |
-|--------------------------|----------|-------|-------|
-| **Wave2Vec2**            | 2 ядра   | 8 ГБ  | 40 ГБ |
-| **WaveLM**               | 2 ядра   | 8 ГБ  | 40 ГБ |
-| **Hubert**               | 2 ядра   | 8 ГБ  | 40 ГБ |
-| **UniSpeechSAT**         | 2 ядра   | 8 ГБ  | 40 ГБ |
-| **Bert_Tiny/Bert_Tiny2** | 2 ядра   | 4 ГБ  | 40 ГБ |
-| **Bert_Base**            | 2 ядра   | 4 ГБ  | 40 ГБ |
-| **Bert_Large**           | 2 ядра   | 8 ГБ  | 40 ГБ |
-| **Whisper Tiny**         | 2 ядра   | 4 ГБ  | 40 ГБ |
-| **Whisper Base**         | 2 ядра   | 4 ГБ  | 40 ГБ |
-| **Whisper Small**        | 2 ядра   | 4 ГБ  | 40 ГБ |
-| **Whisper Medium**       | 2 ядра   | 8 ГБ  | 40 ГБ |
-| **Whisper Large**        | 2 ядра   | 16 ГБ | 40 ГБ |
-| **TextEnhancer**         | 2 ядра   | 4 ГБ  | 40 ГБ |
+| Архитектура              | ЦПУ    | ОЗУ   | SSD   |
+|--------------------------|--------|-------|-------|
+| **Wave2Vec2**            | 2 ядра | 8 ГБ  | 40 ГБ |
+| **WaveLM**               | 2 ядра | 8 ГБ  | 40 ГБ |
+| **Hubert**               | 2 ядра | 8 ГБ  | 40 ГБ |
+| **UniSpeechSAT**         | 2 ядра | 8 ГБ  | 40 ГБ |
+| **Bert_Tiny/Bert_Tiny2** | 2 ядра | 4 ГБ  | 40 ГБ |
+| **Bert_Base**            | 2 ядра | 4 ГБ  | 40 ГБ |
+| **Bert_Large**           | 2 ядра | 8 ГБ  | 40 ГБ |
+| **WavLM Bert Base**      | 2 ядра | 16 ГБ | 40 ГБ |
+| **WavLM Bert Fusion**    | 2 ядра | 16 ГБ | 40 ГБ |
+| **Whisper Tiny**         | 2 ядра | 4 ГБ  | 40 ГБ |
+| **Whisper Base**         | 2 ядра | 4 ГБ  | 40 ГБ |
+| **Whisper Small**        | 2 ядра | 4 ГБ  | 40 ГБ |
+| **Whisper Medium**       | 2 ядра | 8 ГБ  | 40 ГБ |
+| **Whisper Large**        | 2 ядра | 16 ГБ | 40 ГБ |
+| **TextEnhancer**         | 2 ядра | 4 ГБ  | 40 ГБ |
 <hr>
 
 ### Пример использования
 
 Ниже приведены простые примеры использования библиотеки. Для более детальных примеров, в том числе **загрузка cобственной модели** - смотрите сделанный для этого *Google Colab*
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_W2ngr_ShrLdTLVTBP3XF176JW1zdChl)
@@ -163,15 +167,15 @@
 
 ```python
 import torch
 from aniemore.recognizers.multimodal import VoiceTextRecognizer
 from aniemore.utils.speech2text import SmallSpeech2Text
 from aniemore.models import HuggingFaceModel
 
-model = HuggingFaceModel.MultiModal.WavLMBertBase
+model = HuggingFaceModel.MultiModal.WavLMBertFusion
 s2t_model = SmallSpeech2Text()
 
 text = SmallSpeech2Text.recognize('/content/ваш-звуковой-файл.wav').text
 device = 'cuda' if torch.cuda.is_available() else 'cpu'
 
 vtr = VoiceTextRecognizer(model=model, device=device)
 vtr.recognize(('/content/ваш-звуковой-файл.wav', text), return_single_label=True)
@@ -180,15 +184,15 @@
 
 ```python
 import torch
 from aniemore.recognizers.multimodal import MultiModalRecognizer
 from aniemore.utils.speech2text import SmallSpeech2Text
 from aniemore.models import HuggingFaceModel
 
-model = HuggingFaceModel.MultiModal.WavLMBertBase
+model = HuggingFaceModel.MultiModal.WavLMBertFusion
 device = 'cuda' if torch.cuda.is_available() else 'cpu'
 mr = MultiModalRecognizer(model=model, s2t_model=SmallSpeech2Text(), device=device)
 mr.recognize('/content/ваш-звуковой-файл.wav', return_single_label=True)
 ```
 <hr>
 
 ## Доп. ссылки
```

