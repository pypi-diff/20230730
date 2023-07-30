# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.7.2.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.3.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.7.2.tar", last modified: Fri Jul 28 08:34:13 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.3.9.8.tar", last modified: Sun Jul 30 08:55:22 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2.tar` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/LICENSE
--rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    27633 2023-07-27 04:38:23.778936 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6188 2023-07-28 08:33:16.986476 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     4259 2023-07-23 09:16:00.588115 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    16209 2023-07-24 18:35:40.523775 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     6967 2023-07-24 18:35:51.029539 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    19049 2023-07-24 18:32:19.159565 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0    10785 2023-07-25 03:34:42.018245 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     2699 2023-07-24 18:34:46.822788 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11332 2023-07-24 18:23:17.528164 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     4139 2023-07-22 04:35:59.105979 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    44380 2023-07-27 04:38:58.160130 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     6353 2023-07-24 18:32:11.211285 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     4677 2023-07-22 03:29:42.199501 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     6148 2023-07-24 18:32:12.882405 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      726 2023-07-20 08:05:34.470705 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      730 2023-07-28 08:34:13.810804 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/pyproject.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.3.9.8/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-31 13:01:37.260789 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    27817 2023-07-30 08:48:48.842194 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6188 2023-07-28 08:33:16.986476 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     4259 2023-07-23 09:16:00.588115 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    16671 2023-07-30 07:13:41.115825 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     7294 2023-07-30 08:49:00.116288 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    19686 2023-07-30 08:52:20.735415 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0    10785 2023-07-25 03:34:42.018245 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     2054 2023-07-10 12:39:09.576540 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     2699 2023-07-24 18:34:46.822788 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11332 2023-07-24 18:23:17.528164 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     4139 2023-07-22 04:35:59.105979 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    46162 2023-07-30 08:50:24.757084 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     6353 2023-07-24 18:32:11.211285 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     4677 2023-07-22 03:29:42.199501 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2111 2023-07-03 03:51:06.635888 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     6148 2023-07-24 18:32:12.882405 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      726 2023-07-20 08:05:34.470705 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      733 2023-07-05 13:24:21.506297 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1985 2023-07-10 14:03:49.047428 nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      728 2023-07-30 08:55:22.656544 nonebot_plugin_stable_diffusion_diao-0.3.9.8/pyproject.toml
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.3.9.8/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from .utils.save import save_img
 from .utils.prepocess import prepocess_tags
 from .version import version
 from .utils import sendtosuperuser, tags_to_list
 from .extension.safe_method import send_forward_msg
 from .extension.sd_extra_api_func import change_model, get_random_tags
 cd = {}
+user_models_dict = {}
 gennerating = False
 wait_list = deque([])
 
 aidraw_parser = ArgumentParser()
 aidraw_parser.add_argument("tags", nargs="*", help="标签", type=str)
 aidraw_parser.add_argument("-r", "--resolution", "-形状",
                            help="画布形状/分辨率", dest="man_shape")
@@ -73,14 +74,16 @@
                            type=float, help="高清修复倍率", dest="hiresfix_scale")
 aidraw_parser.add_argument("-m",
                            type=str, help="更换模型", dest="model_index")
 aidraw_parser.add_argument("-match_off","-match-off",
                            action="store_true", help="关闭自动匹配", dest="match")
 aidraw_parser.add_argument("-sr_on", "-sr-on", "-sr",
                            action="store_true", help="图片生产后再次超分", dest="sr")
+aidraw_parser.add_argument("-td", "--tiled-diffusion",
+                           action="store_true", help="使用tiled-diffusion来生成图片", dest="td")
 
 
 async def get_message_at(data: str) -> int:
     '''
     获取at列表
     :param data: event.json()
     '''
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         model: str = None,
         sampler: None or str = None,
         backend_index: str = None,
         disable_hr: bool = False if config.novelai_hr else True,
         hiresfix_scale: float = None,
         event: MessageEvent = None,
         sr: bool = False,
