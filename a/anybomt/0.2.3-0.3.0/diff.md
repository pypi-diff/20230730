# Comparing `tmp/anybomt-0.2.3.tar.gz` & `tmp/anybomt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anybomt-0.2.3.tar", last modified: Thu Jul 27 07:09:07 2023, max compression
+gzip compressed data, was "anybomt-0.3.0.tar", last modified: Sat Jul 29 16:57:31 2023, max compression
```

## Comparing `anybomt-0.2.3.tar` & `anybomt-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 07:09:07.666002 anybomt-0.2.3/
--rw-rw-rw-   0        0        0     1092 2023-07-21 08:26:10.000000 anybomt-0.2.3/LICENSE
--rw-rw-rw-   0        0        0    24402 2023-07-27 07:09:07.664998 anybomt-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    23973 2023-07-22 09:55:41.000000 anybomt-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 07:09:07.661457 anybomt-0.2.3/anybomt.egg-info/
--rw-rw-rw-   0        0        0    24402 2023-07-27 07:09:07.000000 anybomt-0.2.3/anybomt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-07-27 07:09:07.000000 anybomt-0.2.3/anybomt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 07:09:07.000000 anybomt-0.2.3/anybomt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-27 07:09:07.000000 anybomt-0.2.3/anybomt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 07:09:07.000000 anybomt-0.2.3/anybomt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    90356 2023-07-27 07:07:31.000000 anybomt-0.2.3/anybomt.py
--rw-rw-rw-   0        0        0       42 2023-07-27 07:09:07.667047 anybomt-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      980 2023-07-27 07:08:50.000000 anybomt-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:57:31.741777 anybomt-0.3.0/
+-rw-rw-rw-   0        0        0     1092 2023-07-21 08:26:10.000000 anybomt-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0    59012 2023-07-29 16:57:31.740769 anybomt-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    58570 2023-07-29 16:54:10.000000 anybomt-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 16:57:31.736631 anybomt-0.3.0/anybomt.egg-info/
+-rw-rw-rw-   0        0        0    59012 2023-07-29 16:57:31.000000 anybomt-0.3.0/anybomt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-07-29 16:57:31.000000 anybomt-0.3.0/anybomt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 16:57:31.000000 anybomt-0.3.0/anybomt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-29 16:57:31.000000 anybomt-0.3.0/anybomt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 16:57:31.000000 anybomt-0.3.0/anybomt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   108105 2023-07-29 16:14:29.000000 anybomt-0.3.0/anybomt.py
+-rw-rw-rw-   0        0        0       42 2023-07-29 16:57:31.742769 anybomt-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2023-07-29 16:56:33.000000 anybomt-0.3.0/setup.py
```

### Comparing `anybomt-0.2.3/LICENSE` & `anybomt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anybomt-0.2.3/anybomt.py` & `anybomt-0.3.0/anybomt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 
+def printar(printa):
+    print(printa)
 
 # Função para calcular o math.factorial de um número inteiro
 def fatorial(n):
     try:
          import math
          return math.factorial(n)
     except Exception as e:
@@ -64,97 +66,21 @@
     import os
     import platform
     if platform.system() == "Windows":
         os.system('cls')
     else:
         os.system('clear')
 
-
-
-# Classe Trigonometria
-class Trigonometria:
-    # Função para calcular o seno de um ângulo em radianos
-    def seno(angle):
-        try:
-            import math
-            return math.sin(angle)
-        except Exception as e:
-            return e
-
-    # Função para calcular o cosseno de um ângulo em radianos
-    def cosseno(angle):
-        try:
-            import math
-            return math.cos(angle)
-        except Exception as e:
-            return e
-
-    # Função para calcular a tangente de um ângulo em radianos
-    def tangente(angle):
-        try:
-            import math
-            return math.tan(angle)
-        except Exception as e:
-            return e
-
-    # Função para calcular o cosseno hiperbólico de um número
-    def cosseno_hiperbolico(num):
-        try:
-            import math
-            return math.cosh(num)
-        except Exception as e:
-            return e
-
-    # Função para calcular o seno hiperbólico de um número
-    def seno_hiperbolico(num):
-        try:
-            import math
-            return math.sinh(num)
-        except Exception as e:
-            return e
-
-    # Função para calcular a tangente hiperbólica de um número
-    def tangente_hiperbolica(num):
-        try:
-            import math
-            return math.tanh(num)
-        except Exception as e:
-            return e
-
-    # Função para calcular o arco cosseno de um número
-    def arco_cosseno(num):
-        try:
-            import math
-            return math.acos(num)
-        except Exception as e:
-            return e
-
-    # Função para calcular o arco seno de um número
-    def arco_seno(num):
-        try:
-            import math
-            return math.asin(num)
-        except Exception as e:
-            return e
-
-    # Função para calcular o arco tangente de um número
-    def arco_tangente(num):
-        try:
-            import math
-            return math.atan(num)
-        except Exception as e:
-            return e
-
-    # Função para calcular o arco tangente de um número com dois argumentos (y, x)
-    def arco_tangente2(y, x):
-        try:
-            import math
-            return math.atan2(y, x)
-        except Exception as e:
-            return e
+def vetor(*args: list):
+    try:
+        import numpy as np
+        return np.array(args)
+    except Exception as e:
+        return e
+    
 
 # Função para calcular o logaritmo natural de um número
 def logaritmo_natural(num):
     try:
         import math
         return math.log(num)
     except Exception as e:
