<div align='center'>
  <h1>🗂 Data Structure 🗂</h1>
</div>

> 질문은 <strong>[WeareSoft님의 tech-interview](https://github.com/WeareSoft/tech-interview)</strong>를 참고하였으며, 질문에 대한 답변은 직접 작성하였습니다.

---

## Table of Contents

- [linked list](#1)
  - [single linked list](#1-1)
  - [double linked list](#1-2)
  - [circular linked list](#1-3)
- [hash table](#2)
- [stack](#3)
- [queue](#4)
  - [circular queue](#4-1)
- [graph](#5)
- [tree](#6)
  - [binary tree](#6-1)
  - [full binary tree](#6-2)
  - [complete binary tree](#6-3)
  - [bst(binary search tree)](#6-4)
- [heap(binary heap)](#7)
  - [min heap](#7-1)
  - [max heap](#7-2)
- [Red-black Tree](#8)
- [B-Tree](#9)

---

## #1

### linked list

Linked List는 Array List와 달리 엘리먼트와 엘리먼트 간의 연결(link)을 이용해 리스트를 구현한 것

**+) Array List와 Linked List 간단 비교**

<div align='center'>
     <img src=".\images\ds_1_1.png" style="zoom:40%;"/>
   </div>

메모리 관점에서 **array list** 는 한 곳에 모여있어야 해서 정해진 크기를 넘어 설 경우 다시 설계를 해서 더 큰 메모리 공간을 만들어 이동을 해야한다. 하지만 인덱싱하기에는 빠르다. 그리고 엘리먼트를 중간에 추가/삭제할 경우 엘리먼트 뒤에 있는 모든 엘리먼트의 자리 이동 필요하므로 추가/삭제가 느리다.

**linked list** 의 경우 새로운 엘리먼트가 들어올 경우 비어있는 메모리 공간에 들어가기만 하면 된다. 하지만 어느 위치에 있는지 한번에 알 수 없기 때문에 인덱싱하기 힘들다. 그리고 추가/삭제의 경우 노트의 참조값(next)만 변경하면 되기 때문에 추가/삭제 속도가 빠르다.

##### Linked list의 구조

<div align='center'>
     <img src=".\images\ds_1_2.png" style="zoom:40%;"/>
   </div>

<u>**리스트는 노드(엘리먼드, vertex)의 모임**</u>

=> 이들을 이어지게 만들어야 하니 현재 노드의 값과 다음 노드의 위치 정보(포인터나 참조 값)를 알고 있어야한다.

또한 첫번째 노드의 위치를 알려줄 **Head** 도 갖는다.

#### 1) single linked list

위의 Linked list의 구조와 같은 구성을 갖는다.

#### 2) double linked list

<div align='center'>
     <img src=".\images\ds_1_3.png" style="zoom:40%;"/>
   </div>

노드와 노드가 **<u>서로 연결</u>** 되어있다.

##### 장점

이를 통해 <u>양방향으로 탐색</u>이 가능하다는 장점을 갖는다. 이런 양방향 탐색의 이점은 <u>특정 인덱스 위치의 엘리먼트를 가져올 때와 반복을 이용해서 탐색</u>을 할 때 큰 이점을 갖는다.

<div align='center'>
     <img src=".\images\ds_1_4.png" style="zoom:40%;"/>
   </div>

탐색을 할 곳이 앞에서 가까우면 앞에서 부터 탐색 시작, 뒤에서 가까우면 뒤에서부터 앞으로 이동하며 탐색 => 빅오(***O***)가 반으로 줆

##### 단점

이전 노드 지정을 위한 변수를 더 사용해야함 -> 메모리 사용 증가

구현이 복잡

하지만 장점이 크기에 현실에서 사용하는 연결 리스트 대부분은 이중 연결 리스트

#### 3) circular linked list

단일 연결리스트와 다르게 마지막 노드가 첫 노드와 연결되어있는 리스트

리스트에 몇개의 노드가 들어가 있는지 알기위한 index값과 노드를 탐색할 때 기준 노드를 제시하기 위한 **head** 와 **tail** 로 나뉨

<div align='center'>
     <img src=".\images\ds_1_5.png" style="zoom:40%;"/>
   </div>

#### Reference

- [Linked list](https://opentutorials.org/module/1335/8821)

- [Doubly linked list (이중 연결 리스트)](https://opentutorials.org/module/1335/8940)
- [원형 연결 리스트(Circular Linked List)](https://supark7.tistory.com/entry/원형-연결-리스트-Circular-Linked-List?category=448614)

## #4

### queue(큐) : 순차 queue

<div align='center'>
     <img src=".\images\ds_4_queue.png">
   </div>

- FIFO(First In First Out) 구조 : 먼저 삽입된 item이 먼저 삭제됨
  - 한쪽 끝(Rear)에서는 삽입연산만 이뤄지고
  - 다른 한쪽 끝(Front)에서는 삭제만 이뤄지는 리스트
- 초기에는 `Front == Rear == -1`로 초기화
- 공백일 땐 `Front == Rear`
- 삽입될 땐 Rear가 점차 증가하며 `Rear == n-1`인 경우 꽉 찬 상태

##### 순차 queue의 문제점
- 정말 `Rear == n-1`일 때 queue는 꽉 찼을까?
  - front에서 삭제가 일어났다면 그만큼 공간이 비어있을 것!
- 따라서 `Rear == n-1`인 상태에는 queue의 첫번째 원소의 위치를 0번 index로 이동시켜줘야 한다.
  - queue 원소 이동에 따른 비용이 발생

#### Reference
- [진짜 개발자 : 자료구조 Queue](https://galid1.tistory.com/483)
---
## #4-1
### circular queue

<div align='center'>
     <img src=".\images\ds_4_circular_queue.png">
   </div>

- queue를 원형으로 구현
- 초기에는 `Front == Rear == 0`로 초기화
- 공백일 땐 `Front == Rear`
- 삽입될 땐 Rear가 점차 증가하며 `Rear+1 == Front`인 경우 꽉 찬 상태
  - 원형이기 때문에 full상태에서 원소 이동이 필요 없어짐!!!

 ### python deque
- python에는 queue를 쉽게 쓸 수 있는 collections.deque 클래스가 있음
- deque는 양방향 queue
  - 양방향으로 삽입할 수 있으며
    - `deque.append(item)` : deque의 오른쪽으로 append
    - `deque.appendleft(item)` : deque의 왼쪽으로 append
  - 양뱡향으로 삭제할 수 있음
    - `deque.pop()` : deque의 맨 오른쪽 원소 pop
    - `deque.popleft() : deque의 맨 왼쪽 원소 pop
      - 리스트의 경우 pop(0)을 하면 같음
##### 그러면 리스트 쓰면 될 것이지, 굳이 deque 왜 씀?
  - 빠르니까!
    - 리스트는 ***O(N)***
    - deque는 ***O(1)*** 연산을 수행
 ```python
from collections import deque
d = deque([1,2,3,4,5])
d.append(6)
print(d) #deque([1, 2, 3, 4, 5, 6])

d.appendleft(0)
print(d) #deque([0, 1, 2, 3, 4, 5, 6])

d.pop() #6

print(d) #deque([0, 1, 2, 3, 4, 5])

d.popleft() #0

print(d) #deque([1, 2, 3, 4, 5])
 ```

#### Reference
- [진짜 개발자 : 자료구조 Queue](https://galid1.tistory.com/483)
- [원형큐](https://daeguowl.tistory.com/112)



## #7

### heap(binary heap)

#### 힙이란?

트리 기반 자료구조로 힙 속성을 만족하는 거의 완전한 트리

##### 힙 속성이란?

예를 들어, 최대 힙(Max Heap)일 경우 부모 노드는 반드시 자식 노드보다 값이 커야한다는 법칙

-> 최상위 노드는 최대값을 가지게 됨

=> 이러한 힙의 특성으로 힙은 우선순위 큐를 구현하는데 적합한 자료구조

***참고.*** 힙은 부모와 자식 노드간의 관계만이 정의되어 있지, 형제 또는 사촌 노드 (선으로 직접 연결이 안된 노드) 간의 우선 순위는 정해진 것이 없다.

#### 이진 힙(binary heap)

힙 중에서 가장 널리 쓰이는 형태중 하나로 * **이진 트리** 형태의 힙

이진 힙은 힙 정렬 알고리즘을 위한 자료구조로 * **완전 이진 트리** 라는 조건을 만족해야 한다.

*이진 트리 : 각 노드의 자식 노드가 반드시 2개 이하인 트리

*완전 이진 트리 : 모든 레벨의 노드가 채워져있어야 하며, 마지막 레벨은 왼쪽부터 차 있어야한다.

#### 힙의 동작 (삽입 / 삭제)

기준은 위에서 언급한 것 처럼 max heap 기준 (파이썬은 heapq는 최소 힙(min heap)으로 구현되어 있다.)

##### 삽입(insert)

힙에 원소를 추가하기 위해 '업힙' 이라는 작업 수행. 아래는 15를 최대 힙에 추가하는 과정에 대한 예시

1. 원소를 힙의 가장 마지막 노드에 추가

   <div align='center'>
        <img src=".\images\ds_7_1.png" style="zoom:40%;"/>
      </div>

2. 추가한 원소를 부모와 비교, 순서가 힙 조건과 일치한다면 중지

   <div align='center'>
        <img src=".\images\ds_7_2.png" style="zoom:40%;"/>
      </div>

3. 힙 조건과 순서가 맞지 않다면 부모와 위치를 교환, 힙 조건과 일치할 때 까지 2~3반복

   <div align='center'>
        <img src=".\images\ds_7_3.png" style="zoom:40%;"/>
      </div>

##### 삭제(Delete)

루트 노드(가장 최상위 노드)는 힙의 종류에 따라 최대 값 혹은 최소 값을 가지게 된다. 따라서 최대값이거나 최소값을 탐색할 때 걸리는 시간은 항상 ***O***(1)이다.

값을 추출하고 다음 값을 루트로 만드는 작업을 '다운힙'이라고 한다.

다음은 최대 힙에서 삭제하는 과정의 예시이다

1. 힙의 루트 노드를 삭제

   <div align='center'>
        <img src=".\images\ds_7_4.png" style="zoom:40%;"/>
      </div>

2. 마지막 노드를 루트로 이동, 루트를 자식 노드와 비교. 이 때, 두 자식 노드 중 최대 힙인 경우 더 큰 자식과 비교하며 최소 힙인 경우 더 작은 자식과 비교함. 순서가 힙 조건(최대, 최소)과 일치하면 중지

   <div align='center'>
        <img src=".\images\ds_7_5.png" style="zoom:40%;"/>
      </div>

3. 만약 순서가 맞지 않는다면 위치 교환, 힙 조건이 일치 할 때 까지 2~3번 반복

   <div align='center'>
        <img src=".\images\ds_7_6.png" style="zoom:40%;"/>
      </div>

#### Reference

- [이진 힙](https://kayuse88.github.io/binary-heap/)



## #7-1

### Min Heap

heap의 규칙은 위에서 설명한 것과 같다.

min heap의 규칙은 <u>**부모 노드는 항상 자식 노드에 들어있는 값 보다 작다**</u>

## #7-2

### Max Heap

max heap의 규칙은 **<u>부모 노드는 항상 자식 노드에 들어 있는 값보다 크다</u>**





