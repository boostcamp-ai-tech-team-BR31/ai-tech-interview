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

## #2

### hash table

key, value의 데이터를 
key를 해시함수를 이용해 고정된 크기값에 맵핑한 데이터 구조

다른 내용의 데이터가 같은 키를 갖는 경우가 많으면 해시 충돌 --> 성능 하락.

![](images/hash.JPG)

충돌방지

체이닝 방식(separate chaining)

![](images/hash2.JPG)

선형검색(linear probing)

![](images/hash3.JPG)

각각의 key값은 해시함수에 의해 고유한 index를 가지게 되어 바로 접근할 수 있으므로 보통 O(1)의 시간복잡도로 데이터를 조회할 수 있다. 하지만 충돌이 발생한 경우 연결된 리스트들까지 검색해야하므로 O(N)까지 시간복잡도가 증가할 수 있다.

### Reference

+ [Hash Table interview](https://www.fullstack.cafe/blog/hash-tables-interview-questions)

## #4

### queue
- 미완성 >~< by tttangmin
- First In First out
- push
- pop
### Reference
- []()
---
## #4-1
### circular queue
- queue를 원형으로 구현
  - 기존 queue는 linear
### Reference
- []()



