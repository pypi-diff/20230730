# Comparing `tmp/mathslib-3.0.0.tar.gz` & `tmp/mathslib-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathslib-3.0.0.tar", last modified: Sat Jun 10 05:31:22 2023, max compression
+gzip compressed data, was "mathslib-3.1.0.tar", last modified: Sun Jul 30 09:28:18 2023, max compression
```

## Comparing `mathslib-3.0.0.tar` & `mathslib-3.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 05:31:22.756217 mathslib-3.0.0/
--rw-rw-rw-   0        0        0     1211 2022-05-22 14:55:29.000000 mathslib-3.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     7058 2023-06-10 05:31:22.759302 mathslib-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6133 2023-06-10 05:18:50.000000 mathslib-3.0.0/README.rst
--rw-rw-rw-   0        0        0       85 2022-05-22 15:02:53.000000 mathslib-3.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-06-10 05:31:22.767650 mathslib-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1560 2023-06-10 04:10:31.000000 mathslib-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 05:31:22.689290 mathslib-3.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-10 05:31:22.734510 mathslib-3.0.0/src/mathslib/
--rw-rw-rw-   0        0        0     1543 2022-06-10 07:50:59.000000 mathslib-3.0.0/src/mathslib/__init__.py
--rw-rw-rw-   0        0        0    15906 2023-05-14 09:39:13.000000 mathslib-3.0.0/src/mathslib/algorithms.py
--rw-rw-rw-   0        0        0     5092 2023-06-10 05:27:26.000000 mathslib-3.0.0/src/mathslib/divisors.py
--rw-rw-rw-   0        0        0     3314 2023-05-14 09:50:54.000000 mathslib-3.0.0/src/mathslib/fib.py
--rw-rw-rw-   0        0        0     9961 2023-05-14 09:49:26.000000 mathslib-3.0.0/src/mathslib/linalg.py
--rw-rw-rw-   0        0        0    19783 2023-06-10 04:09:38.000000 mathslib-3.0.0/src/mathslib/numtheory.py
--rw-rw-rw-   0        0        0    14540 2023-06-10 04:36:27.000000 mathslib-3.0.0/src/mathslib/primes.py
--rw-rw-rw-   0        0        0     5272 2023-05-14 09:45:48.000000 mathslib-3.0.0/src/mathslib/simple.py
-drwxrwxrwx   0        0        0        0 2023-06-10 05:31:22.756217 mathslib-3.0.0/src/mathslib.egg-info/
--rw-rw-rw-   0        0        0     7058 2023-06-10 05:31:22.000000 mathslib-3.0.0/src/mathslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-06-10 05:31:22.000000 mathslib-3.0.0/src/mathslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 05:31:22.000000 mathslib-3.0.0/src/mathslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-10 05:31:22.000000 mathslib-3.0.0/src/mathslib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-10 05:31:22.000000 mathslib-3.0.0/src/mathslib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 09:28:18.671820 mathslib-3.1.0/
+-rw-rw-rw-   0        0        0     1211 2022-05-22 14:55:29.000000 mathslib-3.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     7220 2023-07-30 09:28:18.671820 mathslib-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6293 2023-07-30 09:13:30.000000 mathslib-3.1.0/README.rst
+-rw-rw-rw-   0        0        0       85 2022-05-22 15:02:53.000000 mathslib-3.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-07-30 09:28:18.671820 mathslib-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1560 2023-07-05 08:18:30.000000 mathslib-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 09:28:18.593278 mathslib-3.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-30 09:28:18.656193 mathslib-3.1.0/src/mathslib/
+-rw-rw-rw-   0        0        0     1543 2022-06-10 07:50:59.000000 mathslib-3.1.0/src/mathslib/__init__.py
+-rw-rw-rw-   0        0        0    15906 2023-05-14 09:39:13.000000 mathslib-3.1.0/src/mathslib/algorithms.py
+-rw-rw-rw-   0        0        0     5123 2023-06-10 05:37:16.000000 mathslib-3.1.0/src/mathslib/divisors.py
+-rw-rw-rw-   0        0        0     3791 2023-07-05 08:16:40.000000 mathslib-3.1.0/src/mathslib/fib.py
+-rw-rw-rw-   0        0        0    10774 2023-06-18 10:38:06.000000 mathslib-3.1.0/src/mathslib/linalg.py
+-rw-rw-rw-   0        0        0    21591 2023-07-30 09:16:32.000000 mathslib-3.1.0/src/mathslib/numtheory.py
+-rw-rw-rw-   0        0        0    14540 2023-06-10 04:36:27.000000 mathslib-3.1.0/src/mathslib/primes.py
+-rw-rw-rw-   0        0        0     6269 2023-06-18 12:55:40.000000 mathslib-3.1.0/src/mathslib/simple.py
+drwxrwxrwx   0        0        0        0 2023-07-30 09:28:18.671820 mathslib-3.1.0/src/mathslib.egg-info/
+-rw-rw-rw-   0        0        0     7220 2023-07-30 09:28:18.000000 mathslib-3.1.0/src/mathslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-07-30 09:28:18.000000 mathslib-3.1.0/src/mathslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 09:28:18.000000 mathslib-3.1.0/src/mathslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-30 09:28:18.000000 mathslib-3.1.0/src/mathslib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-30 09:28:18.000000 mathslib-3.1.0/src/mathslib.egg-info/top_level.txt
```

### Comparing `mathslib-3.0.0/LICENSE.txt` & `mathslib-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mathslib-3.0.0/PKG-INFO` & `mathslib-3.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathslib
-Version: 3.0.0
+Version: 3.1.0
 Summary: Library of Mathematical functions and Algorithms
 Home-page: https://github.com/igorvanloo/mathslib
 Author: Igor van Loo
 Author-email: igorvanloo@gmail.com
 Project-URL: Bug Reports, https://github.com/igorvanloo/mathslib/issues
 Project-URL: Source, https://github.com/igorvanloo/mathslib
 Keywords: numbertheory,maths,algorithms
