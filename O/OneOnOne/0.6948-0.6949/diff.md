# Comparing `tmp/OneOnOne-0.6948.tar.gz` & `tmp/OneOnOne-0.6949.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6948.tar", last modified: Tue Jul 25 07:28:27 2023, max compression
+gzip compressed data, was "OneOnOne-0.6949.tar", last modified: Sun Jul 30 06:03:21 2023, max compression
```

## Comparing `OneOnOne-0.6948.tar` & `OneOnOne-0.6949.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-25 07:28:27.457652 OneOnOne-0.6948/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6948/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-25 07:28:27.450254 OneOnOne-0.6948/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    55677 2023-07-25 06:44:50.000000 OneOnOne-0.6948/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6948/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6948/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6948/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6948/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6948/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6948/OneOnOne/sampling.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-25 07:28:27.456045 OneOnOne-0.6948/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-25 07:28:27.000000 OneOnOne-0.6948/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-25 07:28:27.000000 OneOnOne-0.6948/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-25 07:28:27.000000 OneOnOne-0.6948/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      166 2023-07-25 07:28:27.000000 OneOnOne-0.6948/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-25 07:28:27.000000 OneOnOne-0.6948/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-25 07:28:27.456916 OneOnOne-0.6948/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3491 2023-07-24 15:56:25.000000 OneOnOne-0.6948/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-25 07:28:27.457914 OneOnOne-0.6948/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1972 2023-07-25 07:28:16.000000 OneOnOne-0.6948/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:03:21.595991 OneOnOne-0.6949/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6949/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:03:21.591879 OneOnOne-0.6949/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    70464 2023-07-29 19:06:01.000000 OneOnOne-0.6949/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6949/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14251 2023-07-28 06:59:10.000000 OneOnOne-0.6949/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     7164 2023-07-29 12:25:37.000000 OneOnOne-0.6949/OneOnOne/clustering.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6949/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3403 2023-07-29 18:08:15.000000 OneOnOne-0.6949/OneOnOne/conversation.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6949/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1930 2023-07-29 18:38:09.000000 OneOnOne-0.6949/OneOnOne/imagetranslator.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      995 2023-07-29 18:59:58.000000 OneOnOne-0.6949/OneOnOne/pdftotext.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     1880 2023-07-28 06:59:09.000000 OneOnOne-0.6949/OneOnOne/pretrainedmodel.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6949/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    23928 2023-07-28 06:59:10.000000 OneOnOne-0.6949/OneOnOne/sampling.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      888 2023-07-29 17:53:14.000000 OneOnOne-0.6949/OneOnOne/texttranslator.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-30 06:03:21.595028 OneOnOne-0.6949/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1597 2023-07-30 06:03:21.000000 OneOnOne-0.6949/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      504 2023-07-30 06:03:21.000000 OneOnOne-0.6949/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-30 06:03:21.000000 OneOnOne-0.6949/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      218 2023-07-30 06:03:21.000000 OneOnOne-0.6949/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-30 06:03:21.000000 OneOnOne-0.6949/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1597 2023-07-30 06:03:21.595544 OneOnOne-0.6949/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3701 2023-07-29 19:02:55.000000 OneOnOne-0.6949/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-30 06:03:21.596127 OneOnOne-0.6949/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     2055 2023-07-29 18:08:15.000000 OneOnOne-0.6949/setup.py
```

### Comparing `OneOnOne-0.6948/LICENSE` & `OneOnOne-0.6949/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6948/OneOnOne/__init__.py` & `OneOnOne-0.6949/OneOnOne/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 from transformers import pipeline
 from transformers import BlipProcessor, BlipForQuestionAnswering
 from transformers import GPT2Tokenizer, GPT2ForQuestionAnswering
 from transformers import AutoTokenizer, AutoModel
 from transformers import AutoTokenizer, RobertaForQuestionAnswering
 from transformers import BertForQuestionAnswering, BertTokenizer
 from transformers import AutoTokenizer, ErnieModel
+from transformers import pipeline, Conversation
+
 import torch
 from torchvision import transforms
 
 from bs4 import BeautifulSoup
 import re
 from tqdm import keras
 import pkgutil
@@ -55,14 +57,25 @@
 
 import warnings
 
 import copy
 from bayes_opt import BayesianOptimization
 tf.config.run_functions_eagerly(True)
 
+from pydub import AudioSegment
+import speech_recognition as sr
+import pyttsx3
+import pytesseract
+from googletrans import Translator
+from io import BytesIO
+from base64 import b64decode
+from google.colab import output
+from IPython.display import Javascript
+import PyPDF2
+
 class PretrainedModel:
     def __init__(self, model_type="resnet50", dataset="cifar10", samplingtype="none"):
         warnings.filterwarnings("ignore")
 
         self.model_type=model_type.lower()
         self.dataset=dataset.lower()
         self.samplingtype=samplingtype.lower()
@@ -892,15 +905,15 @@
             y_temp.append(self.y_train_copy[values_lc[i][0]])
 
         for i in range(0, hc_jump):
             x_temp.append(self.X_train_copy[values_hc[i][0]])
             y_temp.append(self.y_train_copy[values_hc[i][0]])
 
         h = temp_model.fit(datagen.flow(np.array(x_temp), np.array(y_temp), batch_size=self.batch_size),
-                           validation_data=(self.X_test, self.y_test), epochs=10, callbacks=[lr_scheduler,lr_reducer], verbose=1,
+                           validation_data=(self.X_test, self.y_test), epochs=50, callbacks=[lr_scheduler,lr_reducer], verbose=1,
                            workers=4)
 
         score = temp_model.evaluate(self.X_test, self.y_test)
 
         return 100 * float(score[1])
 
     def get_bayes_coeff(self):
@@ -1152,21 +1165,20 @@
         return datagen
 
     def decide_context(self):
 
         from classes import i2d
 
         predicted_list = []
-        classes_prob_list = []
         prediction_index = []
         final_classes = []
 
         output = []
 
-        labels = self.val_it.class_indices
+        labels = self.train_it.class_indices+self.val_it.class_indices
         labels2 = dict((v, k) for k, v in labels.items())
 
         for i in range(0, self.pred.shape[0]):
             classes_prob_list = []
             for j in range(0, self.output_layer_classes):
                 classes_prob_list.append([int(j), self.pred[i][j]])
 
@@ -1376,10 +1388,392 @@
 
             if not flag:
                 break
 
             print(self.question_answer(question))
 
 
