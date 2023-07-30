# Comparing `tmp/happyaccidentsapi-0.0.2.tar.gz` & `tmp/happyaccidentsapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happyaccidentsapi-0.0.2.tar", max compression
+gzip compressed data, was "happyaccidentsapi-0.0.3.tar", max compression
```

## Comparing `happyaccidentsapi-0.0.2.tar` & `happyaccidentsapi-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10198 2023-07-27 11:31:34.153331 happyaccidentsapi-0.0.2/LICENSE
--rw-r--r--   0        0        0     1831 2023-07-28 17:01:49.246542 happyaccidentsapi-0.0.2/PYPI.md
--rw-r--r--   0        0        0      288 2023-07-28 14:05:49.494814 happyaccidentsapi-0.0.2/happyaccidentsapi/__init__.py
--rw-r--r--   0        0        0     8071 2023-07-28 17:39:42.259527 happyaccidentsapi-0.0.2/happyaccidentsapi/_happyaccidentsapi.py
--rw-r--r--   0        0        0      520 2023-07-28 14:05:19.811055 happyaccidentsapi-0.0.2/happyaccidentsapi/_token.py
--rw-r--r--   0        0        0     2847 2023-07-28 13:23:32.859138 happyaccidentsapi-0.0.2/happyaccidentsapi/enums.py
--rw-r--r--   0        0        0      805 2023-07-28 14:05:33.284581 happyaccidentsapi-0.0.2/happyaccidentsapi/errors.py
--rw-r--r--   0        0        0    12912 2023-07-28 17:39:45.639578 happyaccidentsapi-0.0.2/happyaccidentsapi/models.py
--rw-r--r--   0        0        0     1118 2023-07-28 17:39:54.293041 happyaccidentsapi-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 happyaccidentsapi-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    10198 2023-07-27 11:31:34.153331 happyaccidentsapi-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1831 2023-07-28 17:01:49.246542 happyaccidentsapi-0.0.3/PYPI.md
+-rw-r--r--   0        0        0      288 2023-07-28 14:05:49.494814 happyaccidentsapi-0.0.3/happyaccidentsapi/__init__.py
+-rw-r--r--   0        0        0     8071 2023-07-28 17:39:42.259527 happyaccidentsapi-0.0.3/happyaccidentsapi/_happyaccidentsapi.py
+-rw-r--r--   0        0        0      520 2023-07-28 14:05:19.811055 happyaccidentsapi-0.0.3/happyaccidentsapi/_token.py
+-rw-r--r--   0        0        0     2912 2023-07-30 12:38:56.679689 happyaccidentsapi-0.0.3/happyaccidentsapi/enums.py
+-rw-r--r--   0        0        0      805 2023-07-28 14:05:33.284581 happyaccidentsapi-0.0.3/happyaccidentsapi/errors.py
+-rw-r--r--   0        0        0    13197 2023-07-30 13:21:37.501464 happyaccidentsapi-0.0.3/happyaccidentsapi/models.py
+-rw-r--r--   0        0        0     1118 2023-07-30 13:23:28.143038 happyaccidentsapi-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 happyaccidentsapi-0.0.3/PKG-INFO
```

### Comparing `happyaccidentsapi-0.0.2/LICENSE` & `happyaccidentsapi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.2/PYPI.md` & `happyaccidentsapi-0.0.3/PYPI.md`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.2/happyaccidentsapi/_happyaccidentsapi.py` & `happyaccidentsapi-0.0.3/happyaccidentsapi/_happyaccidentsapi.py`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.2/happyaccidentsapi/_token.py` & `happyaccidentsapi-0.0.3/happyaccidentsapi/_token.py`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.2/happyaccidentsapi/enums.py` & `happyaccidentsapi-0.0.3/happyaccidentsapi/enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,98 +1,98 @@
 from enum import Enum
 
 
-class AccountStatus(Enum):
+class AccountStatus(str, Enum):
     ACTIVE = "ACTIVE"
     BANNED = "BANNED"
 
 
-class CivitAiBaseModelType(Enum):
+class CivitAiBaseModelType(str, Enum):
     SD14 = "SD 1.4"
     SD15 = "SD 1.5"
     SD20 = "SD 2.0"
     SD20_768 = "SD 2.0 768"
     SD21 = "SD 2.1"
     SD21_768 = "SD 2.1 768"
     OTHER = "Other"
 
 
-class CivitAiModelType(Enum):
+class CivitAiModelType(str, Enum):
     CHECKPOINT = "Checkpoint"
     TEXTUAL_INVERSION = "TextualInversion"
     HYPERNETWORK = "Hypernetwork"
     AESTHETIC_GRADIENT = "AestheticGradient"
     LORA = "LORA"
     LOCON = "LoCon"
     CONTROLNET = "Controlnet"
     POSES = "Poses"
     OTHER = "Other"
     WILCARDS = "Wildcards"
 
 
-class CivitAiSortByType(Enum):
+class CivitAiSortByType(str, Enum):
     HIGHEST_RATED = "Highest Rated"
     MOST_DOWNLOADED = "Most Downloaded"
     NEWEST = "Newest"
     FAVORITED = "Favorited"
 
 
-class DownloadStatus(Enum):
+class DownloadStatus(str, Enum):
     QUEUE = "QUEUED"
     DOWNLOADING = "DOWNLOADING"
     CONVERTING = "CONVERTING"
     COMPLETED = "COMPLETED"
     FAILED = "FAILED"
 
 
-class InferenceStatus(Enum):
+class InferenceStatus(str, Enum):
     PENDING = "PENDING"
     COMPLETED = "COMPLETED"
     FAILED = "FAILED"
 
 
-class InferenceType(Enum):
+class InferenceType(str, Enum):
     FACE_RESTORE = "FACE_RESTORE"
     UPSCALING = "UPSCALING"
     IMAGE_TO_IMAGE = "IMAGE_TO_IMAGE"
     TEXT_TO_IMAGE = "TEXT_TO_IMAGE"
     INPAINTING = "INPAINTING"
     CONTROLNET_TXT2IMG = "CONTROLNET_TXT2IMG"
     CONTROLNET_IMG2IMG = "CONTROLNET_IMG2IMG"
     CONTROLNET_INPAINTING = "CONTROLNET_INPAINTING"
 
 
-class NotificationStatus(Enum):
+class NotificationStatus(str, Enum):
     PENDING = "PENDING"
     APPROVED = "APPROVED"
     REJECTED = "REJECTED"
     SEND_SUCCESSFUL = "SEND_SUCCESSFUL"
     SEND_FAILURE = "SEND_FAILURE"
 
 
-class PreprocessingTechnique(Enum):
+class PreprocessingTechnique(str, Enum):
     CANNY_EDGES = "CANNY_EDGES"
     OPENPOSE = "OPENPOSE"
     SCRIBBLE = "SCRIBBLE"
     SEGMENT = "SEGMENT"
     MLSD = "MLSD"
     HED = "HED"
     MIDAS_DEPTH = "MIDAS_DEPTH"
     REFERENCE_ONLY = "REFERENCE_ONLY"
     TILE = "TILE"
 
 
-class QueuePriority(Enum):
+class QueuePriority(str, Enum):
     TEN_MINUTES = "10m"
     ONE_MINUTE = "1m"
     TEN_SECONDS = "10s"
     ONE_SECOND = "1s"
 
 
-class SamplingMethod(Enum):
+class SamplingMethod(str, Enum):
     EULER = "EULER"
     EULER_A = "EULER_A"
     LMS = "LMS"
     LMS_KARRAS = "LMS_KARRAS"
     DDPM = "DDPM"
     DDIM = "DDIM"
     DPM_SOLVER_MULTISTEP = "DPM_SOLVER_MULTISTEP"
@@ -102,17 +102,17 @@
     DPM_2PLUS_SDE = "DPM_++_SDE"
     DPM_2PLUS_SDE_KARRAS = "DPM_++_SDE_KARRAS"
     UNI_PC = "UNI_PC"
     DPM_DISCRETE_SCHEDULER = "DPM_DISCRETE_SCHEDULER"
     DPM_DISCRETE_SCHEDULER_ANCESTRAL = "DPM_DISCRETE_SCHEDULER_ANCESTRAL"
 
 
-class VariationalAutoEncoder(Enum):
+class VariationalAutoEncoder(str, Enum):
     SD_VAE_FT_EMA = "stabilityai/sd-vae-ft-ema"
     SD_VAE_FT_MSE = "stabilityai/sd-vae-ft-mse"
     ABYSS_ORANGE_MIX = "abyss-orange-mix"
     KL_F8_ANIME2 = "kl-f8-anime2"
 
 
-class UserRole(Enum):
+class UserRole(str, Enum):
     ADMIN = "ADMIN"
     MOD = "MOD"
```