@@ -44,15 +44,16 @@
 +----------------+------------------------------------------------------------+
 |numtheory.py    | * phi(x)                                                   |
 |                | * phi_sieve(x)                                             |
 |                | * phi_sum(x)                                               |
 |                | * mobius(x)                                                |
 |                | * mobius_k_sieve(limit, k)                                 |
 |                | * count_k_free(n, k)                                       |
-|                | * ppt(limit, non_primitive)                                |
+|                | * pythagorean_triples(limit, non_primitive)                |
+|                | * count_primitive_pythagorean_triples(n)                   |
 |                | * k_smooth_numbers(max_prime, limit)                       |
 |                | * k_powerful(k, limit, count)                              |
 |                | * legendre_factorial(x)                                    |
 |                | * tonelli_shanks(a, p)                                     |
 |                | * chinese_remainder_theorem(a1, a2, n1, n2)                |
 |                | * generalised_CRT(a1, a2, n1, n2)                          |
 |                | * frobenius_number(\*integers)                             |
@@ -79,30 +80,31 @@
 |                | * determinant(matrix)                                      |
 |                | * matrix_addition(A, B, subtract)                          |
 |                | * identity(l, val)                                         |
 |                | * concatenate(A, B)                                        |
 |                | * argmax(alist)                                            |
 |                | * fillmatrix(size, val)                                    |
 |                | * matrix_mul(A, B)                                         |
+|                | * matrix_pow(A, n)                                         |
 +----------------+------------------------------------------------------------+
-|fib.py          | * fibonacci(n)                                             |
+|fib.py          | * fibonacci(n, m)                                          |
 |                | * fib_till(limit)                                          |
 |                | * zeckendorf_representation(x)                             |
 +----------------+------------------------------------------------------------+
 |algorithms.py   | * prims_algorithm(matrix)                                  |
 |                | * dijkstras_algorithm(graph, start_node, INFINITY)         |
 |                | * floyd_warshall_algorithm(graph, INFINITY)                |
 |                | * knap_sack(values, weights, n, W, no_values)              |
 |                | * knap_sack_values(values, weights, n, W, no_values)       |
 |                | * BFS(g, start_node, end_node)                             |
 |                | * DFS(g, start_node, end_node)                             |
 |                | * convex_hull_gift_wrapping(pts)                           |
 |                | * convex_hull_DC(pts)                                      |
 +----------------+------------------------------------------------------------+