+# https://tesseract-ocr.github.io/tessdoc/Data-Files-in-different-versions.html
+class TextTranslator:
+    def __init__(self, file_bool=False,filepath="", translate_from_language="ben", translate_to_language="en", speak_bool=False):
+        self.file_bool=file_bool
+        self.filepath=filepath
+        self.translate_from_language = translate_from_language
+        self.translate_to_language = translate_to_language
+        self.speak_bool = speak_bool
+
+        if self.file_bool:
+            file = open(os.getcwd()+f"/{self.filepath}","r")
+            text=file.readlines()[0]
+            print(file.readlines())
+        else:
+            text=input("What do you want to translate?:     ")
+
+        k = translator.translate(text, dest=self.translate_to_language)
+        with open(f'{self.imgpath}_text_{self.translate_to_language}.txt', mode='w') as file:
+            file.write(k.text)
+        print(k.text)
+
+        if speak_bool:
+            self.speak(k.text)
+
+
+class ImageTranslator:
+    def __init__(self, imgpath, translate_from_language="ben", translate_to_language="en", speak_bool=False):
+        self.translate_from_language=translate_from_language
+        self.translate_to_language=translate_to_language
+        self.imgpath=imgpath
+        self.speak_bool=speak_bool
+
+    def speak(self, command):
+
+        engine = pyttsx3.init()
+        engine.say(command)
+        engine.runAndWait()
+
+        if speak:
+            try:
+                os.system("sudo apt install espeak")
+                os.system("sudo apt install libespeak-dev")
+            except:
+                os.system("!sudo apt install espeak")
+                os.system("!sudo apt install libespeak-dev")
+
+
+        try:
+            os.system("sudo apt install tesseract-ocr")
+            os.system("apt install libtesseract-dev")
+            os.system(f"apt install tesseract-ocr-{self.translate_from_language}")
+            os.system(f"apt install tesseract-ocr-{self.translate_to_language}")
+        except:
+            os.system("!sudo apt install tesseract-ocr")
+            os.system("!apt install libtesseract-dev")
+            os.system(f"!apt install tesseract-ocr-{self.translate_from_language}")
+            os.system(f"!apt install tesseract-ocr-{self.translate_to_language}")
+
+        img = Image.open(os.getcwd()+"/"+self.imgpath)
+
+        result = pytesseract.image_to_string(img,lang=self.translate_from_language)
+        with open(f'{self.imgpath}_text_{self.translate_from_language}.txt', mode='w') as file:
+            file.write(result)
+            print(result)
+
+        translator = Translator()
+
+        k = translator.translate(result.replace("\n"," ")[:-5], dest=self.translate_to_language)
+        with open(f'{self.imgpath}_text_{self.translate_to_language}.txt', mode='w') as file:
+            file.write(k.text)
+        print(k.text)
+
+        if speak_bool:
+            self.speak(k.text)
+
+
+class Conversation:
+    def __init__(self):
+        warnings.filterwarnings("ignore")
+
+        self.conversational_pipeline = pipeline("conversational")
+
+        try:
+            os.system("apt install libasound2-dev portaudio19-dev libportaudio2 libportaudiocpp0 ffmpeg")
+        except:
+            os.system("!apt install libasound2-dev portaudio19-dev libportaudio2 libportaudiocpp0 ffmpeg")
+
+        self.recognizer = sr.Recognizer()
+
+        self.RECORD = """
+                const sleep  = time => new Promise(resolve => setTimeout(resolve, time))
+                const b2text = blob => new Promise(resolve => {
+                  const reader = new FileReader()
+                  reader.onloadend = e => resolve(e.srcElement.result)
+                  reader.readAsDataURL(blob)
+                })
+                var record = time => new Promise(async resolve => {
+                  stream = await navigator.mediaDevices.getUserMedia({ audio: true })
+                  recorder = new MediaRecorder(stream)
+                  chunks = []
+                  recorder.ondataavailable = e => chunks.push(e.data)
+                  recorder.start()
+                  await sleep(time)
+                  recorder.onstop = async ()=>{
+                    blob = new Blob(chunks)
+                    text = await b2text(blob)
+                    resolve(text)
+                  }
+                  recorder.stop()
+                })
+                """
+    def record(self,sec=3):
+        display(Javascript(RECORD))
+        sec += 1
+        s = output.eval_js('record(%d)' % (sec*1000))
+        b = b64decode(s.split(',')[1])
+        return b
+
+    def speak(self,command):
+
+        engine = pyttsx3.init()
+        engine.say(command)
+        engine.runAndWait()
+
+    def answer(self,question):
+        output = self.conversational_pipeline([question])
+        out_list = str(output).split("\n")
+        temp = out_list[2].split(">>")
+        output = temp[1].replace("\n", "")
+        return output
+
+    def converse(self):
+
+        while True:
+
+            try:
+
+                audio_source = sr.AudioData(self.record(), 16000, 2)
+
+                question = self.recognize_google(audio_data=audio_source,language = 'en-IN')
+                question = question.lower()
+
+                print(f"{question}?")
+                # self.speak(question)
+
+                answer_output=self.answer(question)
+                self.speak(answer_output)
+                #
+                # with sr.Microphone() as source2:
+                #
+                #     r.adjust_for_ambient_noise(source2,duration=5)
+                #     print("Listening...")
+                #
+                #     audio2 = r.listen(source2,timeout=5,phrase_time_limit=5)
+                #
+                #     print("Recognizing...")
+                #
+                #     question = self.recognizer.recognize_google(audio2,language = 'en-IN')
+                #     question = question.lower()
+                #
+                #     print("Did you say " + question)
+                #     self.speak(question)
+                #
+                #     answer_output=self.answer(question)
+                #     self.speak(answer_output)
+
+            except sr.RequestError as e:
+                print("Could not request results; {0}".format(e))
+
+            except sr.UnknownValueError:
+                print("Unknown Error Occured")
+
+
+class PDFtoText:
+    def __init__(self, pdfpath, speak_bool=False):
+        self.pdfpath = imgpath
+        self.speak_bool = speak_bool
+
+    def convert(self, command):
+
+        engine = pyttsx3.init()
+        engine.say(command)
+        engine.runAndWait()
+
+        if speak:
+            try:
+                os.system("sudo apt install espeak")
+                os.system("sudo apt install libespeak-dev")
+            except:
+                os.system("!sudo apt install espeak")
+                os.system("!sudo apt install libespeak-dev")
+
+        path = open(os.getcwd() + f'/{self.pdfpath}', 'rb')
+
+        pdfReader = PyPDF2.PdfFileReader(path)
+
+        output = ""
+        for i in range(pdfReader.numPages):
+            pageObj = pdfReader.getPage(i)
+            output += pageObj.extractText()
+
+        with open(f'{self.pdfpath}_text.txt', mode='w') as file:
+            file.write(output)
+
+        print(output)
+
+        if speak_bool:
+            self.speak(k.text)
+
+        return output
+
+
+class Clustering:
+    def __init__(self, data, score_type="silhouette", pca_plot=False, type="kmeans"):
+
+        self.data = data.dropna(axis=1)
+
+        self.pca_plot = pca_plot
+        self.type = type
+        self.score_type = score_type
+        self.n_components = self.get_n_components()
+
+        print(f"no. of components: {self.n_components}")
+        self.preprocessor = Pipeline([("scaler", MinMaxScaler()), ("pca", PCA())])
+        self.preprocessor.fit(self.data)
+        self.preprocessed_data = self.preprocessor.transform(self.data)
+
+        if self.type == "kmeans":
+            self.kmeans_kwargs = {"init": "random", "n_init": 50, "max_iter": 500, "random_state": 22, }
+            self.n_clusters = self.get_n_clusters()
+            self.kmeans = KMeans(n_clusters=self.n_clusters, **self.kmeans_kwargs)
+            self.kmeans.fit(self.preprocessed_data)
+            self.labels = self.kmeans.labels_
+
+        elif self.type == "spectral":
+            self.spectral_kwargs = {"n_init": 50, "random_state": 22, "affinity": 'nearest_neighbors', }
+            # 'eigen_solver':"arpack",
+            self.n_clusters = self.get_n_clusters()
+            self.spectral = SpectralClustering(n_clusters=self.n_clusters, **self.spectral_kwargs)
+            self.spectral.fit(self.preprocessed_data)
+            self.labels = self.spectral.labels_
+
+        elif self.type == "heirarchical":
+            self.heirarchical_kwargs = {"metric": 'euclidean', "linkage": 'ward'}
+            self.n_clusters = self.get_n_clusters()
+            self.heirarchical = AgglomerativeClustering(n_clusters=self.n_clusters, **self.heirarchical_kwargs)
+            self.heirarchical.fit(self.preprocessed_data)
+            self.labels = self.heirarchical.labels_
+
+        print(f"no. of clusters: {self.n_clusters}")
+
+    def plot_groups(self):
+        fte_colors = {
+            -1: "#003428",
+            0: "#008fd5",
+            1: "#fc4f30",
+            2: "#000000",
+            3: "#ffffff",
+            4: "#389241",
+            5: "#434822"}
+
+        if self.type == "kmeans":
+            a = self.kmeans.fit_predict(self.preprocessed_data)
+            fig, ax = plt.subplots()
+            sns.scatterplot(x=self.preprocessed_data[:, 0], y=self.preprocessed_data[:, 1], hue=a, ax=ax)
+            kmeans_silhouette = silhouette_score(self.preprocessed_data, self.kmeans.labels_).round(2)
+            ax.set(title=f"{self.type} Clustering:    Silhouette: {kmeans_silhouette}")
+
+        elif self.type == "spectral":
+            a = self.spectral.fit_predict(self.preprocessed_data)
+            fig, ax = plt.subplots()
+            sns.scatterplot(x=self.preprocessed_data[:, 0], y=self.preprocessed_data[:, 1], hue=a, ax=ax)
+            spectral_silhouette = silhouette_score(self.preprocessed_data, self.spectral.labels_).round(2)
+            ax.set(title=f"{self.type} Clustering:    Silhouette: {spectral_silhouette}")
+
+        elif self.type == "heirarchical":
+            a = self.heirarchical.fit_predict(self.preprocessed_data)
+            fig, ax = plt.subplots()
+            sns.scatterplot(x=self.preprocessed_data[:, 0], y=self.preprocessed_data[:, 1], hue=a, ax=ax)
+            heirarchical_silhouette = silhouette_score(self.preprocessed_data, self.heirarchical.labels_).round(2)
+            ax.set(title=f"{self.type} Clustering:    Silhouette: {heirarchical_silhouette}")
+
+        else:
+            print("Invalid Input!")
+
+    def get_n_components(self):
+        pca = PCA(random_state=22)
+
+        x_pca = pca.fit_transform(self.data)
+
+        exp_var_pca = pca.explained_variance_ratio_
+
+        cum_sum_eigenvalues = np.cumsum(exp_var_pca)
+
+        n = -1
+
+        for i in range(len(cum_sum_eigenvalues)):
+            if cum_sum_eigenvalues[i] > 0.90:
+                n = i
+                break
+
+        if n == -1:
+            for i in range(len(cum_sum_eigenvalues)):
+                if cum_sum_eigenvalues[i] > 0.85:
+                    n = i
+                    break
+
+        if self.pca_plot:
+            plt.bar(range(0, len(exp_var_pca)), exp_var_pca, alpha=0.5, align='center',
+                    label='Individual explained variance')
+            plt.step(range(0, len(cum_sum_eigenvalues)), cum_sum_eigenvalues, where='mid',
+                     label='Cumulative explained variance')
+            plt.ylabel('Explained variance ratio')
+            plt.xlabel('Principal component index')
+            plt.legend(loc='best')
+            plt.tight_layout()
+            plt.show()
+
+        return n
+
+    def get_n_clusters(self):
+
+        coeff = []
+
+        if self.score_type == "silhouette":
+            if self.type == "kmeans":
+                for k in range(2, 11):
+                    kmeans = KMeans(n_clusters=k, **self.kmeans_kwargs)
+                    kmeans.fit(self.preprocessed_data)
+                    score = silhouette_score(self.preprocessed_data, kmeans.labels_)
+                    coeff.append(score)
+            elif self.type == "spectral":
+                for k in range(2, 11):
+                    spectral = SpectralClustering(n_clusters=k, **self.spectral_kwargs)
+                    spectral.fit(self.preprocessed_data)
+                    score = silhouette_score(self.preprocessed_data, spectral.labels_)
+                    coeff.append(score)
+            elif self.type == "heirarchical":
+                for k in range(2, 11):
+                    heirarchical = AgglomerativeClustering(n_clusters=k, **self.heirarchical_kwargs)
+                    heirarchical.fit(self.preprocessed_data)
+                    score = silhouette_score(self.preprocessed_data, heirarchical.labels_)
+                    coeff.append(score)
+
+            plt.style.use("fivethirtyeight")
+            plt.plot(range(2, 11), coeff)
+            plt.xticks(range(2, 11))
+            plt.xlabel("Number of Clusters")
+            plt.ylabel("Silhouette Coefficient")
+            plt.show()
+
+        elif self.score_type == "sse":
+            if self.type == "kmeans":
+                for k in range(2, 11):
+                    kmeans = KMeans(n_clusters=k, **self.kmeans_kwargs)
+                    kmeans.fit(self.preprocessed_data)
+                    coeff.append(kmeans.inertia_)
+            elif self.type == "spectral":
+                for k in range(2, 11):
+                    spectral = SpectralClustering(n_clusters=k, **self.spectral_kwargs)
+                    spectral.fit(self.preprocessed_data)
+                    coeff.append(spectral.inertia_)
+            elif self.type == "heirarchical":
+                for k in range(2, 11):
+                    heirarchical = AgglomerativeClustering(n_clusters=k, **self.heirarchical_kwargs)
+                    heirarchical.fit(self.preprocessed_data)
+                    coeff.append(heirarchical.inertia_)
+
+            plt.style.use("fivethirtyeight")
+            plt.plot(range(2, 11), coeff)
+            plt.xticks(range(2, 11))
+            plt.xlabel("Number of Clusters")
+            plt.ylabel("SSE")
+            plt.show()
+
+        kl = KneeLocator(range(2, 11), coeff, curve="convex", direction="decreasing")
+        print(kl.elbow)
+
+        return kl.elbow
+
+
+
```

### Comparing `OneOnOne-0.6948/OneOnOne/classes.py` & `OneOnOne-0.6949/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6948/OneOnOne/classification.py` & `OneOnOne-0.6949/OneOnOne/classification.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-
 class Classification:
     def __init__(self, model_type="resnet50", batch_size=16, epochs=250, dataset="cifar10", validation_split=0.3, shuffle_bool=True, early_stopping_patience=10, lr_reducer_patience=10):