### Comparing `happyaccidentsapi-0.0.2/happyaccidentsapi/errors.py` & `happyaccidentsapi-0.0.3/happyaccidentsapi/errors.py`

 * *Files identical despite different names*

### Comparing `happyaccidentsapi-0.0.2/happyaccidentsapi/models.py` & `happyaccidentsapi-0.0.3/happyaccidentsapi/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,16 +146,16 @@
     metadata: ModelsMetadata
 
     def first(self):
         return self.items[0]
 
 
 class CannyEdgesPayload(BaseModel):
-    lowThreshold: int = Field(title="Lowthreshold")
-    upperThreshold: int = Field(title="Upperthreshold")
+    lowThreshold: int = Field(ge=1, le=255, title="Lowthreshold")
+    upperThreshold: int = Field(ge=1, le=255, title="Upperthreshold")
 
 
 class Esrgan4xUpscalingParams(BaseModel):
     parentInferenceId: Optional[str] = Field(None, title="Parentinferenceid")
     imageUrl: str = Field(title="Imageurl")
     scale: Optional[float] = Field(4.0, title="Scale")
     faceEnhance: Optional[bool] = Field(False, title="Faceenhance")
@@ -172,16 +172,16 @@
 
 class HedPayload(BaseModel):
     scribble: bool = Field(title="Scribble")
 
 
 class HighResFixParams(BaseModel):
     enabled: Optional[bool] = Field(False, title="Enabled")