-|simple.py       | * n_choose_r(n, r)                                         | 
+|simple.py       | * bin_exp(a, b, c, n, m)                                   | 
 |                | * number_to_base(n, b)                                     |
 |                | * extended_euclidean_algorithm(n, b)                       |
 |                | * lcm(a_list)                                              |
 |                | * mod_division(a, b, m)                                    |
 |                | * bisect(alist, goal)                                      |
 |                | * is_clockwise(a, b, c)                                    |
 +----------------+------------------------------------------------------------+
```

### Comparing `mathslib-3.0.0/README.rst` & `mathslib-3.1.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 +----------------+------------------------------------------------------------+
 |numtheory.py    | * phi(x)                                                   |
 |                | * phi_sieve(x)                                             |
 |                | * phi_sum(x)                                               |
 |                | * mobius(x)                                                |
 |                | * mobius_k_sieve(limit, k)                                 |
 |                | * count_k_free(n, k)                                       |
-|                | * ppt(limit, non_primitive)                                |
+|                | * pythagorean_triples(limit, non_primitive)                |
+|                | * count_primitive_pythagorean_triples(n)                   |
 |                | * k_smooth_numbers(max_prime, limit)                       |
 |                | * k_powerful(k, limit, count)                              |
 |                | * legendre_factorial(x)                                    |
 |                | * tonelli_shanks(a, p)                                     |
 |                | * chinese_remainder_theorem(a1, a2, n1, n2)                |
 |                | * generalised_CRT(a1, a2, n1, n2)                          |
 |                | * frobenius_number(\*integers)                             |
@@ -58,30 +59,31 @@
 |                | * determinant(matrix)                                      |
 |                | * matrix_addition(A, B, subtract)                          |
 |                | * identity(l, val)                                         |
 |                | * concatenate(A, B)                                        |
 |                | * argmax(alist)                                            |
 |                | * fillmatrix(size, val)                                    |
 |                | * matrix_mul(A, B)                                         |
+|                | * matrix_pow(A, n)                                         |
 +----------------+------------------------------------------------------------+
-|fib.py          | * fibonacci(n)                                             |
+|fib.py          | * fibonacci(n, m)                                          |
 |                | * fib_till(limit)                                          |
 |                | * zeckendorf_representation(x)                             |
 +----------------+------------------------------------------------------------+
 |algorithms.py   | * prims_algorithm(matrix)                                  |
 |                | * dijkstras_algorithm(graph, start_node, INFINITY)         |
 |                | * floyd_warshall_algorithm(graph, INFINITY)                |
 |                | * knap_sack(values, weights, n, W, no_values)              |
 |                | * knap_sack_values(values, weights, n, W, no_values)       |
 |                | * BFS(g, start_node, end_node)                             |
 |                | * DFS(g, start_node, end_node)                             |
 |                | * convex_hull_gift_wrapping(pts)                           |
 |                | * convex_hull_DC(pts)                                      |
 +----------------+------------------------------------------------------------+
-|simple.py       | * n_choose_r(n, r)                                         | 
+|simple.py       | * bin_exp(a, b, c, n, m)                                   | 
 |                | * number_to_base(n, b)                                     |
 |                | * extended_euclidean_algorithm(n, b)                       |
 |                | * lcm(a_list)                                              |
 |                | * mod_division(a, b, m)                                    |
 |                | * bisect(alist, goal)                                      |
 |                | * is_clockwise(a, b, c)                                    |
 +----------------+------------------------------------------------------------+
```

### Comparing `mathslib-3.0.0/setup.py` & `mathslib-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (here / "README.rst").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name = "mathslib",  # Required
-    version="3.0.0",  # Required
+    version="3.1.0",  # Required
     description="Library of Mathematical functions and Algorithms",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/x-rst",  # Optional
     url="https://github.com/igorvanloo/mathslib",  # Optional
     author="Igor van Loo",  # Optional
     author_email="igorvanloo@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `mathslib-3.0.0/src/mathslib/__init__.py` & `mathslib-3.1.0/src/mathslib/__init__.py`

 * *Files identical despite different names*

### Comparing `mathslib-3.0.0/src/mathslib/algorithms.py` & `mathslib-3.1.0/src/mathslib/algorithms.py`

 * *Files identical despite different names*

### Comparing `mathslib-3.0.0/src/mathslib/divisors.py` & `mathslib-3.1.0/src/mathslib/divisors.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     Implementation of `Divisor function 
     <https://en.wikipedia.org/wiki/Divisor_function#Definition>`_ sigma(x, n) sieve. 
     It returns an array such that array[x] = sigma(x, n)
     
     :param x: An integer
     :param n: An integer, denotes the length of the array
     