+        warnings.filterwarnings("ignore")
 
-        self.model_type = model_type
-        self.date = datetime.datetime.now()
-        self.dataset=dataset
+        self.model_type = model_type.lower()
+        self.date=datetime.datetime.now()
+        self.dataset=dataset.lower()
         self.shuffle_bool = shuffle
         self.batch_size = batch_size
         self.epochs = epochs
         self.output_layer_classes=0
         self.input_shape = (32,32,3)
         self.early_stopping_patience=early_stopping_patience
         self.lr_reducer_patience=lr_reducer_patience
@@ -16,71 +16,80 @@
         self.callbacks = self.get_callbacks()
         self.datagen = self.get_datagen()
 
         if self.dataset=="cifar10":
             self.output_layer_classes = 10
             self.input_shape = (224,224,3)
 
+        elif self.dataset == "cifar100":
+            self.output_layer_classes = 100
+            self.input_shape = (224, 224, 3)
 
         elif self.dataset=="tinyimagenet":
             self.output_layer_classes = 200
             self.input_shape = (32, 32, 3)
-            from classes import i2d
             self.download_dataset()
+            from classes import i2d
 
         else:
             print("Invalid Input!")
 
         self.token=input("Train/Load?  :   ")
         self.train_it, self.val_it = self.get_dataset()
 