@@ -216,15 +142,14 @@
     try:
         import math as mp
         phi = (1 + mp.sqrt(5)) / 2
         return phi
     except Exception as e: return e
 
 
-
 def Num_catalan(n):
     try:
         import math 
         numero = math.factorial(2*n) // (math.factorial(n+1) * math.factorial(n))
         return numero
     except Exception as e: return e
 
@@ -309,80 +234,758 @@
 # Função para calcular o teto de um número
 def teto_do_numero(num):
     try:
         import math
         return math.ceil(num)
     except Exception as e:
         return e
+    
+    
 
-def equacaoPrimeiroGrauEx(a, b, c):
-    try:
-        if a == 0:
-            return "A equação não é do primeiro grau."
-        else:
-             x = (c - b) /a
-             sinal = '+' if b >= 0 else ''
-             expl= f"{a}x {sinal}{b} = {c}\n{b} vai trocar de lado e vai no lado do {c}\nmais vai trocar de sinal\nvai ficar {a}x = {c} - ({sinal}{b})\n{a}x = {c-b}\nx = {c-b}/{a}\nx = {x}"
-             return f"{a}x {sinal}{b} = {c}  (x: {x})\n--EXPLICAÇÃO--\n{expl}"
-    except Exception as e:
-        return e
+class Espera:
+    def espera_s(n):
+        import time
+        time.sleep(n)
+
+    def espera_m(n):
+        import time
+        time.sleep(n*60)
+
+    def espera_h(n):
+        import time
+        time.sleep(n*3600)
+
+    def espera_d(n):
+        import time
+        time.sleep(n*86400)
+    
+    def espera_me28(n):
+        import time
+        time.sleep(n*2419200)
+    
+    def espera_me29(n):
+        import time
+        time.sleep(n*2505600)
+    
+    def espera_me30(n):
+        import time
+        time.sleep(n*2592000)
+    
+    def espera_me31(n):
+        import time
+        time.sleep(n*2678400)
+    
+    def espera_tr30(n):
+        import time
+        time.sleep(n*7776000)
+
+    def espera_tr31(n):
+        import time
+        time.sleep(n*2678400*3)
+
+    def espera_sem(n):
+        import time
+        time.sleep(n * 604800)
+    
+    def espera_ano365(n):
+        import time
+        time.sleep(n*31536000)
+    
+    def espera_ano366(n):
+        import time
+        time.sleep(n*31622400)
+    
+    def espera_dec365(n):
+        import time
+        time.sleep(n*31536000*10)
+    
+    def espera_dec366(n):
+        import time
+        time.sleep(n*31622400*10)
+    
+    def miliseg(n):
+        import time
+        time.sleep(n / 1000)
+
+    def esperar_e_desligar_m(n:int):
+        try:
+            import time
+            import os
+            n = n * 60
+            os.system(f'shutdown /s /t {n}')
+        except Exception as e:
+            return e 
+        
+    def esperar_e_desligar_s(n:int):
+        try:
+            import os
+            os.system(f'shutdown /s /t {n}')
+        except Exception as e:
+            return e 
+        
+    def esperar_e_reiniciar_m(n:int):
+        try:
+            import os
+            n = n * 60
+            os.system(f'shutdown /r /t {n}')
+        except Exception as e:
+            return e
+    
+    def esperar_e_reiniciar_s(n:int):
+        try:
+            import os
+            os.system(f'shutdown /r /t {n}')
+        except Exception as e:
+            return e 
 
-def equacaoSegundoGrauEx(a, b, c):
-    try:
-        import math
-        if a == 0:
-            return "A equação não é do segundo grau."
 
-        delta = b ** 2 - 4 * a * c
+class Aleator:
 
-        if delta < 0:
-            return "A equação não possui raízes reais."
-        elif delta == 0:
-            x = -b / (2 * a)
-            return f"A equação possui uma raiz real: x = {x}"
-        else:
-             sinalb = '+' if b >=0 else ''
-             sinalc = '+' if c >=0 else ''
-             x1 = (-b + math.sqrt(delta)) / (2*a)
-             x2 = (-b - math.sqrt(delta)) / (2*a)
-             exp = f"delta = {b}² - 4*{a}*{c}\nse a delta é menor que 0, a equação não possui raiz reais\nsenão vai ser:\nx = {sinalb}{b} / (2*{a})\nx1 = ({sinalb}{b} + √{delta} / 2*{a})\nx2 = ({sinalb}{b} - √{delta} / 2*{a})\ne x1 = {x1}, x2 = {x2}"
+    def alea_inteiro_a_b(a:int, b:int):
+        try:
+            import random
+            if b < a:
+                return "\033[4;7;31mO 'b' nao pode ser maior que 'a'\033[m"
+            else:
+                return random.randint(a, b)
+        except Exception as e:
+            return e
         