-        model_index: int = None,
+        model_index: str = None,
+        td: bool = False,
         **kwargs,
     ):
         """
         AI绘画的核心部分,将与服务器通信的过程包装起来,并方便扩展服务器类型
 
         :user_id: 用户id,必须
         :group_id: 群聊id,如果是私聊则应置为0,必须
@@ -110,15 +111,15 @@
             self.sampler: str = (sampler if sampler else 
                                 self.weighted_choice(config.novelai_random_sampler_list) or 
                                 "Euler a")
         else:
             self.sampler: str = sampler if sampler else config.novelai_sampler or "Euler a"
         self.start_time: float = None
         self.spend_time: float = None
-        self.backend_site: str = None
+        self.backend_site: str = config.backend_site_list[backend_index] if backend_index else None
         self.backend_name: str = ''
         self.backend_index: int = backend_index
         self.vram: str = ""
         self.hiresfix_scale: float = hiresfix_scale or config.novelai_hr_scale
         self.novelai_hr_payload = config.novelai_hr_payload
         self.novelai_hr_payload["hr_scale"] = self.hiresfix_scale
         self.hiresfix: bool = True if config.novelai_hr else False
@@ -131,14 +132,16 @@
         self.task_type: str = None
         self.img_hash = None
         self.extra_info = ""
         self.audit_info = ""
         self.sr = sr or config.novelai_SuperRes_generate
         self.model_index = model_index
         self.is_random_model = False
+        self.model_dict = None
+        self.td = td
         
         # 数值合法检查
         if self.steps <= 0 or self.steps > (36 if config.novelai_paid else 28):
             self.steps = 28
         if self.strength < 0 or self.strength > 1:
             self.strength = 0.7
         if self.noise < 0 or self.noise > 1:
@@ -397,9 +400,16 @@
                     if resp.status not in [200, 201]:
                         return ""
                     else:
                         webui_config = await resp.json(encoding="utf-8")
                         return webui_config
         except:
             return ""
+        
+    async def get_model_index(self, model_name):
+        reverse_dict = {value: key for key, value in self.models_dict.items()}
+        for model in list(self.models_dict.values()):
+            if model_name in model:
+                model_index = reverse_dict[model]
+                return model_index
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from .base import AIDRAW_BASE
 from ..config import config
 import time
 from ..utils.load_balance import sd_LoadBalance, get_vram
 from ..utils import get_generate_info
 from nonebot import logger
+from copy import deepcopy
 import json, aiofiles
 import asyncio
 import traceback
 import random
 
+
 header = {
                 "content-type": "application/json",
                 "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.36",
 }
 
 
 class AIDRAW(AIDRAW_BASE):
@@ -66,22 +68,19 @@
             "width": self.width,
             "height": self.height,
             "negative_prompt": self.ntags,
             "sampler_name": self.sampler,
         }
         
         if self.model_index:
-            from ..extension.sd_extra_api_func import sd
-            await sd(self.backend_index or config.backend_site_list.index(self.backend_site))
-            async with aiofiles.open("data/novelai/models.json", "r", encoding="utf-8") as f:
-                content = await f.read()
-                model_dict = json.loads(content)
             if self.is_random_model:
-                self.model_index = random.randint(1, len(list(model_dict.keys())))
-            self.model = model_dict[str(self.model_index)]
+                from ..extension.sd_extra_api_func import sd
+                self.model_dict = await sd(self.backend_index or config.backend_site_list.index(self.backend_site), True)
+                self.model_index = random.randint(1, len(list(self.model_dict.keys())))
+            self.model = self.model_dict[int(self.model_index)]
             parameters.update({"override_settings": {"sd_model_checkpoint": self.model}, 
                                "override_settings_restore_afterwards": "true"}
                             )
 
         if self.img2img:
             if self.control_net["control_net"] and config.novelai_hr:
                 parameters.update(self.novelai_hr_payload)
@@ -91,32 +90,39 @@
             }
             )
         else:
             if config.novelai_hr and self.disable_hr is False:
                 parameters.update(self.novelai_hr_payload)
             else:
                 self.hiresfix = False
+        if self.td or config.tiled_diffusion:
+            parameters.update({"alwayson_scripts": config.custom_scripts})
         if self.control_net["control_net"] == True and config.novelai_hr:
             if config.hr_off_when_cn:
                 parameters.update({"enable_hr": "false"})
             else:
                 org_scale = parameters["hr_scale"]
                 parameters.update({"hr_scale": org_scale * 0.75}) # control较吃显存, 高清修复倍率恢复为1.5
             del parameters["init_images"]
             if config.novelai_ControlNet_post_method == 0:
                 post_api = f"http://{site}/sdapi/v1/txt2img"
                 parameters.update(config.novelai_ControlNet_payload[0])
                 parameters["alwayson_scripts"]["controlnet"]["args"][0]["input_image"] = self.image
             else:
                 post_api = f"http://{site}/controlnet/txt2img"
                 parameters.update(config.novelai_ControlNet_payload[1])
-                parameters["controlnet_units"][0]["input_image"] = self.image           
+                parameters["controlnet_units"][0]["input_image"] = self.image
+        logger.debug(str(parameters))         
         return header, post_api, parameters
 
     async def post(self):
+        if self.model_index:
+            self.model_index = self.model_index if self.model_index.isdigit() else await self.get_model_index(self.model_index)
+            from ..extension.sd_extra_api_func import sd
+            self.model_dict = await sd(self.backend_index, True)
         global defult_site
         defult_site = None # 所有后端失效后, 尝试使用默认后端
         # 失效自动重试 
         for retry_times in range(config.novelai_retry):
             try:
                 self.start_time = time.time()
                 parameters_tuple = await self.post_parameters()
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,36 +64,44 @@
     novelai_load_balance_weight: list = []  # 设置列表, 列表长度为你的后端数量, 数值为随机权重, 例[0.2, 0.5, 0.3]
     novelai_backend_url_dict: dict = {"雕雕的后端": "la.iamdiao.lol:5938", "雕雕的后端2": "la.iamdiao.lol:1521"} # 你能用到的后端, 键为名称, 值为url, 例:backend_url_dict = {"NVIDIA P102-100": "192.168.5.197:7860","NVIDIA CMP 40HX": "127.0.0.1:7860"
     novelai_sampler: str = None  # 默认采样器,不写的话默认Euler a, Euler a系画人物可能比较好点, DDIM系, 如UniPC画出来的背景比较丰富, DPM系采样器一般速度较慢, 请你自己尝试(以上为个人感觉
     novelai_hr: bool = True  # 是否启动高清修复
     novelai_hr_scale: float = 1.5  # 高清修复放大比例
     novelai_hr_payload: dict = {
         "enable_hr": "true", 
-        "denoising_strength": 0.55,  # 重绘幅度
+        "denoising_strength": 0.4,  # 重绘幅度
         "hr_scale": novelai_hr_scale,  # 高清修复比例, 1.5为长宽分辨率各X1.5
-        "hr_upscaler": "Lanczos",  # 超分模型, 使用前请先确认此模型是否可用, 推荐使用R-ESRGAN 4x+ Anime6B
+        "hr_upscaler": "R-ESRGAN 4x+ Anime6B",  # 超分模型, 使用前请先确认此模型是否可用, 推荐使用R-ESRGAN 4x+ Anime6B
         "hr_second_pass_steps": 7,  # 高清修复步数, 个人建议7是个不错的选择, 速度质量都不错
     } # 以上为个人推荐值
     novelai_SuperRes_MaxPixels: int = 2000  # 超分最大像素值, 对应(值)^2, 为了避免有人用超高分辨率的图来超分导致爆显存(
     novelai_SuperRes_generate: bool = False  # 图片生成后是否再次进行一次超分
     novelai_SuperRes_generate_payload: dict = {
         "upscaling_resize": 1.2,  # 超分倍率, 为长宽分辨率各X1.2
         "upscaler_1": "Lanczos",  # 第一次超分使用的方法
         "upscaler_2": "R-ESRGAN 4x+ Anime6B",  # 第二次超分使用的方法
         "extras_upscaler_2_visibility": 0.6  # 第二层upscaler力度
     } # 以上为个人推荐值
     novelai_ControlNet_post_method: int = 0
+    '''post方法有 0: /sdapi/v1/txt2img 和 1: /controlnet/txt2img 
+    个人使用第一种方法post显卡占用率反复横跳TAT 
+    tips:使用/controlnet/txt2img会提示warning: consider using the '/sdapi/v1/txt2img' route with the 'alwayson_scripts' json property instead''' 
     novelai_size_org: int = 640  # 最大分辨率
     if novelai_hr:
         novelai_size: int = novelai_size_org
     else:
         novelai_size: int = novelai_size_org * novelai_hr_payload["hr_scale"]
-    '''post方法有 0: /sdapi/v1/txt2img 和 1: /controlnet/txt2img 
-    个人使用第一种方法post显卡占用率反复横跳TAT 
-    tips:使用/controlnet/txt2img会提示warning: consider using the '/sdapi/v1/txt2img' route with the 'alwayson_scripts' json property instead''' 
+    custom_scripts = {  # 自定义脚本此功能就可以使用webui上才能调用的插件, 需要自己去抓包
+    "Tiled Diffusion": {
+        "args": [True, "MultiDiffusion", False, True, 1024, 1024, 96, 96, 48, 1, "None", 2, False, 10, 1, []]
+    },
+    "Tiled VAE": {
+        "args": [True, 1536, 96, False, True, True]
+    }
+    }
     novelai_ControlNet_payload: list = [
         {
             "alwayson_scripts": {
             "controlnet": {
             "args": [
                 {
                 "input_image": "",
@@ -144,14 +152,16 @@
     run_screenshot = False  # 获取服务器的屏幕截图
     is_redis_enable = True  # 是否启动redis, 启动redis以获得更多功能
     auto_match = True  # 是否自动匹配
     hr_off_when_cn = True  # 使用controlnet功能的时候关闭高清修复
     backend_name_list = []
     backend_site_list = []
     only_super_user = True  # 只有超级用户才能永久更换模型, 雕雕没有小号来测试了, 悲
+    tiled_diffusion = False  # 使用tiled-diffusion来生成图片
+    enable_scripts = False  # 是否启动custom_scripts中设置的自定义脚本
     # 允许单群设置的设置
     def keys(cls):
         return ("novelai_cd", "novelai_tags", "novelai_on", "novelai_ntags", "novelai_revoke", "novelai_h", "novelai_htype", "novelai_picaudit", "novelai_pure", "novelai_site")
 
     def __getitem__(cls, item):
         return getattr(cls, item)
 
@@ -267,19 +277,19 @@
                 if resp.status in [200, 201]:
                     resp_json: list = await resp.json()
                     return resp_json
                 else:
                     return None
     except Exception:
         return None
-
+    
 
 async def this_is_a_func(end_point_index):
     task_list = []
-    end_point_list = ["/sdapi/v1/prompt-styles", "/sdapi/v1/embeddings", "/sdapi/v1/loras"]
+    end_point_list = ["/sdapi/v1/prompt-styles", "/sdapi/v1/embeddings", "/sdapi/v1/loras", "/sdapi/v1/interrupt"]
     for site in config.backend_site_list:
         task_list.append(get_(site, end_point_list[end_point_index]))
     all_resp = await asyncio.gather(*task_list, return_exceptions=False)
     return all_resp
 
 config = Config(**get_driver().config.dict())
 config.backend_name_list = list(config.novelai_backend_url_dict.keys())
@@ -366,22 +376,24 @@
                 else:
                     backend_lora[config.backend_name_list[normal_backend_index]] = None
                     
             logger.info("存入数据库...")
             if r2.exists("emb"):
                 r2.delete(*["style", "emb", "lora"])
             pipe = r2.pipeline()
-            pipe.rpush("style", *all_style_list)
+            if len(all_style_list) != 0:
+                pipe.rpush("style", *all_style_list)
             pipe.set("emb", str(backend_emb))
             pipe.set("lora", str(backend_lora))
             pipe.execute()
             
             return redis_client
         
         redis_client = asyncio.run(main())
     except Exception:
         redis_client = None
+        logger.warning(traceback.print_exc())
         logger.warning("redis初始化失败, 已经禁用redis")
 
 logger.info(f"加载config完成" + str(config))
 logger.info(f"后端数据加载完成, 共有{len(config.backend_name_list)}个后端被加载")
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,16 @@
 audit = on_command("审核")
 genera_aging = on_command("再来一张")
 reload_ = on_command("卸载模型", aliases={"释放显存"})
 style_ = on_command("预设")
 rembg = on_command("去背景", aliases={"rembg", "抠图"})
 read_png_info = on_command("读图", aliases={"读png", "读PNG"})
 random_pic = on_command("随机出图", aliases={"随机模型", "随机画图"})
+refresh_models = on_command("刷新模型")
+stop_all_mission = on_command("终止生成")
 
 more_func_parser, style_parser = ArgumentParser(), ArgumentParser()
 more_func_parser.add_argument("-i", "--index", type=int, help="设置索引", dest="index")
 more_func_parser.add_argument("-v", "--value", type=str, help="设置值", dest="value")
 more_func_parser.add_argument("-s", "--search", type=str, help="搜索设置名", dest="search")
 style_parser.add_argument("tags", type=str, nargs="*", help="正面提示词")
 style_parser.add_argument("-f", "--find", type=str, help="寻找预设", dest="find_style_name")
@@ -245,32 +247,36 @@
             else:
                 resp_json = await resp.json()
                 resp_img = resp_json["image"]
                 bytes_img = base64.b64decode(resp_img)
                 return bytes_img, msg, resp.status
 
 
-async def sd(backend_site_index):
+async def sd(backend_site_index, return_models=False):
     site = list(config.novelai_backend_url_dict.values())[int(backend_site_index)]
     dict_model = {}
+    all_models_list = []
     message = []
     message1 = []
     n = 1
     resp_ = await aiohttp_func("get", "http://"+site+"/sdapi/v1/options")
     currents_model = resp_[0]["sd_model_checkpoint"]
     message1.append("当前使用模型:" + currents_model + ",\t\n\n")
     models_info_dict = await aiohttp_func("get", "http://"+site+"/sdapi/v1/sd-models")
     for x in models_info_dict[0]:
         models_info_dict = x['title']
+        all_models_list.append(models_info_dict)
         dict_model[n] = models_info_dict
         num = str(n) + ". "
         message.append(num + models_info_dict + ",\t\n")
         n = n + 1
     message.append("总计%d个模型" % int(n - 1))
     message_all = message1 + message
+    if return_models:
+        return dict_model
     with open("data/novelai/models.json", "w", encoding='utf-8') as f:
         f.write(json.dumps(dict_model, indent=4))
     return message_all
 
 
 async def set_config(data, backend_site):
     payload = {"sd_model_checkpoint": data}
@@ -357,25 +363,28 @@
             await bot.send(event=event, message="更换模型%s成功" % str(data) + spend_time_msg , at_sender=True) 
         else:
             await bot.send(event=event, message="更换模型失败，错误代码%s" % str(code), at_sender=True)
     except KeyError:
         await get_models.finish("输入错误,索引错误")
 
 
-async def aiohttp_func(way, url, payload=""):
-    if way == "post":
-        async with aiohttp.ClientSession() as session:
-            async with session.post(url=url, json=payload) as resp:
-                resp_data = await resp.json()
-                return resp_data, resp.status
-    else:
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url=url) as resp:
-                resp_data = await resp.json()
-                return resp_data, resp.status
+async def aiohttp_func(way, url, payload={}):
+    try:
+        if way == "post":
+            async with aiohttp.ClientSession() as session:
+                async with session.post(url=url, json=payload) as resp:
+                    resp_data = await resp.json()
+                    return resp_data, resp.status
+        else:
+            async with aiohttp.ClientSession() as session:
+                async with session.get(url=url) as resp:
+                    resp_data = await resp.json()
+                    return resp_data, resp.status
+    except Exception:
+        return None
 
 
 @set_sd_config.handle()
 async def _(event: MessageEvent, bot: Bot, args: Namespace = ShellCommandArgs()):
     await func_init(event)
     msg_list = ["Stable-Diffusion-WebUI设置\ntips: 可以使用 -s 来搜索设置项, 例如 设置 -s model\n"]
     n = 0
@@ -1055,15 +1064,15 @@
     _, __, normal_backend = await sd_LoadBalance()
     random_site = random.choice(normal_backend)
     index = config.backend_site_list.index(random_site)
     init_dict["backend_index"] = index
     fifo = AIDRAW(**init_dict)
     fifo.backend_site = random_site
     fifo.is_random_model = True
-    fifo.model_index = 20204 
+    fifo.model_index = "20204" 
     fifo.ntags = lowQuality
     fifo.disable_hr = True
     fifo.width, fifo.height = fifo.width * 1.25, fifo.height * 1.25
     await bot.send(event=event, message=f"{nickname}祈祷中...让我们看看随机了什么好模型\nprompts: {fifo.tags}")
     
     try:
         await fifo.post()
@@ -1081,8 +1090,42 @@
                 await bot.send(event=event, 
                             message=to_user, 
                             at_sender=True, reply_message=True)
             except ActionFailed:
                 await bot.send(event=event, 
                             message=img_msg+f"\n{fifo.img_hash}", 
                             at_sender=True, reply_message=True)
-    await save_img(fifo=fifo, img_bytes=fifo.result[0], extra=fifo.group_id+"_random_model")
+    await save_img(fifo=fifo, img_bytes=fifo.result[0], extra=fifo.group_id+"_random_model")
+    
+    
+@refresh_models.handle()
+async def _():
+    post_end_point_list = ["/sdapi/v1/refresh-loras", "/sdapi/v1/refresh-checkpoints"]
+    task_list = []
+    for backend in config.backend_site_list:
+        for end_point in post_end_point_list:
+            backend_url = f"http://{backend}{end_point}"
+            task_list.append(aiohttp_func("post", backend_url, {}))
+    _ = await asyncio.gather(*task_list, return_exceptions=False)
+    await refresh_models.finish("为所有后端刷新模型成功...")
+        
+    
+@stop_all_mission.handle()
+async def _(msg: Message = CommandArg()):
+    task_list = []
+    extra_msg = ""
+    if msg is not None:
+        text_msg = msg.extract_plain_text()
+        if text_msg.isdigit():
+            backend = config.backend_site_list[int(text_msg)]
+            backend_url = f"http://{backend}/sdapi/v1/interrupt"
+            task_list.append(aiohttp_func("post", backend_url))
+            extra_msg = f"{text_msg}号后端"
+        else:
+            await stop_all_mission.finish("笨蛋!后端编号是数字啦!!")
+    else:
+        extra_msg = "所有"
+        for backend in config.backend_site_list:
+            backend_url = f"http://{backend}/sdapi/v1/interrupt" 
+            task_list.append(aiohttp_func("post", backend_url))
+    _ = await asyncio.gather(*task_list, return_exceptions=False)
+    await stop_all_mission.finish(f"终止{extra_msg}任务成功")
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.3.9.7.2/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.3.9.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.3.9.7.2"
+version = "0.3.9.8"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