-        if self.token.lower() == 'train':
-            print("training")
+        if self.token.lower()=='train':
+            print("Training...")
 
             self.model = self.define_compile_model()
             self.model.summary()
 
-            history = self.model.fit(self.train_it, validation_data=self.val_it,
-                                     epochs=self.epochs, verbose=1, workers=4,
-                                     callbacks=self.callbacks)
+            if self.dataset=="tinyimagenet":
+                history = self.model.fit(self.train_it, validation_data=self.val_it,
+                                         epochs=self.epochs, verbose=1, workers=4,
+                                         callbacks=self.callbacks)
+            else:
+                history = self.model.fit(self.datagen.flow(self.X_train, self.y_train, batch_size=self.batch_size), validation_data=(self.X_test, self.y_test),
+                                         epochs=self.epochs, verbose=1, workers=4,
+                                         callbacks=self.callbacks)
 
-            self.model.save(os.getcwd()+f"/fully_trained/{self.model_type}_{self.dataset}_{self.date}")
+
+            self.model.save(os.getcwd()+f"/trained_models/{self.model_type}_{self.dataset}_{self.date}_completed")
 
             history_token = input("Save/Discard?  :   ")
 
             if history_token.lower()=="save":
-                keys,history_list=self.get_history_details(history)
-                self.save_history_details(history_list,keys)
-                print("saved")
+                with open(f'{self.model_type}_{self.dataset}_{self.date}_history', 'wb') as file_pi:
+                    pickle.dump(history.history, file_pi)
+                print("Saved.")
             elif history_token.lower()=="save":
-                print("discarded")
+                print("Discarded.")
             else:
                 print("Invalid Input!")
 
         elif self.token.lower() == 'load':
-            print("loading")
+            print("Loading...")
 
-            print(os.getcwd())
+            self.model = load_model(os.getcwd()+"/models_to_load/"+f"{self.model_type}_{self.dataset}")
 
-            self.model = load_model(os.getcwd()+"models_to_load/"+f'{self.model_type}_{self.dataset}_none')
+            PRINT("Loading Completed.")
 
         else:
-            print("invalid input")
+            print("Invalid Input!")
 
     def lr_schedule(self, epoch):
         lr = 1e-3
         if epoch > 180:
             lr *= 0.5e-3
         elif epoch > 160:
             lr *= 1e-3
         elif epoch > 120:
             lr *= 1e-2
         elif epoch > 80:
             lr *= 1e-1
-        print('Learning rate: ', lr)
+        print('Learning Rate: ', lr)
 
         return lr
 
     def classifier(self, inputs):
         x = tf.keras.layers.GlobalAveragePooling2D()(inputs)
         x = tf.keras.layers.Flatten()(x)
         x = tf.keras.layers.Dense(self.output_layer_classes, activation="softmax", name="classification")(x)
@@ -111,15 +120,15 @@
                                                             classifier_activation="softmax")(inputs)
         else:
             feature_extractor = tf.keras.applications.resnet.ResNet50(input_shape=self.input_shape,
                                                                       include_top=False,
                                                                       weights='imagenet',
                                                                       classes=self.output_layer_classes,
                                                                       classifier_activation="softmax")(inputs)
-            print("Invalid argument for model type")
+            print("Invalid argument for model type.")
 
         return feature_extractor
 
     def final_model(self, inputs):
 
         if self.dataset=="cifar10":
             resize = tf.keras.layers.UpSampling2D(size=(7,7))(inputs)
@@ -163,15 +172,15 @@
             input_images = input_images.astype('float32')
             output_ims = tf.keras.applications.resnet50.preprocess_input(input_images)
 
         return output_ims
 
     def get_callbacks(self):
 
-        save_dir = os.path.join(os.getcwd(), f'saved_models_{self.model_type}_{self.dataset}_{self.date}')
+        save_dir = os.getcwd()+f'/trained_models/{self.model_type}_{self.dataset}'
         model_name = self.model_type + '_model_' + str(self.date.day) + '_' + str(self.date.month) + '_' + str(
             self.date.year) + '.{epoch:03d}.h5'
 
         if not os.path.isdir(save_dir):
             os.makedirs(save_dir)
         filepath = os.path.join(save_dir, model_name)
         checkpoint = ModelCheckpoint(filepath=filepath,
@@ -188,14 +197,15 @@
                                        min_lr=0.5e-6)
 
         callbacks = [checkpoint, lr_reducer, lr_scheduler, early_stopping]
 
         return callbacks
 
     def get_datagen(self):