-             return f"A equação {a}x² {sinalb}{b}x {sinalc}{c} = 0 possui duas raízes reais: [x1 = {x1}, x2 = {x2}]\n--EXPLICAÇÂO--\n{exp}"
-    except Exception as e:
-        return e
+    def alea_inteiro_a(a:int):
+        try:
+            import numpy as radom
+            return radom.random.randint(a)
+        except Exception as e:
+            return e
+        
+    def alea():
+        import numpy as radom
+        return radom.random.rand()
 
-def equacaoPrimeiroGrau(a, b, c):
-    try:
-        if a == 0:
-            return "A equação não é do primeiro grau."
-        else:
-            x = (c - b) / a
-            return x
-    except Exception as e:
-        return e
+    def alea_num():
+        import numpy as radom
+        return radom.random.randn()
+    
+    
+    def escolhe(escolha):
+        try:
+            from random import choice
+            return choice(escolha)
+        except Exception as e:
+            return e
+    
 
-def equacaoSegundoGrau(a, b, c):
-    try:
-        if a == 0:
-            return "A equação não é do segundo grau."
+class Grafico:
 
-        delta = b ** 2 - 4 * a * c
+    def grafico_barra(x=None, y=None, eixox=None, eixoy=None, titulo=None, cor=None, legenda=None, tamanho_d_figura=(8, 6), salvar_como=None, xlimite=None, ylimite=None):
+        try:
+            import matplotlib.pyplot as plt
+            plt.rcParams['toolbar'] = 'None'
+            if x is not None and y is not None:
+                plt.figure(figsize=tamanho_d_figura)
+                bars = plt.bar(x, y, color=cor)
 
-        if delta < 0:
-            return "A equação não possui raízes reais."
-        elif delta == 0:
-            x = -b / (2 * a)
-            return f"A equação possui uma raiz real: x = {x}"
-        else:
-            x1 = (-b + raiz_quadrada(delta)) / (2 * a)
-            x2 = (-b - raiz_quadrada(delta)) / (2 * a)
-            return f"A equação possui duas raízes reais: x1 = {x1}, x2 = {x2}"
-    except Exception as e:
-        return e
+                if eixox:
+                    plt.xlabel(eixox)
+                if eixoy:
+                    plt.ylabel(eixoy)
+                if titulo:
+                    plt.title(titulo)
+                if legenda:
+                    plt.legend(bars, legenda)
+
+                if xlimite:
+                    plt.xlim(xlimite)
+                if ylimite:
+                    plt.ylim(ylimite)
+
+                if salvar_como:
+                    plt.savefig(salvar_como)
+                else:
+                    plt.show()
+
+            else:
+                # Aqui você pode adicionar alguma lógica para lidar com o caso em que x e y não são fornecidos.
+                # Por exemplo, levantar um erro ou exibir uma mensagem informativa.
+                pass
+
+        except Exception as e:
+            return e
+    
+    def grafico_dispersao(x=None, y=None, eixox=None, eixoy=None, titulo=None, cor=None, marcador='o', tamanho_d_figura=(8, 6), salvar_como=None, xlimite=None, ylimite=None):
+        try:
+            import matplotlib.pyplot as plt
+            plt.rcParams['toolbar'] = 'None'
+            if x is not None and y is not None:
+                plt.figure(figsize=tamanho_d_figura)
+                plt.scatter(x, y, color=cor, marker=marcador)
+
+                if eixox:
+                    plt.xlabel(eixox)
+                if eixoy:
+                    plt.ylabel(eixoy)
+                if titulo:
+                    plt.title(titulo)
+
+                if xlimite:
+                    plt.xlim(xlimite)
+                if ylimite:
+                    plt.ylim(ylimite)
+
+                if salvar_como:
+                    plt.savefig(salvar_como)
+                else:
+                    plt.show()
+
+            else:
+                # Aqui você pode adicionar alguma lógica para lidar com o caso em que x e y não são fornecidos.
+                # Por exemplo, levantar um erro ou exibir uma mensagem informativa.
+                pass
 
