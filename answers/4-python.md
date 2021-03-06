<div align='center'>
  <h1>π Python Programming Language π</h1>
</div>

> μ§λ¬Έμ <strong>[Top 100 Python Interview Questions You Must Prepare In 2021 - edureka!](https://www.edureka.co/blog/interview-questions/python-interview-questions/)</strong>μ μ°Έκ³ νμμΌλ©°, μ§λ¬Έμ λν λ΅λ³ μ€ μΌλΆλ μμ μ¬μ΄νΈμ λ΅λ³μ μ°Έκ³ νμ¬ μμ±λμμ΅λλ€.

## Table of Contents

- [What is the difference between list and tuples in Python?](#1)
- [What are the key features of Python?](#2)
- [What type of language is python? Programming or scripting?](#3)
- [Python an interpreted language. Explain.](#4)
- [What is pep 8?](#5)
- [How is memory managed in Python?](#6)
- [What is namespace in Python?](#7)
- [What is PYTHONPATH?](#8)
- [What are python modules? Name some commonly used built-in modules in Python?](#9)
- [What are local variables and global variables in Python?](#10)
- [Is python case sensitive?](#11)
- [What is type conversion in Python?](#12)
- [How to install Python on Windows and set path variable?](#13)
- [Is indentation required in python?](#14)
- [What is the difference between Python Arrays and lists?](#15)
- [What are functions in Python?](#16)
- [What is `__init__`?](#17)
- [What is a lambda function?](#18)
- [What is self in Python?](#19)
- [How does break, continue and pass work?](#20)
- [What does `[::-1]` do?](#21)
- [How can you randomize the items of a list in place in Python?](#22)
- [Whatβs the difference between iterator and iterable?](#23)
- [How can you generate random numbers in Python?](#24)
- [What is the difference between range & xrange?](#25)
- [How do you write comments in python?](#26)
- [What is pickling and unpickling?](#27)
- [What are the generators in python?](#28)
- [How will you capitalize the first letter of string?](#29)
- [How will you convert a string to all lowercase?](#30)
- [How to comment multiple lines in python?](#31)
- [What are docstrings in Python?](#32)
- [What is the purpose of is, not and in operators?](#33)
- [What is the usage of help() and dir() function in Python?](#34)
- [Whenever Python exits, why isnβt all the memory de-allocated?](#35)
- [What is a dictionary in Python?](#36)
- [How can the ternary operators be used in python?](#37)
- [What does this mean: `*args`, `**kwargs`? And why would we use it?](#38)
- [What does len() do?](#39)
- [Explain split(), sub(), subn() methods of βreβ module in Python.](#40)
- [What are negative indexes and why are they used?](#41)
- [What are Python packages?](#42)
- [How can files be deleted in Python?](#43)
- [What are the built-in types of python?](#44)
- [What advantages do NumPy arrays offer over (nested) Python lists?](#45)
- [How to add values to a python array?](#46)
- [How to remove values to a python array?](#47)
- [Does Python have OOps concepts?](#48)
- [What is the difference between deep and shallow copy?](#49)
- [How is Multithreading achieved in Python?](#50)
- [What is the process of compilation and linking in python?](#51)
- [What are Python libraries? Name a few of them.](#52)
- [What is split used for?](#53)
- [How to import modules in python?](#54)
- [Explain Inheritance in Python.](#55)
- [How are classes created in Python?](#56)
- [What is monkey patching in Python?](#57)
- [Does python support multiple inheritance?](#58)
- [What is Polymorphism in Python?](#59)
- [Define encapsulation in Python?](#60)
- [How do you do data abstraction in Python?](#61)
- [Does python make use of access specifiers?](#62)
- [How to create an empty class in Python?](#63)
- [What does an object() do?](#64)
- [What is map function in Python?](#65)
- [Is python numpy better than lists?](#66)
- [What is GIL in Python language?](#67)
- [What makes the CPython different from Python?](#68)
- [What are Decorators in Python?](#69)
- [What is object interning?](#70)
- [What is @classmethod, @staticmethod, @property?](#71)

---

## #1

### What is the difference between list and tuples in Python?

- λ¦¬μ€νΈλ [], ννμ ()λ‘ μμ±
- λ¦¬μ€νΈλ κ°μ μμ ν  μ μμ§λ§ , ννμ κ°μ λ³κ²½ν  μ μλ€.

λ¦¬μ€νΈμ ννμ κ°μ₯ **ν° μ°¨μ΄μ μ κ°μ λ³κ²½ν  μ μλκ°μ μ¬λΆ**μ΄λ―λ‘, νλ‘κ·Έλ¨μ΄ μ€νλλ λμ **κ°μ΄ λ³κ²½λλ©΄ μ λλ κ²½μ° νν**μ μ¬μ©νλ€. ννμ λ¦¬μ€νΈμ λΉν΄ λ μ μ λ©λͺ¨λ¦¬λ₯Ό νμλ‘ νκ³ , μλκ° λΉ λ₯΄λ€.

## #2

### What are the key features of Python?

#### Features of Python

- Script Language
  - μ€ν¬λ¦½νΈ μΈμ΄λ, μ»΄νμΌ κ³Όμ  μμ΄ μ€νκ³Όμ μμ λ²μ­κ³Ό μ€νμ΄ λμμ μΌμ΄λλ μΈμ΄μλλ€.
  - μμ μ΄ λΉ λ₯΄μ§λ§ μ»΄νμΌ μΈμ΄λ³΄λ€ λλ¦° μ€νμλλ₯Ό λ³΄μ¬μ€λλ€.
  - μμΈνκ±΄ [4λ²](#4)μΌλ‘!
- Dynamic typing
  - λ³μμ μλ£νμ μ§μ νμ§ μκ³  μ μΈνλ κ²λ§μΌλ‘ μ¬μ©ν  μ μμ
  - κ°λ° λΉμμ νΈλ¦¬νμ§λ§ type error debugingμ΄ λ°μν  μ μμ
  - νμ§λ§ μ λ μ μμ νΈλ¦¬ν¨μ΄ λ ν¬λ€κ³  μκ°ν©λλ€ ^^
  ```c
  # C, java
  int a = 10
  ```
  ```python
  # Python
  a = 10
  ```
- platform-independent
  - linux, unix, windows, mac... λλΆλΆ OSμμ λͺ¨λ μ λμν©λλ€.
  - μ»΄νμΌ ν  νμκ° μκΈ° λλ¬Έμ!
- Multi paradigm
  - μ μ°¨μ , κ°μ²΄μ§ν₯, ν¨μν, κ΄μ ν νλ‘κ·Έλλ° λͺ¨λ κ°λ₯

#### Pros

- μ¬μ©νκΈ° μ½κΈ°μ λΉ λ₯Έ κ°λ°μλ(μμ°μ±)
- λμ νμ₯μ±, μ΄μμ±
  - κ³ μ±λ₯μ΄ νμνλ€λ©΄ C/C++μΈμ΄μ κ²°ν©ν΄ μ¬μ© κ°λ₯
- νλ°ν μνκ³
  - μλ§μ λΌμ΄λΈλ¬λ¦¬ μ‘΄μ¬
  - μΈκΈ°κ° λ§κΈ° λλ¬Έ

#### Cons

- λλ¦¬λ€
  - Script Languageμ΄κΈ° λλ¬Έ
- type error
  - Dynamic typing μ΄κΈ° λλ¬Έ

#### Reference

- [νμ΄μ¬(Python) νΉμ§ λ° μ₯/λ¨μ  μ λ¦¬](https://velog.io/@jnine/%ED%8C%8C%EC%9D%B4%EC%8D%ACPython-%ED%8A%B9%EC%A7%95-%EB%B0%8F-%EC%9E%A5%EB%8B%A8%EC%A0%90-%EC%A0%95%EB%A6%AC)
- [python λ°λ‘ μκΈ°](https://library.gabia.com/contents/9256/)

## #3

### What type of language is python? Programming or scripting?

**νμ΄μ¬ μ€ν¬λ¦½νΈ μΈμ΄μ΄μ νλ‘κ·Έλλ° μΈμ΄μ΄λ€.**

νμ΄μ¬μ μμ€μ½λλ₯Ό κΈ°κ³μ΄λ‘ λ¨Όμ  λ²μ­νλ μ»΄νμΌ κ³Όμ μ κ±°μΉμ§ μκΈ° λλ¬Έμ μ€ν¬λ¦½νΈ μΈμ΄λ‘ λ³Ό μ μλ€. νμ§λ§ λ§μ μ¬λλ€μ΄ νμ΄μ¬μ΄ Java, C++κ³Ό κ°μ μΈμ΄λ₯Ό λμ²΄νμ¬ κ°λ°μ μ¬μ©λ  μ μκΈ° λλ¬Έμ νλ‘κ·Έλλ° μΈμ΄λΌκ³ λ νλ€. νλ‘κ·Έλλ° μΈμ΄λΌλ λ§ μμ²΄κ° μ€ν¬λ¦½νΈ μΈμ΄λ₯Ό ν¬ν¨νκΈ° λλ¬Έμ νμ΄μ¬λ ν΄λΉλλ€κ³  μκ°νλ€.

**References**

[codingninjas](https://www.codingninjas.com/blog/2018/12/08/difference-between-a-programming-language-and-a-scripting-language/)

[ThePythonGuru](https://thepythonguru.com/is-python-a-programming-language-or-scripting-language/)

[Javatpoint](https://www.javatpoint.com/scripting-vs-programming)

## #4

### Python an interpreted language. Explain.

#### μ»΄νμΌλ¬ vs μΈν°νλ¦¬ν°

μ»΄νμΌλ μΈμ΄λ μ»΄νμΌλ¬λ₯Ό ν΅ν΄ κ΅¬νλλ©° μμ€ μ½λλ₯Ό κΈ°κ³μ΄λ‘ λ°κΎΈλ κ³Όμ μ μ¬μ μ μ²λ¦¬ νμ¬ λΉ λ₯΄κ² μ»΄ν¨ν°μμ κ΅¬λλ  μ μλλ‘ ν λ°©λ² μ΄λ©°, μΈν°νλ¦¬ν° μΈμ΄λ λλΆλΆ μμ€μ½λλ₯Ό κΈ°κ³μ΄λ‘ μ»΄νμΌνμ§ μκ³  μΈν°νλ¦¬ν°λ₯Ό ν΅ν΄ μμ€μ½λ μ€νμ κ° μ€νμ΄νΈλ¨ΌνΈ(μμ€μ½λ κ΅¬λ¬Έ)λ₯Ό νλ μ΄μμ μλΈλ£¨ν΄ μμλ‘ λ³νν ν, κΈ°κ³μ΄λ λ°μ΄νΈμ½λλ± λ€λ₯Έ μΈμ΄λ‘ λ³νλμ΄ κ΅¬ν

<div align='center'>
<img src="https://s3.us-west-2.amazonaws.com/secure.notion-static.com/1cdbfd7a-9479-46fb-8cdf-670a10df3394/_2021-06-03__2.43.34.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5%2F20211016%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211016T154051Z&X-Amz-Expires=86400&X-Amz-Signature=e60d071a61f2e2b8aa2ca27543adb73d78c2a7dc190cc655f6bd3475307b29bd&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22_2021-06-03__2.43.34.png%22" width="60%">

</div>

## #5

### What is pep 8?

PEP8(Python Enhencement Propsals)λ κ°λμ±μ΄ μ’μ νμ΄μ¬ μ½λ©μ νκ³ μ μ μλ μ€νμΌ κ°μ΄λ
μ¬λλ§λ€ κ°μ λ€λ₯Έ μ½λ©μ€νμΌμ΄ μκΈ°μ μ€νμΌκ° μΆ©λμ νΌνκ³ μ νμ΄μ¬ μ½λ© κ°μ΄λλ₯Ό μ μνλ€. from κ·λ λ° λ‘μΈ

example)

- Indentation(4κ° κ³΅λ°±),
- Maximul Line Length(ν μ€μ μ΅λ 79μ, μ£Όμ 72μ)
- Whitesapece in Expressions and Statements(νμ μλ κ³΅λ°± μ κ±°)
- etc...(λ λ€λ₯Έ μ¬λ¬ λ°©λ²μ΄ μλ€.)

code example)

```python
# example-1) λ°νλμ§ μλ return λ¬Έλ NoneμΌλ‘ λ¦¬ν΄λ¬Έμ λͺμν΄ μ€μΌνλ€.
# Wrong:
def foo(x):
    if x >= 0:
        return math.sqrt(x)

# Correct:
def foo(x):
    if x >= 0:
        return math.sqrt(x)
    else:
        return None

# example-2) κ°μ²΄ νμμ λΉκ΅λ isinstance μ΄μ©νλ€ μ§μ λΉκ΅ λμ μ
# Correct:
if isinstance(obj, int):

# Wrong:
if type(obj) is type(1):

# example-3) Sequence(strings, lists, tuples)μ κ²½μ° λΉ sequenceλ falseλΌλ μ¬μ€μ μ΄μ©νλ€.
# Correct:
if not seq:
if seq:

# Wrong:
if len(seq):
if not len(seq):

```

#### Reference

- [PEP8 κ³΅μμ¬μ΄νΈ](https://www.python.org/dev/peps/pep-0008/#maximum-line-length)

## #6

### How is memory managed in Python?

CPythonμμμ λ©λͺ¨λ¦¬ κ΄λ¦¬μ Garbage Collectionμ λ κ°μ§ μΈ‘λ©΄μ΄ μλ€.

1. λ νΌλ°μ€ μΉ΄μ΄ν(Reference counting)
2. μΈλλ³ κ°λΉμ§ μ»¬λ μ(Generational garbage collection)

CPythonμμμ μ£Όμ garbage collection mechanismμ [reference counts](https://docs.python.org/3.6/c-api/intro.html#reference-counts) λ°©μμ΄λ€. Pythonμμ κ°μ²΄λ₯Ό λ§λ€ λλ§λ€ κΈ°λ³Έ C κ°μ²΄μμλ Python μ ν(list, dict λλ function)κ³Ό reference countκ° μμ±λλ€.

λ§€μ° κΈ°λ³Έμ μΌλ‘ Python κ°μ²΄μ reference countλ κ°μ²΄κ° μ°Έμ‘°λ  λλ§λ€ μ¦κ°νκ³  κ°μ²΄μ μ°Έμ‘°κ° ν΄μ λ  λ κ°μνλ€. κ°μ²΄μ reference countκ° 0μ΄ λλ©΄ κ°μ²΄μ λ©λͺ¨λ¦¬ ν λΉμ΄ ν΄μ λλ€.

CPythonμ μ¬μ΄λλ‘ μΈλλ³ κ°λΉμ§ μ»¬λ μμ΄λΌλ κΈ°λ₯λ μλ€.

μ΄κ²μ μ°Έμ‘°λ λμ΄ μμ§λ§, μ κ·Όν  μ μλ κ°μ²΄λ₯Ό λ©λͺ¨λ¦¬μμ λ¦΄λ¦¬μ¦νλ μ­ν μ νλ€. μνμ°Έμ‘°(Circular References) μμ λνλ  μ μλλ°..

```
l = []
l.append(l)
del
```

μμ²λΌ μ°Έμ‘°λ λμ΄ μμ§λ§, ν΄λΉ κ°μ²΄μ μ κ·Όν  μ μλ κ²½μ°λ₯Ό ν΄κ²°νλ€.

λ€μμ μ½μ΄λ³΄λ©΄ μ’κ² λ€.

[python memory allocation](https://leemoney93.tistory.com/25)

#### Reference

- [Garbage Collection in Python](https://medium.com/dmsfordsm/garbage-collection-in-python-777916fd3189)
- [[PYTHON] Garbage Collector ](https://dingrr.com/blog/post/python-garbage-collector)

## #7

### What is namespace in Python?

## #8

### What is PYTHONPATH?

importλ‘ λ€λ₯Έ νμ΄μ¬ νμΌμ λΆλ¬μ¬ λ, pythonμ λ΄λΆμ μΌλ‘ νμΌμ μ°ΎκΈ° μν΄ **sys.path**μ **PYTHONPATH**μ μλ κ²½λ‘λ₯Ό νμν©λλ€.

**sys.path**λ directory path λ¬Έμμ΄μ λͺ¨μλ λ¦¬μ€νΈμλλ€. μ΄ λ¦¬μ€νΈμ pathλ₯Ό μΆκ°νλ©΄ ν΄λΉ pathμ μλ python νμΌμ importν  μ μμ΅λλ€.

```python
sys.path.append('/tttangmin/hobby')

# /tttangmin/hobby/badminton.py
import badminton
```

#### sys.pathμ κΈ°λ³Έκ° (μ°μ μμ μ)

- νμ¬ .py νμΌμ΄ μν directoryμ absolute path
- PYTHONPATH νκ²½λ³μμ μΆκ°λ path
  - sys.path.append()λ **μΌμμ μΌλ‘** pathλ₯Ό μΆκ°νλ κ²μ΄λΌλ©΄
  - PYTHONPATH νκ²½λ³μλ **μκ΅¬μ μΌλ‘** pathλ₯Ό μΆκ°νλ κ²
  - OSμ λ°λΌ μΆκ°νλ λ°©λ²μ΄ λ€λ¦. reference μ°Έκ³ 
- κΈ°ν κΈ°λ³Έ path
  - μ¬λ¬ λ΄μ₯ λͺ¨λλ€μ μν path
  - os, python versionμ λ°λΌ λ€λ¦

#### Reference

- [sys.path, PYTHONPATH: νμ΄μ¬ νμΌ νμ κ²½λ‘](https://www.bangseongbeom.com/sys-path-pythonpath.html)
- [PYTHONPATH μΆκ°νλ λ°©λ²](https://pybasall.tistory.com/201)

## #9

### What are Python modules? Name some commonly used built-in modules in Python?

**Module**μ΄λ Python μ½λλ₯Ό ν¬ν¨νλ νμΌλ‘μ¨, ν¨μλ λ³μ λλ ν΄λμ€λ₯Ό λͺ¨μ λμ νμΌμ΄λ€. λͺ¨λμ λ€λ₯Έ νμ΄μ¬ νλ‘κ·Έλ¨μμ λΆλ¬μ μ¬μ©ν  μ μκ²λ λ§λ  νμ΄μ¬ νμΌμ΄λΌκ³ λ ν  μ μλ€. μ€ν κ°λ₯ν μ½λλ₯Ό ν¬ν¨νλ, νμ΄μ¬ νμ₯μ `.py`λ‘ λ§λ  νμ΄μ¬ νμΌμ λͺ¨λ λͺ¨λμ΄λ€. λͺ¨λμ μ¬μ©νλ©΄, λ€λ₯Έ μ½λμ μ μ©νκΈ°κ° μ¬μμ§λ―λ‘ μ΄μμ±μ΄ μ’μμ§λ€.

**Built-in modules**λ νμ΄μ¬μμ μ κ³΅νλ κ³΅μ λ΄μ₯ λΌμ΄λΈλ¬λ¦¬λ€. λ‘μ»¬μ μ΄λκ³³μμ νμΌμ μμ±νλμ§ μ΄ λ΄μ₯ λͺ¨λλ€μ μ΄λμλ μ¬μ©ν  μ μλ€.

- μμ£Ό μ¬μ©λλ built-in module μ μμ
  - os
  - sys
  - math
  - random
  - datetime
  - JSON
  - itertools

#### Reference

- [λͺ¨λμ΄λ?](https://yganalyst.github.io/data_handling/Py_study14/)
- [ν¨ν€μ§,λͺ¨λ](https://fierycoding.tistory.com/m/60?category=942731)

## #10

### What are local variables and global variables in Python?

ν¨μ μμμ λ§λ€μ΄μ§ λ³μλ₯Ό **μ§μ­λ³μ(local variable)** λΌ νκ³  ν¨μ λ°μμ λ§λ€μ΄μ§ λ³μλ₯Ό **μ μ­λ³μ(global variable)** λΌ νλ€.

μ΄ λ λ³μλ μλμ κ°μ΄ λ κ°μ§ μ°¨μ΄μ μ΄ μ‘΄μ¬νλ€.

1. **λ©λͺ¨λ¦¬μ μ‘΄μ¬νλ μκ°**

   μ§μ­ λ³μλ ν΄λΉ μ§μ­μμ μ μΈλλ μκ° λ©λͺ¨λ¦¬κ° μμ±λκ³  ν΄λΉ μ§μ­μ λ²μ΄λλ©΄ μλμΌλ‘ μλ©Έ

   μ μ­ λ³μλ μ½λκ° μμλμ΄ μ μΈλλ μκ° λ©λͺ¨λ¦¬ μμ±, μ½λ μ μ²΄ λλ λ κΉμ§ λ©λͺ¨λ¦¬λ₯Ό μ°¨μ§

2. **λ³μμ μ κ·Όν  μ μλ λ²μ**

   μ§μ­ λ³μλ μ μΈ λ ν¨μ λ΄μμλ§ μ¬μ©μ΄ κ°λ₯

   μ μ­ λ³μλ νλ‘κ·Έλ¨ μ€ν μ€μ μ°μ΄λ λͺ¨λ  ν¨μκ° μ¬μ© κ°λ₯

#### Reference

- [3.3 μ§μ­λ³μ, μ μ­λ³μ](https://wikidocs.net/62)
- [μ μ­λ³μμ μ§μ­λ³μ](https://edu.goorm.io/learn/lecture/2010/ν-λμ-λλ΄λ-κ³ λ­-κΈ°μ΄/lesson/174452/μ μ­λ³μμ-μ§μ­λ³μ)

## #11

### Is Python case sensitive?

λμλ¬Έμ κ΅¬λΆνλ€.

PHP κ°μ κ²½μ° λ³μμ΄λ¦μ λμλ¬Έμ κ΅¬λΆμ΄ μκ³ , ν¨μμ΄λ¦μ μλ€. ν¨μλ₯Ό μλ¬Έμλ‘ μ μνκ³  λλ¬Έμλ‘ νΈμΆνλ κ²μ΄ κ°λ₯νλ€.

#### Reference

- [Wikipedia](https://en.wikipedia.org/wiki/Case_sensitivity#:~:text=are%20strictly%20lowercase.-,In%20programming%20languages,Ruby%2C%20Python%20and%20Swift)

## #12

### What is type conversion in Python

Type conversionμ λ°μ΄ν° νμμ λ€λ₯Έ νμμΌλ‘ λ°κΎΈλ κ²μ μλ―Ένλ€.

~~(λ°μ΄ν° νμμ μ’λ₯: int, float, complex, string, fuple, set, list, dictionary, .... )~~

Pythonμμλ 2κ°μ§μ type conversionμ΄ μ‘΄μ¬νλ€.

1. Implicit Type Conversion(μμμ  ν λ³ν)
2. Explicit Type Conversion(λͺμμ  ν λ³ν)

**Implicit Type Conversion**

Implicit Type Conversionμ Pythonμ΄ μλμΌλ‘ ν λ³νμ μ€ννλ€. μ΄ λ dataμ lossλ₯Ό μ€μ΄κΈ° μν΄ lower data type(int)λ₯Ό higher data typeμΌλ‘ λ°κΏμ€λ€.

```python
num_int = 123
num_flo = 1.23

num_new = num_int + num_flo

print("datatype of num_int:",type(num_int)) # -> <class 'int'>
print("datatype of num_flo:",type(num_flo)) # -> <class 'float'>

print("Value of num_new:",num_new) # -> 24.23
print("datatype of num_new:",type(num_new)) # -> <class 'float'>
```

(μ°Έκ³ λ‘ λ¬Έμμ΄μ΄λ μ«μλ λνλ©΄ μ€λ₯(TypeError)λκΈ° λλ¬Έμ μ΄λλ λͺμμ  ν λ³νμ ν΄μ€μΌ νλ€.)

**Explicit Type Conversion**

μ¬μ©μκ° κ°μ±μ νμμ λͺμμ μΌλ‘ λ°κΏμ£Όλ κ². μ¬μ  μ μλ `int`(), `float()`, `str()`, etc ν¨μλ₯Ό μ΄μ©νλ€.

μ΄λ¬ν type of conversionμ μ μ κ° μ§μ  κ°μ±μ data typeμ cast(change) ν΄μ£ΌκΈ° λλ¬Έμ typecastingμ΄λΌκ³ λ λΆλ¦°λ€.

```python
num_int = 123
num_str = "456"

print("Data type of num_int:",type(num_int))#  --> <class 'int'>
print("Data type of num_str before Type Casting:",type(num_str)) #  --> <class 'str'>

num_str = int(num_str)
print("Data type of num_str after Type Casting:",type(num_str)) #  --> <class 'int'>

num_sum = num_int + num_str

print("Sum of num_int and num_str:",num_sum) #  --> 579
print("Data type of the sum:",type(num_sum)) #  --> <class 'int'>
```

#### Reference

[Type-conversion & Casting](https://www.programiz.com/python-programming/type-conversion-and-casting)

## #14

### Is indentation required in python?

λ€μ¬μ°κΈ°. pythonμμλ λ€μ¬μ°κΈ°λ **λ¬Έλ²μ μΈ κ°μ μ¬ν­**μλλ€.
λ€λ₯Έ νλ‘κ·Έλ¨ μΈμ΄μμλ {}λ₯Ό μ¬μ©νμ¬ μμ­μ μ§μ ν©λλ€.

```c
if (victor(human)) {
human_wins++;
printf("I am your humble servant.\n");
} else {
computer_wins++;
printf("Your destiny is under my control!\n");
}
```

λ¬Όλ‘  cμΈμ΄μμλ indentationμ μ μ©ν  μ μμ΅λλ€λ§, ;λ₯Ό μ¬μ©ν΄μΌ ν©λλ€.

```c
if (victor(human)) {
	human_wins++;
	printf("I am your humble servant.\n");
} else {
	computer_wins++;
	printf("Your destiny is under my control!\n");
}
```

python μμλ {}λ ;λ₯Ό μ°μ§ μλ λμ , indentationμΌλ‘ μ½λμ μμ­μ μ§μ ν©λλ€.

```python
if victor == 'human':
    human_win++
    print("I am your humble servant.\n")
else:
    computer_wins++;
	print("Your destiny is under my control!\n");
```

indentationμ λ°©λ²μ λμ΄μ°κΈ° νμΉΈ, λμΉΈ, 4μΉΈ, ν­ λ± μ¬λ¬κ°μ§ λ°©λ²μ΄ μμ§λ§,

> μ€μν κ²μ κ°μ λΈλ‘ λ΄μμλ λ€μ¬μ°κΈ° μΉΈ μκ° κ°μμΌ ν©λλ€.
>
> μλ°μ Indentation Errorκ° μΆλ ₯λ©λλ€.

#### Reference

- [python κ³λ¨λ°κΈ° : λ€μ¬μ°κΈ°(indent)](https://wikidocs.net/20368)
- [c indentation](https://www2.cs.arizona.edu/~mccann/indent_c.html)

## #15

### What is the difference between Python Arrays and lists?

νμ΄μ¬μμλ λ°°μ΄μ΄λΌλ λΆλΆμ΄ μμ§λ§ λ°°μ΄μ νΈμμ± λλ¬Έμ `array` λΌλ λͺ¨λμ μ κ³΅νκ³  μμ΅λλ€.

**array**μ **list**λ λμΌν λ°©μμΌλ‘ λ°μ΄ν°λ₯Ό μ μ₯νμ§λ§

**array**λ **λ¨μΌ λ°μ΄ν° νμ μμ**λ§μ ν¬ν¨ν  μ μλ λ°λ©΄,

**list**λ **λ€μν νμμ μμ**λ€μ΄ λ€μ΄κ° μ μμ΅λλ€.

arrayλ `arrayName = arrary(type, [Values])`μ²λΌ μλ£νμ μ μ₯νκ³ , μ§μ ν μλ£νλ§μ λ£μμ μμ΅λλ€.

listλ λ³μμ []λ‘ μ¬λ¬ νμμ λ³μλ₯Ό λ¬Άμ΄μ μ μΈν  μ μμ΅λλ€.

#### Reference

- [νμ΄μ¬[Python] 036 Array(λ°°μ΄) μ¬μ©νκΈ°](https://appia.tistory.com/125)

## #16

### What are functions in Python?

**Pythonμμ ν¨μλ νΉμ  μμμ μννλ κ΄λ ¨ λͺλ Ήλ¬Έμ κ·Έλ£Ήμ΄λ€.**

ν¨μλ₯Ό μ¬μ©ν¨μΌλ‘μ¨ νλ‘κ·Έλ¨μ λ μκ³  **λͺ¨λν**λκ² λλλλ° λμμ΄ λκ³  νλ‘κ·Έλ¨μ λ³΄λ€ **μ²΄κ³μ **μ΄κ³  **κ΄λ¦¬νκΈ° μ½κ²** λ§λ€ μ μλ€.

λν λ°λ³΅μ νΌνκ³  **μ½λλ₯Ό μ¬μ¬μ©**νκΈ° μ©μ΄ν΄μ§λ€.

λ¬Έλ²μ μλμ κ°λ€.

```python
def function_name(parameters):
	"""docstring"""
	statement(s)
```

1. `def` : ν¨μμ ν€λμ μμμ μλ¦¬λ ν€μλ
2. ν¨μμ μ΄λ¦μ κΈ°λ₯μ μ λνλΌ μ μκ² μ ν΄μΌνλ€.
3. `parameters` : ν¨μμ κ°μ μ λ¬νλ λ§€κ°λ³μ (μ νμ¬ν­)
4. `:` : ν¨μ ν€λμ λμ νμ
5. `docstring` : ν¨μκ° νλ μΌμ μ€λͺνλ λ¬Έμμ΄ (μ νμ¬ν­)
6. `statemet` : ν¨μμ λ³Έλ¬Έμ κ΅¬μ νλ νλ μ΄μμ νμ΄μ¬ λ¬Έ, λ€μ¬μ°κΈ° μ λκ° κ°μμΌνλ€.
7. `return` : ν¨μμμ κ°μ λ°ννλ λ°νλ¬Έ (μ νμ¬ν­)

#### Reference

- [Python Functions (def): Definition with Examples - Programiz](https://www.programiz.com/python-programming/function)

## #17

### What is \_\_init\_\_?

- μ΄κΈ°ν ν¨μ
- μΈμ€ν΄μ€λ₯Ό μμ±ν  λ λ°λμ μ²μμ νΈμΆλλ ν¨μ
- μμ±μλ‘μ ν΄λμ€λ§λ€ νλμ‘΄μ¬

#### Reference

- [python λ¬Έλ²](https://wikidocs.net/89)
- [python selfμ init](https://engineer-mole.tistory.com/190)
- [inflearn](https://www.inflearn.com/questions/4642)

## #18

### What is a lambda function?

λλ€ν¨μλ μ΄λ¦ μμ΄ μ μλλ μ΅λͺ ν¨μ(anonymous functions)μλλ€. `def`λ₯Ό μ΄μ©νμ¬ μ μ λλ μΌλ° ν¨μμ λ¬λ¦¬ `lambda` ν€μλλ₯Ό μ΄μ©νμ¬ μ μλ©λλ€. λ³΄ν΅ νμ€λ‘ ν¨μλ₯Ό νννκΈ°μ μ½λκ° κ°κ²°ν΄μ§κ³  ν λ² μ¬μ©λκ³  λ€μ μ¬μ© ν  μ μκΈ°μ λ©λͺ¨λ¦¬λ₯Ό μ μ½ ν  μ μμ§λ§ μ¬λ¬μ€λ‘ ννν  μ μκ³  ν¨μμ λν μ€λͺμ μ μ μ μλ λ¨μ μ΄ μμ΅λλ€.(doc string λΆκ°). μ΄λ° κ²½μ° def ν¨μλ₯Ό μ΄μ©νμ¬ ν¨μλ₯Ό μ μ ν΄μΌ νλ€.

```python
# μμ1
my_list = [1, 5, 4, 6, 8, 11, 3, 12]
new_list = list(filter(lambda x: (x%2 == 0) , my_list)) # [4,6,8,12]

# μμ2
my_list = [1, 5, 4, 6, 8, 11, 3, 12]
new_list = list(map(lambda x: x * 2 , my_list)) # [2, 10, 8, 12, 16, 22, 6, 24]

# μ€μ§ νλμ arguemntκ° νμν ν¨μλ₯Ό μΈ κ²½μ° labmda μ¬μ© νμ μλ€.
#Bad
map(lambda x:abs(x), list_3)
#Good
map(abs, list_3)

# ν¨μ μ μνλ€λ©΄ defλ₯Ό μ¬μ©νλ κ²μ΄ μ’λ€
#Bad
triple = lambda x: x*3
#Good
def triple(x):
     return x*3
```

#### Reference

- [νμ΄μ¬ μ΅λͺν¨μ μμ: Programiz](https://www.programiz.com/python-programming/anonymous-function)
- [Towards Data Science: Lambda Functions with Practical Examples in Python](

## #19

### What is self in Python

ν΄λμ€ λ΄μ μ μλ selfλ ν΄λμ€ μΈμ€ν΄μ€μ΄λ€.

μμλ₯Ό ν΅ν μ΄ν΄

```python
class Foo:
    def func1():
        print("function 1")

    def func2(self):
        print(id(self))
        print("function 2")
```

ν΄λμ€ λ΄μ μ μλ ν¨μλ₯Ό λ©μλλΌ λΆλ₯΄κ³  λ©μλμ μ²« μΈμλ λ³΄ν΅ self μ΄λ€. κ·Έλ¬λ ν­μ self μ΄μ΄μΌ νλκ²μ μλλ€ μ°¨μ΄λ₯Ό ν λ² μ΄ν΄λ³΄μ

```python
a = Foo()

## example-1
a.func1()
>> TypeError: func1() takes 0 positional arguments but 1 was given

a.func2()
>> 140660141772432
>> function 2

FOO.func1()
>> function 1

## example-2
id(a)
>> 140660141772432

## example-3
Foo.func2()
>> TypeError: func2() missing 1 required positional argument: 'self'


Foo.func2(a) ## == a.func2()
>> 140660141772432
>> function 2
```

1. - λ©μλλ₯Ό νΈμΆν  λ selfμ λν κ°μ νμ΄μ¬μ΄ μλμΌλ‘ λκ²¨μ£ΌκΈ° λλ¬Έμ a.func1() == a.func1(self)μ λμΌνλ€ κ·Έλ°λ° ν¨μ func1μ μΈμλ₯Ό λ°μ§ μκΈ° λλ¬Έμ μ€λ₯κ° λλ€.

   - func1μ νΈμΆνλ €λ©΄ μΈμ€ν΄μ€ λ©μλκ° μλ class λ©μλλ‘ λΆλ¬μ£Όλ©΄ func1μ νΈμΆ ν  μ μλ€

2. μΆκ°μ μΌλ‘ selfλ μΈμ€ν΄μ€μμ νμ΄λ³κΈ° μν΄ func2μ μλ id(self)μ id(a)λ₯Ό λΉκ΅νλ©΄ μΈμ€ν΄μ€μ μ£Όμκ°μ΄ λμΌν κ²μ μ μ μλ€.

3. ν΄λμ€ μ΄λ¦μ μ΄μ©ν λ©μλ νΈμΆ self λΆλΆμ μΈμ€ν΄μ€ λ£μ΄μ£Όλ©΄ ν΄κ²°

#### Reference

- [self μ΄ν΄νκΈ° - νμ΄μ¬μΌλ‘ λ°°μ°λ μκ³ λ¦¬μ¦ νΈλ μ΄λ©](

## #20

### How does break, continue and pass work?

break λ¬Έμ΄ μ‘΄μ¬νλ λ£¨νλ₯Ό μ’λ£νκΈ° μν΄ μ¬μ©λ¨.

continue λ¬Έ λ€μμ λ£¨ν λ΄λΆ μ½λλ κ±΄λλ°κ³  λ£¨νμ λ€μ λ°λ³΅μΌλ‘ λμ΄κ°.

pass λ¬Έμ λͺλ Ήμ΄λ μ½λλ₯Ό μ€ννκ³  μΆμ§ μμ§λ§ κ΅¬λ¬Έμ μ±μμΌ ν  λ μ¬μ©λ¨.

#### Reference

- [break, continue and pass in Python](https://www.geeksforgeeks.org/break-continue-and-pass-in-python/#break)

## #21

### What does `[::-1]` do?

νμ΄μ¬ μνμ€ μλ£νμ κ°μ΄ μ°μμ μΌλ‘ μ΄μ΄μ§ μλ£νμΌλ‘, **λ¦¬μ€νΈ, νν, range, λ¬Έμμ΄**μ΄ μλ€. μνμ€ μλ£νμ μνμ€ κ°μ²΄μ μΌλΆλ₯Ό μλΌλΌ μ μλ **μ¬λΌμ΄μ±(slicing)**μ΄λΌλ κΈ°λ₯μ μΈ μ μλ€. μ¬λΌμ΄μ±μ `seq[start:end:step]`μ²λΌ μΈ μ μμΌλ©°, `start`λ μμ μΈλ±μ€, `end`λ λ μΈλ±μ€, `step`μ μΈλ±μ€ μ¦κ°ν­μ λ§νλ€. `step`μ΄ μμμ΄λ©΄ μ¦κ°νκ³ , μμμ΄λ©΄ κ°μνλ€.

`seq[::-1]`μ `start`μ `end`λ μμ μΈλ±μ€μ λ μΈλ±μ€λ₯Ό μλ΅νμλλ°, μ΄λ΄ κ²½μ° μ μ²΄ μνμ€λ₯Ό κ°μ Έμ¨λ€. μ¦, `seq[::-1]`μ μ μ²΄ μνμ€λ₯Ό μ­μ (reverse)μν¨λ€.

#### Reference

- [μνμ€ μλ£ν νμ©νκΈ°](https://dojang.io/mod/page/view.php?id=2205)
- [μ¬λΌμ΄μ€ μ¬μ©νκΈ°](https://dojang.io/mod/page/view.php?id=2208)

## #22

### How can you randomize the items of a list in place in Python?

**random λͺ¨λμ `shuffle` ν¨μ** λ₯Ό μ¬μ©νλ©΄ κ΅¬νν  μ μλ€. `random.shuffle` μ μνμ€ κ°μ²΄μ μμλ₯Ό μμλ‘ μμ΄μ ν΄λΉ μνΈμ€λ₯Ό λ°ννλ€.

```python
import random

random.seed(42) # 42λ ν΅μμ μΌλ‘ μ¬μ©νλ μλ κ³ μ  μμ΄λ€. λ±ν μλ―Έλ μκ³  μ¬λ¬ κ°μ€μ΄ μ‘΄μ¬ν¨.
lst = list(range(10))
print(lst) # [0, 1, 2, 3, ... , 9]
random.shuffle(lst)
print(lst) # [2, 7, 9, 3, 0, ...]
```

## #23

### Whatβs the difference between iterator and iterable?

#### Iterable

- Iterable κ°μ²΄λΌκ³  ν¨. λ°λ³΅κ°λ₯ν κ°μ²΄
- λνμ μΌλ‘ ist, dict, set, str, bytes, tuple, rangeμ΄ μμ
- μλμ λ°©λ²μΌλ‘ iterable κ°μ²΄ μ νν νμΈ

```python
  # iterable ν νμ
  >>> var_list = [1, 3, 5, 7]
  >>> isinstance(var_list, collections.Iterable)
  True

  # iterableνμ§ μμ νμ
  >>> var_int = 932
  >>> isinstance(var_int, collections.Iterable)
  False
```

#### Iterator

- Iterator κ°μ²΄λΌκ³  ν¨. κ°μ μ°¨λ‘λλ‘ κΊΌλΌ μ μλ κ°μ²΄μλλ€.
- iterableν κ°μ²΄λ₯Ό λ΄μ₯ν¨μ λλ iterableκ°μ²΄μ λ©μλλ‘ κ°μ²΄λ₯Ό μμ±ν  μ μμ΅λλ€.

```python
>>> a = [1, 2, 3]

# νμ΄μ¬ λ΄μ₯ν¨μ iter()
>>> iter(a)

# iterableκ°μ²΄λ λ§€μ§λ©μλ __iter__()
>>> a.__iter__()
```

- next()ν¨μλ‘ κ°μ μμλλ‘ κΊΌλΌμ μμ(pop)

```python
>>> next(a_iter)
1
>>> next(a_iter)
2
>>> next(a_iter)
3
>>> next(a_iter)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
StopIteration
```

#### Reference

- [νμ΄μ¬-κΈ°λ³Έμ κ°κ³  λ¦μ! : 38. Iterable κ³Ό Iterator](https://wikidocs.net/16068)
- [Python(νμ΄μ¬) κΈ°λ³Έ - 19. for in λ°λ³΅λ¬Έ, Range, enumerate](https://suwoni-codelab.com/python%20%EA%B8%B0%EB%B3%B8/2018/03/03/Python-Basic-for-in/)

## #24

### How can you generate random numbers in Python?

νμ΄μ¬ λ΄μ₯ λͺ¨λμΈ `random` μ ν΅ν΄ μ¬μ©ν  μ μμ.

**μ μ** μ λν΄μλ, λ²μμμ κ· μΌν μ νμ΄ μμ.

**μνμ€** μ λν΄μλ, λ¬΄μμ μμμ κ· μΌν μ ν, λ¦¬μ€νΈλ₯Ό μ μλ¦¬(in-place)μμ μμ μμ΄μ μμ±νλ ν¨μ λ° μ€λ³΅ μλ(without replacement) λ¬΄μμ νλ³Έ μΆμΆ(sampling)μ μν ν¨μκ° μμ.

**μ€μ** μ λν΄μλ, κ· μΌ(uniform), μ κ·(normal) (κ°μ°μμ(Gaussian)), λ‘κ·Έ μ κ·(lognormal), μμ μ§μ(negative exponential), κ°λ§(gamma) λ° λ² ν(beta) λΆν¬λ₯Ό κ³μ°νλ ν¨μκ° μμ.

#### κΈ°λ³Έμ μΈ random λ©μλ

1. random.seed(_a=None_, _version=2_)

   : λμ μμ±κΈ°λ₯Ό μ΄κΈ°νν©λλ€.

2. μ μ ν¨μ

   1. **random.randrange(_stop_), random.randrange(_start_, _stop_[, *step*])**

      `range(start, stop, step)`μμ μμλ‘ μ νλ μμλ₯Ό λ°ν. `choice(range(start, stop,step))`μ λλ±νμ§λ§, μ€μ λ‘ range κ°μ²΄λ₯Ό λ§λ€μ§λ μμ.

   2. **random.randint(_a_, _b_)**

      `a <= N <= b`λ₯Ό λ§μ‘±νλ μμμ μ μ *N*μ λ°ν

3. μνΈμ€ ν¨μ

   1. **random.choice(_seq_)**

      λΉμ΄ μμ§ μμ μνμ€ *seq*μμ μμμ μμλ₯Ό λ°ν

   2. **random.choices**(_population_, _weights=None_, *\*\*, *cum_weights=None*, *k=1\*)

      *population*μμ μ€λ³΅μ νλ½νλ©΄μ(with replacement) μ νν _k_ ν¬κΈ°μ μμ λ¦¬μ€νΈλ₯Ό λ°νν©λλ€. *population*μ΄ λΉμ΄ μμΌλ©΄, [`IndexError`](https://docs.python.org/ko/3/library/exceptions.html#IndexError)λ₯Ό λ°μ

   3. **random.shuffle(_x_[, *random*])**

      μνμ€ *x*λ₯Ό μ μλ¦¬μμ μμ. μ¦, x μμ²΄ μμμ μμ΄κ² λ¨ sorted, sort μ€ sortλΌ λ³΄λ©΄ λ¨

   4. **random.sample**(_population_, _k_, *\*\*, *counts=None\*)

      population μνμ€λ μ§ν©μμ μ νν κ³ μ ν μμμ _k_ κΈΈμ΄ λ¦¬μ€νΈλ₯Ό λ°ν. μ€λ³΅ μλ(without replacement) λ¬΄μμ νλ³Έ μΆμΆ(sampling)μ μ¬μ©.

4. μ€μ ν¨μ

   1. **random.random()**

      [0.0, 1.0) κ΅¬κ°μμ λ€μ μμμ λΆλ μμμ  μ«μλ₯Ό λ°ν.

   2. **random.uniform(_a_, _b_)**

      `a <= b` μΌ λ `a <= N <= b`, `b < a` μΌ λ `b <= N <= a`λ₯Ό λ§μ‘±νλ μμμ λΆλ μμμ  μ«μ *N*μ λ°ν

   3. **random.normalvariate(_mu_, _sigma_)**

      μ κ· λΆν¬. *mu*λ νκ· μ΄κ³ , *sigma*λ νμ€ νΈμ°¨

#### μμ 

```python
>>> random()                             # Random float:  0.0 <= x < 1.0
0.37444887175646646

>>> uniform(2.5, 10.0)                   # Random float:  2.5 <= x <= 10.0
3.1800146073117523

>>> expovariate(1 / 5)                   # Interval between arrivals averaging 5 seconds
5.148957571865031

>>> randrange(10)                        # Integer from 0 to 9 inclusive
7

>>> randrange(0, 101, 2)                 # Even integer from 0 to 100 inclusive
26

>>> choice(['win', 'lose', 'draw'])      # Single random element from a sequence
'draw'

>>> deck = 'ace two three four'.split()
>>> shuffle(deck)                        # Shuffle a list
>>> deck
['four', 'two', 'ace', 'three']

>>> sample([10, 20, 30, 40, 50], k=4)    # Four samples without replacement
[40, 10, 50, 30]
```

#### Reference

- [python κ³΅μ document - random (μμ¬ λμ μμ±)](https://docs.python.org/ko/3/library/random.html)

## #25

#### What is the difference between range & xrange?

> νμ΄μ¬2μμλ `range`μ `xrange` λͺ¨λ μ‘΄μ¬νμ§λ§, νμ΄μ¬3λΆν°λ `range`κ° λ΄λΆμ μΌλ‘ `xrange`λ‘ λμνλλ‘ λ°λμ΄μ `range`λ§ μ‘΄μ¬νλ€. κ·Έλ¬λ―λ‘ **νμ΄μ¬2**λ₯Ό κΈ°μ€μΌλ‘ `range`μ `xrange`λ₯Ό μ€λͺνλ€.

`range` κ°μ²΄λ μλ ₯μΌλ‘ λ°μ μ μ λ²μμ κ°μ μμλ‘ κ°λ λ¦¬μ€νΈλ₯Ό λ§νλ€. κ·Έλ¬λ―λ‘ `range(3)`κ³Ό `[0, 1, 2]`λ μμ ν λμΌνλ€.

(a type of iterable)

```
# python2
r = range(5)
print(r)            # [0, 1, 2, 3, 4]
print(type(r))      # <type 'list'>
print (sys.getsizeof(r)) # 112
```

`xrange`λ μ λλ μ΄ν° κ°μ²΄λ‘, μ€μ§ λ£¨νλ₯Ό λλλ§ ν΄λΉ λ²μμ μ μλ₯Ό νλμ© λ°ννλ€. μ λλ μ΄ν°μ κ΄ν μ€λͺμ [μ¬κΈ°](https://github.com/boostcamp-ai-tech-4/ai-tech-interview/blob/main/answers/4-python.md#28)μμ! (lazy evaluationμΌλ‘ λΆλ¦¬κΈ°λν¨ μκ΅¬μ μν΄μλ§ κ°μ λ°ννκΈ°μ)

```
#python2
r = xrange(5)
print(r)            # xrange(5)
print(type(r))      # <type 'xrange'>
print (sys.getsizeof(r)) # 48

for i in r:
    print i,
# >> 0 1 2 3 4
```

- xrangeλ μ λλ μ΄ν°μ΄κΈ° λλ¬Έμ κ°μ λ°ννκ³  μ΄μ  κ°μ λ©λͺ¨λ¦¬μμ μ§μ΄λ€. νμ§λ§ rangeλ list typeμ΄κΈ° λλ¬Έμ λͺ¨λ  κ°μ λ©λͺ¨λ¦¬μ μ μ₯νκΈ° λλ¬Έμ λ©λͺ¨λ¦¬κ° ν¨μ¨μ μ΄μ§ λͺ»νλ€.

- rangeλ λ¦¬μ€νΈ μ΄κΈ° λλ¬Έμ λ¦¬μ€νΈμ κ΄λ ¨ν indexiing, list μ°μ°μ΄ κ°λ₯νμ§λ§ xrangeλ κ·Έλ μ§ λͺ»νλ€.

#### Reference

- [μλ³Έ λ΅λ³](https://github.com/SEOzizou/ai-tech-interview)
- [range() vs xrange() in Python](https://www.geeksforgeeks.org/range-vs-xrange-python/)

## #26

### How do you write comments in Python?

λΌμΈ λ§¨ μμ #μ μ¬μ©νκ±°λ, μ¬λ¬μ€μ νλ²μ μ²λ¦¬νκ³  μΆλ€λ©΄ """ ... """ λλ '''...'''ννλ‘ μ¬μ©ν  μ μλ€.

#### Reference

- [Python Statement, Indentation and Comments](https://www.programiz.com/python-programming/statement-indentation-comments)

## #27

### What is pickling and unpickling?

νμ΄μ¬ κ°μ²΄λ₯Ό νμΌμ μ μ₯νλ κ³Όμ μ **pickling,**

νμΌμμ κ°μ²΄λ₯Ό μ½μ΄μ€λ κ³Όμ μ **unplicking** μ΄λΌκ³  νλ€.

pickle λͺ¨λμ μ΄μ©νλ©΄ μνλ λ°μ΄ν°λ₯Ό μλ£νμ λ³κ²½μμ΄ νμΌλ‘ μ μ₯νμ¬ κ·Έλλ‘ λ‘λν  μ μκ³ ,

pickleλ‘ λ°μ΄ν°λ₯Ό μ μ₯νκ±°λ λΆλ¬μ¬ λλ νμΌμ **λ°μ΄νΈ νμμΌλ‘ μ½κ±°λ μ¨μΌ**νλ€.(wb,rb)

λν pickleμ λͺ¨λ  νμ΄μ¬ κ°μ²΄λ₯Ό μ μ₯νκ³  μ½μ μ μλ€.

#### Reference

- [νμ΄μ¬ κ°μ²΄λ₯Ό νμΌμ μ μ₯νκΈ°, κ°μ Έμ€κΈ°](https://dojang.io/mod/page/view.php?id=2327)
- [pickle λͺ¨λ](https://wayhome25.github.io/cs/2017/04/04/cs-04/)

## #28

### What are the generators in python?

Generatorλ Iterator κ°μ²΄λ₯Ό κ°λ¨ν λ§λ€ μ μλ ν¨μλ₯Ό λ§νλ€. μ λλ μ΄ν°λ λ€μκ³Ό κ°μ΄ (1) yieldλ¬Έκ³Ό ν¨μ, (2) ννμ ννλ‘ λ§λ€ μ μλ€.

> yieldλ¬Έκ³Ό ν¨μ

- μ λλ μ΄ν° ν¨μ μ μ

```python
def generator_list(value):
  for i in range(value):
    # κ°μ λ°ννκ³  μ¬κΈ°λ₯Ό κΈ°μ΅
    yield i
```

- μ λλ μ΄ν° κ°μ²΄ μμ± λ° next ν¨μλ‘ νΈμΆ

```python
gen = generator_list(2)
print(next(gen)) # 0
print(next(gen)) # 1
print(next(gen)) # StopIteration μλ¬ λ°μ
```

> ννλ¬Έ

```python
value = 2
gen = (i for i in range(value))
print(next(gen)) # 0
print(next(gen)) # 1
print(next(gen)) # StopIteration μλ¬ λ°μ
```

**_μ λ¦¬μ€νΈ λμ  μ λλ μ΄ν°λ₯Ό μ¬μ©ν κΉ?_**

- λ¦¬μ€νΈλ₯Ό μ¬μ©νλ©΄ λ¦¬μ€νΈμ ν¬κΈ°λ§νΌ λ©λͺ¨λ¦¬μ κ³΅κ°μ΄ ν λΉλλ€. λ°λ©΄ μ λλ μ΄ν°λ λ§ κ·Έλλ‘ next ν¨μλ‘ νΈμΆλ  λ κ°μ μμ±νκ³  ν΄λΉ κ°λ§ λ©λͺ¨λ¦¬μ μ¬λ¦°λ€. μ¦, λ©λͺ¨λ¦¬λ₯Ό μ μ½ν  μ μλ€. μμ λ°μ΄ν°λΌλ©΄ μκ΄μμ§λ§ ν° λ°μ΄ν°μμλ μ λλ μ΄ν° μ¬μ©μ΄ νμμ΄λ€.

**References**

- [γγγγ·](https://bluese05.tistory.com/56)

## #29

### How will you capitalize the first letter of string?

λ¬Έμμ΄ λ©μλ `capitalize` μ¬μ©νλ©΄ λ©λλ€.

```python
s = 'purple'
v = 'is'
o = 'best'
print(capitalize(s) + capitalize(v) + capitalize (o)) # PurpleIsBest
```

#### Reference

- [Python String Methods](https://www.w3schools.com/python/python_ref_string.asp)

## #30

### How will you convert a string to all lowercase?

`str` μ `lower('text')` λ₯Ό ν΅ν΄ λͺ¨λ  μΌμ΄μ€μ λ¬Έμλ₯Ό μλ¬Έμλ‘ λ³ννλ©° λ¬Έμμ΄μ λ³΅μ¬λ³Έμ λλ € λ°μ stringμ λͺ¨λ lowercaseλ‘ λ°κΏ μ μλ€.

#### Reference

- [Python κ³΅μ document - str.lower()](https://docs.python.org/ko/3/library/stdtypes.html?highlight=lower#str.lower)

## #31

### How to comment multiple lines in python?

μ¬λ¬ μ€μ μ£Όμ(comment)νλ λ°©λ²μ ν¬κ² 2κ°μ§κ° μλ€.

**μ²«μ§Έ,** `#` **μ΄μ©νκΈ°**

ν μ€μ μ£Όμνλ `#` μ μ¬λ¬λ² λ°λ³΅νμ¬ μ¬μ©μ ν΅ν΄ μ¬λ¬ μ€μ μ£Όμμ΄ κ°λ₯νλ€.

**λμ§Έ,** `""" """` **μ΄μ©νκΈ°**

docstringμΌλ‘λ μ¬μ©νλ """ """μ μ΄μ©νμ¬ μ¬λ¬ μ€μ μ£Όμ ν  μ μλ€.

**μ°Έκ³ ,** `/*`, `*/`

`/*`, `*/` λ Java, C, C++ μμλ μ¬λ¬μ€ μ£ΌμμΌλ‘ λ§μ΄ μ¬μ©μ΄ λμ§λ§ <u>Pythonμμλ μ¬μ©μ΄ λΆκ°λ₯ νλ€.</u>

#### Reference

- [Python Comment Block: How To Write Multi-Line Comments](https://appdividend.com/2021/02/23/python-comment-block-how-to-write-multi-line-comments/)

## #32

### What are Docstrings in Python?

Document stringμ Python module, class, function or methodμ μ μλ₯Ό μ€λͺνλ λ¬Έμμ΄ λ‘ μ½λλ₯Ό λ¬Έμν νκΈ°μν΄ μ¬μ©λλ€. λ³΄ν΅ """ """λ₯Ό μ΄μ©νμ¬ μμ±λκ³  `__doc__` μμ±μ΄λ `help()` λ΄μ₯ ν¨μλ‘ μ κ·Όν  μ μμ΅λλ€.

λ³΄ν΅ μ²«μ€μλ κ°λ¨ν μ€λͺ, κ·Έ λ€μ μμΈν μ€λͺμ μ κ³  μΆκ°μ μΌλ‘ Parameterλ μ΄λ€κ² μλμ§ μ΄λ€κ°μ return νλμ§λ₯Ό μΆκ°μ μΌλ‘ μ λλ€.

μμ

```python
def function_with_pep484_type_annotations(param1: int, param2: str) -> bool:
    """Example function with PEP 484 type annotations.

    The return type must be duplicated in the docstring to comply
    with the NumPy docstring style.

    Parameters
    ----------
    param1
        The first parameter.
    param2
        The second parameter.

    Returns
    -------
    bool
        True if successful, False otherwise.

    """
function_with_pep484_type_annotations.__doc__
help(function_with_pep484_type_annotations)
```

μΆκ°

- sphinxλΌλ νλ‘κ·Έλ¨ μ΄μ©νλ©΄ Docstring μλμΌλ‘ λ¬Έμν Pytorch κ³΅μλ¬Έμ λν μ΄λ¬ν λ°©μμΌλ‘ μμ± λλ―
- Docstring Guide κ³ μ λκ±΄ μλλ―..

#### Reference

- [μ½λ©νλν­κ· λ΅λ³](https://github.com/boostcamp-ai-tech-4/ai-tech-interview/blob/main/answers/4-python.md)
- [Sphinx μ© numpydoc νμ₯κ³Ό ν¨κ» μ¬μ©λλ λμ€νΈλ§](https://numpydoc.readthedocs.io/en/latest/format.html)

## #33

### What is the purpose of is, not and in operators?

`is`λ κ°μ²΄λ₯Ό λΉκ΅νλ **Identity Operator**μλλ€.

```python
# κ°μΌλ©΄
a = 1
b = 1
print(a is b) # True
```

```python
# λ€λ₯΄λ©΄
a = 1
b = 2
print(a is b) # False
```

`not`μ logic valueλ₯Ό λ°λλ‘ returnνλ **Logical Operator**μλλ€.

```python
print(not True) # False
```

`in`μ valueκ° sequenceμ μλμ§ νμΈνλ **Membership Operator**μλλ€.

```python
purple_list = ['Purple', 'Lavandula', 'Bora']
print('Red' in purple_list) # False
```

#### Reference

- [Python Operators](https://www.w3schools.com/python/python_operators.asp)

## #34

### What is the usage of help() and dir() function in Python?

`help()` λ docstringμ μμ±νμλ€λ©΄ docstringμ μΆλ ₯νλ€.

```python
def myfunc(x):
	  """xμ 1μ λν΄μ μΆλ ₯νλ ν¨μ

    Args:
        x (int): [intν μ μ]

    Returns:
        x+1: [xμ 1μ λν΄μ λ¦¬ν΄]
    """
    return x+1

help(myfunc) # docstringμ΄ μΆλ ₯λ¨
```

`dir()` μ μΈμλ‘ λ£μ κ°μ²΄μ μμ±κ³Ό λ©μλλ₯Ό λ¬Έμμ΄λ‘ λ³ννκ³  κ·Έκ²μ μμλ‘ κ°λ μ λ ¬λ λ¦¬μ€νΈλ₯Ό λ°ννλ€. `dir` μ μ¬μ©ν  κ°μ²΄μ λ©μλμ μμ±μ λν μ λ³΄λ₯Ό μ»κ³  μΆμ λ μ μ©νλ€. λ€λ§ μΈμκ° μλ€λ©΄ νμ¬ μ§μ­ μ€μ½νμμ μ μλ ν¨μμ λ³μλ€μ λ¦¬μ€νΈλ₯Ό λ°ννλ€.

```python
def myfunc(x):
  return x

a = 3
print(dir(a)) # ['__abs__', '__add__', '__and__', '__bool__', '__ceil__', '__class__', ...]
print(dir(myfunc)) # ['__annotations__', '__call__', '__class__', '__closure__', '__code__', ]
print(dir()) # ['In', 'Out', '_', '__', '___', '__builtin__', '__builtins__',...]

print(a.__add__(3)) # 6
```

## #35

### Whenever Python exits, why isnβt all the memory de-allocated?

νμ΄μ¬μ΄ μ’λ£λλ©΄ νμ΄μ¬μ λ΄μ₯λ λ§€μ»€λμ¦μ΄ μλνμ¬ λ€λ₯Έ κ°μ²΄λ₯Ό ν λΉ ν΄μ νλ €κ³  μλν©λλ€.

νμ§λ§ CλΌμ΄λΈλ¬λ¦¬μμ μμ½ν λ©λͺ¨λ¦¬λΆλΆμ ν λΉ ν΄μ ν  μ μκΈ° λλ¬Έμ λ€λ₯Έ κ°μ²΄ λλ μ μ­ λ€μμ€νμ΄μ€μμ μ°Έμ‘°λλ κ°μ²΄μ λν **μν μ°Έμ‘°**κ° μλ νμ΄μ¬ λͺ¨λμ΄ ν λΉ ν΄μ λμ§ μμ΅λλ€.

#### Reference

- [Whenever Python exits, all the memory isnβt deallocated. Why is it so?](https://madanswer.com/48777/whenever-python-exits-all-the-memory-isnt-deallocated-why-is)

## #36

### What is a dictionary in python?

immutableν keyμ mutableν valueλ‘ λ§΅νλμ΄ μλ€.

νμ΄μ¬ 3.6λΆν° μλ ₯ν μμκ° μ μ§λλ€.

#### Reference

- [dictionary](https://wikidocs.net/16043)

## #37

### How can the ternary operators be used in python?

λλΆλΆ λ€λ₯Έ μΈμ΄μμλ conditionμ΄ μ°Έμ΄λ©΄ true_value κ°μ κ±°μ§μ΄λ©΄ false_value κ°μ μ·¨ν¨

```java
[condition] ? [true_value] : [false_value]
```

νμ΄μ¬μμλ μ νν μ§μ X. μλμ κ°μ΄ μ¬μ©

```python
[true_value] if [condition] else [false_value]
```

μμ

```python
n=155
value = 'ten' if n==10 else 'not ten'
# value = 'not ten'
```

#### Reference

- [PEP 308: Conditional Expressions](https://docs.python.org/2.5/whatsnew/pep-308.html)

## #38

### What does this mean: `*args`, `**kwargs`? And why would we use it?

### \*args

`*args`λ `*arguments`μ μ€μλ§λ‘ argsλ₯Ό κΌ­ μ¬μ©ν  νμ μμ΄ \*λ§ λΆμ΄λ©΄ λλ€.

`*args`λ ν¨μμ μ λ¬λλ argumentμ μλ₯Ό μ μ μκ±°λ, listλ tupleμ argumentλ₯Ό ν¨μμ μ λ¬ν  λ μ¬μ©νλ€.

```python
def name(*args):
    print(args)

name('λ―Όκ·', 'μ¬μ±', 'μ±λ―Ό', 'λκ²½', 'μ¬ν', 'λμ§')
```

```
('λ―Όκ·', 'μ¬μ±', 'μ±λ―Ό', 'λκ²½', 'μ¬ν', 'λμ§')
```

### \*\*kwargs

`**kwargs`λ `**keyword arguments`μ μ€μλ§λ‘ μ­μ \*\*λ€μ μ΄λ¦μ λ€λ₯΄κ²ν΄λ μκ΄μλ€.

`**kwargs`λ ν¨μμ μ λ¬λλ keyword argumentμ μλ₯Ό λͺ¨λ₯΄κ±°λ, dictionaryμ keyword argumentλ€μ ν¨μμ μ λ¬ν  λ μ¬μ©νλ€.

```python
def name(**kargs):
    print(kwargs)

name( m = 'λ―Όκ·', n = 'λκ²½', d = 'λμ§', j = 'μ¬μ±', s = 'μ±λ―Ό')
```

```
{'m': 'λ―Όκ·', 'n': 'λκ²½', 'd': 'λμ§', 'j': 'μ¬μ±', 's': 'μ±λ―Ό'}
```

\*argsμ \*\*kargsλ₯Ό ν¨κ» μ¬μ©ν  λλ argsκ° kwargsλ³΄λ€ μμμ¨λ€.

## #39

### What does len() do?

νμ΄μ¬ κ³΅μλ¬Έμ

> Return the length (the number of items) of an object. The argument may be a sequence (such as a string, bytes, tuple, list, or range) or a collection (such as a dictionary, set, or frozen set).

λ²μ­νμλ©΄ κ°μ²΄μ κΈΈμ΄(μμ΄νμ μ)λ₯Ό λ¦¬ν΄νλ€.

```python
a = '123'
b = [1, 2, 3]
c = {'first': 1, 'second':2}

print(len(a)) # 3
print(len(b)) # 3
print(len(c)) # 2
```

## #40

### Explain split(), sub(), subn() methods of βreβ module in Python.

`re` moduleμ νμ΄μ¬μ μ κ·ννμ λͺ¨λμλλ€. μ κ·ννμμ λ΄μ λ¬Έμμ΄μ μ²λ¦¬νκΈ° μν΄ `re.split()`, `re.sub()`, `re.subn()` λ©μλλ₯Ό μ¬μ©ν©λλ€.

- re.split(pattern, string))
  - patternμ κ΅¬λΆμλ‘ stringμ λΆλ¦¬νμ¬ λ¦¬μ€νΈλ‘ λ°νν©λλ€.

```python
>>> re.split('<[^<>]*>', '<html> Wow <head> header </head> <body> Hey </body> </html>')
['', ' Wow ', ' header ', ' ', ' Hey ', ' ', '']
```

- re.sub(pattern, repl, string[, count=0])
  - stringμμ patternκ³Ό μΌμΉνλ λΆλΆμ λνμ¬ replλ‘ κ΅μ²΄νμ¬ κ²°κ³Ό λ¬Έμμ΄μ λ°νν©λλ€.

```python
>>> re.sub('\d{4}', 'XXXX', '010-1234-5678')
'010-XXXX-XXXX'
```

- re.subn(pattern, repl, string, count=0)
  - subμ λμΌνλ, κ²°κ³Όλ‘ (κ²°κ³Όλ¬Έμμ΄, λ§€μΉ­νμ)λ₯Ό ννλ‘ λ°νν©λλ€.

```python
>>> re.subn('\d{4}', 'XXXX', '010-1234-5678')
('010-XXXX-XXXX', 2)
```

#### Reference

- [νμ΄μ¬ μ κ·ννμ λͺ¨μ](https://devanix.tistory.com/296)
- [νμ΄μ¬ μ κ·ννμ μ€κΈ](<https://greeksharifa.github.io/%EC%A0%95%EA%B7%9C%ED%91%9C%ED%98%84%EC%8B%9D(re)/2018/08/04/regex-usage-05-intermediate/>)

## #41

### What are negative indexes and why are they used?

negative indexλ indexλ‘ μ κ·Όν  μ μλ containerμμ(list, tuple, string...) μμμ΄ μλ λμμλΆν° μ κ·Όν μ μλλ‘ ν΄μ£Όλ λ°©λ²μλλ€. containerμ λ§μ§λ§ elementμ indexκ° -1μ΄κ³  λ€μμ μμΌλ‘ μ¬ μλ‘ -1μ© indexκ° κ°μν©λλ€.

λμ±λ ν¨μ¨μ΄ μ’κ³  κ°λμ±μ΄ μ’μλκ° μμ΅λλ€.

```python
>>> l = [0,1,2,3,4,5] # negative index [-6,-5,-4,-3,-2,-1]
# ex-1
>>> l[-1]
5
>>> l[len(l) - 1]
5

# ex-2
>>> l = [0,1,2,3,4,5]
>>> l[-3:-1]
[3,4]

# ex-3
>>> l = [0,1,2,3,4,5]
>>> l[-1:-4:-1]
[5,4,3]

```

#### Reference

- [What is negative index in python from Quora](https://www.quora.com/What-is-negative-index-in-Python)

## #42

### What are Python packages?

#### μλ―Έ

Python packageλ μ¬λ¬ moduleλ‘ κ΅¬μ±μ΄ λλ€.

Packageλ moduleμ ν¬ν¨νλ ν΄λμ΄λ©° κ·Έ μμ λ λ§μ ν΄λμ λͺ¨λμ ν¬ν¨ ν  μλ μλ€.

κ°λμ μΌλ‘λ namespaceλ‘ λ³Ό μ μλ€. μ¦, ν¨ν€μ§μ λͺ¨λμ΄ μ°Έμ‘°λ  μ μλ ν¨ν€μ§ μ΄λ¦μΌλ‘ ν¨κ» λ¬Άμ¬ μμμ μλ―Έ

#### κ΅¬μ±

Package ν΄λμλ μΌλ°μ μΌλ‘ Pythonμ "μ΄ λλ ν λ¦¬λ packageμλλ€!" λΌκ³  μλ €μ£Όλ `__init__.py` κ° νλ λ€μ΄κ° μλ€.

`__init__.py` μ΄ νμΌ μμλ μ½λκ° μμ΄ λΉμ΄ μμ μλ μκ³ , package μ΄κΈ°νμ μ€νν  μ½λκ° ν¬ν¨ λ  μλ μλ€.

##### namespace

: λ³μ μ΄λ¦μ΄λ ν¨μ μ΄λ¦κ³Ό κ°μ΄ λͺμΉ­μ μ¬μ©νλ κ³΅κ°, μμμ νλλΈλ€κ³  ννν  μ μλ€.

#### Reference

- [What Is a Python Package?](https://www.udacity.com/blog/2021/01/what-is-a-python-package.html)
- [namespace κ΄λ ¨](https://thinkpro.tistory.com/22)

## #43

### How can files be deleted in Python?

os λͺ¨λμ import νκ³ , os.remove()ν¨μλ₯Ό μ¬μ©νμ¬ νμΌμ μ­μ νλ€.

```python
import os
os.remove('interview.txt')
```

- os.rmdir() : μΈμκ°μΌλ‘ μ­μ ν  λλ ν λ¦¬ κ²½λ‘λ₯Ό λ°λλ€. μ΄λ ν΄λΉ λλ ν λ¦¬κ° λΉμ΄μμΌλ©΄ μ­μ λκ³  νμΌμ΄ μμΌλ©΄ μλ¬κ° λλ€.
- shutil.rmtree: λλ ν λ¦¬ λ° νμΌμ λͺ¨λ μ§μ΄λ€. λλ ν λ¦¬μ νμΌμ΄ μλλΌλ μλ¬λ₯Ό λ°μμν€μ§ μκ³  μ­μ νλ€.

#### Reference

- [How to Delete a File in Python](https://www.dummies.com/programming/python/how-to-delete-a-file-in-python/)
- [νμ΄μ¬ λλ ν λ¦¬ λ° νμΌ μ­μ ](https://hongku.tistory.com/305)

## #44

### What are the built-in types of python?

- bulit-in type of python : νμ΄μ¬ λ΄μ₯ μλ£ν
  - bulit-in type μ€μμλ mutableν μλ£νλ μκ³ , bulit-in methoodλ₯Ό νμ©ν΄ νΈλ¦¬νκ² programmingμ ν  μ μμ΅λλ€.
- boolean, numeric type, sequence type, text type, binary sequence type, set type, mapping type λ±μ΄ μμ΅λλ€.

#### ##1 boolean type

- FalseμΈ κ²½μ°
  - None
  - zero of any numeric
    - 0, 0.0
    - 0j : complex, λ³΅μμ
    - Decimal(0) : μ­μ§λ² λΆλμμμ 
    - Fraction(0, 1) : μ λ¦¬μ, Fraction(λΆμ, λΆλͺ¨)
  - empty sequences and collections
    - ''
    - ()
    - []
    - {}
    - set()
    - range(0)

#### ##2 numeric type

- int
- float
- complex : λ³΅μμ

#### ##3 sequence type

- list
- tuple
- range

#### ##4 text sequence type

- str

#### ##5 binary sequence types

- bytes
- bytearray
- memoryview

#### ##6 set type

- set
- frozenset : μμ  λΆκ°λ₯ν set
  - tupleμ setλ²μ 

#### ##7 mapping type

- dictionary

#### Reference

- [ python document : built in type](https://docs.python.org/3/library/stdtypes.html)

## #45

### What advantages do NumPy arrays offer over (nested) Python lists?

Pythonμ λ°°μ΄(array)λ₯Ό μ§μνμ§ μλλ€. μΌλ°μ μΌλ‘ μ°©κ°νκΈ° μ¬μ΄ λΆλΆμΌλ‘ Listμ Arrayλ μ ννλ λ€λ₯Έ κ²μ΄λ€. λν `Numpy`λ₯Ό μ¬μ©νλ©΄ `Array`λ₯Ό Pythonμμ μ¬μ©ν  μ μλ€.

**Array**

- μ μ ν λΉ(κ³ μ λ ν¬κΈ°λ₯Ό κ°λλ€. Sizeλ₯Ό λ³ννλ €λ©΄ κΈ°μ‘΄μ arrayλ₯Ό μ­μ νκ³  μλ‘μ΄ arrayλ₯Ό μμ±ν΄μΌ ν¨)

**List**

- λμ ν λΉ(κ³ μ λ ν¬κΈ°λ₯Ό κ°μ§ μκ³  λμ μΌλ‘ Size μ‘°μ μ΄ κ°λ₯ν¨)

#### NumPy Arrayμ μ₯μ 

- κ°λ ₯ν N-μ°¨μ λ°°μ΄ κ°μ²΄λ₯Ό μ¬μ©ν  μ μλ€.
- C μΈμ΄ λ² μ΄μ€λ‘ μμ±λμ΄ μκΈ° λλ¬Έμ λ©λͺ¨λ¦¬λ₯Ό ν¨κ³Όμ μΌλ‘ μ¬μ©νλ©° λΉ λ₯΄λ€.
- λ€λ₯Έ λΌμ΄λΈλ¬λ¦¬μ μ°κ΄μ±μ΄ λ§€μ° λλ€. λ€μν νμ΄μ¬ ν¨ν€μ§λ€μ΄ numpyμ ndarrayλ₯Ό κΈ°λ³Έ μλ£νμΌλ‘ μ¬μ©νλ€.
- μ κ΅ν λΈλ‘λμΊμ€ν κΈ°λ₯
- μ νλμ, νΈλ¦¬μ λ³ν, λμ κΈ°λ₯μ΄ μ μ©νλ€.
- Forλ¬Έκ³Ό κ°μ΄ λ°λ³΅μ μΈ μ°μ° μμμ vectorized operationμ μ¬μ©νμ¬ ν¨μ¨μ μΈ μ½λ©μ΄ κ°λ₯νλ€.

#### References

- https://medium.com/@5eo1ab/numpy-%EC%93%B0%EB%8A%94-%EC%9D%B4%EC%9C%A0-37895f4fdc03
- https://chancoding.tistory.com/10

## #46

### How to add values to a python list?

**append()**, **extend()** κ·Έλ¦¬κ³  **insert (i,x)** ν¨μλ₯Ό μ΄μ©νμ¬ valuesλ₯Ό λν  μ μλ€.

- `By using append() function`: arrayμ λμλ€κ° elementsλ₯Ό λνλ€.
- `By using insert() function`: μ£Όμ΄μ§ indexμ elementsλ₯Ό λ£λλ€.
- `By using extend() function`: λ¦¬μ€νΈμ elementsλ₯Ό λΆμμΌλ‘μ¨ λ¦¬μ€νΈλ₯Ό μλλ€.

- `By using + operator`: λ μ΄λ μ΄λ₯Ό elementμ concatνλ€. (list, array ν΄λΉ, numpy arrayμ΄λ element λ§μ)

**append**

```python
import array

s1 = array.array('i', [1, 2, 3])
s2 = array.array('i', [4, 5, 6])

s3 = s1 + s2
print(s3)
>> array.array('i', [1, 2, 3, 4, 5, 6])

s1.append(4)
print(s1)
>> array.array('i', [1, 2, 3, 4])
# a = [1,2,3]; b = [4, 5, 6]
# a.append(4) -> [1,2,3,4]
# a.append(b) -> [1,2,3,[4,5,6]]

s1.insert(0, 10)
print(s1)
>> array.array('i', [10, 1, 2, 3, 4])

s1.extend(s2)
print(s1)
>> array.array('i', [10, 1, 2, 3, 4, 4, 5, 6])
```

#### Reference

- [Python add elements to an array](https://www.askpython.com/python/array/python-add-elements-to-an-array)

## #47

### How to remove values to a python array?

ν¬κ² 4κ°μ§μ λ°©λ²μΌλ‘ arrayμ κ°μ μ κ±°ν  μ μλ€.

#### list.pop()

`list.pop()` : Indexλ₯Ό μ¬μ©νμ¬ Listμ elementλ₯Ό μ κ±°ν  μ μλ€

```python
a_list = ["a", "b", "c"]
a_list.pop(1)
print(a_list)
# ['a', 'c']
```

#### del

`del` : `pop()`κ³Ό κ°μ΄ indexλ₯Ό μ¬μ©νμ¬ Listμ elementλ₯Ό μ κ±° ν  μ μλ€.

```python
a_list = ["a", "b", "c"]
del a_list[1]

print(a_list)
# ['a', 'c']
```

#### list.remove()

`list.remove(value)` : listμμ κ°μ₯ λ¨Όμ  λνλλ valueλ₯Ό μ κ±°

```python
a_list = ["a", "b", "c"]
a_list.remove("b")

print(a_list)
# ['a', 'c']
```

#### np.delete()

`np.delete(arr, obj)` : numpy arrayμμ elementλ₯Ό μ κ±°

`arr` μμ index `obj` μ elementλ₯Ό μ κ±°νλ€.

```python
array = np.array([1, 2, 3])
array = np.delete(array, 2)

print(array)
[1 2]
```

#### Reference

- [How to remove an element from an array in Python](https://www.kite.com/python/answers/how-to-remove-an-element-from-an-array-in-python)

## #48

### Does Python have OOps concepts?

classλΌλ κΈ°λ₯μ μ΄μ©ν΄μ κ°μ²΄λ₯Ό λ§λ€ μ μμ΅λλ€.

κ°μ²΄ μ§ν₯ νλ‘κ·Έλλ°μ νλ©΄ νλ‘κ·Έλ¨ λ³κ²½μ μ©μ΄νκ² ν  μ μμ΅λλ€.

κ°μ²΄ μ§ν₯μ νΉμ±

1. μΆμν

   κ°μ²΄λ€μ κ³΅ν΅μ μΈ νΉμ§(μμ±, κΈ°λ₯)μ λμΆνλ κ²μΌλ‘ ν΄λμ€λ₯Ό μ μνλ κ²μ΄λΌ ν  μ μλ€.

2. μΊ‘μν

   κ°μ²΄ λ΄λΆλ₯Ό μ¨κ²¨ μΈλΆλ‘λΆν°μ μμΈμ€λ₯Ό μ°¨λ¨. νμ΄μ¬μ μΊ‘μνλ₯Ό μ§μνμ§ μμ§λ§ μ½μμ κ°λμΌλ‘ λ³μμ μ§μ μ κ·Όμ λ§λλ€.

3. μμμ±

   λΆλͺ¨ ν΄λμ€λ₯Ό λ¬Όλ €λ°μ μ½λμ¬μ¬μ©μ±μ λμ.

4. λ€νμ±

   νλμ κ°μ²΄κ° μ¬λ¬κ°μ νμμ κ°λ¦¬ν¬ μ μλ κ². μμμ ν΅ν΄ μ΄λ£¨μ΄μ§ μ μμ.

#### Reference

- [κ°μ²΄ μ§ν₯ νλ‘κ·Έλλ° κ°λ1](https://seungjuitmemo.tistory.com/50)
- [κ°μ²΄ μ§ν₯ νλ‘κ·Έλλ° κ°λ2](https://seungjuitmemo.tistory.com/51)

## #49

### What is the difference between deep and shallow copy?

**Shallow copy**

- Shallow copyλ μλ‘μ΄ κ°μ²΄λ₯Ό λ§λ  νμ μλ³Έμ μ κ·Όν  μ μλ referenceλ₯Ό μλ ₯νλ€.
  - μ΄λ° κ²½μ° μλ‘ λ€λ₯Έ λ³μλͺμ΄μ§λ§ λ³Έμ§μ μΌλ‘ μλ‘ κ°μ λμμ μλ―Ένλ―λ‘ νλμ λ³μ μ­μ μμ μ΄ λλ€.
- κ°λ³ν(mutable) μλ£νμ λν΄μ μ μ©μ΄ κ°λ₯νλ€.
  - κ°λ³ν(mutable) μλ£νμ κ°μ μ£Όμμμ κ°(value)μ΄ λ³κ²½ κ°λ₯νκΈ° λλ¬Έμ μμ λ³΅μ¬κ° κ°λ₯νλ€.
  - λΆλ³ν(immutable) μλ£νμ λ³Έμ§μ μΌλ‘ λ³κ²½μ΄ λΆκ°λ₯νλ―λ‘ μ¬λ°°μ μ ν΅ν΄ λ³μλ₯Ό λ°κΎΌλ€. λ°λΌμ μ¬λ°°μ μ΄ μ΄λ£¨μ΄μ§λ―λ‘ κ°μ²΄κ° μλ‘ λ¬λΌμ§λ€.

```python
a = [1,2,3]
b = a
a[1] = 0
print(a, b)
```

```
[0,2,3] [0,2,3]
```

**Deep copy**

- Deep copyλ λ΄λΆμ κ°μ²΄λ€κΉμ§ λͺ¨λ μλ‘­κ² copy νλ€.
  - μλ‘ κ°λ§ κ°μ λΏ λ³Έμ§μ μΌλ‘ μλ‘ λ€λ₯΄κΈ° λλ¬Έμ ν λ³μκ° μμ λ  μ λ€λ₯Έ λ³μκ° μμ λμ§ μλλ€.
  - copy.deepcopyλ©μλλ₯Ό μ¬μ©νλ€.

```python
import copy

a = [1,2,3]
b = cop.deepcopy(a)
a[1] = 0
print(a, b)
```

```
[0,2,3] [1,2,3]
```

#### Reference

- [νμ΄μ¬ - κΈ°λ³Έμ κ°κ³  λ¦μ!](https://wikidocs.net/16038)

## #50

### How is multithreading achieved in python?

pythonμ multithreadingλͺ¨λμ threadingλͺ¨λ(high level)κ³Ό threadλͺ¨λ(low level)μ΄ μμ§λ§, μ§κΈμ μ£Όλ‘ threadingλͺ¨λμ μ¬μ©ν©λλ€.

multi threadingμ μ¬μ©νλ©΄ λ³λ ¬μ  μ²λ¦¬ λλΆμ μλκ° λΉ¨λΌμ§λ€κ³  μκ°νκ² μ§λ§ pythonμ GIL(Global Interpreter Lock)μ μ± λλ¬Έμ μλλ single threadingκ³Ό λ³λ° μ°¨μ΄κ° μμ΅λλ€.

νλμ μμμ μ¬λ¬ νλ‘μΈμ€κ° μλ¬΄λ° κ·μΉμμ΄ μ κ·Όνλ©΄, μμ λκΈ°ν λ¬Έμ κ° λ°μν  μ μμ΅λλ€. μ΄λ₯Ό λ°©μ§νκΈ° μν΄μ μμμ lockμ λλλ°, Pythonμ λͺ¨λ  μμμ lockμ globalνκ² κ΄λ¦¬νκ³  μμ΅λλ€. κ·Έλμ pythonμ μ°λ λ νλμ CPUμμμ λ€ μ°κΈ° λλ¬Έμ multithreadingμ μ΄μ μ μ¨μ ν κ°μ Έμ¬ μ μμ΅λλ€.

νμ§λ§ I/Oμμμ CPUμμμ΄ μλλΌμ GIL μν₯μ λ°μ§ μμ΅λλ€. κ·Έλμ I/Oμμ(μμΆλ ₯, νμΌ λ€μ΄λ‘λ λ±)μΌλ‘ μ΄λ£¨μ΄μ§ μμμ multi threadingμΌλ‘ μ±λ₯μ κ°μ ν  μ μμ΅λλ€. μ°Έκ³ λ‘ νμΌμ°κΈ°λ I/Oμμμ΄ μλλλ€.

λΆκ°μ μΌλ‘ pythonμ multiprocessingλͺ¨λμ multiprocessingλͺ¨λ, concurrentλͺ¨λ λ±μ΄ μμ΅λλ€.

#### Reference

- [python multithreading, multiprocessing](https://monkey3199.github.io/develop/python/2018/12/04/python-pararrel.html)

- [python multithreading, multiprocessing μ¬μ΄ μμ ](https://zephyrus1111.tistory.com/111)

- [μμ λ‘ λ°°μ°λ νμ΄μ¬ νλ‘κ·Έλλ° - μ°λ λ (Thread)](http://pythonstudy.xyz/python/article/24-%EC%93%B0%EB%A0%88%EB%93%9C-Thread)

## #51

### What is the process of compilation and linking in python?

νμ΄μ¬ νμΌ(.py)λ₯Ό μ€ννλ©΄, μμ€ μ½λλ λ°μ΄νΈ μ½λ(byte code)λ‘ λ³νλλ©°, `.pyc` , `.pyo` νμΌ νμμΌλ‘ μ μ₯λλ€. μ΄ λ μμ€ μ½λλ₯Ό λ°μ΄νΈ μ½λλ‘ λ³ννλ κ³Όμ μ **μ»΄νμΌ(compilation) λ¨κ³** λΌκ³  νλ€.

νμ΄μ¬ κ°μλ¨Έμ (Python Virtual Machine)μ΄ λ°μ΄νΈ μ½λλ₯Ό κΈ°κ³μ΄(Machine code)λ‘ λ³ννμ¬ μ΄λ€ μ΄μμ²΄μ λ  μ€νν  μ μλλ‘ νλ€. μ΄ λ μ°λ¦¬μ μ½λμ μΈν°νλ¦¬ν°κ° νμν λΌμ΄λΈλ¬λ¦¬λ₯Ό μ°κ²°μν€λ κ³Όμ μ΄ μλλ°, μ΄λ₯Ό **λ§ν¬(linking) λ¨κ³**λΌκ³  νλ€.

μ°Έκ³  `dis` λͺ¨λμ μ¬μ©νμ¬ μμ€ μ½λκ° μ΄λ€ λ°μ΄νΈ μ½λλ‘ λ³νλλμ§ νμΈν  μ μλ€.

> μμ€μ½λ

```python
import dis

def mult(a, b):
  return a*b

dis.dis(mult)
```

> μΆλ ₯ κ²°κ³Ό

```shell
4				0 LOAD_FAST				0 (a)
				2 LOAD_FAST				1 (b)
				4 BINARY_MULTIPLY
				6 RETURN_VALUE
```

#### References

- https://www.tutorialspoint.com/what-is-the-process-of-compilation-and-linking-in-python
- https://github.com/boostcamp-ai-tech-4/ai-tech-interview/blob/main/answers/4-python.md#51

## #52

### What are Python libraries? Name a few of them.

- Module: λͺ¨λμ κΈ°λ³Έμ μΌλ‘ νμ₯μκ° .pyμΈ νμΌμ μ μ₯λ κ΄λ ¨ μ½λ λ¬Άμ, ν¨μ, ν΄λμ€, λ³μλ±μ΄ μ μ λμ΄ μλ€.
- Packages: Python ν¨ν€μ§λ κΈ°λ³Έμ μΌλ‘ λͺ¨λμ λͺ¨μλ λλ ν λ¦¬, \_\_init\_\_.py μ μ λμ΄ μμ
- libraray: Python λΌμ΄λΈλ¬λ¦¬μλ κ΄λ ¨ λͺ¨λ λ° ν¨ν€μ§ λͺ¨μ, μ’μ’ Packageλ λμΌν μλ―Έλ‘ μ°μΈλ€.(packageλ subpackage ν¬ν¨ κ°λ₯) κ·Έλ¬λ μΌλ°μ μΌλ‘ ν¨ν€μ§λ λͺ¨λ λͺ¨μμ΄κ³  λΌμ΄λΈλ¬λ¦¬λ ν¨ν€μ§ λͺ¨μ
  - Matplotlb, Pytorch, Beautiful Soup, ..
- Franework: Python νλ μμν¬λ νλ‘κ·Έλλ¨Έκ° κ°λ° νλ‘μΈμ€λ₯Ό λΉ λ₯΄κ² μΆμ νλ λ° λμμ΄ λλ λͺ¨λ λ° ν¨ν€μ§ λͺ¨μ, νλ μμν¬λ μΌλ°μ μΌλ‘ λΌμ΄λΈλ¬λ¦¬λ³΄λ€ λ λ³΅μ‘, λΌμ΄λΈλ¬λ¦¬μλ νΉμ  μμμ μννλ ν¨ν€μ§κ° ν¬ν¨λμ΄ μμ§λ§ νλ μμν¬μλ μ νλ¦¬μΌμ΄μμ κΈ°λ³Έ νλ¦κ³Ό μν€νμ²κ° ν¬ν¨
  - Flask, Django, Bottle

#### Reference

- [Difference Between Python Modules, Packages, Libraries, and Frameworks](https://learnpython.com/blog/python-modules-packages-libraries-frameworks/)
- [νλ μμν¬μ λΌμ΄λΈλ¬λ¦¬μ μ°¨μ΄μ ](https://webclub.tistory.com/458)

## #53

### What is split used for?

Stringμ κ° μ§μ ν `separator` λ₯Ό κΈ°μ€μΌλ‘ λλ λ¨μ΄λ€μ listλ‘ λ§λ€μ΄ μ€λ€.

```python
string.split(separator, maxsplit)
```

`separator` : λ¬Έμμ΄μ λλ λ μ¬μ©ν  κ΅¬λΆ κΈ°νΈ, default : whitespace(κ³΅λ°± κΈ°νΈ)

`maxsplit` : λͺ κ°λ‘ λλμ§ μ§μ , default : -1 (λμμ§λ λͺ¨λ  κ²½μ°)

#### Reference

- [Python String split() Method](https://www.w3schools.com/python/ref_string_split.asp)

## #54

### How to import modules in python?

νμ΄μ¬ νμ₯μ .pyλ‘ λ§λ  νμ΄μ¬ νμΌμ λͺ¨λ λͺ¨λμ΄λ€.

```python
import [module]
```

module.pyλΌλ νμΌμ importν  λ μμ κ°μ΄ μ¬μ©ν  μ μλ€.

module.pyμμ μλ ν¨μλ₯Ό μ¬μ©νλ €λ©΄

```python
module.add(1,2)
```

κ³Ό κ°μ΄ μ¬μ©ν΄μΌ νλ€.

module.add() κ° μλ add() λ‘ μ¬μ©νκ³  μΆλ€λ©΄

```python
from module import add
```

μ κ°μ΄ import ν΄μΌ νλ€.

```python
from module import *
```

μΌλ‘ μ¬μ©νλ©΄ moduleνμΌμμ μλ λͺ¨λ  ν¨μλ₯Ό add() , sub()λ±μΌλ‘ νμΌ μ΄λ¦μ μ λΆμ΄κ³  μ¬μ©ν  μ μλ€.

νΉμ  λλ ν°λ¦¬μ λͺ¨λ λͺ¨λλ₯Ό \*μ μ΄μ©νμ¬ import ν  λλ λλ ν°λ¦¬\_\_init\_\_.py

μ \_\_all\_\_ λ³μλ₯Ό μ€μ νκ³  λͺ¨λμ μ μν΄ μ£Όμ΄μΌ νλ€.

```python
>>> import sys
>>> sys.path
[..., `'/usr/lib/python36.zip'`, `'/usr/lib/python3.6'`, `'/usr/lib/python3.6/lib-dynload'`,
`'/usr/local/lib/python3.6/dist-packages'`, `'/usr/lib/python3/dist-packages'`]

```

sys.pathλ νμ΄μ¬ λΌμ΄λΈλ¬λ¦¬λ€μ΄ μ€μΉλμ΄ μλ λλ ν°λ¦¬λ€μ λ³΄μ¬ μ€λ€. νμ΄μ¬ λͺ¨λμ΄ μμ λλ ν°λ¦¬μ λ€μ΄ μλ€λ©΄ λͺ¨λμ΄ μ μ₯λ λλ ν°λ¦¬λ‘ μ΄λν  νμμμ΄ λ°λ‘ λΆλ¬μ μ¬μ©ν  μ μλ€.

νμ¬ κ²½λ‘μ μλ /opt/ml/detection.pyλ₯Ό μ¬μ©νλ €κ³  ν λ

```python
import sys
sys.path.append("/opt/ml")
import detction
```

κ³Ό κ°μ΄ μ¬μ©ν  μ μλ€.

νμ΄μ¬ μ½λ λ΄μμ μμ²λΌ μ¬μ©νλ€λ©΄, μ½λ λ°μμ sys.pathλ₯Ό μ‘°μν  μ μλ€.

PYTHONPATHλ₯Ό μ΄μ©νμ¬ sys.pathμ κ²½λ‘λ₯Ό λμμ μ¬λ¬κ° μΆκ°ν  μ μλ€.

μλμ°μμλ /foo;/bar κ³Ό κ°μ΄ κ²½λ‘λ₯Ό κ΅¬λΆν  μ μλ€.

<div align='center'>
     <img src="./images/54.PNG">
   </div>

#### Reference

- [λͺ¨λ](https://wikidocs.net/29)
- [ν¨ν€μ§](https://wikidocs.net/1418#9595all9595)
- [sys.path,PYHONPATH](https://www.bangseongbeom.com/sys-path-pythonpath.html)

## #55

### Explain Inheritance in Python.

#### Inheritance

ν΄λμ€μμ μμμ΄λ λ¬Όλ €μ£Όλ ν΄λμ€(**Parent Class, Super class**)μ λ΄μ©(**μμ±κ³Ό λ©μλ**)μ λ¬Όλ €λ°λ ν΄λμ€(**Child class, sub class**)κ° κ°μ§κ² λλ κ²μ΄λ€.

νμ΄μ¬μ λΆλͺ¨ ν΄λμ€ A λ₯Ό μμ ν΄λμ€ B κ° μμνλ **Single Inheritance**, λΆλͺ¨ ν΄λμ€ A λ₯Ό μμ ν΄λμ€ B κ° λ€μ B λ₯Ό μμ ν΄λμ€ C κ° μμνλ **Multi-level Inheritance**, λΆλͺ¨ ν΄λμ€ A κ° μ¬λ¬ μμ ν΄λμ€μ μμλλ **Hierarchical Inheritance**, νλμ μμ ν΄λμ€κ° μ¬λ¬ λΆλͺ¨ ν΄λμ€λ₯Ό μμνλ **Multiple Inheritance** κ° μλ€.

#### Reference

- [νμ΄μ¬ - κΈ°λ³Έμ κ°κ³  λ¦μ!](https://wikidocs.net/16073)

## #56

### How are classes created in Python?

pythonμμλ `class`ν€μλλ₯Ό νμ©ν΄μ classλ₯Ό λ§λ€ μ μμ΅λλ€.

`__init__`μ΄λΌλ magic methodλ₯Ό νμ©ν΄ κ°μ²΄(instance)κ° μ μΈλ  λ λ©€λ²λ³μλ€μ μ΄κΈ°ν ν  μ μμ΅λλ€.

λν class methodλ₯Ό μ μν  λ, μ²« μΈμλ ν­μ `self`μ¬μΌ ν©λλ€. κ·Έ μ΄μ λ [python #19](#19)μ μ λ¦¬λμ΄ μμ΅λλ€. κ°λ¨νκ² μΈκΈνμλ©΄ selfμ κ°μ²΄(instance)λ₯Ό λ΄μ λκ³ , instanceμ methodλ₯Ό μ€νν  λ selfκ° νμνκΈ° λλ¬Έμλλ€.

μλ μμλ₯Ό λ³΄μλ©΄ μ²μμ `FourCal`λΌλ μ¬μΉμ°μ° ν΄λμ€λ₯Ό λ§λ€μμ΅λλ€.

κ·Έλ¦¬κ³  FourCal ν΄λμ€λ₯Ό `μμ(inheritance)`λ°λ `MoreFourCal`λΌλ ν΄λμ€λ₯Ό λ§λ€μμ΅λλ€. MoreFourCal ν΄λμ€μμλ FourCal ν΄λμ€μ methodλ₯Ό λͺ¨λ μ¬μ©ν  μ μμΌλ©°, μ κ³±μ°μ°μ νλ `pow` methodλ₯Ό μλ‘ μΆκ°ν  μ μμ΅λλ€. λν FourCal ν΄λμ€μ div methodλ₯Ό μ¬μ μνλ `method overriding`μ ν  μλ μλ΅λλ€.

```python
class FourCal:
     def __init__(self, first, second):
         self.first = first
         self.second = second
     def setdata(self, first, second):
         self.first = first
         self.second = second
     def add(self):
         result = self.first + self.second
         return result
     def mul(self):
         result = self.first * self.second
         return result
     def sub(self):
         result = self.first - self.second
         return result
     def div(self):
         result = self.first / self.second
         return result


class MoreFourCal(FourCal): # Inheritance FourCal class
   def pow(self): # set new method
      result = self.first ** self.second
      return result
   def div(self): # method overriding : div -> floor div
      result = self.first // self.second
      return reslut
```

#### Reference

- [μ νν¬νμ΄μ¬ class](https://wikidocs.net/28)

## #57

### What is monkey patching in Python?

μ£Όλ‘ νμ€νΈλ₯Ό μν΄ λ§μ΄ μ¬μ©λλ λ°©λ²μΌλ‘, μ΄λ€ ν΄λμ€λ λͺ¨λμ μΌλΆ (ν¨μλ λ³μ λ±)λ₯Ό λ‘μ»¬μμ λ°νμμΌλ‘λ§ instanceλ₯Ό ν΅ν΄ μμ νλ λ°©λ²μ λ§νλ€.

μμλ‘ test.py νμΌμ A ν΄λμ€μ a λΌλ ν¨μκ° μλλ°, λ€λ₯Έ νμΌμμ Aλ₯Ό importνμ¬ a ν¨μ λμ  new_aλ₯Ό ν λΉνμ¬ μ¬μ©νλ λ°©λ²μ΄ μλ€.

```python
from test import A

A.a = new_a
my_A = A() # A ν΄λμ€ κ°μ²΄ ν λΉ
my_A.a # new_aκ° λμ
```

Monkey patchingμ μμ κ°μ΄ κ°λ¨νλ€. κ·Έλ λ€λ©΄ μΈμ  μ¬μ©ν κΉ? κ΅¬μ²΄μ μΈ μμλ μλ λ§ν¬λ₯Ό ν΅ν΄ νμΈνμ.

#### Reference

- https://newbiestory.tistory.com/60

## #58

### Does Python support multiple inheritance?

μμ ν΄λμ€κ° μ¬λ¬κ°μ λΆλͺ¨ ν΄λμ€λ‘ λΆν° μμ λ°μμ λ, μ΄λ₯Ό multiple inheritanceλΌκ³  ν©λλ€.

```python
# Python example to show the working of multiple
# inheritance
class Base1(object):
    def __init__(self):
        self.str1 = "Geek1"
        print("Base1")

class Base2(object):
    def __init__(self):
        self.str2 = "Geek2"
        print("Base2")

class Derived(Base1, Base2):
    def __init__(self):

        # Calling constructors of Base1
        # and Base2 classes
        Base1.__init__(self)
        Base2.__init__(self)
        print("Derived")

    def printStrs(self):
        print(self.str1, self.str2)


ob = Derived()
ob.printStrs()


>> Base1
>> Base2
>> Derived
>> Geek1 Geek2
```

Multi-level inheritance

child and grandchild κ΄κ³λ₯Ό κ°κ² λ  λ

```python
# A Python program to demonstrate inheritance

# Base or Super class. Note object in bracket.
# (Generally, object is made ancestor of all classes)
# In Python 3.x "class Person" is
# equivalent to "class Person(object)"
class Base(object):

    # Constructor
    def __init__(self, name):
        self.name = name

    # To get name
    def getName(self):
        return self.name


# Inherited or Sub class (Note Person in bracket)
class Child(Base):

    # Constructor
    def __init__(self, name, age):
        Base.__init__(self, name)
	# super().__init__(name) # μμ λμΌν κ²°κ³Ό
	# super(Child, self).__init__(name)
        self.age = age

    # To get name
    def getAge(self):
        return self.age

# Inherited or Sub class (Note Person in bracket)
class GrandChild(Child):

    # Constructor
    def __init__(self, name, age, address):
        Child.__init__(self, name, age)
	# super().__init__(name, age) # μμ λμΌν κ²°κ³Ό
	# super(GrandChild, self).__init__(name, age)
        self.address = address

    # To get address
    def getAddress(self):
        return self.address

# Driver code
g = GrandChild("Geek1", 23, "Noida")
print(g.getName(), g.getAge(), g.getAddress())
>> Geek1 23 Noida
```

#### Reference

- [inheritance-in-python](https://www.geeksforgeeks.org/inheritance-in-python/)

## #59

### What is Polymorphism in Python?

Polymorphism(λ€νμ±) μ΄λ κ°μ λ¨μ΄(ν¨μ)μ΄λλΌλ λ€λ₯Έ ννλ₯Ό νν  μ μλ κ²μ λ§νλ€.

```python
# Python program to demonstrate in-built poly-
# morphic functions

# len() being used for a string
print(len("geeks"))

# len() being used for a list
print(len([10, 20, 30]))
```

Pythonμμ Polymorphismμ μ¬μ©νλ©΄ λΆλͺ¨ classμμ μ μλ κ²κ³Ό λμΌν μ΄λ¦μ κ°μ§ μμ ν΄λμ€μ methodλ₯Ό μ μ ν  μ μλ€. μ¦, μμ classλ λΆλͺ¨ classμ λͺ¨λ  methodλ₯Ό μμνλ€.

νμ§λ§ μ΄λ€ κ²½μ°μλ μμ λ°μ methodκ° μμ classμ λ§μ§ μλ κ²½μ°κ° μλλ° μ΄λ μμ classμμ λ€μ κ΅¬νν΄μΌνλ€. (_Method Overriding_)

```python
class Bird:
     def intro(self):
       print("There are different types of birds")

     def flight(self):
       print("Most of the birds can fly but some cannot")

class parrot(Bird):
     def flight(self):
       print("Parrots can fly")

class penguin(Bird):
     def flight(self):
       print("Penguins do not fly")

obj_bird = Bird()
obj_parr = parrot()
obj_peng = penguin()

obj_bird.intro()
obj_bird.flight()

obj_parr.intro()
obj_parr.flight()

obj_peng.intro()
obj_peng.flight()

# output :
# There are different types of birds
# Most of the birds can fly but some cannot
# There are different types of bird
# Parrots can fly
# There are many types of birds
# Penguins do not fly
```

#### Reference

- [What is Polymorphism in OOPs programming?](https://www.edureka.co/blog/polymorphism-in-python/)
- [Polymorphism in Python](https://www.geeksforgeeks.org/polymorphism-in-python/)

## #60

### Define encapsulation in Python?

κ°μ²΄ μμ μλ λ°μ΄ν°κ° μΈλΆλ‘λΆν° μν₯μ λ°μ§ μμ.

κ°μ²΄κ° λλ¦½μ μΌλ‘ μ­ν μ ν  μ μλλ‘ λ°μ΄ν°μ κΈ°λ₯μ νλλ‘ λ¬Άμ.

μ΄λ₯Ό ν΅ν΄ μ¬μ©μκ° λ³μμ λ©μλμ μ§μ μ μΌλ‘ μ κ·Όνμ¬ μ€μ/κ³ μλ‘ λ°μ΄ν°λ₯Ό λ³κ²½νλ νμλ₯Ό λ―Έμ°μ λ°©μ§.

1. λ³μλ ν¨μ μμ \_\_(μΈλλ° λκ°)λ₯Ό μ°λ©΄ μΈλΆλ‘λΆν° μ§μ μ κ·Όμ λ§μ μ μλ€. (ν¨μ μ€ μ λ€λ‘ λκ° μλ κ²μ μ κ·Ό κ°λ₯) :private

   -->\_{ν΄λμ€μ΄λ¦}\_\_{λ³μμ΄λ¦} μΌλ‘ μ κ·Όν  μ μλλ‘ μμ±μ΄ λ°λ κ²

2. λ³μ μμ \_(μΈλλ° νκ°)κ° μλ€λ©΄ λ³μλ₯Ό κ±΄λλ¦¬μ§ λ§μκ³  μ½μ (ν΄λΉ ν΄λμ€ λ΄λΆμ νμ ν΄λμ€μμλ§ μ¬μ©νμ) :protect

#### Reference

- [Encapsulation](https://velog.io/@kyeongraekim/Python-TIL14-Encapsulation)
- [κ°μ²΄μ§ν₯ νλ‘κ·Έλλ° κ°λ](https://seungjuitmemo.tistory.com/51)

## #62

### Does python make use of access specifiers?

- access specifier : μ κ·Ό μ νμ, access modifierλΌκ³ λ ν¨

κ°λ¨ν μ κ·Ό μ νμμ λν΄ μΈκΈνκ² μ΅λλ€. 

μ κ·Ό μ νμλ μ κ·Όν  κΆνμ λ²μλ₯Ό μ ν΄μ£Όλ μμμ΄λ‘ μΊ‘μνμ ν λ°©λ²μλλ€.

|access specifier|ν΄λμ€ λ΄λΆ|λμΌ ν¨ν€μ§|νμ ν΄λμ€|κ·Έ μΈμ μμ­|
|-----|-----|-----|-----|-----|
|public|O|O|O|O|
|protected|O|O|O|X|
|default|O|O|X|X|
|private|O|X|X|X|

#### pythonμ access specifier

pythonμ μ κ·Ό μ νμλ₯Ό λ°λ‘ κ°μ§ μμ΅λλ€. νμ§λ§ μΈλλ°(_)λ₯Ό νμ©ν΄ μ κ·Όμ νμλ₯Ό μ¬μ©ν  μ μμ΅λλ€.

κΈ°λ³Έμ μΌλ‘ λͺ¨λ  λ©€λ²κ° publicμλλ€. pythonμ λ³μ μμ μΈλλ°(_)λ₯Ό namingνλ κ²μΌλ‘ λ³μμ μ κ·Όμ μ μ΄νλ€. 

μΈλλ° νλ(_)λ₯Ό μ°λ©΄ protected memberλ‘ μ¬μ©ν  μ μμ΅λλ€.

μΈλλΆ λκ°(__)λ₯Ό μ°λ©΄ private memberλ‘ μ¬μ©ν  μ μμ΅λλ€.

#### Reference
- [Python μ κ·Όμ μ΄μ](https://lambda2.tistory.com/3)
- [κ°μ²΄μ§ν₯ (public, private, protected)](https://www.fun-coding.org/PL&OOP1-5.html)
- [Python μ κ·Όμ μ΄μ](https://lambda2.tistory.com/3)


## #63 

### How to create an empty class in Python?

```python
# jaewook.py
class Jaewook:
```

μ νμΌμ μ€ννλ©΄ μλ μλ¬κ° λ°μνλ€.

> SyntaxError: unexpected EOF while parsing

λΉ ν΄λμ€λ₯Ό μμ±νλ €λ©΄ `pass` λ₯Ό μ¬μ©νλ©΄ λλ€!!

```python
# jaewook.py
class Jaewook:
  	pass
```

`pass` λ νμ΄μ¬μμ μλ¬΄ λμλ νμ§ μλ special statementμ΄λ€. λΉ ν¨μλ ν΄λμ€λ₯Ό μ¬μ  μ μν λ μ¬μ©λλ€.

## #64

#### What does an object() do?

νμ΄μ¬μ λͺ¨λ κ²μ΄ κ°μ²΄λ‘ μ΄λ ν value(μμ±κ°)κ³Ό method(νλ)μ κ°μ§κ³  μλ λ°μ΄ν°μ΄λ€.

**Python object() function** λΉ κ°μ²΄λ₯Ό λ¦¬ν΄νλ€ κ·Έλ¦¬κ³  μ΄λ ν parameterλ λ°μ§ μλλ€.

```python
# declaring the object of class object
obj = object()

# printing its type
print("The type of object class object is : ")
print(type(obj))

# printing its attributes
# dir() λ΄μ₯ ν¨μλ μ΄λ€ κ°μ²΄λ₯Ό μΈμλ‘ λ£μ΄μ£Όλ©΄ ν΄λΉ κ°μ²΄κ° μ΄λ€ λ³μμ λ©μλ(method)λ₯Ό κ°μ§κ³  μλμ§ λμ΄ν΄μ€λλ€.
print("The attributes of its class are : ")
print(dir(obj))

>> The type of object class object is :
>> <class 'object'>
>> The attributes of its class are :
>> [β__class__β, β__delattr__β, β__dir__β, β__doc__β, β__eq__β, β__format__β, β__ge__β, β__getattribute__β, >> β__gt__β, β__hash__β, β__init__β, β__le__β, β__lt__β, β__ne__β, β__new__β, β__reduce__β, β__reduce_ex__β, >> β__repr__β, β__setattr__β, β__sizeof__β, β__str__β, β__subclasshook__β]
```

**Properties of object()**

- Objects of object class μλ‘μ΄ μμ±μ λν  μ μλ€.
- object ν΄λμ€λ‘ λ§λ€μ΄μ§ κ°μ²΄λ€μ μ μΌνκ² λ§λ€μ΄μ§λ€. μ¦ λμΌν κ°μ²΄κ° μλλ€.
- the object acts as a base class for all the custom objects that we make. (μ°λ¦¬κ° λ§λλ κ°μ²΄λ€μ base classκ° λλ€λ λ―)

```python
# declaring the objects of class object
obj1 = object()
obj2 = object()

# checking for object equality
print("Is obj1 equal to obj2 : " + str(obj1 == obj2))

# trying to add attribute to object
obj1.name = "GeeksforGeeks"

>> Is obj1 equal to obj2 : False
>> Traceback (most recent call last):
>>  File "/home/46b67ee266145958c7cc22d9ee0ae759.py", line 12, in
>>    obj1.name = "GeeksforGeeks"
>> AttributeError: 'object' object has no attribute 'name'
```

#### Reference

- [κ°μ²΄λ? - μ λλ‘ νμ΄μ¬](https://wikidocs.net/20457)

- [python-object-method from geeksforgeeks](https://www.geeksforgeeks.org/python-object-method/)

## #65

### What is map function in Python?

Pythonμ `map()`μ μΌλ°μ μΌλ‘ mapping ν  λ μ°μ΄λ `for loop`μ μ¬μ©νμ§ μκ³  iterable ν κ° itemsμ μ²λ¦¬νκ³  λ³νν  μ μλ λ΄μ₯ ν¨μμ΄λ€.

λν νμ΄μ¬μμ ν¨μν νλ‘κ·Έλλ° μ€νμΌμ μ§μνλ tool μ€ νλμ΄λ€.

map()μ ν¨μ κ°μ²΄μ iterable(λλ μ¬λ¬ iterables)λ₯Ό argumentsλ‘€ κ°κ³ , μμ²­μ λ³ν ν­λͺ©μ μμ±νλ iteratorλ₯Ό λ°ν (generator μ²λΌ yield λ‘ λ°ν)

μμλ μλμ κ°λ€.

```python
map(function, iterable[, iterable1, iterable2,..., iterableN])
```

μ¬κΈ°μ μ£Όμ ν  μ μ map() μ μ²«λ²μ§Έ μΈμλ function object(ν¨μ κ°μ²΄) μ΄κΈ° λλ¬Έμ ν¨μλ₯Ό νΈμΆνμ§ μκ³  λ£μ΄μΌ νλ€. <u>μ¦, ν μμ κ΄νΈλ₯Ό λ£μΌλ©΄ μλλ€.</u>

μ½λ μ¬μ© μμ

```python
# for λ‘ κ΅¬ν μ
>>> numbers = [1, 2, 3, 4, 5]
>>> squared = []

>>> for num in numbers:
...     squared.append(num ** 2)
...

>>> squared
[1, 4, 9, 16, 25]

# forλ₯Ό μ¬μ©νμ§ μκ³  mapλ§ μ¬μ©νμ¬ κ΅¬ν μ
>>> def square(number):
...     return number ** 2
...

>>> numbers = [1, 2, 3, 4, 5]

>>> squared = map(square, numbers)

>>> list(squared)
[1, 4, 9, 16, 25]
```

μ μ²΄μ μΈ λμ κ΅¬μ‘°λ `for` μ κ°μ λΉμ€ κ³μ°λ forμ κ°λ€.

#### Reference

- [Python's map(): Processing Iterables Without a Loop](https://realpython.com/python-map-function/)
- [λΉμ€ κ³μ° λΉκ΅ Loop vs Map vs List](https://leadsift.com/loop-map-list-comprehension/)

## #66

### Is Python numpy better than lists?

ν arrayμμ μ μ(int), λΆνΈμλ μ μ(uint), μ€μ(float), λ³΅μμ(complex), λΌλ¦¬(bool), λ¬Έμν(string)μ λμΌν μλ£νλ§μ λ€λ£¨κ³ , λμ μΌλ‘ ν¬κΈ° μ‘°μ μ΄ νμμλ€λ©΄ numpyκ° μ’λ€.

1. λ©λͺ¨λ¦¬

<div align='center'>
     <img src="./images/4_66_1.PNG">
   </div>

```python
import numpy as np
import sys

py_arr = [1,2,3,4,5,6]
numpy_arr = np.array([1,2,3,4,5,6])

sizeof_py_arr = sys.getsizeof(1) * len(py_arr)           # Size = 168
sizeof_numpy_arr = numpy_arr.itemsize * numpy_arr.size   # Size = 48
```

```python
# For NumPy arrays elements limited to 1 Byte / 8 Bits
numpy_arr = np.array([1,2,3,4,5,6], dtype = np.int8)
sizeof_numpy_arr = numpy_arr.itemsize * numpy_arr.size   # Size = 6

# For NumPy arrays elements limited to 2 Bytes / 16 Bits

numpy_arr = np.array([1,2,3,4,5,6], dtype = np.int16)
sizeof_numpy_arr = numpy_arr.itemsize * numpy_arr.size   # Size = 12
```

μ¬μ©νλ €λ λ°μ΄ν°μ λ§κ² μλ£ν μ§μ  κ°λ₯

=> λ©λͺ¨λ¦¬ μ μ½

2. λΈλ‘λμΊμ€ν

   <div align='center'>
        <img src="./images/py_66_br.JPG">
      </div>

## #67

### What is GIL in Python language?

λ©ν°μ°λ λ©μ ν  λ, κ³΅μ  μμμ λν΄ μ¬λ¬ μ°λ λκ° λμμ μ κ·Όνλ€λ©΄ κ°±μ λ λ΄μ©μ΄ μ μ€λλ λ±μ λ¬Έμ κ° λ°μν  μ μλ€. μ΄λ₯Ό λ§κΈ° μν΄ νμ΄μ¬μ GIL (Global Interpreter Lock) μ ν΅ν΄ python interpreter μ ν μ°λ λλ§ μ κ·Όνμ¬ λͺ¨λ  μμμ μ¬μ©ν  μ μκ² νλ€.

μ ννλ λ©ν° μ°λ λκ° bytecode(=instruction) ν λΌμΈμ©μ λ€κ³  μκΈ° λλ¬Έμ, ν μ°λ λμ bytecode ν μ€μ λν΄μλ§ GIL μ νμ©νλ€.

#### References

- [[python\] GIL, Global interpreter Lockμ λ¬΄μμΌκΉ? - μνκ³Όμ μ’μΆ©μ°λ νλ‘κ·Έλλ°](https://ssungkang.tistory.com/entry/python-GIL-Global-interpreter-Lockμ-λ¬΄μμΌκΉ)
- [μ Pythonμλ GILμ΄ μλκ° - κ°λ°μλ°λΈλ‘κ·Έ](https://dgkim5360.tistory.com/entry/understanding-the-global-interpreter-lock-of-cpython)

## #68

### What is the CPython?

Cλ‘ μμ±λ νμ΄μ¬ κ΅¬νμ²΄λ₯Ό μλ―Έν©λλ€. κ°μ₯ λλ¦¬ μ¬μ©λλ νμ΄μ¬ κ΅¬νμ²΄μλλ€.

Cνμ΄μ¬μ μΈν°νλ¦¬νΈ κ³Όμ  μ΄μ μ νμ΄μ¬ μ½λλ₯ΌΒ λ°μ΄νΈμ½λλ‘ μ»΄νμΌνκΈ° λλ¬ΈμΒ μΈν°νλ¦¬ν°μ΄κΈ°λ νκ³ Β μ»΄νμΌλ¬μ΄κΈ°λ νλ€. Cλ₯Ό ν¬ν¨ν μ¬λ¬ μΈμ΄μΒ μΈλΆ ν¨μ μΈν°νμ΄μ€λ₯Ό λ³΄μ νκ³  μμΌλ©° μ¬κΈ°μ νμ΄μ¬ μΈμ μΈμ΄λ‘Β λ°μΈλ©μ λͺμμ μΌλ‘ μμ±ν΄μΌ ν©λλ€. CPythonμΈμ Jyto, Pypy λ±μ΄ μμ΅λλ€.

#### Reference
- [Cνμ΄μ¬ - μν€λ°±κ³Ό, μ°λ¦¬ λͺ¨λμ λ°±κ³Όμ¬μ ](https://ko.m.wikipedia.org/wiki/C%ED%8C%8C%EC%9D%B4%EC%8D%AC)
- [1. Introduction - Python 3.10.0 documentation](https://docs.python.org/ko/3/reference/introduction.html)   
  

## #69 

### What are Decorators in Python?

**λ°μ½λ μ΄ν°λ λ€λ₯Έ ν¨μλ₯Ό κΎΈλ©°μ£Όλ ν¨μ!**

***μΈμ  μΈκΉ?***

- κΈ°μ‘΄ structureλ κ±΄λλ¦¬μ§ μκ³  ν¨μμ λμ λ°©μμ μ μ½μ΄λ λ³νλ₯Ό μ£Όκ³ μΆμ λ μ¬μ©

***μμ***

κ°λ Ή ν¨μμ μ€ν μλλ₯Ό μΈ‘μ νκ³  μΆλ€κ³  νμ. μ½λλ§λ€ time.time()μ μ¬μ©νλ λ°©λ²λ μμ§λ§ λ°μ½λ μ΄ν°λ₯Ό μ¬μ©νλ©΄ ν¨μ¬ κ°λ¨νκ² ν΄κ²°κ°λ₯νλ€!

```python
def time_decorator(func):
  def decorated():
    start_time = time.time()
    func()
    end_time = time.time()
    print(end_time - start_time)
  return decorated

@time_decorator
def my_func1():
  print('my func1 is running')

@time_decorator
def my_func2():
  print('my func2 is running')

@time_decorator
def my_func3():
  print('my func3 is running')
  
  
'''μ€νκ²°κ³Ό
my func1 is running
0.24ms
my func2 is running
0.22ms
my func1 is running
0.27ms
'''
```

#### Reference

- [γγγγ·](https://bluese05.tistory.com/30)

## #70

### What is object interning?

Interningμ΄λ μ΄λ―Έ μμ±λ κ°μ²΄(object)λ₯Ό μ¬μ¬μ©(reuse)νλ κ²μ λ§νλλ°, λ³΄ν΅ Immutable κ°μ²΄(ex: int, string, tuple)μ λν΄ Interningμ μ¬μ©νλ€. νμ΄μ¬μ κΈ°λ³Έμ μΌλ‘ λͺκ°μ§ μ νλ κ²½μ°μ λν΄ λν΄νΈλ‘ Interningμ μ¬μ©νκ³  μμΌλ©°, λν κ°λ°μκ° νμν κ²½μ° ν¨μλ₯Ό μ¨μ Interningμ μ§μ ν  μλ μλ€.

μμ£Ό λ§μ΄ μ¬μ©λλ Immutable κ°μ²΄μ κ²½μ° Interningμ μ¬μ©νκ² λλ©΄ λ©λͺ¨λ¦¬λ₯Ό μ€μΌ μ μλ ν¨κ³Όκ° μλ€.

- νμ΄μ¬μ κΈ°λ³Έμ μΌλ‘ λͺκ°μ§ κ²½μ°μ λν΄ μμ€ν λν΄νΈλ‘ Object Interningμ μ¬μ©νλ€.
  - λ¬Έμμ΄: 20μ λ―Έλ§μ κ³΅λ°±μ ν¬ν¨νμ§ μμ λ¬Έμμ΄
  - μ μ: -5λΆν° 256 μ¬μ΄μ μ«μ

```python
a = "Test"   # string intern
b = "Test"   # string intern
# id(a), id(b) λ λμΌν λ©λͺ¨λ¦¬ κ°λ¦¬ν΄
print(id(a), id(b))  # 2611825223136 2611825223136

i = 10
j = 10
print(id(i), id(j), i is j) #2008444256 2008444256 True

x = 257
y = 257
print(id(x), id(y), x is y) #2611825055632 2611825055568 False
```

```python
from sys import intern  # Python 3
c = intern("Alex Lee")
d = "Alex Lee"
print(id(c), id(d), c is d) # 2987210077360 2987210078704 False

e = intern("Alex Lee")
print(id(c), id(e), c is e) # 2987210077360 2987210077360 True
```

#### Reference

- [νμ΄μ¬-Object-Interning](http://pythonstudy.xyz/python/article/512-%ED%8C%8C%EC%9D%B4%EC%8D%AC-Object-Interning)


## #71

### What is @classmethod, @staticmethod, @property?

#### λ€μ΄κ°κΈ° μ μ @(decorator) κ° λ¬΄μμ΄λ?

`@` κ° λ€μ΄κ° κ²μ decoratorλΌ λΆλ¦°λ€. decoratorλ?

- μ΄λ€ ν¨μλ₯Ό λ°μ λͺλ Ήμ μΆκ°ν λ€ μ΄λ₯Ό λ€μ ν¨μμ ννλ‘ λ°ννλ ν¨μ
- μ΄λ€ ν¨μμ λ΄λΆλ₯Ό μμ νμ§ μκ³  κΈ°λ₯μ λ³νλ₯Ό μ£Όκ³  μΆμ λ μ¬μ©
- <u>**λ§ κ·Έλλ‘ λ€λ₯Έ ν¨μλ₯Ό κΎΈλ©°μ£Όλ ν¨μ!**</u>

**λ°μ½λ μ΄ν°μ κΈ°λ³Έ κ΅¬μ‘°**

```python
def λ°μ½λ μ΄ν°μ΄λ¦(func):  # κΈ°λ₯μ μΆκ°ν  ν¨μλ₯Ό μΈμλ‘ λ°μμ¨λ€.
    def λ΄λΆν¨μμ΄λ¦(*args, **kwargs):
        κΈ°μ‘΄ ν¨μμ μΆκ°ν  λͺλ Ή
        return func(*args, **kwargs)
    return λ΄λΆν¨μμ΄λ¦
```

**μμ**

```python
def decorator(func):
    def wrapper(*args, **kwargs):
        print('Hello')
        return func(*args, **kwargs)
    return wrapper

@decorator  # λ°μ½λ μ΄ν° ν¨μλ₯Ό μ μ©ν  ν¨μ λ°λ‘ μμ '@λ°μ½λ μ΄ν°μ΄λ¦'μ λΆμ¬μ€λ€.
def introduce(name):
    print(f'My name is {name}!')

introduce('JaeHyun')
# κ²°κ³Ό :
# Hello
# My name is JaeHyun!
```


#### @classmethod

methodλ₯Ό class methodλ‘ λ³ν

class methodλ instance methodκ° instanceλ₯Ό λ°λ κ² μ²λΌ, class(`cls`)λ₯Ό μ²«λ²μ§Έ μΈμλ‘ λ°λλ€.

```python
class C:
    @classmethod
    def f(cls, arg1, arg2, ...): ...
```

κ·Έλ¦¬κ³  @classmethodλ @staticmethodμ ν¨κ» `μ μ λ©μλ`λΌ λΆλ¦¬λλ° μ΄λ μλμ μ€λͺνκ² λ€.

#### μ μ λ©μλ

- μ μ λ©μλλΌ ν¨μ ν΄λμ€μμ μ§μ  μ κ·Όν  μ μλ λ©μλμ΄λ€.

- νμ΄μ¬μμλ ν΄λμ€μμ μ§μ  μ κ·Όν  μ μλ λ©μλκ° λκ°μ§ μλ€. (staticmethodμ classmethod) - ν΄λμ€ λ³μμ λ§μ°¬κ°μ§λ‘ κ°μ²΄λ₯Ό μμ±νμ§ μκ³  **ν΄λμ€λͺ, λ©μλλͺ** μΌλ‘ νΈμΆμ΄ κ°λ₯νλ€

- ν΄λμ€ λ΄λΆμ μ μνμ§λ§, μΈμ€ν΄μ€μλ μνμ§ μλλ€.

**λΉκ΅ μμ**

```python
class CustomClass:

    # instance method
    def add_instance_method(self, a,b):
        return a + b

    # classmethod
    @classmethod
    def add_class_method(cls, a, b):
        return a + b

    # staticmethod
    @staticmethod
    def add_static_method(a, b):
        return a + b


# instance methodμμ instance λ³μμ μ κ·ΌνκΈ° μν΄μλ μ²«λ²μ§Έ μΈμμ κ°μ²΄λ₯Ό ν λΉ ν΄μΌνλ€(None μ²λΌ)
>>> from static_method import CustomClass
>>> CustomClass.add_instance_method(None, 3, 5)
8

# μ²«λ²μ§Έ μΈμκ° ν΄λμ€μ§λ§ μλ΅νκ³  μ κ·Όν΄μΌνλ€.
>>> CustomClass.add_class_method(CustomClass, 3, 5)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: add_class_method() takes 3 positional arguments but 4 were given


>>> CustomClass.add_class_method(3, 5)
8

# staticmethodλ λ§μ°¬κ°μ§
>>> CustomClass.add_static_method(3, 5)
8

```

#### @classmethodμ @staticmethod μ μ°¨μ΄

λμ μ°¨μ΄λ **μμ** μμ λλλ¬μ§κ² λνλλ€.

**μμ**

```python
class Language:
    default_language = "English"

    def __init__(self):
        self.show = 'λμ μΈμ΄λ' + self.default_language

    @classmethod
    def class_my_language(cls):
        return cls()

    @staticmethod
    def static_my_language():
        return Language()

    def print_language(self):
        print(self.show)


class KoreanLanguage(Language):
    default_language = "νκ΅­μ΄"

```

```python
>>> from language import *
>>> a = KoreanLanguage.static_my_language()
>>> b = KoreanLanguage.class_my_language()
>>> a.print_language()
λμ μΈμ΄λEnglish
>>> b.print_language()
λμ μΈμ΄λνκ΅­μ΄
```

μ¬κΈ°μ λ³Ό μ μλ―, static methodλ λΆλͺ¨ ν΄λμ€μ ν΄λμ€ μμ± κ°μ κ°μ Έμ€μ§λ§ class methodμμλ clsμΈμλ₯Ό νμ©νμ¬ clsμ ν΄λμ€ μμ±μ κ°μ Έμ¨λ€.

#### @property

**νμ΄μ¬ κ°μ²΄ μ§ν₯ νλ‘κ·Έλλ°** μμ κ²ν°(getter)μ μΈν°(setter)λ₯Ό μ½κ² μ¬μ©ν  μ μκ² νμ΄μ¬ λ€μ΄ λ°©λ²μ μ κ³΅

##### Gatterμ Setterκ° μλ ν΄λμ€

λ¨Όμ  μμλ‘ κ°μ²΄λ₯Ό μμ±νκ³  temperature attributeλ₯Ό μ¬μ©

```python
class Celsius:
    def __init__(self, temperature) -> None:
        self.temperature = temperature

    def to_fahrenheit(self):
        return (self.temperature * 1.8) + 32

# κ°μ²΄ λ§λ€κΈ°
human = Celsius()

# μ¨λ μΈν
human.temperature = 37

# μ¨λ μ½κΈ°
print(human.temperature)

# to_fahrenheit λ©μλ μ€ν
print(human.to_fahrenheit)

# 37
# 98.6
```

μμ κ°μ΄ temperatureμ κ°μ κ°μ²΄ attributeλ₯Ό ν λΉ(assign, set)νκ±°λ κ²μ(retrieve, get) ν  λλ§λ€ νμ΄μ¬μ κ°μ²΄μ λΉνΈμΈ `__dict__` λμλλ¦¬ μμ±(attribute)μμ κ²μνλ€.

```python
>>> human.__dict__
{'temperature' : 37}
```

λ°λΌμ human.temperatureλ λ΄λΆμ μΌλ‘ `human.__dict__['temperature']` λ‘ μ μ₯μ΄ λ¨

##### Getter λ° Setterμ μ¬μ©

μμ

```python
class Celsius:
    def __init__(self, temperature = 0) -> None:
        self.set_temperature(temperature)

    def to_fahrenheit(self):
        return (self.get_temperature() * 1.8) + 32

    # getter λ©μλ
    def get_temperature(self):
        return self._temperature

    # setter λ©μλ
    def set_temperature(self, value):
        if value < -273.15:
            raise ValueError("-273.15 λ―Έλ§μ μ¨λλ μμ΅λλ€.")
        self._temperature = value

# κ°μ²΄ μμ±, __init__()κ° λ΄λΆμ μΌλ‘ set_temperature()λ₯Ό νΈμΆ
human = Celsius(37)

# getterλ₯Ό μ¬μ©ν΄ temperature attributeλ₯Ό κ΅¬νλ€.
print(human.get_temperature())

# νμ¨ λ³νμ μνμ¬ to_fahrenheit λ©μλ μ¬μ©, get_temperature()κ° νΈμΆλλ€.
print(human.to_fahrenheit())

# 37
# 98.6
```

μ΄λ°μμΌλ‘ getterμ setterλ₯Ό μ¬μ©νκ² μλ°μ΄νΈλ₯Ό νκ² λλ©΄ μ΄μ μ getter, setterκ° μλ ν΄λμ€μμ μ¬μ©ν  μ μκ² λλ€.

##### @property λ°μ½λ μ΄ν°μ μ¬μ©

μμ

``` python
class Celsius:
    def __init__(self, temperature = 0) -> None:
        self.temperature = temperature

    def to_fahrenheit(self):
        return (self.temperature * 1.8) + 32

		@property
    def temperature(self):
        print("Getting value...")
        return self._temperature

		@temperature.setter
    def temperature(self, value):
	      print("Setting value...")
        if value < -273.15:
            raise ValueError("-273.15 λ―Έλ§μ μ¨λλ μμ΅λλ€.")
        self._temperature = value

# κ°μ²΄ μμ±, __init__()κ° λ΄λΆμ μΌλ‘ set_temperature()λ₯Ό νΈμΆ
human = Celsius(37)

# getterλ₯Ό μ¬μ©ν΄ temperature attributeλ₯Ό κ΅¬νλ€.
print(human.get_temperature())

# νμ¨ λ³νμ μνμ¬ to_fahrenheit λ©μλ μ¬μ©, get_temperature()κ° νΈμΆλλ€.
print(human.to_fahrenheit())

# Setting value...
# Getting value...
# 37
# Getting value...
# 98.6000001
# Setting value...
```



μμΈν λμ μλ¦¬λ μλμ reference μ°Έκ³ 

#### Reference

- [[Python λ¬Έλ²] λ°μ½λ μ΄ν° (Decorator)](https://nachwon.github.io/decorator/)

- [Python κ³΅μ doc](https://docs.python.org/3/library/functions.html?highlight=classmethod#classmethod)

- [44. class μ λ¦¬ - μ μ λ©μλ @classmethodμ @staticmethodμ μ λ¦¬](https://wikidocs.net/16074)

- [Static method VS Instance method](https://jihyehwang09.github.io/2020/03/21/java-static-method-and-instance-method/)

- [OOP-@property λ°μ½λ μ΄ν°(decorator)](https://m.blog.naver.com/hankrah/221976126435)