-    imageStrength: Optional[float] = Field(0.2, title="Imagestrength")
-    steps: Optional[int] = Field(25, title="Steps")
+    imageStrength: Optional[float] = Field(0.2, ge=0.0, le=0.9, title="Imagestrength")
+    steps: Optional[int] = Field(25, ge=1, le=75, title="Steps")
 
 
 class ImageRecord(BaseModel):
     id: str = Field(title="Id")
     folderPath: str = Field(title="Folderpath")
     filename: str = Field(title="Filename")
     createdAt: str = Field(title="Createdat")
@@ -233,26 +233,26 @@
 
     def get_url(self) -> HttpUrl:
         return f"https://ik.imagekit.io/hb42m9hh0/{self.folderPath}/{self.filename}"
 
 
 class LoraParams(BaseModel):
     id: str = Field(title="Id")
-    weight: float = Field(title="Weight")
+    weight: float = Field(ge=0, le=1, title="Weight")
 
 
 class MidasDepthPayload(BaseModel):
     surfaceNormalAngleRadians: float = Field(title="Surfacenormalangleradians")
-    backgroundThreshold: float = Field(title="Backgroundthreshold")
+    backgroundThreshold: float = Field(ge=0.0, le=1.0, title="Backgroundthreshold")
     depthAndNormal: bool = Field(title="Depthandnormal")
 
 
 class MlsdPayload(BaseModel):
-    valueThreshold: float = Field(title="Valuethreshold")
-    distanceThreshold: float = Field(title="Distancethreshold")
+    valueThreshold: float = Field(ge=0.0, le=2.0, title="Valuethreshold")
+    distanceThreshold: float = Field(ge=1, le=20, title="Distancethreshold")
 
 
 class ModelDownloadRequestParams(BaseModel):
     externalId: str = Field(title="Externalid")
     modelVersionExternalId: Optional[str] = Field(None, title="Modelversionexternalid")
 
 
@@ -292,18 +292,22 @@
             OpenposePayload,
             MlsdPayload,
             HedPayload,
             MidasDepthPayload,
         ]
     ] = Field(None, title="Preprocessingpayload")
     controlnetConditioningScale: Optional[float] = Field(
-        1, title="Controlnetconditioningscale"
+        1, ge=0.1, le=2.0, title="Controlnetconditioningscale"
+    )
+    controlGuidanceStart: Optional[float] = Field(
+        [0.0], ge=0.0, le=1.0, title="Controlguidancestart"
+    )
+    controlGuidanceEnd: Optional[float] = Field(
+        [1.0], ge=0.0, le=1.0, title="Controlguidanceend"
     )