+        except Exception as e:
+            return e
+    
+    def grafico_pizza(dados=None, tamanhos=None, titulo=None, cor=None, destaca=None, tamanho_d_figura=(8, 6), salvar_como=None):
+        try:
+            import matplotlib.pyplot as plt
+            plt.rcParams['toolbar'] = 'None'
+            if dados is not None and tamanhos is not None:
+                plt.figure(figsize=tamanho_d_figura)
+                plt.pie(tamanhos, labels=dados, colors=cor, explode=destaca, autopct='%1.1f%%', shadow=True)
+
+                if titulo:
+                    plt.title(titulo)
+
+                if salvar_como:
+                    plt.savefig(salvar_como)
+                else:
+                    plt.show()
+
+            else:
+                # Aqui você pode adicionar alguma lógica para lidar com o caso em que labels e sizes não são fornecidos.
+                # Por exemplo, levantar um erro ou exibir uma mensagem informativa.
+                pass
+
+        except Exception as e:
+            return e
+    
+    def grafico_linhas(x, y, titulo=None, eixox=None, eixoy=None, tamanho_d_figura=(8, 6), salvar_como=None):
+        try:
+            import matplotlib.pyplot as plt
+            plt.rcParams['toolbar'] = 'None'
+            plt.figure(figsize=tamanho_d_figura)
+            plt.plot(x, y)
+
+            if titulo:
+                plt.title(titulo)
+
+            if eixox:
+                plt.xlabel(eixox)
+
+            if eixoy:
+                plt.ylabel(eixoy)
+
+            if salvar_como:
+                plt.savefig(salvar_como)
+            else:
+                plt.show()
+
+        except Exception as e:
+            return e
+    
+    def grafico_area(x, y, titulo=None, eixox=None, eixoy=None, tamanho_d_figura=(8, 6), salvar_como=None):
+        try:
+            import matplotlib.pyplot as plt
+            plt.rcParams['toolbar'] = 'None'
+            plt.figure(figsize=tamanho_d_figura)
+            plt.fill_between(x, y)
+
+            if titulo:
+                plt.title(titulo)
+
+            if eixox:
+                plt.xlabel(eixox)
+
+            if eixoy:
+                plt.ylabel(eixoy)
+
+            if salvar_como:
+                plt.savefig(salvar_como)
+            else:
+                plt.show()
+
+        except Exception as e:
+            return e
+        
+    
+
+    def grafico_histograma(valores, titulo=None, eixox=None, eixoy=None, tamanho_d_figura=(8, 6), salvar_como=None):
+        try:
+            import matplotlib.pyplot as plt
+            plt.rcParams['toolbar'] = 'None'
+            plt.figure(figsize=tamanho_d_figura)
+            plt.hist(valores, bins='auto', alpha=0.7, color='blue', edgecolor='black')
+
+            if titulo:
+                plt.title(titulo)
+
+            if eixox:
+                plt.xlabel(eixox)
+
+            if eixoy:
+                plt.ylabel(eixoy)
+
+            if salvar_como:
+                plt.savefig(salvar_como)
+            else:
+                plt.show()
+
+        except Exception as e:
+            return e
+    
+    
+
+    def grafico_boxplot_(dados, titulo=None, eixox=None, tamanho_d_figura=(8, 6), salvar_como=None):
+        try:
+            import matplotlib.pyplot as plt
+            plt.figure(figsize=tamanho_d_figura)
+            plt.boxplot(dados)
+
+            if titulo:
+                plt.title(titulo)
+
+            if eixox:
+                plt.xlabel(eixox)
+
+            if salvar_como:
+                plt.savefig(salvar_como)
+            else:
+                plt.show()
+
+        except Exception as e:
+            return e
+    
+    
+
+    def grafico_boxplot(dados, titulo=None, eixox=None, tamanho_d_figura=(8, 6), salvar_como=None):
+        try:
+            import matplotlib.pyplot as plt
+            plt.figure(figsize=tamanho_d_figura)
+            plt.boxplot(dados)
+
+            if titulo:
+                plt.title(titulo)
+
+            if eixox:
+                plt.xlabel(eixox)
+
+            if salvar_como:
+                plt.savefig(salvar_como)
+            else:
+                plt.show()
+
+        except Exception as e:
+            return e
+
+        
+        
+
+    def surface_plot(x, y, z, titulo=None, eixox=None, eixoy=None, eixoz=None, tamanho_d_figura=(10, 8), salvar_como=None):
+        try:
+            import matplotlib.pyplot as plt
+            import numpy as np
+            fig = plt.figure(figsize=tamanho_d_figura)
+            ax = fig.add_subplot(111, projection='3d')
+            ax.plot_surface(x, y, z, cmap='viridis')
+
+            if titulo:
+                plt.title(titulo)
+
+            if eixox:
+                ax.set_xlabel(eixox)
+
+            if eixoy:
+                ax.set_ylabel(eixoy)
+
+            if eixoz:
+                ax.set_zlabel(eixoz)
+
+            if salvar_como:
+                plt.savefig(salvar_como)
+            else:
+                plt.show()
+
+        except Exception as e:
+            return e
+
+
+    def grafico_contorno(x, y, z, titulo=None, eixox=None, eixoy=None, tamanho_d_figura=(8, 6), salvar_como=None):
+        try:
+            import numpy as np
+            import matplotlib.pyplot as plt
+            plt.rcParams['toolbar'] = 'None'
+            X, Y = np.meshgrid(x, y)
+            plt.figure(figsize=tamanho_d_figura)
+            plt.contour(X, Y, z)
+
+            if titulo:
+                plt.title(titulo)
+
+            if eixox:
+                plt.xlabel(eixox)
+
+            if eixoy:
+                plt.ylabel(eixoy)
+
+            if salvar_como:
+                plt.savefig(salvar_como)
+            else:
+                plt.show()
+
+        except Exception as e:
+            return e
+
+    
+
+    def grafico_polar(angulos, valores, titulo=None, tamanho_d_figura=(8, 6), salvar_como=None):
+        try:
+            import matplotlib.pyplot as plt
+            plt.rcParams['toolbar'] = 'None'
+            plt.figure(figsize=tamanho_d_figura)
+            plt.polar(angulos, valores)
+
+            if titulo:
+                plt.title(titulo)
+
+            if salvar_como:
+                plt.savefig(salvar_como)
+            else:
+                plt.show()
+
+        except Exception as e:
+            return e
+
+
+
+
+
+#Classe de Equações    
+class Equacao:
+    
+    def equacaoPrimeiroGrauEx(a, b, c):
+        try:
+            if a == 0:
+                return "\033[2;12;31mA equação não é do primeiro grau.\033[m"
+            else:
+                x = (c - b) / a
+                sinal = '+' if b >= 0 else ''
+                expl = (
+                    f"{a}x {sinal}{b} = {c}\n"
+                    f"{b} vai trocar de lado e vai no lado do {c}\n"
+                    f"mais vai trocar de sinal\n"
+                    f"vai ficar {a}x = {c} - ({sinal}{b})\n"
+                    f"{a}x = {c-b}\n"
+                    f"x = {c-b}/{a}\n"
+                    f"x = {x}"
+                )
+                return f"\033[2;12;44m{a}x {sinal}{b} = {c}  (x: {x})\n--EXPLICAÇÃO--\n{expl}\033[m"
+        except Exception as e:
+            return str(e)
+
+
+    def equacaoSegundoGrauEx(a, b, c):
+        try:
+            import math
+
+            if a == 0:
+                return "\033[2;12;31mA equação não é do segundo grau.\033[m"
+
+            delta = b ** 2 - 4 * a * c
+
+            if delta < 0:
+                return "\033[2;12;31mA equação não possui raízes reais.\033[m"
+            elif delta == 0:
+                x = -b / (2 * a)
+                return f"A equação possui uma raiz real: x = {x}"
+            else:
+                sinal_b = '+' if b >= 0 else ''
+                sinal_c = '+' if c >= 0 else ''
+
+                x1 = (-b + math.sqrt(delta)) / (2 * a)
+                x2 = (-b - math.sqrt(delta)) / (2 * a)
+
+                exp = (
+                    f"delta = {b}² - 4 * {a} * {c}\n"
+                    f"\033[2;12;31mSe delta < 0, a equação não possui raízes reais\033[m\n"
+                    f"Senão, as raízes são:\n"
+                    f"x = {sinal_b}{b} / (2 * {a})\n"
+                    f"x1 = ({sinal_b}{b} + √{delta}) / (2 * {a})\n"
+                    f"x2 = ({sinal_b}{b} - √{delta}) / (2 * {a})\n"
+                    f"x1 = {x1}, x2 = {x2}"
+                )
+
+                return (
+                    f"\033[2;12;44mA equação {a}x² {sinal_b}{b}x {sinal_c}{c} = 0 possui duas raízes reais:\n"
+                    f"\033[2;12;44mx1 = {x1}, x2 = {x2}"
+                    f"\033[2;12;44m--EXPLICAÇÃO--\n{exp}\033[m"
+                )
+        except Exception as e:
+            return str(e)
+
+
+    def equacaoPrimeiroGrau(a, b, c):
+        try:
+            if a == 0:
+                return "A equação não é do primeiro grau."
+            else:
+                x = (c - b) / a
+                return x
+        except Exception as e:
+            return e
+
+    def equacaoSegundoGrau(a, b, c):
+        try:
+            if a == 0:
+                return "A equação não é do segundo grau."
+
+            delta = b ** 2 - 4 * a * c
+
+            if delta < 0:
+                return "A equação não possui raízes reais."
+            elif delta == 0:
+                x = -b / (2 * a)
+                return f"A equação possui uma raiz real: x = {x}"
+            else:
+                x1 = (-b + raiz_quadrada(delta)) / (2 * a)
+                x2 = (-b - raiz_quadrada(delta)) / (2 * a)
+                return f"A equação possui duas raízes reais: x1 = {x1}, x2 = {x2}"
+        except Exception as e:
+            return e
+    
+#Classes de Sistema Operacional
+class SO:
+    def diretorio_atual():
+        try:
+            import os
+            return f"(\033[2;12;34m{os.getcwd()}\033[m)"
+        except Exception as e:
+            return e
+
+    def lista_arq_dir(caminho):
+        try:
+            import os
+            return os.listdir(caminho)
+        except Exception as e:
+            return e
+
+    def criar_diretorio(novo_diretorio):
+        try:
+            import os
+            os.mkdir(novo_diretorio)
+        except Exception as e:
+            return e
+
+    def remover_arq(arquivo):
+        try:
+            import os
+            os.remove(arquivo)
+        except Exception as e:
+            return e
+
+    def remover_dir(diretorio):
+        try:
+            import os
+            os.rmdir(diretorio)
+        except Exception as e:
+            return e
+
+    def remover_dir_td(diretorio):
+        try:
+            import os
+            os.system(f'rm -rf{diretorio}')
+        except Exception as e:
+            return e
+        
+    def eh_arquivo(caminho):
+        try:
+            import os
+            if os.path.isfile(caminho):
+                return f"'{caminho}'\033[2;12;34mÉ um arquivo\033[m"
+            elif not os.path.isfile(caminho) and os.path.isdir(caminho):
+                return f"'{caminho}'\033[2;12;31mNão é um arquivo, é um diretório\033[m"
+            else:
+                return f"\033[2;12;31mArquivo '{caminho}' Inválido\033[m"
+        except Exception as e:
+            return e
+        
+    def eh_diretorio(caminho):
+        try:
+            import os
+            if os.path.isdir(caminho):
+                return f"'{caminho}'\033[2;12;34mÉ um diretorio\033[m"
+            elif not os.path.isdir(caminho)  and os.path.isfile(caminho):
+                return f"'{caminho}'\033[2;12;31mNão é um diretório, é um arquivo\033[m"
+            else:
+                return f"\033[2;12;31mDiretório '{caminho}' Inválido\033[m"
+        except Exception as e:
+            return e
+        
+
+    def versao_python():
+        try:
+            import sys
+            return f'\033[2;12;44mversão:{sys.version}\033[m'
+        except Exception as e:
+            return e
+
+    def sistema_operacional():
+        try:
+            import sys
+            return sys.platform
+        except Exception as e: return e
+        
+    def plataforma():
+        try:
+            import sys
+            pla = [s for s in sys.platform]
+            return f'plataforma: {pla}'
+        except Exception as e: return e
+
+    def mostrar_arq_dir(caminho):
+        try:
+            import os
+            if not os.path.exists(caminho):
+                return f"\033[2;12;31m{caminho} Não existe\033[m"
+            else:
+                os.system('dir')
+        except Exception as e:
+            return e
+
+    def existe_arq_dir(arquivo_ou_diretorio):
+        try:
+            import os
+            if os.path.exists(arquivo_ou_diretorio):
+                if os.path.isfile(arquivo_ou_diretorio):
+                    return "\033[2;12;34mEste Arquivo existe\033[m"
+                elif os.path.isdir(arquivo_ou_diretorio):
+                    return "\033[2;12;34mEste diretorio existe\033[m"
+                else:
+                    return "\033[2;12;31mNão existe\033[m"
+            else:
+                return "\033[2;12;31mCaminho Inválido\033[m"
+        except Exception as e:
+            return e
+        
+    def mover_arq_dir(nome_atual:str, caminho:str):
+        try:
+            import os
+            if os.path.exists(nome_atual) and os.path.exists(caminho):
+                os.rename(nome_atual, os.path.join(caminho, nome_atual))
+                return f"\033[2;12;34mO Arquivo '{nome_atual}' Foi movido pelo diretorio '{caminho}'\033[m"
+            elif not os.path.exists(nome_atual):
+                return f"\033[2;12;31m{nome_atual} Não existe\033[m"
+            elif not os.path.exists(caminho):
+                return f"\033[2;12;31m{caminho} Não existe\033[m"
+        except Exception as e:
+            return e
+
+    def mostra_arq_dire():
+         import platform, os
+         if platform.system() == "Windows":
+            os.system('dir')
+         else:
+            os.system('ls')
+
+        
+        
+
+   
+# Classe Trigonometria
+class Trigonometria:
+    # Função para calcular o seno de um ângulo em radianos
+    def seno(angle):
+        try:
+            import math
+            return math.sin(angle)
+        except Exception as e:
+            return e
+
+    # Função para calcular o cosseno de um ângulo em radianos
+    def cosseno(angle):
+        try:
+            import math
+            return math.cos(angle)
+        except Exception as e:
+            return e
+
+    # Função para calcular a tangente de um ângulo em radianos
+    def tangente(angle):
+        try:
+            import math
+            return math.tan(angle)
+        except Exception as e:
+            return e
+
+    # Função para calcular o cosseno hiperbólico de um número
+    def cosseno_hiperbolico(num):
+        try:
+            import math
+            return math.cosh(num)
+        except Exception as e:
+            return e
+
+    # Função para calcular o seno hiperbólico de um número
+    def seno_hiperbolico(num):
+        try:
+            import math
+            return math.sinh(num)
+        except Exception as e:
+            return e
+
+    # Função para calcular a tangente hiperbólica de um número
+    def tangente_hiperbolica(num):
+        try:
+            import math
+            return math.tanh(num)
+        except Exception as e:
+            return e
+
+    # Função para calcular o arco cosseno de um número
+    def arco_cosseno(num):
+        try:
+            import math
+            return math.acos(num)
+        except Exception as e:
+            return e
+
+    # Função para calcular o arco seno de um número
+    def arco_seno(num):
+        try:
+            import math
+            return math.asin(num)
+        except Exception as e:
+            return e
+
+    # Função para calcular o arco tangente de um número
+    def arco_tangente(num):
+        try:
+            import math
+            return math.atan(num)
+        except Exception as e:
+            return e
+
+    # Função para calcular o arco tangente de um número com dois argumentos (y, x)
+    def arco_tangente2(y, x):
+        try:
+            import math
+            return math.atan2(y, x)
+        except Exception as e:
+            return e
+
+#Classe de Estatistica
 class Estatistica:
     def media(*args):
         try:
             return sum(args) / len(args)
         except Exception as e:
             return e
 