-    :returns: An integer
+    :returns: An array such that array[x] = sigma(x, n)
     
     .. code-block:: python
     
         print(divisors_sieve(0, 10)) #[0, 1, 2, 2, 3, 2, 4, 2, 4, 3, 4]
         print(divisors_sieve(1, 10)) #[0, 1, 3, 4, 7, 6, 12, 8, 15, 13, 18]
         print(divisors_sieve(2, 10)) #[0, 1, 5, 10, 21, 26, 50, 50, 85, 91, 130]
```

### Comparing `mathslib-3.0.0/src/mathslib/fib.py` & `mathslib-3.1.0/src/mathslib/fib.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,36 +24,51 @@
 # For more information, please refer to <https://unlicense.org>
 '''
 Fibonacci related functions
 
 Author: Igor van Loo
 '''
 
-def fibonacci(n):
+def fibonacci(n, m = None):
     '''
-    Finds the n-th Fibonacci using matrix exponentiation
-    Method is outlined `here <https://stackoverflow.com/questions/18172257/efficient-calculation-of-fibonacci-series/23462371#23462371>`__
+    Finds the n-th Fibonacci using matrix exponentiation by squaring
+    Method is outlined `here <http://homepages.math.uic.edu/~leon/cs-mcs401-s08/handouts/fastexp.pdf>`__
+    Specifically, this is an implementation of the third algorithm.
+    
+    Also includes an option to calculate with a given modulus
 
     :param n: An integer
+    :param m: An integer, default is None, if specificed will find F(n) (mod m)
 
-    :returns: The n-th Fibonacci number
+    :returns: The n-th Fibonacci number (modulus m if specified)
     
     .. code-block:: python
     
         print(fibonacci(100)) #354224848179261915075
+        print(fibonacci(100, 10**7 + 9)) #5475613
+        
     '''
     if type(n) != int:
         return "n must be an integer"
-    v1, v2, v3 = 1, 1, 0    # initialise a matrix [[1,1],[1,0]]
-    for rec in bin(n)[3:]:  # perform fast exponentiation of the matrix (quickly raise it to the nth power)
-        calc = v2*v2
-        v1, v2, v3 = v1*v1+calc, (v1+v3)*v2, calc+v3*v3
-        if rec=='1':
-            v1, v2, v3 = v1+v2, v1, v2  
-    return v2
+    
+    if m != None:
+        f2, f1, f0 = 1, 1, 0
+        for bit in bin(n)[3:]:
+            v = (f1*f1) % m
+            f2, f1, f0 = (f2 * f2 + v) % m, ((f2 + f0) * f1) % m, (v + f0 * f0) % m
+            if bit == '1':
+                f2, f1, f0 = f2 + f1, f2, f1 
+    else:
+        f2, f1, f0 = 1, 1, 0
+        for bit in bin(n)[3:]:
+            v = f1*f1
+            f2, f1, f0 = f2 * f2 + v, (f2 + f0) * f1, v + f0 * f0
+            if bit == '1':
+                f2, f1, f0 = f2 + f1, f2, f1   
+    return f1
 
 def fib_till(limit):
     '''
     Finds all Fibonacci number up till a limit
 
     :param limit: An integer
```

### Comparing `mathslib-3.0.0/src/mathslib/linalg.py` & `mathslib-3.1.0/src/mathslib/linalg.py`

 * *Files 6% similar despite different names*

```diff
@@ -344,7 +344,35 @@
     matrix = fillmatrix((m1, n2))
     for row in range(m1): 
         for col in range(n2):
             for elt in range(len(B)):
               matrix[row][col] += A[row][elt] * B[elt][col]
     return matrix
 
+def matrix_pow(A, n):
+    '''
+    Matrix exponentiation. Uses the `Exponentiation by squaring <https://en.wikipedia.org/wiki/Exponentiation_by_squaring>`_ method 
+
+    :param A: Matrix
+    :param n: exponenent
+
+    :returns: Matrix A^n
+    
+    .. code-block:: python
+    
+        A = [[1, 1], 
+             [1, 0]]
+        print(matrix_pow(A, 10)) #[[89, 55], [55, 34]]
+        
+    .. note::
+        
+        Seem familiar? These are fibonacci numbers! 
+        This is nearly identical to my fibonacci generation function as it uses the same method, 
+        however the fibonacci is slightly more optimized due to it's properties
+        
+    '''
+    A_res = A
+    for bit in bin(n)[3:]:
+        A_res = matrix_mul(A_res, A_res)
+        if bit == "1":
+            A_res = matrix_mul(A_res, A)
+    return A_res
```

### Comparing `mathslib-3.0.0/src/mathslib/numtheory.py` & `mathslib-3.1.0/src/mathslib/numtheory.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,28 +175,29 @@
         d = d + 1
         if d*d > n:
             if n > 1: 
                 num_of_primes += 1
             break
     return pow(-1, num_of_primes)
 
-def mobius_k_sieve(limit, k):
+def mobius_k_sieve(limit, k = 2):
     '''
     A sieve for the Generalized `Mobius function
     <https://en.wikipedia.org/wiki/M%C3%B6bius_function>`_, the mathematics of this function can be read
     in the following `PDF <https://projecteuclid.org/journals/pacific-journal-of-mathematics/volume-32/issue-1/M%C3%B6bius-functions-of-order-k/pjm/1102977519.pdf>`_
