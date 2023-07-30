# Comparing `tmp/zood-0.7.6.tar.gz` & `tmp/zood-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zood-0.7.6.tar", max compression
+gzip compressed data, was "zood-0.8.1.tar", max compression
```

## Comparing `zood-0.7.6.tar` & `zood-0.8.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      550 2023-06-04 01:33:59.251613 zood-0.7.6/pyproject.toml
--rw-r--r--   0        0        0      449 2023-01-13 08:15:49.760695 zood-0.7.6/README.md
--rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.7.6/zood/__init__.py
--rw-r--r--   0        0        0     6308 2023-05-19 00:23:30.751193 zood-0.7.6/zood/config/_config.yml
--rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.7.6/zood/config/img/after_copy.png
--rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.7.6/zood/config/img/before_copy.png
--rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.7.6/zood/config/img/enter.png
--rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.7.6/zood/config/img/enter.svg
--rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.7.6/zood/config/img/moon.png
--rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.7.6/zood/config/img/search.svg
--rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.7.6/zood/config/img/sun.png
--rw-r--r--   0        0        0    18776 2023-05-24 15:13:42.054920 zood-0.7.6/zood/config/index.css
--rw-r--r--   0        0        0     3993 2023-04-29 02:33:40.621393 zood-0.7.6/zood/config/js/change_mode.js
--rw-r--r--   0        0        0     1039 2023-05-18 23:52:12.867359 zood-0.7.6/zood/config/js/check_box.js
--rw-r--r--   0        0        0     2654 2023-04-29 06:50:24.299560 zood-0.7.6/zood/config/js/copy_code.js
--rw-r--r--   0        0        0     2253 2023-05-19 00:21:16.921967 zood-0.7.6/zood/config/js/navigator.js
--rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.7.6/zood/config/js/next_front.js
--rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.7.6/zood/config/js/picture_preview.js
--rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.7.6/zood/config/js/picture_title.js
--rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.7.6/zood/config/js/prismjs/prism.css
--rw-r--r--   0        0        0    64866 2023-04-27 06:47:33.381797 zood-0.7.6/zood/config/js/prismjs/prism.js
--rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.7.6/zood/config/js/search.js
--rw-r--r--   0        0        0      546 2023-04-27 06:18:09.762970 zood-0.7.6/zood/config/template.html
--rw-r--r--   0        0        0     4552 2023-06-04 01:33:22.050257 zood-0.7.6/zood/main.py
--rw-r--r--   0        0        0     3535 2023-01-14 05:32:31.481099 zood-0.7.6/zood/md_parser.py
--rw-r--r--   0        0        0     4292 2023-06-04 01:12:09.286908 zood-0.7.6/zood/util.py
--rw-r--r--   0        0        0     8743 2023-06-04 01:05:49.331724 zood-0.7.6/zood/zood.py
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 zood-0.7.6/setup.py
--rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 zood-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0      566 2023-07-30 03:45:14.060768 zood-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      657 2023-07-28 05:47:50.290823 zood-0.8.1/README.md
+-rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.8.1/zood/__init__.py
+-rw-r--r--   0        0        0     4975 2023-07-30 02:58:53.277878 zood-0.8.1/zood/config/_config.yml
+-rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.8.1/zood/config/img/after_copy.png
+-rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.8.1/zood/config/img/before_copy.png
+-rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.8.1/zood/config/img/enter.png
+-rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.8.1/zood/config/img/enter.svg
+-rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.8.1/zood/config/img/moon.png
+-rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.8.1/zood/config/img/search.svg
+-rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.8.1/zood/config/img/sun.png
+-rw-r--r--   0        0        0    14998 2023-07-30 03:04:00.968032 zood-0.8.1/zood/config/index.css
+-rw-r--r--   0        0        0     3991 2023-07-13 02:52:54.473602 zood-0.8.1/zood/config/js/change_mode.js
+-rw-r--r--   0        0        0     2646 2023-07-28 00:49:18.358387 zood-0.8.1/zood/config/js/copy_code.js
+-rw-r--r--   0        0        0     1251 2023-07-28 01:20:50.114459 zood-0.8.1/zood/config/js/global_js_configuration.js
+-rw-r--r--   0        0        0     2154 2023-07-13 02:53:27.953277 zood-0.8.1/zood/config/js/navigator.js
+-rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.8.1/zood/config/js/next_front.js
+-rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.8.1/zood/config/js/picture_preview.js
+-rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.8.1/zood/config/js/picture_title.js
+-rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.8.1/zood/config/js/prismjs/prism.css
+-rw-r--r--   0        0        0    64866 2023-04-27 06:47:33.381797 zood-0.8.1/zood/config/js/prismjs/prism.js
+-rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.8.1/zood/config/js/search.js
+-rw-r--r--   0        0        0      583 2023-07-29 15:25:41.350255 zood-0.8.1/zood/config/template.html
+-rw-r--r--   0        0        0       69 2023-06-24 15:37:55.849962 zood-0.8.1/zood/extensions/__init__.py
+-rw-r--r--   0        0        0     4109 2023-07-03 06:30:14.058101 zood-0.8.1/zood/extensions/poetry_update.py
+-rw-r--r--   0        0        0     6699 2023-07-29 16:25:01.045516 zood-0.8.1/zood/gen_doc.py
+-rw-r--r--   0        0        0     5547 2023-07-29 15:04:26.207636 zood-0.8.1/zood/main.py
+-rw-r--r--   0        0        0     6809 2023-07-29 04:00:11.279113 zood-0.8.1/zood/util.py
+-rw-r--r--   0        0        0     8041 2023-07-29 15:38:58.625505 zood-0.8.1/zood/zood.py
+-rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 zood-0.8.1/PKG-INFO
```

### Comparing `zood-0.7.6/pyproject.toml` & `zood-0.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "zood"
-version = "0.7.6"
+version = "0.8.1"
 description = "web page documentation & comment generation documentation"
 license = "MIT"
 authors = ["kamilu <luzhixing12345@163.com>"]
 readme = "README.md"
 repository = "https://github.com/luzhixing12345/zood"
 documentation = "https://luzhixing12345.github.io/zood/"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