@@ -742,16 +1345,23 @@
         mean_squared_deviations_within = squared_deviations_total / df_within
 
         f_statistic = mean_squared_deviations_between / mean_squared_deviations_within
         critical_value = f.ppf(1 - alpha, dfn=df_between, dfd=df_within)
 
         return f_statistic <= critical_value
 
+#Classe de Calculo
 class Calculo:
-   
+    def newton_raphson(funcao, derivada, x0, tolerancia=1e-6, max_iter=100):
+        x = x0
+        iteracoes = 0
+        while abs(funcao(x)) > tolerancia and iteracoes < max_iter:
+            x = x - funcao(x) / derivada(x)
+            iteracoes += 1
+        return x
 
     def derivada(expressao, variavel):
         from sympy import symbols, diff
         x = symbols(variavel)
         return diff(expressao, x)
 
 
@@ -878,16 +1488,14 @@
             if i % 2 == 0:
                 integral += 2 * expressao.subs(x, pontos[i])
             else:
                 integral += 4 * expressao.subs(x, pontos[i])
         integral += expressao.subs(x, limite_inferior) + expressao.subs(x, limite_superior)
         integral *= h / 3
         return integral
-
-
   
 
     def serie_taylor(expressao, variavel, ponto, ordem):
         from sympy import symbols, series
         x = symbols(variavel)
         return series(expressao, x, x0=ponto, n=ordem).removeO()
 