-
+    Note that when k = 2 we get the normal mobius function shown above.
+    
     :param limit: An integer
-    :param k: An integer
+    :param k: Optional integer, default value is 2 which gives a regular mobius sieve
 
     :returns: An array where array[x] = μ(k, x)
     
     .. code-block:: python
     
-        print(mobius_k_sieve(10, 2)) #[0, 1, -1, -1, 0, -1, 1, -1, 0, 0, 1]
+        print(mobius_k_sieve(10)) #[0, 1, -1, -1, 0, -1, 1, -1, 0, 0, 1]
         print(mobius_k_sieve(10, 3)) #[0, 1, -1, -1, -1, -1, 1, -1, 0, -1, 1]
     
     '''
     isprime = [1]*(limit + 1)
     isprime[0] = isprime[1] = 0
     mob = [0] + [1]*(limit)
     for p in range(2, limit + 1):
@@ -226,52 +227,103 @@
     
     .. code-block:: python
     
         print(count_k_free(2**50, 2)) #684465067343069
         
     '''
     sq = math.floor(n**(1/k))
-    mobius_k = mobius_k_sieve(sq, 2)
+    mobius_k = mobius_k_sieve(sq)
     return sum([mobius_k[i]*(n//pow(i, k)) for i in range(1, sq + 1)])
 
-def pythagoren_triples(limit, non_primitive = True):
+def pythagorean_triples(limit, non_primitive = True):
     '''
     Generates all `Pythagorean Triplets 
     <https://en.wikipedia.org/wiki/Pythagorean_triple>`_ up to the limit
 
     :param limit: An integer, will generate all Pythagorean Triplets such that no side is longer than the limit
     :param non_primitive: Optional boolean value, If True, returns all triplets, if False returns only primitive triplets
 
     :returns: A list containing all desired triplets
     
     .. code-block:: python
         
-        print(ppt(20)) #[[3, 4, 5], [6, 8, 10], [9, 12, 15], [12, 16, 20], [5, 12, 13], [15, 8, 17]]
-        print(ppt(20, False)) #[[3, 4, 5], [5, 12, 13], [15, 8, 17]]
-        print(len(ppt(100, False))) #16
+        print(pythagorean_triples(20)) #[[3, 4, 5], [6, 8, 10], [9, 12, 15], [12, 16, 20], [5, 12, 13], [15, 8, 17]]
+        print(pythagorean_triples(20, False)) #[[3, 4, 5], [5, 12, 13], [15, 8, 17]]
+        print(len(pythagorean_triples(100, False))) #16
     
     '''
     if (type(limit) != int):
         return "All values must be integers"
     triples = []
     for m in range(2,int(math.sqrt(limit))+1):
-        for n in range(1,m):
-            if (m+n) % 2 == 1 and math.gcd(m,n) == 1:
+        for n in range(1 + m % 2, m, 2):
+            if math.gcd(m,n) == 1:
                 a = m**2 + n**2
                 b = m**2 - n**2
                 c = 2*m*n
-                p = max(a,b,c)
-                if p < limit:
+                if a < limit:
                     if non_primitive:
-                        for k in range(1,int(limit/p)+1):
+                        for k in range(1,int(limit/a)+1):
                             triples.append([k*b,k*c,k*a])
                     else:
                         triples.append([b,c,a])
     return triples
 
+def count_primitive_pythagorean_triples(n):
+    '''
+    Function counts the number of primitive `Pythagorean Triplets 
+    <https://en.wikipedia.org/wiki/Pythagorean_triple>`_ with hypotenuse less than n.
+    Algorithm is adapted from the following paper `Pythagorean triangles with legs less than n <https://www.sciencedirect.com/science/article/pii/S0377042701004964#aep-abstract-id6>`_
+
+    :param n: An integer
+
+    :returns: Number of primitive Pythagorean triplets with hypotenuse less than n
+    
+    .. code-block:: python
+        
+        print(count_primitive_pythagorean_triples(10**10)) #1591549475
+        print(count_primitive_pythagorean_triples(10**8)) #15915493
+        
+    .. note::
+        Due to some precision errors the answer can somtimes be a few numbers off for example the correct answer
+        for n = 10^8 is actually 15915492, one less than what my function gives.
+    
+    '''
+    if (type(n) != int):
+        return "All values must be integers"
+    mu = mobius_k_sieve(int(math.sqrt(n)) + 1)
+    
+    R_cache = {}
+    def R(n):
+        if n in R_cache:
+            return R_cache[n]
+        c = 0 
+        for x in range(int(math.sqrt(n)) + 1):
+            min_y, max_y = x + 1, int(math.sqrt(n - x*x))
+            if max_y < min_y:
+                break
+            c += max_y - min_y + 1
+        R_cache[n] = c
+        return c
+    
+    def Q(n):
+        total = 0
+        m = math.sqrt(n)
+        for d in range(1, int(m) + 1):
+            total += mu[d] * R(n // (d*d))
+        return total
+    
+    c = 0
+    k = 0
+    while 2**k <= n:
+        x = Q(n // pow(2, k))
+        c += pow(-1, k) * x
+        k += 1
+    return c
+
 def legendre_factorial(x):
     '''
     Implementation of `Legendres' Formula
     <https://en.wikipedia.org/wiki/Legendre%27s_formula>`_
 
     :param x: An integer
```

### Comparing `mathslib-3.0.0/src/mathslib/primes.py` & `mathslib-3.1.0/src/mathslib/primes.py`

 * *Files identical despite different names*

### Comparing `mathslib-3.0.0/src/mathslib/simple.py` & `mathslib-3.1.0/src/mathslib/simple.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,34 +27,51 @@
 '''
 Various simple functions
 
 Author: Igor van Loo
 '''
 import math
 
-def n_choose_r(n, r):
+def bin_exp(a, b, c, n, m = None):
     '''
-    n choose r function
+    If (a + b√(c))^n (mod m) = x + y√(c), then this function finds x, y by using binary exponentiation.
 
-    :param n: An integer
-    :param r: An integer
+    :param a: An integer, coefficient of nonsqrt term
+    :param b: An integer, coefficient of sqrt
+    :param c: An integer, inside the sqrt
+    :param n: An integer, exponent
+    :param m: An integer, the modulus
 
-    :returns: n choose r
-    
+    :returns: x, y such that (a + b√(c))^n (mod m) = x + y√(c)
+        
     .. code-block:: python
-    
-        print(n_choose_r(50, 30)) #47129212243960
+        #Using fibonacci relation to golden ratio we know
+        #(((1 + sqrt(5))/2)^n - ((1 + sqrt(5))/2)^n)/sqrt(5) = F(n)
+        
+        x = bin_exp(1/2, 1/2, 5, 10)  #x = (61.5, 27.5) represents 61.5 + 27.5*sqrt(5)
+        y = bin_exp(1/2, -1/2, 5, 10) #y = (61.5, -27.5) represents 61.5 - 27.5*sqrt(5)
+        
+        #Therefore, F(10) = (61.5 + 27.5*sqrt(5) - (61.5 - 27.5*sqrt(5)))/sqrt(5)) = 55
+        
+        print(x[1] - y[1]) #55.0
         
     '''
-    if (type(n) != int) or (type(r) != int):
-        return "n and r must be an integers"
-    if r > n:
-        return "n must be greter than r"
+    if m == None:
+        a_res, b_res = a, b
+        for bit in bin(n)[3:]:
+            a_res, b_res = (a_res*a_res + c*b_res*b_res), 2*a_res*b_res
+            if bit == "1":
+                a_res, b_res = (a*a_res + b*c*b_res), (b*a_res + a*b_res)
     else:
-        return int(math.factorial(n) / (math.factorial(r) * math.factorial(n-r)))
+        a_res, b_res = a, b
+        for bit in bin(n)[3:]:
+            a_res, b_res = (a_res*a_res + c*b_res*b_res) % m, 2*a_res*b_res % m
+            if bit == "1":
+                a_res, b_res = (a*a_res + b*c*b_res) % m, (b*a_res + a*b_res) % m
+    return a_res, b_res
     
 def number_to_base(n, b):
     '''
     Changes n from base 10 to base b
 
     :param n: An integer, number to be changed
     :param b: An integer, base in question
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mathslib-3.0.0/src/mathslib.egg-info/PKG-INFO` & `mathslib-3.1.0/src/mathslib.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathslib
-Version: 3.0.0
+Version: 3.1.0
 Summary: Library of Mathematical functions and Algorithms
 Home-page: https://github.com/igorvanloo/mathslib
 Author: Igor van Loo
 Author-email: igorvanloo@gmail.com
 Project-URL: Bug Reports, https://github.com/igorvanloo/mathslib/issues
 Project-URL: Source, https://github.com/igorvanloo/mathslib
 Keywords: numbertheory,maths,algorithms
@@ -44,15 +44,16 @@
 +----------------+------------------------------------------------------------+
 |numtheory.py    | * phi(x)                                                   |
 |                | * phi_sieve(x)                                             |
 |                | * phi_sum(x)                                               |
 |                | * mobius(x)                                                |
 |                | * mobius_k_sieve(limit, k)                                 |
 |                | * count_k_free(n, k)                                       |
-|                | * ppt(limit, non_primitive)                                |
+|                | * pythagorean_triples(limit, non_primitive)                |
+|                | * count_primitive_pythagorean_triples(n)                   |
 |                | * k_smooth_numbers(max_prime, limit)                       |
 |                | * k_powerful(k, limit, count)                              |
 |                | * legendre_factorial(x)                                    |
 |                | * tonelli_shanks(a, p)                                     |
 |                | * chinese_remainder_theorem(a1, a2, n1, n2)                |
 |                | * generalised_CRT(a1, a2, n1, n2)                          |
 |                | * frobenius_number(\*integers)                             |
@@ -79,30 +80,31 @@
 |                | * determinant(matrix)                                      |
 |                | * matrix_addition(A, B, subtract)                          |
 |                | * identity(l, val)                                         |
 |                | * concatenate(A, B)                                        |
 |                | * argmax(alist)                                            |
 |                | * fillmatrix(size, val)                                    |
 |                | * matrix_mul(A, B)                                         |
+|                | * matrix_pow(A, n)                                         |
 +----------------+------------------------------------------------------------+
-|fib.py          | * fibonacci(n)                                             |
+|fib.py          | * fibonacci(n, m)                                          |
 |                | * fib_till(limit)                                          |
 |                | * zeckendorf_representation(x)                             |
 +----------------+------------------------------------------------------------+
 |algorithms.py   | * prims_algorithm(matrix)                                  |
 |                | * dijkstras_algorithm(graph, start_node, INFINITY)         |
 |                | * floyd_warshall_algorithm(graph, INFINITY)                |
 |                | * knap_sack(values, weights, n, W, no_values)              |
 |                | * knap_sack_values(values, weights, n, W, no_values)       |
 |                | * BFS(g, start_node, end_node)                             |
 |                | * DFS(g, start_node, end_node)                             |
 |                | * convex_hull_gift_wrapping(pts)                           |
 |                | * convex_hull_DC(pts)                                      |
 +----------------+------------------------------------------------------------+
-|simple.py       | * n_choose_r(n, r)                                         | 
+|simple.py       | * bin_exp(a, b, c, n, m)                                   | 
 |                | * number_to_base(n, b)                                     |
 |                | * extended_euclidean_algorithm(n, b)                       |
 |                | * lcm(a_list)                                              |
 |                | * mod_division(a, b, m)                                    |
 |                | * bisect(alist, goal)                                      |
 |                | * is_clockwise(a, b, c)                                    |
 +----------------+------------------------------------------------------------+
```