+
         datagen = ImageDataGenerator(
             featurewise_center=False,
             samplewise_center=False,
             featurewise_std_normalization=False,
             samplewise_std_normalization=False,
             zca_whitening=False,
             zca_epsilon=1e-06,
@@ -214,43 +224,82 @@
             data_format=None,
             validation_split=self.validation_split)
 
         return datagen
 
     def download_dataset(self):
 
-        print("extracting")
+        print("Extracting...")
         if not 'tiny-imagenet-200.zip' in os.listdir(os.getcwd()):
             url = 'http://cs231n.stanford.edu/tiny-imagenet-200.zip'
-            tiny_imgdataset = wget.download('http://cs231n.stanford.edu/tiny-imagenet-200.zip', out=os.getcwd())
+            tiny_imgdataset = wget.download(url, out=os.getcwd())
 
         for file in os.listdir(os.getcwd()):
             if file.endswith("tiny-imagenet-200.zip"):
                 zip_file = ZipFile(file)
                 zip_file.extractall()
-            else:
-                print("not found")
+
+        try:
+            os.system("gdown --id 1JgRlpet7-P-x7Exweb8HC-zUcYsF5fGN")
+        except:
+            os.system("!gdown --id 1JgRlpet7-P-x7Exweb8HC-zUcYsF5fGN")
+
+        print("Done.")
 
     def get_dataset(self):
 
         if self.dataset=="tinyimagenet":