@@ -901,54 +1509,56 @@
 
   
 
     def inversa_transformada_laplace(expressao, variavel, t):
         from sympy import symbols, inverse_laplace_transform
         s = symbols(variavel)
         return inverse_laplace_transform(expressao, s, t)
+    
 
-class Matrix:
+#Classe de Matrize
+class Matrize:
     def __init__(self, data):
         self.data = data
         self.rows = len(data)
         self.cols = len(data[0])
 
     def __str__(self):
         return "\n".join([" ".join(map(str, row)) for row in self.data])
 
     def __add__(self, other):
         if self.rows != other.rows or self.cols != other.cols:
             raise ValueError("As matrizes devem ter o mesmo tamanho para soma.")
         
         result = [[self.data[i][j] + other.data[i][j] for j in range(self.cols)] for i in range(self.rows)]
-        return Matrix(result)
+        return Matrize(result)
     
     def __sub__(self, other):
         if self.rows != other.rows or self.cols != other.cols:
             raise ValueError("As matrizes devem ter o mesmo tamanho para subtração.")
         
         result = [[self.data[i][j] - other.data[i][j] for j in range(self.cols)] for i in range(self.rows)]
-        return Matrix(result)
+        return Matrize(result)
 
     def __mul__(self, other):
         if isinstance(other, (int, float)):
             result = [[self.data[i][j] * other for j in range(self.cols)] for i in range(self.rows)]
