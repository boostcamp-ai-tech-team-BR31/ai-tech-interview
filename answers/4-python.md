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

## #1

### What is the difference between list and tuples in Python?

- 리스트는 [], 튜플은 ()로 작성
- 리스트는 값을 수정할 수 있지만 , 튜플은 값을 변경할  수 없다.

리스트와 튜플의 가장 **큰 차이점은 값을 변경할 수 있는가의 여부**이므로,  프로그램이 실행되는 동안 **값이 변경되면 안 되는 경우 튜플**을 사용한다. 튜플은 리스트에 비해 더 적은 메모리를 필요로 하고, 속도가 빠르다.



**References**

- [튜플과 리스트 비교](https://bigdaheta.tistory.com/8)

## #2

### What are the key features of Python?

#### Features of Python

- Script Language
  - 스크립트 언어란, 컴파일 과정 없이 실행과정에서 번역과 실행이 동시에 일어나는 언어입니다.
  - 수정이 빠르지만 컴파일 언어보다 느린 실행속도를 보여줍니다.
  - 자세한건 [4번](#4)으로!
- Dynamic typing
  - 변수의 자료형을 지정하지 않고 선언하는 것만으로 사용할 수 있음
  - 개발 당시엔 편리하지만 type error debuging이 발생할 수 있음
  - 하지만 저는 전자의 편리함이 더 크다고 생각합니다 ^^
  ```c
  # C, java
  int a = 10
  ```
  ```python
  # Python
  a = 10
  ```
- platform-independent
  - linux, unix, windows, mac... 대부분 OS에서 모두 잘 동작합니다.
  - 컴파일 할 필요가 없기 때문에!
- Multi paradigm
  - 절차적, 객체지향, 함수형, 관점형 프로그래밍 모두 가능

#### Pros

- 사용하기 쉽기에 빠른 개발속도(생산성)
- 높은 확장성, 이식성
  - 고성능이 필요하다면 C/C++언어와 결합해 사용 가능
- 활발한 생태계
  - 수많은 라이브러리 존재
  - 인기가 많기 때문

#### Cons

- 느리다
  - Script Language이기 때문
- type error
  - Dynamic typing 이기 때문

#### Reference

- [파이썬(Python) 특징 및 장/단점 정리](https://velog.io/@jnine/%ED%8C%8C%EC%9D%B4%EC%8D%ACPython-%ED%8A%B9%EC%A7%95-%EB%B0%8F-%EC%9E%A5%EB%8B%A8%EC%A0%90-%EC%A0%95%EB%A6%AC)
- [python 바로 알기](https://library.gabia.com/contents/9256/)

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

#### Reference

- [PEP8 공식사이트](https://www.python.org/dev/peps/pep-0008/#maximum-line-length)

## #6

### How is memory managed in Python?

CPython에서의 메모리 관리와 Garbage Collection은 두 가지 측면이 있다.

1. 레퍼런스 카운팅(Reference counting)
2. 세대별 가비지 컬렉션(Generational garbage collection)

CPython에서의 주요 garbage collection mechanism은 [reference counts](https://docs.python.org/3.6/c-api/intro.html#reference-counts) 방식이다. Python에서 객체를 만들 때마다 기본 C 객체에서는 Python 유형(list, dict 또는 function)과 reference count가 생성된다.

매우 기본적으로 Python 객체의 reference count는 객체가 참조될 대마다 증가하고 객체의 참조가 해제될 때 감소한다. 객체의 reference count가 0이 되면 객체의 메모리 할당이 해제된다.

CPython은 사이드로 세대별 가비지 컬렉션이라는 기능도 있다.

이것은 참조는 되어 있지만, 접근할 수 없는 객체를 메모리에서 릴리즈하는 역할을 한다. 순환참조(Circular References) 에서 나타날 수 있는데..

```
l = []
l.append(l)
del
```

위처럼 참조는 되어 있지만, 해당 객체에 접근할 수 없는 경우를 해결한다.

다음을 읽어보면 좋겠다.

[python memory allocation](https://leemoney93.tistory.com/25)

#### Reference

- [Garbage Collection in Python](https://medium.com/dmsfordsm/garbage-collection-in-python-777916fd3189)
- [[PYTHON] Garbage Collector ](https://dingrr.com/blog/post/python-garbage-collector)

## #8

### What is PYTHONPATH?

import로 다른 파이썬 파일을 불러올 때, python은 내부적으로 파일을 찾기 위해 **sys.path**와 **PYTHONPATH**에 있는 경로를 탐색합니다.

**sys.path**는 directory path 문자열을 모아둔 리스트입니다. 이 리스트에 path를 추가하면 해당 path에 있는 python 파일을 import할 수 있습니다.

```python
sys.path.append('/tttangmin/hobby')

# /tttangmin/hobby/badminton.py
import badminton
```

#### sys.path의 기본값 (우선순위 순)

- 현재 .py 파일이 속한 directory의 absolute path
- PYTHONPATH 환경변수에 추가된 path
  - sys.path.append()는 **일시적으로** path를 추가하는 것이라면
  - PYTHONPATH 환경변수는 **영구적으로** path를 추가하는 것
  - OS에 따라 추가하는 방법이 다름. reference 참고
- 기타 기본 path
  - 여러 내장 모듈들을 위한 path
  - os, python version에 따라 다름

#### Reference

- [sys.path, PYTHONPATH: 파이썬 파일 탐색 경로](https://www.bangseongbeom.com/sys-path-pythonpath.html)
- [PYTHONPATH 추가하는 방법](https://pybasall.tistory.com/201)

## #9

### What are Python modules? Name some commonly used built-in modules in Python?

**Module**이란 Python 코드를 포함하는 파일로써, 함수나 변수 또는 클래스를 모아 놓은 파일이다. 모듈은 다른 파이썬 프로그램에서 불러와 사용할 수 있게끔 만든 파이썬 파일이라고도 할 수 있다. 실행 가능한 코드를 포함하는, 파이썬 확장자 `.py`로 만든 파이썬 파일은 모두 모듈이다. 모듈을 사용하면, 다른 코드에 적용하기가 쉬워지므로 이식성이 좋아진다.

**Built-in modules**란 파이썬에서 제공하는 공식 내장 라이브러리다.  로컬의 어느곳에서 파일을 작성하던지 이 내장 모듈들은 어디서나 사용할 수 있다. 

- 자주 사용되는 built-in module 의 예시
  - os
  - sys
  - math
  - random
  - datetime
  - JSON
  - itertools



#### Reference

- [모듈이란?](https://yganalyst.github.io/data_handling/Py_study14/)
- [패키지,모듈](https://fierycoding.tistory.com/m/60?category=942731)

## #10

### What are local variables and global variables in Python?

함수 안에서 만들어진 변수를 **지역변수(local variable)**라 하고 함수 밖에서 만들어진 변수를 **전역변수(global variable)**라 한다.

이 두 변수는 아래와 같이 두 가지 차이점이 존재한다.

1. **메모리에 존재하는 시간**

   지역 변수는 해당 지역에서 선언되는 순간 메모리가 생성되고 해당 지역을 벗어나면 자동으로 소멸

   전역 변수는 코드가 시작되어 선언된느 순간 메모리 생성, 코드 전체 끝날때 까지 메모리를 차지

2. **변수에 접근할 수 있는 범위**

   지역 변수는 선언 된 함수 내에서만 사용이 가능

   전역 변수는 프로그램 실행 중에 쓰이는 모든 함수가 사용 가능

#### Reference

- [3.3 지역변수, 전역변수](https://wikidocs.net/62)
- [전역변수와 지역변수](https://edu.goorm.io/learn/lecture/2010/한-눈에-끝내는-고랭-기초/lesson/174452/전역변수와-지역변수)

## #11

### Is Python case sensitive?

대소문자 구분한다.

PHP 같은 경우 변수이름은 대소문자 구분이 있고, 함수이름엔 없다. 함수를 소문자로 정의하고 대문자로 호출하는 것이 가능하다.

#### Reference

- [Wikipedia](https://en.wikipedia.org/wiki/Case_sensitivity#:~:text=are%20strictly%20lowercase.-,In%20programming%20languages,Ruby%2C%20Python%20and%20Swift)

## #12

### What is type conversion in Python

Type conversion은 데이터 타입을 다른 타입으로 바꾸는 것을 의미한다.

~~(데이터 타입의 종류: int, float, complex, string, fuple, set, list, dictionary, .... )~~

Python에서는 2가지의 type conversion이 존재한다.

1. Implicit Type Conversion(암시적 형 변환)
2. Explicit Type Conversion(명시적 형 변환)

**Implicit Type Conversion**

Implicit Type Conversion은 Python이 자동으로 형 변환을 실행한다. 이 때 data의 loss를 줄이기 위해 lower data type(int)를 higher data type으로 바꿔준다.

```python
num_int = 123
num_flo = 1.23

num_new = num_int + num_flo

print("datatype of num_int:",type(num_int)) # -> <class 'int'>
print("datatype of num_flo:",type(num_flo)) # -> <class 'float'>

print("Value of num_new:",num_new) # -> 24.23
print("datatype of num_new:",type(num_new)) # -> <class 'float'>
```

(참고로 문자열이랑 숫자랑 더하면 오류(TypeError)나기 때문에 이떄는 명시적 형 변환을 해줘야 한다.)

**Explicit Type Conversion**

사용자가 객채의 타입을 명시적으로 바꿔주는 것. 사전 정의된 `int`(), `float()`, `str()`, etc 함수를 이용한다.

이러한 type of conversion은 유저가 직접 객채의 data type을 cast(change) 해주기 때문에 typecasting이라고도 불린다.

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

들여쓰기. python에서는 들여쓰기는 **문법적인 강제사항**입니다.
다른 프로그램 언어에서는 {}를 사용하여 영역을 지정합니다.

```c
if (victor(human)) {
human_wins++;
printf("I am your humble servant.\n");
} else {
computer_wins++;
printf("Your destiny is under my control!\n");
}
```

물론 c언어에서도 indentation을 적용할 수 있습니다만, ;를 사용해야 합니다.

```c
if (victor(human)) {
	human_wins++;
	printf("I am your humble servant.\n");
} else {
	computer_wins++;
	printf("Your destiny is under my control!\n");
}
```

python 에서는 {}나 ;를 쓰지 않는 대신, indentation으로 코드의 영역을 지정합니다.

```python
if victor == 'human':
    human_win++
    print("I am your humble servant.\n")
else:
    computer_wins++;
	print("Your destiny is under my control!\n");
```

indentation의 방법은 띄어쓰기 한칸, 두칸, 4칸, 탭 등 여러가지 방법이 있지만,

> 중요한 것은 같은 블록 내에서는 들여쓰기 칸 수가 같아야 합니다.
>
> 위반시 Indentation Error가 출력됩니다.

#### Reference

- [python 계단밟기 : 들여쓰기(indent)](https://wikidocs.net/20368)
- [c indentation](https://www2.cs.arizona.edu/~mccann/indent_c.html)

## #15

### What is the difference between Python Arrays and lists?

파이썬에서는 배열이라는 부분이 없지만 배열의 편의성 때문에 ` array ` 라는 모듈을 제공하고 있습니다.

**array**와 **list**는 동일한 방식으로 데이터를 저장하지만 

**array**는 **단일 데이터 타입 요소**만을 포함할 수 있는 반면,

**list**는 **다양한 타입의 요소**들이 들어갈 수 있습니다.



array는 `arrayName = arrary(type, [Values])`처럼 자료형을 저장하고, 지정한 자료형만을 넣을수 있습니다.

list는 변수에 []로 여러 타입의 변수를 묶어서 선언할 수 있습니다.

#### Reference

- [파이썬[Python] 036 Array(배열) 사용하기](https://appia.tistory.com/125)

## #16

### What are functions in Python?

**Python에서 함수란 특정 작업을 수행하는 관련 명령문의 그룹이다.**

함수를 사용함으로써 프로그램을 더 작고 **모듈화**되게 나누는데 도움이 되고 프로그램을 보다 **체계적**이고 **관리하기 쉽게** 만들 수 있다.

또한 반복을 피하고 **코드를 재사용**하기 용이해진다.

문법은 아래와 같다.

```python
def function_name(parameters):
	"""docstring"""
	statement(s)
```

1. `def` : 함수의 헤더의 시작을 알리는 키워드
2. 함수의 이름은 기능을 잘 나타낼 수 있게 정해야한다.
3. `parameters` : 함수에 값을 전달하는 매개변수 (선택사항)
4. `:` : 함수 헤더의 끝을 표시
5. `docstring` : 함수가 하는 일을 설명하는 문자열 (선택사항)
6. `statemet` : 함수의 본문을 구선하는 하나 이상의 파이썬 문, 들여쓰기 정도가 같아야한다.
7. `return` : 함수에서 값을 반환하는 반환문 (선택사항)

#### Reference

- [Python Functions (def): Definition with Examples - Programiz](https://www.programiz.com/python-programming/function)

## #17

### What is \_\_init\_\_?

- 초기화 함수
- 인스턴스를 생성할 때 반드시 처음에 호출되는 함수
- 생성자로서 클래스마다 하나존재

#### Reference

- [python 문법](https://wikidocs.net/89)
- [python self와 init](https://engineer-mole.tistory.com/190)
- [inflearn](https://www.inflearn.com/questions/4642)

## #18

### What is a lambda function?

람다함수는 이름 없이 정의되는 익명 함수(anonymous functions)입니다. `def`를 이용하여 정의 되는 일반 함수와 달리 `lambda` 키워드를 이용하여 정의됩니다. 보통 한줄로 함수를 표현하기에 코드가 간결해지고 한 번 사용되고 다시 사용 할 수 없기에 메모리를 절약 할 수 있지만 여러줄로 표현할 수 없고 함수에 대한 설명을 적을 수 없는 단점이 있습니다.(doc string 불가). 이런 경우 def 함수를 이용하여 함수를 정의 해야 한다.

```python
# 예시1
my_list = [1, 5, 4, 6, 8, 11, 3, 12]
new_list = list(filter(lambda x: (x%2 == 0) , my_list)) # [4,6,8,12]

# 예시2
my_list = [1, 5, 4, 6, 8, 11, 3, 12]
new_list = list(map(lambda x: x * 2 , my_list)) # [2, 10, 8, 12, 16, 22, 6, 24]

# 오직 하나의 arguemnt가 필요한 함수를 쓸 경우 labmda 사용 필요 없다.
#Bad
map(lambda x:abs(x), list_3)
#Good
map(abs, list_3)

# 함수 정의한다면 def를 사용하는 것이 좋다
#Bad
triple = lambda x: x*3
#Good
def triple(x):
     return x*3
```

#### Reference

- [파이썬 익명함수 예시: Programiz](https://www.programiz.com/python-programming/anonymous-function)
- [Towards Data Science: Lambda Functions with Practical Examples in Python](