-            train_it = self.datagen.flow_from_directory('/home/sb355/testing/tiny-imagenet-200/train',
+            train_it = self.datagen.flow_from_directory(os.getcwd()+'/tiny-imagenet-200/train',
                                                         batch_size=self.batch_size, subset="training", shuffle=self.shuffle_bool)
-            val_it = self.datagen.flow_from_directory('/home/sb355/testing/tiny-imagenet-200/train', batch_size=self.batch_size,
+            val_it = self.datagen.flow_from_directory(os.getcwd()+'/tiny-imagenet-200/train', batch_size=self.batch_size,
                                                       subset="validation", shuffle=self.shuffle_bool)
             train_filenames = train_it.filenames
             val_filenames = val_it.filenames
             number_of_val_samples = len(val_filenames)
             number_of_train_samples = len(train_filenames)
             # class_mode='categorical',
-            print(number_of_train_samples)
-            print(number_of_val_samples)
+            # print(number_of_train_samples)
+            # print(number_of_val_samples)
         else:
-            (train_it), (val_it) = tf.keras.datasets.cifar10.load_data()
-
+            if self.dataset == "cifar10":
+                classes = ['airplane', 'automobile', 'bird', 'cat', 'deer', 'dog', 'frog', 'horse', 'ship', 'truck']
+                num_classes = len(classes)
+                (training_images, training_labels), (
+                    validation_images, validation_labels) = tf.keras.datasets.cifar10.load_data()
+
+                train_X = self.preprocess_image_input(training_images)
+                valid_X = self.preprocess_image_input(validation_images)
+
+            elif self.dataset == "mnist":
+                num_classes = 10
+                (training_images, training_labels), (
+                    validation_images, validation_labels) = tf.keras.datasets.mnist.load_data()
+
+                train_X = self.preprocess_image_input(training_images)
+                valid_X = self.preprocess_image_input(validation_images)
+
+            elif self.dataset == "cifar100":
+                num_classes = 100
+                (training_images, training_labels), (
+                    validation_images, validation_labels) = tf.keras.datasets.cifar100.load_data()
+
+                train_X = self.preprocess_image_input(training_images)
+                valid_X = self.preprocess_image_input(validation_images)
+
+            training_labels = to_categorical(training_labels, num_classes)
+            validation_labels = to_categorical(validation_labels, num_classes)
+            self.datagen.fit(train_X)
+
+            train_it = self.datagen.flow(train_X, training_labels, batch_size=self.batch_size)
+            val_it = (valid_X, validation_labels)
+
+            self.X_train = train_X
+            self.X_test = valid_X
+            self.y_train = training_labels
+            self.y_test = validation_labels
 
         return train_it, val_it
 
     def save_history_details(self, history_data, keys):
 
         pd.DataFrame(history_data).to_csv(os.getcwd()+f"history_{self.model_type}_{self.dataset}_{self.date}.csv", header=keys)
 
@@ -268,55 +317,9 @@
                 a = history[i].history[key]
                 individual_keys_list_history.append(a)
 
             total_list_parameter_history.append(individual_keys_list_history)
 
         return keys, total_list_parameter_history
 
-    def context_decider_for_bert(self, val_it, prediction_list):
-        pred = self.model.predict_generator(val_it, 1)
-
-        predicted_list = []
-        classes_prob_list = []
-        prediction_index = []
-        final_classes = []
-
-        output = []
-
-        labels = self.val_it.class_indices
-        labels2 = dict((v, k) for k, v in labels.items())
-
-        for i in range(0, pred.shape[0]):
-            classes_prob_list = []
-            for j in range(0, self.output_layer_classes):
-                classes_prob_list.append([int(j), pred[i][j]])
-
-            classes_prob_list.sort(key=lambda x: x[1], reverse=True)
-
-            first_highest_predicted_classes = classes_prob_list[0][0]
-            first_highest_predicted_class_confidence = classes_prob_list[0][1]
-
-            second_highest_predicted_classes = classes_prob_list[1][0]
-            second_highest_predicted_class_confidence = classes_prob_list[1][1]
-
-            predicted_list.append([first_highest_predicted_classes, first_highest_predicted_class_confidence,
-                                   second_highest_predicted_classes, second_highest_predicted_class_confidence])
-
-        if (predicted_list[0][1] - predicted_list[0][3]) >= 0.2:
-            prediction_index.append(predicted_list[0][0])
-        elif (predicted_list[0][1] - predicted_list[0][3]) < 0.2:
-            prediction_index.append(predicted_list[0][0])
-            prediction_index.append(predicted_list[0][2])
-
-        for i in range(0, len(prediction_index)):
-            final_classes.append(i2d[labels2[prediction_index[i]]])
-
-        for ele in final_classes:
-            b = ele.split(',')
-            output = output + b
-
-        return output
-
-
     def evaluate(self):
         loss, accuracy = self.model.evaluate(self.val_it, batch_size=self.batch_size, verbose=1)
-
```

### Comparing `OneOnOne-0.6948/OneOnOne/contextdecider.py` & `OneOnOne-0.6949/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6948/OneOnOne/htmlparser.py` & `OneOnOne-0.6949/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6948/OneOnOne/questionanswer.py` & `OneOnOne-0.6949/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6948/OneOnOne/sampling.py` & `OneOnOne-0.6949/OneOnOne/sampling.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 class Sampling:
-    def __init__(self, samplingtype, dataset="cifar10", model_type="resnet50", goal=99, jump=5000,
+    def __init__(self, samplingtype, dataset="cifar10", model_type="resnet50", goal=99, jump=5000, validation_split=0.3,
                  first_data_samples=10000, batch_size=16, epochs=250, shuffle_bool=True, early_stopping_patience=10,
                  lr_reducer_patience=10):
+        warnings.filterwarnings("ignore")
 
-        self.validation_split = 0
+        self.validation_split = validation_split
         self.model_type = model_type.lower()
         self.epochs = epochs
         self.jump = jump
         self.samplingtype = samplingtype.lower()
         self.goal = goal
         self.shuffle_bool = shuffle
         self.batch_size = batch_size
@@ -16,30 +17,27 @@
         self.input_shape = (32, 32, 3)
         self.date = datetime.datetime.now()
         self.first_data_samples = first_data_samples
         self.early_stopping_patience = early_stopping_patience
         self.lr_reducer_patience = lr_reducer_patience
         self.callbacks = self.get_callbacks()
         self.datagen = self.get_datagen()
-        self.train_it, self.val_it = self.get_dataset()
-
         if self.dataset == "cifar10" or self.dataset == "mnist":
             self.output_layer_classes = 10
             self.input_shape = (224, 224, 3)
-
-
         elif self.dataset == "tinyimagenet":
             self.output_layer_classes = 200
             self.input_shape = (32, 32, 3)
-            from classes import i2d
             self.download_dataset()
-
+            from classes import i2d
         else:
             print("Invalid Input!")
 
+        self.train_it, self.val_it = self.get_dataset()
+
         if samplingtype == "random":
             random_num = np.random.randint(self.first_data_samples, self.X_train.shape[0],
                                            size=self.X_train.shape[0] - self.first_data_samples)
             self.random_num = random_num
 
     def lr_schedule(self, epoch):
         lr = 1e-3
@@ -168,19 +166,14 @@
 
         callbacks = [checkpoint, lr_reducer, lr_scheduler, early_stopping]
 
         return callbacks
 
     def get_datagen(self):
 
-        if self.dataset == "tinyimagenet":
-            self.validation_split = input("Validation split (example - 0.3):   ")
-        else:
-            pass
-
         datagen = ImageDataGenerator(
             featurewise_center=False,
             samplewise_center=False,
             featurewise_std_normalization=False,
             samplewise_std_normalization=False,
             zca_whitening=False,
             zca_epsilon=1e-06,
@@ -209,32 +202,37 @@
             tiny_imgdataset = wget.download(url, out=os.getcwd())
 
         for file in os.listdir(os.getcwd()):
             if file.endswith("tiny-imagenet-200.zip"):
                 zip_file = ZipFile(file)
                 zip_file.extractall()
 
+        try:
+            os.system("gdown --id 1JgRlpet7-P-x7Exweb8HC-zUcYsF5fGN")
+        except:
+            os.system("!gdown --id 1JgRlpet7-P-x7Exweb8HC-zUcYsF5fGN")
+
         print("Done.")
 
     def get_dataset(self):
 
         if self.dataset == "tinyimagenet":
-            train_it = self.datagen.flow_from_directory(os.getcwd() + 'tiny-imagenet-200/train',
+            train_it = self.datagen.flow_from_directory(os.getcwd() + '/tiny-imagenet-200/train',
                                                         batch_size=self.batch_size, subset="training",
                                                         shuffle=self.shuffle_bool)
-            val_it = self.datagen.flow_from_directory(os.getcwd() + 'tiny-imagenet-200/train',
+            val_it = self.datagen.flow_from_directory(os.getcwd() + '/tiny-imagenet-200/train',
                                                       batch_size=self.batch_size,
                                                       subset="validation", shuffle=self.shuffle_bool)
             train_filenames = train_it.filenames
             val_filenames = val_it.filenames
             number_of_val_samples = len(val_filenames)
             number_of_train_samples = len(train_filenames)
             # class_mode='categorical',
-            print(number_of_train_samples)
-            print(number_of_val_samples)
+            # print(number_of_train_samples)
+            # print(number_of_val_samples)
 
         else:
 
             shuffle_random_token = input("Do you want to shuffle the training data? (yes/no):  ")
 
             if shuffle_random_token.lower() == "yes":
                 seed_token = input("Enter random seed (int):  ")
@@ -293,37 +291,43 @@
         return train_it, val_it
 
     def get_iterations_rs(self):
 
         e = [0, 0]
 
         k = 0
+        self.accuracy_data = []
+        history_data = []
 
-        num = 0
-
-        y = []
-        x = []
+        self.y = []
+        self.x = []
         for i in range(0, self.first_data_samples):
-            y.append(self.y_train[i])
-            x.append(self.X_train[i])
+            self.y.append(self.y_train[i])
+            self.x.append(self.X_train[i])
 
         while (e[1] < self.goal / 100) & (k + self.jump < self.X_train.shape[0]):
 
             for i in range(0 + k, self.jump + k):
-                x.append(self.X_train[self.random_num[i]])
-                y.append(self.y_train[self.random_num[i]])
+                self.x.append(self.X_train[self.random_num[i]])
+                self.y.append(self.y_train[self.random_num[i]])
 
             k = k + self.jump
-            num = num + 1
 
-            self.model.fit(np.array(x), np.array(y), epochs=50)
+            h = self.model.fit(self.datagen.flow(np.array(self.x), np.array(self.y), batch_size=self.batch_size),
+                               validation_data=self.val_it,
+                               epochs=self.epochs, verbose=1, workers=4,
+                               callbacks=self.callbacks)
+
+            history_data.append(h)
 
-            e = self.model.evaluate(self.X_test, self.y_test)
+            eval_metrics = self.model.evaluate(self.X_test, self.y_test)
+            print(eval_metrics)
+            self.accuracy_data.append(eval_metrics)
 
-        return e[1], num
+        return history_data
 
     def get_entropy(self, y_predicted_en):
         sum_prob = 0
         entropy = []
 
         for i in range(0, y_predicted_en.shape[0]):
             for j in range(0, y_predicted_en.shape[1]):
@@ -411,111 +415,177 @@
             print("Saved.")
 
         else:
 
             self.model = self.define_compile_model()
             self.model.summary()
 
-            history = self.model.fit(self.datagen.flow(self.X_train, self.y_train, batch_size=self.batch_size),
-                                     validation_data=(self.X_test, self.y_test),
-                                     epochs=self.epochs, verbose=1, workers=4,
-                                     callbacks=self.callbacks)
+            history = self.model.fit(
+                self.datagen.flow(self.X_train[:self.first_data_samples], self.y_train[:self.first_data_samples],
+                                  batch_size=self.batch_size), validation_data=(self.X_test, self.y_test),
+                epochs=self.epochs, verbose=1, workers=4,
+                callbacks=self.callbacks)
             self.model.save(
                 os.getcwd() + f"/trained_models/{self.model_type}_{self.dataset}_{self.samplingtype}_{self.first_data_samples}_{self.date}_initial_training")
 
             with open(f'{self.model_type}_{self.dataset}_{self.date}_history', 'wb') as file_pi:
                 pickle.dump(history.history, file_pi)
             print("saved.")
 
+    def bayesian(self, lc_coeff):
+
+        x_temp = copy.deepcopy(self.x)
+        y_temp = copy.deepcopy(self.y)
+
+        lr_scheduler = LearningRateScheduler(self.lr_schedule)
+        lr_reducer = ReduceLROnPlateau(factor=np.sqrt(0.1),
+                                       cooldown=0,
+                                       patience=self.lr_reducer_patience,
+                                       min_lr=0.5e-6)
+
+        params = {'lc_coeff': lc_coeff}
+        hc_coeff = 1 - lc_coeff
+
+        temp_model = load_model(os.getcwd() + "/mixedbayesmodel.h5")
+
+        y_predicted = temp_model.predict(self.X_train_copy)
+
+        values_lc = self.get_lc(y_predicted)
+        values_hc = self.get_hc(y_predicted)
+
+        print(f"lc: {lc_coeff}, hc: {hc_coeff}")
+
+        lc_jump = int(self.jump * lc_coeff)
+        hc_jump = self.jump - lc_jump
+
+        for i in range(0, lc_jump):
+            x_temp.append(self.X_train_copy[values_lc[i][0]])
+            y_temp.append(self.y_train_copy[values_lc[i][0]])
+
+        for i in range(0, hc_jump):
+            x_temp.append(self.X_train_copy[values_hc[i][0]])
+            y_temp.append(self.y_train_copy[values_hc[i][0]])
+
+        h = temp_model.fit(datagen.flow(np.array(x_temp), np.array(y_temp), batch_size=self.batch_size),
+                           validation_data=(self.X_test, self.y_test), epochs=50, callbacks=[lr_scheduler, lr_reducer],
+                           verbose=1,
+                           workers=4)
+
+        score = temp_model.evaluate(self.X_test, self.y_test)
+
+        return 100 * float(score[1])
+
+    def get_bayes_coeff(self):
+
+        params = {'lc_coeff': (0, 1)}
+        bo = BayesianOptimization(self.bayesian, params, random_state=22)
+        bo.maximize(init_points=20, n_iter=10)
+
+        params = bo.max['params']
+        lc_coeff = params["lc_coeff"]
+
+        return lc_coeff
+
     def get_iterations(self):
 
         eval_metrics = [0, 0]
 
         num = 0
-        batch_size_data = [0]
-        acuracy_data = [0]
-        epoch_data = []
+        self.accuracy_data = []
         history_data = []
 
-        y = []
-        x = []
+        self.y = []
+        self.x = []
 
         if self.samplingtype == "random":
-            eval_metrics[1], num = self.get_iterations_rs()
-
-            return eval_metrics[1], num
+            return self.get_iterations_rs()
 
-        X_train_copy = self.X_train[self.first_data_samples:self.X_train.shape[0]]
-        y_train_copy = self.y_train[self.first_data_samples:self.X_train.shape[0]]
+        self.X_train_copy = copy.deepcopy(self.X_train[self.first_data_samples:self.X_train.shape[0]])
+        self.y_train_copy = copy.deepcopy(self.y_train[self.first_data_samples:self.X_train.shape[0]])
 
         for i in range(0, self.first_data_samples):
-            y.append(self.y_train[i])
-            x.append(self.X_train[i])
+            self.y.append(self.y_train[i])
+            self.x.append(self.X_train[i])
 
-        while (eval_metrics[1] < self.goal / 100) & (self.jump <= X_train_copy.shape[0]):
+        while (eval_metrics[1] < self.goal / 100) & (self.jump <= self.X_train_copy.shape[0]):
 
-            total_index = [*range(0, X_train_copy.shape[0], 1)]
-            y_predicted = self.model.predict(X_train_copy)
+            total_index = [*range(0, self.X_train_copy.shape[0], 1)]
+            y_predicted = self.model.predict(self.X_train_copy)
 
             if self.samplingtype == "margin":
                 values = self.get_margin(y_predicted)
             elif self.samplingtype == "leastconfidence":
                 values = self.get_lc(y_predicted)
             elif self.samplingtype == "highestconfidence":
                 values = self.get_hc(y_predicted)
             elif self.samplingtype == "entropy":
                 values = self.get_entropy(y_predicted)
             elif self.samplingtype == "ratio":
                 values = self.get_ratio(y_predicted)
-            elif self.samplingtype == "mixed":
+            elif self.samplingtype == "mixed" or self.samplingtype == "mixedbayes":
                 values_lc = self.get_lc(y_predicted)
                 values_hc = self.get_hc(y_predicted)
             else:
                 print("Invalid Input!")
 
             index = []
 
             if self.samplingtype == "mixed":
                 for i in range(0, self.jump // 2):
                     index.append(values_lc[i][0])
-                    x.append(X_train_copy[values_lc[i][0]])
-                    y.append(y_train_copy[values_lc[i][0]])
+                    self.x.append(self.X_train_copy[values_lc[i][0]])
+                    self.y.append(self.y_train_copy[values_lc[i][0]])
 
                 for i in range(0, self.jump // 2):
                     index.append(values_hc[i][0])
-                    x.append(X_train_copy[values_hc[i][0]])
-                    y.append(y_train_copy[values_hc[i][0]])
+                    self.x.append(self.X_train_copy[values_hc[i][0]])
+                    self.y.append(self.y_train_copy[values_hc[i][0]])
 
+            elif self.samplingtype == "mixedbayes":
+                self.model.save(os.getcwd() + "/mixedbayesmodel.h5")
+
+                lc_coeff = self.get_bayes_coeff()
+
+                lc_jump = int((self.jump) * lc_coeff)
+                hc_jump = self.jump - lc_jump
+
+                for i in range(0, lc_jump):
+                    index.append(values_lc[i][0])
+                    self.x.append(self.X_train_copy[values_lc[i][0]])
+                    self.y.append(self.y_train_copy[values_lc[i][0]])
+
+                for i in range(0, hc_jump):
+                    index.append(values_hc[i][0])
+                    self.x.append(self.X_train_copy[values_hc[i][0]])
+                    self.y.append(self.y_train_copy[values_hc[i][0]])
 
             else:
                 for i in range(0, self.jump):
                     index.append(values[i][0])
-                    x.append(X_train_copy[values[i][0]])
-                    y.append(y_train_copy[values[i][0]])
+                    self.x.append(self.X_train_copy[values[i][0]])
+                    self.y.append(self.y_train_copy[values[i][0]])
 
             num += 1
 
-            h = self.model.fit(self.datagen.flow(np.array(x), np.array(y), batch_size=self.batch_size),
+            h = self.model.fit(self.datagen.flow(np.array(self.x), np.array(self.y), batch_size=self.batch_size),
                                validation_data=self.val_it,
                                epochs=self.epochs, verbose=1, workers=4,
                                callbacks=self.callbacks)
 
-            batch_size_data.append(np.array(x).shape[0])
-            epoch_data.append(num)
             history_data.append(h)
 
             eval_metrics = self.model.evaluate(self.X_test, self.y_test)
             print(eval_metrics)
-            acuracy_data.append(100 * float(eval_metrics[1]))
+            self.accuracy_data.append(eval_metrics)
 
             a = []
             for element in total_index:
                 if element not in index:
                     a.append(element)
 
-            X_train_copy = X_train_copy[a]
-            y_train_copy = y_train_copy[a]
+            self.X_train_copy = self.X_train_copy[a]
+            self.y_train_copy = self.y_train_copy[a]
 
         self.model.save(
             os.getcwd() + f"/trained_models/{self.model_type}_{self.dataset}_{self.samplingtype}_{self.date}_completed")
 
-        return history_data, epoch_data, batch_size_data, acuracy_data
+        return history_data
```

### Comparing `OneOnOne-0.6948/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6949/OneOnOne.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6948
+Version: 0.6949
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
-Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
+Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,speech-recognition,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!
```

### Comparing `OneOnOne-0.6948/PKG-INFO` & `OneOnOne-0.6949/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6948
+Version: 0.6949
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
-Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
+Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,speech-recognition,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!
```

### Comparing `OneOnOne-0.6948/README.md` & `OneOnOne-0.6949/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 <h1 align="center">OneOnOne 🎈</h1>
 <p>
   <a href="https://pypi.org/project/OneOnOne/0.6896/" target="_blank">
   </a>
 </p>
 
-<h3 align="center"><span style="color:#FFC0CB">Your one-stop destination to utilize image-classification models with just one line of code.</span></h3>
+<h3 align="center"><span style="color:#FFC0CB">Your one-stop destination to utilize an interface like GoogleLens with just one line of code.</span></h3>
 
 <h4 align="center">
 A python library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc.
-You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, don't worry! This library has got you covered. Along with that for simple-bridging of NLP with Image Classification and utilization of basic use-cases of NLP frameworks, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about, and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset.
+You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, don't worry! This library has got you covered. Along with that for simple-bridging of NLP with Image Classification and utilization of basic use-cases of NLP frameworks, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about, and you can ask one-on-one questions from the chatbot. You can use speech-to-text or translate image text into your desired language. This is made possible by using the tiny imagenet dataset.
 </h4>
 
 <h4 align="center">____________________________________________________________________________</h4>
 
 <dl>
   <dt><span style="color:#FFC0CB">How to import the library?</span></dt>
     <dd>Just run the following command on your terminal or online coding interface.
@@ -45,14 +45,16 @@
 from OneOnOne import Sampling
 
 sampling=Sampling("mixedbayes","cifar10",first_data_samples=5000)
 sampling.initial_training()
 history_data=sampling.get_iterations()
 ```
 
+This will use the bayes optimization method to find the optimal coefficient for highest confidence and least confidence samples.
+
 <dl>
   <dt><span style="color:#FFC0CB">or, download pretrained models with your desired specifications!</span>
 </dl>
 
 ```python
 from OneOnOne import PretrainedModel
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
                           ****** OneOnOne ð ******
-**** Your one-stop destination to utilize image-classification models with just
-                            one line of code. ****
+  **** Your one-stop destination to utilize an interface like GoogleLens with
+                          just one line of code. ****
   *** A python library meant to simplify your life by providing you with pre-
  trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt
 for training your own models from scratch by just tweaking a few values. If you
  want to try popular active-learning sampling methods on image classification,
   don't worry! This library has got you covered. Along with that for simple-
 bridging of NLP with Image Classification and utilization of basic use-cases of
    NLP frameworks, we have context-deciders, HTML parsers and simple chatbot
   object classes, to create an interface similar to Google Lens. You input an
 image or item that you are curious about, and you can ask one-on-one questions
-from the chatbot. This is made possible by using the tiny imagenet dataset. ***
+from the chatbot. You can use speech-to-text or translate image text into your
+desired language. This is made possible by using the tiny imagenet dataset. ***
                                       ***
  ____________________________________________________________________________
                                       ***
   How to import the library?
       Just run the following command on your terminal or online coding
       interface.
 ``` pip install OneOnOne ```
@@ -22,15 +23,17 @@
       This will use the default values for the class object, as mentioned in
       the original code.
 ```python from OneOnOne import Classification classifier=Classification
 (validation_split=0.4,early_stopping_patience=20) ```
   or,
 ```python from OneOnOne import Sampling sampling=Sampling
 ("mixedbayes","cifar10",first_data_samples=5000) sampling.initial_training()
-history_data=sampling.get_iterations() ```
+history_data=sampling.get_iterations() ``` This will use the bayes optimization
+method to find the optimal coefficient for highest confidence and least
+confidence samples.
   or, download pretrained models with your desired specifications!
 ```python from OneOnOne import PretrainedModel pretrained=PretrainedModel
 (model_type="resnet50", dataset="cifar10", samplingtype="leastconfidence")
 model=pretrained.get_model() ```
                                       ***
  ____________________________________________________________________________
                                       ***
```

### Comparing `OneOnOne-0.6948/setup.py` & `OneOnOne-0.6949/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6948
+VERSION=0.6949
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
-setup(name="OneOnOne",version=VERSION,description=DESCRIPTION, long_description=LONG_DESCRIPTION,author="Sohini Bhattacharya",author_email="mail.sohinibhattacharya@gmail.com",License="MIT",packages=find_packages(),keywords=["python","image-classification","active-learning-sampling","question-answering","pre-trained models","tiny-image-net","cifar10"],classifiers=CLASSIFIERS,install_requires=["wget","bayesian-optimization","copy","torch","transformers","gdown","numpy","pandas","tensorflow==2.12.0","datetime","keras==2.12.0","tensorflow_datasets==4.9.2","scipy==1.10.1","tqdm==4.65.0"])
+setup(name="OneOnOne",version=VERSION,description=DESCRIPTION, long_description=LONG_DESCRIPTION,author="Sohini Bhattacharya",author_email="mail.sohinibhattacharya@gmail.com",License="MIT",packages=find_packages(),keywords=["python","image-classification","active-learning-sampling","question-answering","pre-trained models","tiny-image-net","speech-recognition","cifar10"],classifiers=CLASSIFIERS,install_requires=["wget","pytesseract","bayesian-optimization","speechrecognition","pyttsx3","pydub","pyaudio","copy","torch","transformers","gdown","numpy","pandas","tensorflow==2.12.0","datetime","keras==2.12.0","tensorflow_datasets==4.9.2","scipy==1.10.1","tqdm==4.65.0"])
```