-        elif isinstance(other, Matrix):
+        elif isinstance(other, Matrize):
             if self.cols != other.rows:
                 raise ValueError("O número de colunas da primeira matriz deve ser igual ao número de linhas da segunda matriz para multiplicação.")
             
             result = [[sum(self.data[i][k] * other.data[k][j] for k in range(self.cols)) for j in range(other.cols)] for i in range(self.rows)]
         else:
             raise TypeError("Multiplicação não suportada entre matriz e outro tipo.")
         
-        return Matrix(result)
+        return Matrize(result)
 
     def transposta(self):
         result = [[self.data[j][i] for j in range(self.rows)] for i in range(self.cols)]
-        return Matrix(result)
+        return Matrize(result)
 
     def determinante(self):
         if self.rows != self.cols:
             raise ValueError("O determinante só pode ser calculado para matrizes quadradas.")
         
         return self._determinant_recursive(self.data)
 
@@ -971,34 +1581,33 @@
             mp.dps = 5
             result = mp.inverse(matriz)
             return result
         except Exception as e:
             return e
     
     
-
-def calcular_autovalores_autovetores(matriz):
-    try:
-        from mpmath import mp
-        # Converter a matriz para o formato mpmath
-        A = mp.matrix(matriz)
-        
-        # Calcular os autovalores e autovetores usando a função eig()
-        autovalores, autovetores = mp.eig(A)
-        
-        # Converter os resultados para listas para facilitar a manipulação
-        autovalores = [complex(val) for val in autovalores]
-        autovetores = [[complex(val) for val in vetor] for vetor in autovetores]
-        
-        return autovalores, autovetores
-    except Exception as e:
-        return e
-
+    def calcular_autovalores_autovetores(matriz):
+        try:
+            from mpmath import mp
+            # Converter a matriz para o formato mpmath
+            A = mp.matrix(matriz)
+            
+            # Calcular os autovalores e autovetores usando a função eig()
+            autovalores, autovetores = mp.eig(A)
+            
+            # Converter os resultados para listas para facilitar a manipulação
+            autovalores = [complex(val) for val in autovalores]
+            autovetores = [[complex(val) for val in vetor] for vetor in autovetores]
+            
+            return autovalores, autovetores
+        except Exception as e:
+            return e
 
 
+#Classe de AlgebraLinear
 class AlgebraLinear:
     # Função para multiplicar uma matriz por um escalar
     @staticmethod
     def multiplicar_matriz_por_escalar(matriz, escalar):
         resultado = []
         for linha in matriz:
             nova_linha = [elemento * escalar for elemento in linha]
