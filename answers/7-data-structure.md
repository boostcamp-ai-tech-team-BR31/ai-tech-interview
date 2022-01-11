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
 
#### Reference
- [진짜 개발자 : 자료구조 Queue](https://galid1.tistory.com/483)
- [원형큐](https://daeguowl.tistory.com/112)