-    controlGuidanceStart: Optional[float] = Field([0.0], title="Controlguidancestart")
-    controlGuidanceEnd: Optional[float] = Field([1.0], title="Controlguidanceend")
     preprocessedImageUrl: Optional[str] = Field(None, title="Preprocessedimageurl")
 
 
 class User(BaseModel):
     id: str = Field(title="Id")
     username: Optional[str] = Field(None, title="Username")
     fullName: Optional[str] = Field(None, title="Fullname")
@@ -323,26 +327,28 @@
 class CreateInferenceParams(BaseModel):
     parentInferenceId: Optional[str] = Field(None, title="Parentinferenceid")
     modelId: str = Field(title="Modelid")
     prompt: str = Field(title="Prompt")
     negativePrompt: Optional[str] = Field("", title="Negativeprompt")
     baseImageUrl: Optional[str] = Field(None, title="Baseimageurl")
     maskImageUrl: Optional[str] = Field(None, title="Maskimageurl")
-    inpaintingMaskBlur: Optional[float] = Field(3.0, title="Inpaintingmaskblur")
-    outputWpx: Optional[int] = Field(512, title="Outputwpx")
-    outputHpx: Optional[int] = Field(512, title="Outputhpx")
+    inpaintingMaskBlur: Optional[float] = Field(
+        3.0, ge=0, le=10, title="Inpaintingmaskblur"
+    )
+    outputWpx: Optional[int] = Field(512, ge=1, le=1024, title="Outputwpx")
+    outputHpx: Optional[int] = Field(512, ge=1, le=1024, title="Outputhpx")
     numImagesToGenerate: Optional[int] = Field(1, title="Numimagestogenerate")
-    numInferenceSteps: Optional[int] = Field(25, title="Numinferencesteps")
+    numInferenceSteps: Optional[int] = Field(25, ge=1, le=75, title="Numinferencesteps")
     samplingMethod: Optional[SamplingMethod] = "EULER"  # noqa: F405
     vae: Optional[VariationalAutoEncoder] = "stabilityai/sd-vae-ft-mse"  # noqa: F405
     lora: Optional[LoraParams] = None
     embeddingIds: Optional[List[str]] = Field([], title="Embeddingids")
-    guidanceScale: Optional[float] = Field(7.0, title="Guidancescale")
-    strength: Optional[float] = Field(0.5, title="Strength", le=0.9, ge=0.1)
-    clipSkip: Optional[int] = Field(1, title="Clipskip")
+    guidanceScale: Optional[float] = Field(7.0, ge=1, le=20, title="Guidancescale")
+    strength: Optional[float] = Field(0.5, title="Strength", le=0.9, ge=0.0)
+    clipSkip: Optional[int] = Field(1, ge=1, le=5, title="Clipskip")
     seed: Optional[int] = Field(None, title="Seed")
     controlNetPayloads: Optional[List[PreprocessingParams]] = Field(
         [], title="Controlnetpayloads"
     )
     highResFix: Optional[HighResFixParams] = None
```

### Comparing `happyaccidentsapi-0.0.2/pyproject.toml` & `happyaccidentsapi-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "happyaccidentsapi"
-version = "0.0.2"
+version = "0.0.3"
 description = "API Wrapper for HappyAccidents"
 authors = ["hoopengo <hoopengo@yandex.ru>"]
 readme = ["PYPI.md"]
 license = "Apache-2.0"
 repository = "https://github.com/hoopengo/happyaccidentsapi"
 keywords = ["api", "happyaccidents", "ai"]
 classifiers = [
```

### Comparing `happyaccidentsapi-0.0.2/PKG-INFO` & `happyaccidentsapi-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happyaccidentsapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: API Wrapper for HappyAccidents
 Home-page: https://github.com/hoopengo/happyaccidentsapi
 License: Apache-2.0
 Keywords: api,happyaccidents,ai
 Author: hoopengo
 Author-email: hoopengo@yandex.ru
 Requires-Python: >=3.8,<4.0
```

