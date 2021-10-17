<div align='center'>
  <h1>🐍 Python Programming Language 🐍</h1>
</div>

> 질문은 <strong>[Top 100 Python Interview Questions You Must Prepare In 2021 - edureka!](https://www.edureka.co/blog/interview-questions/python-interview-questions/)</strong>을 참고하였으며, 질문에 대한 답변 중 일부는 위의 사이트의 답변을 참고하여 작성되었습니다.

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
- [What’s the difference between iterator and iterable?](#23)
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
- [Whenever Python exits, why isn’t all the memory de-allocated?](#35)
- [What is a dictionary in Python?](#36)
- [How can the ternary operators be used in python?](#37)
- [What does this mean: `*args`, `**kwargs`? And why would we use it?](#38)
- [What does len() do?](#39)
- [Explain split(), sub(), subn() methods of “re” module in Python.](#40)
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
- [Explain Inheritance in Python with an example.](#55)
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

## #3

### What type of language is python? Programming or scripting?

**파이썬 스크립트 언어이자 프로그래밍 언어이다.**

파이썬은 소스코드를 기계어로 먼저 번역하는 컴파일 과정을 거치지 않기 때문에 스크립트 언어로 볼 수 있다. 하지만 많은 사람들이 파이썬이 Java, C++과 같은 언어를 대체하여 개발에 사용될 수 있기 때문에 프로그래밍 언어라고도 한다. 프로그래밍 언어라는 말 자체가 스크립트 언어를 포함하기 때문에 파이썬도 해당된다고 생각한다.

**References**

[codingninjas](https://www.codingninjas.com/blog/2018/12/08/difference-between-a-programming-language-and-a-scripting-language/)

[ThePythonGuru](https://thepythonguru.com/is-python-a-programming-language-or-scripting-language/)

[Javatpoint](https://www.javatpoint.com/scripting-vs-programming)

## #4

### Python an interpreted language. Explain.

#### 컴파일러 vs 인터프리터

컴파일된 언어는 컴파일러를 통해 구현되며 소스 코드를 기계어로 바꾸는 과정을 사전에 처리 하여 빠르게 컴퓨터에서 구동될 수 있도록 한 방법 이며, 인터프리터 언어는 대부분 소스코드를 기계어로 컴파일하지 않고 인터프리터를 통해 소스코드 실행시 각 스테이트먼트(소스코드 구문)를 하나 이상의 서브루틴 순서로 변환한 후, 기계어나 바이트코드등 다른 언어로 변환되어 구현

<div align='center'>
<img src="https://s3.us-west-2.amazonaws.com/secure.notion-static.com/1cdbfd7a-9479-46fb-8cdf-670a10df3394/_2021-06-03__2.43.34.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5%2F20211016%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211016T154051Z&X-Amz-Expires=86400&X-Amz-Signature=e60d071a61f2e2b8aa2ca27543adb73d78c2a7dc190cc655f6bd3475307b29bd&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22_2021-06-03__2.43.34.png%22" width="60%">

</div>

## #5

### What is pep 8?

PEP8(Python Enhencement Propsals)란 가독성이 좋은 파이썬 코딩을 하고자 제시된 스타일 가이드
사람마다 각자 다른 코딩스타일이 있기에 스타일간 충돌을 피하고자 파이썬 코딩 가이드를 제시했다. from 귀도 반 로썸

example)

- Indentation(4개 공백), 
- Maximul Line Length(한 줄에 최대 79자, 주석 72자)
- Whitesapece in Expressions and Statements(필요 없는 공백 제거)
- etc...(또 다른 여러 방법이 있다.)

code example)

```python
# example-1) 반환되지 않는 return 문도 None으로 리턴문을 명시해 줘야한다.
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

# example-2) 객체 타입의 비교는 isinstance 이용한다 직접비교 대신에
# Correct:
if isinstance(obj, int):

# Wrong:
if type(obj) is type(1):
    
# example-3) Sequence(strings, lists, tuples)의 경우 빈 sequence는 false라는 사실을 이용한다.
# Correct:
if not seq:
if seq:
    
# Wrong:
if len(seq):
if not len(seq):
   
```

### Reference

- [PEP8 공식사이트](https://www.python.org/dev/peps/pep-0008/#maximum-line-length)

## #6

### How is memory managed in Python?