@@ -1483,15 +2092,15 @@
             import networkx as nx
             G = nx.Graph(grafo)
             return nx.is_connected(G)
         except Exception as e:
             return e
 
             
-
+#Classe de Geometria
 class Geometria:
   
     # Distância entre dois pontos no plano 2D
     def distancia_pontos_2D(x1, y1, x2, y2):
         import math
         return math.sqrt((x2 - x1)**2 + (y2 - y1)**2)
 
@@ -1966,15 +2575,15 @@
                 a = v + f - 2
 
             return f"Vertices:{v}, Faces:{f}, Arestas:{a}"
         except Exception as e:
             return e
 
 
-
+#Classe de Criptografia
 class Criptografia:
     # Cifra de César (criptografar)
     def cifra_cesar_encrypt( texto, chave):
         try:
             texto_cifrado = ""
             for char in texto:
                 if char.isalpha():
@@ -2111,15 +2720,15 @@
             num_colunas = len(texto_cifrado) // tamanho_chave
             colunas = [texto_cifrado[i : i + num_colunas] for i in range(0, len(texto_cifrado), num_colunas)]
             texto_decifrado = "".join(colunas[chave.index(letra)] for letra in sorted(chave))
             return texto_decifrado
         except Exception as e:
             return e
 
-
+#Classe de Analise Combinatória
 class Analise_Combinatoria:
     
 
     # Arranjo simples (Permutação)
     def arranjo(n, k):
         import math
         return math.factorial(n) // math.factorial(n - k)
@@ -2424,17 +3033,16 @@
                 if j >= i:
                     partitions[i][j] = partitions[i - 1][j] + partitions[i][j - i]
                 else:
                     partitions[i][j] = partitions[i - 1][j]
 
         return partitions[n][m]
 
-# Testando as funções de análise combinatór
-
 
+#Classe de Probabilidade
 class Probabilidade:
     # Probabilidade de um evento simples
     @staticmethod
     def probabilidade_evento_simples(evento_favoravel, espaco_amostral):
         return evento_favoravel / espaco_amostral
 
     # Probabilidade complementar
```

### Comparing `anybomt-0.2.3/setup.py` & `anybomt-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # Leitura do arquivo README.md
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 # Configuração do pacote
 setup(
     name='anybomt',
-    version='0.2.3',
+    version='0.3.0',
     license='MIT',
-    author='AnyBoMath',
+    author=['AnyBoMath', 'Bidjory'],
     author_email='bidjorys@gmail.com',
     description='Uma biblioteca para facilitar sua jornada em matemática',
     long_description=long_description,
     long_description_content_type='text/markdown',
   # Substitua com o link do seu repositório no GitHub
     packages=[''],  # Lista de pacotes que serão incluídos
     classifiers=[
@@ -22,12 +22,14 @@
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'scipy',
         'numpy',
         'sympy',
         'mpmath',
+        'matplotlib',
         
         # outras dependências da sua biblioteca
     ],
     python_requires='>=3.6',
+    
 )
```