-PyYAML = "^6.0"
+PyYAML = "*"
 MarkdownParser = "*"
+syntaxlight = '*'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 zood = 'zood.main:main'
```

### Comparing `zood-0.7.6/zood/config/img/enter.png` & `zood-0.8.1/zood/config/img/enter.png`

 * *Files identical despite different names*

### Comparing `zood-0.7.6/zood/config/js/change_mode.js` & `zood-0.8.1/zood/config/js/change_mode.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -87,15 +87,15 @@
     change_mode_button.className = 'changeMode'
     change_mode_button.id = 'changeThemeMode'
     change_mode_button.onclick = changeThemeMode
     change_mode_button.state = false; // light: false | dark: true
     document.body.appendChild(change_mode_button)
     // 主题保持
     const savedTheme = localStorage.getItem('theme');
-    // 如果保存的主题存在，则设置当前主题为保存的主题
+    // 如果保存的主题存在,则设置当前主题为保存的主题
     if (savedTheme) {
         let body = document.body;
         let markdown_part = document.querySelector('.markdown-body')
         let change_article_boxes = document.getElementsByClassName('change-article')
         if (savedTheme == "dark") {
             changeToDark(body, markdown_part, change_mode_button, change_article_boxes);
         } else {
```

### Comparing `zood-0.7.6/zood/config/js/check_box.js` & `zood-0.8.1/zood/config/js/global_js_configuration.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,37 @@
+// 这里保存
+
+
+// 美化选择框
+// - [ ] xxx
+// - [x] aaa
 var inputs = document.getElementsByTagName('input')
 for (var i = 0; i < inputs.length; i++) {
     inputs[i].removeAttribute('disabled')
     inputs[i].onclick = function() {
         return false;
     }
 }
 
 var markdown_part = document.querySelector(".markdown-body");
-markdown_part.className = 'markdown-body markdown-light'
+
 
 var currentUrl = window.location.href.slice(0, -1);
 var dirTree = document.querySelector(".dir-tree");
 var links = dirTree.querySelectorAll("a");
-// 主题保持
+
+// 如果保存的主题存在,则设置当前主题为保存的主题
 const savedTheme = localStorage.getItem('theme');
-// 如果保存的主题存在，则设置当前主题为保存的主题
+if (savedTheme !== null) {
+    if (savedTheme === 'light') {
+        markdown_part.className = 'markdown-body markdown-light'
+    } else {
+        markdown_part.className = 'markdown-body markdown-dark'
+    }
+}
 links.forEach(function(link) {
     if (link.href === currentUrl) {
         link.scrollIntoView({
             block: 'center',
             inline: 'nearest',
             container: dirTree
         });
```

### Comparing `zood-0.7.6/zood/config/js/copy_code.js` & `zood-0.8.1/zood/config/js/copy_code.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -25,17 +25,17 @@
     const scrollAmount = event.deltaY * 0.5;
     const imageElement = document.getElementById('code_copy');
     const computedStyle = window.getComputedStyle(imageElement);
     const currentRight = parseInt(computedStyle.getPropertyValue('right'));
 
     // 判断是否已滚动到左右边缘
     if (block.scrollLeft === 0 && scrollAmount < 0) {
-        // 已经滚动到左边缘并且向左滚动，不做任何操作
+        // 已经滚动到左边缘并且向左滚动,不做任何操作
     } else if (maxScroll - block.scrollLeft <= 50 && scrollAmount > 0) {
-        // 已经滚动到右边缘并且向右滚动，不做任何操作
+        // 已经滚动到右边缘并且向右滚动,不做任何操作
         // imageElement.style.right = `${currentRight - scrollAmount}px`;
     } else {
         imageElement.style.right = `${currentRight - scrollAmount}px`;
         // console.log(block.scrollLeft,maxScroll)
         block.scrollLeft += scrollAmount;
     }
 }
@@ -52,14 +52,14 @@
     // 为所有代码段添加可以复制的标记
     var code_blocks = document.getElementsByTagName('pre')
     for (var i = 0; i < code_blocks.length; i++) {
         const code_block = code_blocks[i];
         code_block.addEventListener("mouseenter", () => add(code_block));
         code_block.addEventListener("mouseleave", () => remove(code_block));
         if (code_block.scrollWidth > code_block.clientWidth) {
-            // 如果有横向滚动，阻止页面默认的竖直滚动，并将滚动事件重定向到 <pre> 元素上
+            // 如果有横向滚动,阻止页面默认的竖直滚动,并将滚动事件重定向到 <pre> 元素上
             const blockWidth = code_block.offsetWidth;
             const maxScroll = code_block.scrollWidth - blockWidth;
             code_block.addEventListener('wheel', (event) => horizon_wheel(event, code_block, maxScroll));
         }
     }
 }
```

### Comparing `zood-0.7.6/zood/config/js/navigator.js` & `zood-0.8.1/zood/config/js/navigator.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,25 @@
 const divElement = document.getElementsByClassName("header-navigator")[0]; // 获取目标div元素
-divElement.style.display = "block"; // 将display属性设置为block，以显示元素
+divElement.style.display = "block"; // 将display属性设置为block,以显示元素
 
-let navigator_links = document.querySelectorAll('div a[href^="#"]');
+let navigator_links = document.querySelectorAll('.header-navigator ul li a[href^="#"]');
 navigator_links.forEach(link => {
     link.addEventListener('click', function(event) {
         event.preventDefault();
         let target = document.querySelector(this.getAttribute('href'));
         target.scrollIntoView({
             behavior: 'smooth',
             block: 'start',
             inline: 'nearest'
         });
         // 修改网页 URL
-        let url = window.location.href.split('#')[0]; // 获取当前 URL 并去除 # 及后面的内容
-        let newUrl = url + this.getAttribute('href'); // 将当前 URL 与链接的 href 属性拼接
-        history.pushState(null, null, newUrl); // 修改网页 URL
+        let url = window.location.href.split('#')[0];
+        let newUrl = url + this.getAttribute('href');
+        history.pushState(null, null, newUrl);
+
     });
 });
 
 function isScrolledIntoView(elem) {
     var docViewTop = window.pageYOffset;
     var docViewBottom = docViewTop + window.innerHeight;
     var elemTop = elem.offsetTop;
```

### Comparing `zood-0.7.6/zood/config/js/next_front.js` & `zood-0.8.1/zood/config/js/next_front.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.6/zood/config/js/picture_preview.js` & `zood-0.8.1/zood/config/js/picture_preview.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.6/zood/config/js/prismjs/prism.css` & `zood-0.8.1/zood/config/js/prismjs/prism.css`

 * *Files identical despite different names*

### Comparing `zood-0.7.6/zood/config/js/prismjs/prism.js` & `zood-0.8.1/zood/config/js/prismjs/prism.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.6/zood/config/js/search.js` & `zood-0.8.1/zood/config/js/search.js`

 * *Files identical despite different names*

### Comparing `zood-0.7.6/zood/config/template.html` & `zood-0.8.1/zood/config/template.html`

 * *Files 15% similar despite different names*

```diff
@@ -5,18 +5,20 @@
     <meta charset="UTF-8">
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>
         <%title%>
     </title>
     css-scope
+    hightlight-css
     <link rel="icon" href="<%favicon%>">
 </head>
 
 <body class="light">
+    github-icon
     html-scope
     directory-tree-scope
     <div class="zood"><a class="" href="https://github.com/luzhixing12345/zood" target="_blank">zood</a></div>
     js-scope
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 
 
-css-scope
-html-scope directory-tree-scope
+css-scope hightlight-css
+github-icon html-scope directory-tree-scope
 zood
 js-scope
```

### Comparing `zood-0.7.6/zood/zood.py` & `zood-0.8.1/zood/zood.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,235 +1,233 @@
-
 import shutil
 import os
-import MarkdownParser
-import json 
 from .util import *
 
-def initZood(md_dir_name):
+def init_zood(md_dir_name):
     # 初始化 zood 文件
-    
+
     if os.path.exists(md_dir_name):
-        printInfo(f"{md_dir_name} 已存在,请删除文件夹后重试")
+        print_info(f"{md_dir_name} 已存在,请删除文件夹后重试")
         return
     else:
-        
         os.mkdir(md_dir_name)
 
-        readme = ''
-        if os.path.exists('README.md'):
-            with open('README.md','r',encoding='utf-8') as f:
+        readme = ""
+        if os.path.exists("README.md"):
+            with open("README.md", "r", encoding="utf-8") as f:
                 readme = f.read()
-        # with open('.gitignore','a+',encoding='utf-8') as f:
-        #     gitignore_files = f.read()
-        #     if gitignore_files.find(f'/{md_dir_name}/') == -1:
-        #         gitignore_files += f'\n./{md_dir_name}/\n'
-        #         f.write(gitignore_files)
 
-        initDirYml(md_dir_name)
+        init_dir_yml(md_dir_name)
 
-        with open(os.path.join(md_dir_name,'README.md'),'w',encoding='utf-8') as f:
+        with open(os.path.join(md_dir_name, "README.md"), "w", encoding="utf-8") as f:
             f.write(readme)
 
-        printInfo(f"已初始化 [{md_dir_name}]",'green')
+        print_info(f"已初始化 [{md_dir_name}]", "green")
+
+
+def create_new_file(md_dir_name, dir_name, file_name):
+    file_path = os.path.join(md_dir_name, dir_name, file_name + ".md")
 
-def createNewFile(md_dir_name,dir_name,file_name):
-    
-    file_path = os.path.join(md_dir_name,dir_name,file_name+'.md')
-        
     if os.path.exists(file_path):
-        printInfo(f'{file_path} 已存在')
+        print_info(f"{file_path} 已存在")
         return
-    
-    if not os.path.exists(os.path.join(md_dir_name,dir_name)):
-        os.makedirs(os.path.join(md_dir_name,dir_name))
-    
-    updateDirYml(file_name,dir_name,md_dir_name)
 
-    with open(file_path,'w',encoding='utf-8') as f:
-        basic_info = f'\n# {file_name}\n'
+    if not os.path.exists(os.path.join(md_dir_name, dir_name)):
+        os.makedirs(os.path.join(md_dir_name, dir_name))
+
+    update_dir_yml(file_name, dir_name, md_dir_name)
+
+    with open(file_path, "w", encoding="utf-8") as f:
+        basic_info = f"\n# {file_name}\n"
         f.write(basic_info)
-    
-    printInfo(f"创建文件 {file_path}",color='green')
 
-def initDirYml(md_dir_name):
+    print_info(f"创建文件 {file_path}", color="green")
+
+
+def init_dir_yml(md_dir_name):
     # 生成目录记录
-    dir_yml = {'.':[{'README':1}]}
-    writeConfigFile(dir_yml,os.path.join(md_dir_name,'dir.yml'))
+    dir_yml = {".": [{"README": 1}]}
+    writeConfigFile(dir_yml, os.path.join(md_dir_name, "dir.yml"))
+
 
-def updateDirYml(file_name,dir_name,md_dir_name):
+def update_dir_yml(file_name, dir_name, md_dir_name):
     # 更新当前路径下的 dir.yml
 
     current_dir = os.getcwd()
-    dir_yml_path = os.path.join(current_dir,md_dir_name,'dir.yml')
-    dir_yml = readConfigFile(dir_yml_path)
-    
+    dir_yml_path = os.path.join(current_dir, md_dir_name, "dir.yml")
+    dir_yml = read_configfile(dir_yml_path)
+
     sort(dir_yml)
-    
+
     if dir_name in dir_yml.keys():
         number = list(dir_yml[dir_name][-1].values())[0] + 1
-        dir_yml[dir_name].append({file_name:number})
+        dir_yml[dir_name].append({file_name: number})
     else:
         dir_yml[dir_name] = []
-        dir_yml[dir_name].append({file_name:1})
-    
-    writeConfigFile(dir_yml,dir_yml_path)
+        dir_yml[dir_name].append({file_name: 1})
 
-def parseMarkdownFiles(md_dir_name):
-    
-    current_dir = os.getcwd()
-    dir_yml_path = os.path.join(current_dir,md_dir_name,'dir.yml')
-    dir_yml = readConfigFile(dir_yml_path)
-    sort(dir_yml)
-    directory_tree = []
-    markdown_htmls = {}
-    for dir_name, files in dir_yml.items():
-        file_names = []
-        for i in files:
-            file_name = list(i.keys())[0]
-            file_path = os.path.join(md_dir_name,dir_name,file_name+'.md')
-            if not os.path.exists(file_path):
-                printInfo('[zood解析失败]: 找不到文件' + file_path)
-                print("如手动删除md文件可使用 zood update 更新 dir.yml")
-                exit(0)
-            else:
-                with open(file_path,'r',encoding='utf-8') as f:
-                    markdown_htmls[file_path] = MarkdownParser.parse_withtag(f.read())
-                file_names.append(file_name)
-        directory_tree.append({dir_name:file_names})
-        
-    return directory_tree,markdown_htmls
-            
-
-def parseConfig(config,markdown_htmls):
-    
-    html_dir_name = config['html_folder']
-    html_tempate_path = os.path.join(os.path.dirname(__file__),'config','template.html')
-    css_template_path = os.path.join(os.path.dirname(__file__),'config','index.css')
-    
-    with open(html_tempate_path,'r',encoding='utf-8') as f:
+    writeConfigFile(dir_yml, dir_yml_path)
+
+
+
+
+def parse_config(config, markdown_htmls):
+    html_dir_name = config["html_folder"]
+    html_tempate_path = os.path.join(os.path.dirname(__file__), "config", "template.html")
+    css_template_path = os.path.join(os.path.dirname(__file__), "config", "index.css")
+
+    with open(html_tempate_path, "r", encoding="utf-8") as f:
         basic_html_template = f.read()
-    
-    
+
     # js 部分
-    js_scope = zoodJSOptions(config,markdown_htmls)
-    basic_html_template = basic_html_template.replace('js-scope',js_scope)
-    
+    js_scope = zood_js_options(config, markdown_htmls)
+    basic_html_template = basic_html_template.replace("js-scope", js_scope)
+
     # css 部分
-    prism_src = '../../../css/prism.css'
-    index_src = '../../../css/index.css'
+    # prism_src = "../../../css/prism.css"
+    index_src = "../../../css/index.css"
 
-    css_scope = ''
-    if config['options']['enable_highlight']:
-        css_scope += f"<link rel='stylesheet' href={prism_src} />"
+    css_scope = ""
+    # if config["options"]["enable_highlight"]:
+    #     css_scope += f"<link rel='stylesheet' href={prism_src} />"
     css_scope += f"<link rel='stylesheet' href={index_src} />"
-    basic_html_template = basic_html_template.replace('css-scope',css_scope)
-    
-    with open(css_template_path,'r',encoding='utf-8') as f:
+    basic_html_template = basic_html_template.replace("css-scope", css_scope)
+
+    with open(css_template_path, "r", encoding="utf-8") as f:
         basic_css_template = f.read()
-    favicon_url = config['favicon']
-    if favicon_url[:4] == 'http':
-        basic_html_template = basic_html_template.replace('<%favicon%>',favicon_url)
-        
+    favicon_url: str = config["favicon"]
+    if favicon_url[:4] == "http":
+        basic_html_template = basic_html_template.replace("<%favicon%>", favicon_url)
+
     else:
         img_name = favicon_url.split(os.sep)[-1]
-        shutil.copy(favicon_url,f'./{html_dir_name}/img/'+img_name)
-        basic_html_template = basic_html_template.replace('<%favicon%>','../../../img/'+img_name)
-        
-    title = config['title']
-    basic_html_template = basic_html_template.replace('<%title%>',title)
-    
-    custom_options = getCustomOptions(config,['color','font','position'])
-    
-    for k,v in custom_options:
-        basic_css_template = basic_css_template.replace(f'\"<%{k}%>\"',v)
-        
-    
-    basic_html_template = basic_html_template.replace('css-scope',css_scope)
-    
-    with open(f'./{html_dir_name}/css/index.css','w',encoding='utf-8') as f:
+        shutil.copy(favicon_url, f"./{html_dir_name}/img/" + img_name)
+        basic_html_template = basic_html_template.replace("<%favicon%>", "../../../img/" + img_name)
+
+    title = config["title"]
+    basic_html_template = basic_html_template.replace("<%title%>", title)
+
+    custom_options = get_custom_options(config, ["color", "font", "position"])
+
+    for k, v in custom_options:
+        basic_css_template = basic_css_template.replace(f'"<%{k}%>"', v)
+
+    basic_html_template = basic_html_template.replace("css-scope", css_scope)
+
+    with open(f"./{html_dir_name}/css/index.css", "w", encoding="utf-8") as f:
         f.write(basic_css_template)
-    
+
     return basic_html_template
 
-def getCustomOptions(config,keys):
-    
+
+def get_custom_options(config, keys):
     custom_options = []
     for k in keys:
         custom_options += list(config[k].items())
     return custom_options
 
-def zoodJSOptions(config,markdown_htmls):
-    
-    js_scope = ''
-    html_dir_name = config['html_folder']
-    md_dir_name = config['markdown_folder']
 
-    if config['options']['enable_next_front']:
-        js_code = insertJScode('enable_next_front',html_dir_name)
+def zood_js_options(config, markdown_htmls):
+    js_scope = ""
+    html_dir_name = config["html_folder"]
+    md_dir_name = config["markdown_folder"]
+
+    if config["options"]["enable_next_front"]:
+        js_code = insertJScode("enable_next_front", html_dir_name)
         js_code += f"<script>addLink(<%front_url%>,<%next_url%>,<%control%>)</script>"
         js_scope += js_code
 
-    if config['options']['enable_change_mode']:
-    
-        js_code = insertJScode('enable_change_mode',html_dir_name)
-        js_code += f"<script>addChangeModeButton(\"../../../img/sun.png\",\"../../../img/moon.png\")</script>"
-        js_scope += js_code
-        
-    if config['options']['enable_copy_code']:
-        
-        js_code = insertJScode('enable_copy_code',html_dir_name)
-        js_code += f"<script>addCodeCopy(\"../../../img/before_copy.png\",\"../../../img/after_copy.png\")</script>"
-        js_scope += js_code
-        
-    if config['options']['enable_navigator']:
-        js_code = insertJScode('enable_navigator',html_dir_name)
+    if config["options"]["enable_change_mode"]:
+        js_code = insertJScode("enable_change_mode", html_dir_name)
+        js_code += (
+            f'<script>addChangeModeButton("../../../img/sun.png","../../../img/moon.png")</script>'
+        )
+        js_scope += js_code
+
+    if config["options"]["enable_copy_code"]:
+        js_code = insertJScode("enable_copy_code", html_dir_name)
+        js_code += f'<script>addCodeCopy("../../../img/before_copy.png","../../../img/after_copy.png")</script>'
+        js_scope += js_code
+
+    if config["options"]["enable_navigator"]:
+        js_code = insertJScode("enable_navigator", html_dir_name)
         js_scope += js_code
 
+    # if config["options"]["enable_highlight"]:
+    #     # 复制prismjs
+    #     shutil.copy(
+    #         os.path.join(os.path.dirname(__file__), "config", "js", "prismjs", "prism.css"),
+    #         f"{html_dir_name}/css",
+    #     )
+    #     shutil.copy(
+    #         os.path.join(os.path.dirname(__file__), "config", "js", "prismjs", "prism.js"),
+    #         f"{html_dir_name}/js",
+    #     )
+    #     src = "../../../js/prism.js"
+    #     highlight = f'<script type="text/javascript" src="{src}"></script>'
+    #     js_scope += highlight
 
-    if config['options']['enable_highlight']:
-        # 复制prismjs
-        shutil.copy(os.path.join(os.path.dirname(__file__),'config','js','prismjs','prism.css'),f'{html_dir_name}/css')
-        shutil.copy(os.path.join(os.path.dirname(__file__),'config','js','prismjs','prism.js'),f'{html_dir_name}/js')
-        src = "../../../js/prism.js"
-        highlight = f"<script type=\"text/javascript\" src=\"{src}\"></script>"
-        js_scope += highlight
-        
-
-    if config['options']['enable_picture_title']:
-        js_code = insertJScode('enable_picture_title',html_dir_name)
-        js_scope += js_code
-        
-    if config['options']['enable_picture_preview']:
-        js_code = insertJScode('enable_picture_preview',html_dir_name)
-        js_scope += js_code
-        
-    if config['options']['enable_search']['enable']:
-        js_code = insertJScode('enable_search',html_dir_name)
-        all_api_text = getAllAPIText(markdown_htmls,config['options']['enable_search']['search_scope'],md_dir_name)
-        js_code += f"<script>addSearchBar({all_api_text},\"../../../img/search.svg\",\"../../../img/enter.svg\",\"Ctrl+K\")</script>"
-        js_scope += js_code
-
-    if config['options']['enable_mermaid']:
-        js_code = '<script type=\"module\">\
-const codeBlocks = document.querySelectorAll(\'.language-mermaid\');\
+    if config["options"]["enable_picture_title"]:
+        js_code = insertJScode("enable_picture_title", html_dir_name)
+        js_scope += js_code
+
+    if config["options"]["enable_picture_preview"]:
+        js_code = insertJScode("enable_picture_preview", html_dir_name)
+        js_scope += js_code
+
+    if config["options"]["enable_search"]["enable"]:
+        js_code = insertJScode("enable_search", html_dir_name)
+        all_api_text = getAllAPIText(
+            markdown_htmls,
+            config["options"]["enable_search"]["search_scope"],
+            md_dir_name,
+        )
+        js_code += f'<script>addSearchBar({all_api_text},"../../../img/search.svg","../../../img/enter.svg","Ctrl+K")</script>'
+        js_scope += js_code
+
+    if config["options"]["enable_mermaid"]:
+        js_code = "<script type=\"module\">\
+const codeBlocks = document.querySelectorAll('.language-mermaid');\
 codeBlocks.forEach(codeBlock => {\
-    codeBlock.classList.remove(\'language-mermaid\');\
-    codeBlock.classList.add(\'mermaid\');\
+    codeBlock.classList.remove('language-mermaid');\
+    codeBlock.classList.add('mermaid');\
 });\
-import mermaid from \'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs\';\
+import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';\
 mermaid.initialize({ startOnLoad: true });\
-</script>'
+</script>"
         js_scope += js_code
 
-    js_scope += insertJScode('enable_check_box',html_dir_name)
+    if config["options"]["enable_latex"]:
+        js_code = """
+        <script>
+            MathJax = {
+            tex: {
+                inlineMath: [['$', '$'], ['\\(', '\\)']]
+            }
+            };
+            </script>
+        <script id="MathJax-script" async
+        src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js">
+        </script>
+        """
+        js_scope += js_code
+
+    js_scope += insertJScode("global_js_configuration", html_dir_name)
 
     return js_scope
 
-def insertJScode(file_name,html_dir_name):
-    file_name = file_name[7:] # 跳过enable_
-    # 文件同名
-    shutil.copy(os.path.join(os.path.dirname(__file__),'config','js',f'{file_name}.js'),f'{html_dir_name}/js')
+
+def insertJScode(file_name: str, html_dir_name):
+    if file_name.startswith("enable_"):
+        # 跳过enable_
+        file_name = file_name[7:]
+    js_file_name = os.path.join(os.path.dirname(__file__), "config", "js", f"{file_name}.js")
+    if os.path.exists(js_file_name):
+        shutil.copy(
+            js_file_name,
+            f"{html_dir_name}/js",
+        )
     src = f"../../../js/{file_name}.js"
-    js_code = f"<script type=\"text/javascript\" src=\"{src}\"></script>"
+    js_code = f'<script type="text/javascript" src="{src}"></script>'
     return js_code
-        
+
+
```

### Comparing `zood-0.7.6/PKG-INFO` & `zood-0.8.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 Metadata-Version: 2.1
 Name: zood
-Version: 0.7.6
+Version: 0.8.1
 Summary: web page documentation & comment generation documentation
 Home-page: https://github.com/luzhixing12345/zood
 License: MIT
 Author: kamilu
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: MarkdownParser
-Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: PyYAML
+Requires-Dist: syntaxlight
 Project-URL: Documentation, https://luzhixing12345.github.io/zood/
 Project-URL: Repository, https://github.com/luzhixing12345/zood
 Description-Content-Type: text/markdown
 
 # zood
 
-zood 是一个辅助文档生成的Python库, zood的页面风格更倾向于纯文档内容而非博客
+zood 网页文档生成的 python 库, 可以将本地 Markdown 文件转为 Web 网页
+
+zood 的页面风格更倾向于纯文档内容而非博客, 您可利用 Github Pages 为每一个仓库部署单独的网页文档
 
 ## 主题预览
 
-[![20230101121438](https://raw.githubusercontent.com/learner-lu/picbed/master/20230101121438.png)](https://luzhixing12345.github.io/zood/)
+> 点击图片查看
+
+[![20230728134651](https://raw.githubusercontent.com/learner-lu/picbed/master/20230728134651.png)](https://luzhixing12345.github.io/zood/)
 
 ## 安装与使用
 
 ```bash
 pip install zood
 ```
 
 参见 [用户使用文档](https://luzhixing12345.github.io/zood/)
 
 ## 参考
 
 - [UI](https://remixicon.com/)
+- [tholman github-corners](https://tholman.com/github-corners/)
```

