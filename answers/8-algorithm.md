<div align='center'>
  <h1>🔻 Algorithm 🔻</h1>
</div>

> 질문은 <strong>[WeareSoft님의 tech-interview](https://github.com/WeareSoft/tech-interview)</strong>를 참고하였으며, 질문에 대한 답변은 직접 작성하였습니다.

---

## Table of Contents

- [시간, 공간 복잡도](#1)
- Sort Algorithm
  - [Bubble Sort](#2-1)
  - [Selection Sort](#2-2)
  - [Insertion Sort](#2-3)
  - [Merge Sort](#2-4)
  - [Heap Sort](#2-5)
  - [Quick Sort](#2-6)
  - [Counting Sort](#2-7)
  - [Radix Sort](#2-8)
- [Divide and Conquer](#3)
- [Dynamic Programming](#4)
- [Greedy Algorithm](#5)
- [Graph](#6)
  - [Graph Traversal: BFS, DFS](#6-1)
  - [Shortest Path](#6-2)
    - [Dijkstra](#6-2-1)
    - [Floyd-Warshall](#6-2-2)
    - [Bellman-Ford](#6-2-3)
  - [Minimum Spanning Tree](#6-3)
    - [Prim](#6-3-1)
    - [Kruskal](#6-3-2)
  - [Union-find](#6-4)
  - [Topological Sort](#6-5)

---

## #1

### 시간, 공간 복잡도

복잡도는 알고리즘 성능 평가의 척도
- 시간 복잡도 : 알고리즘의 연산 횟수
- 공간 복잡도 : 알고리즘의 메모리 공간

복잡도는 점근적 표기법(Asymptotic Notation)으로 나타냄
<div align='center'>
    <img src='./images/algo_1_Asymptotic_Notation.jpeg' height='400px'>
</div>
<br>

y축 : 복잡도(시간이나 메모리) -> 낮을수록 좋음
- 빅오(O) 표기법
  - 상한선 : 최악의 경우
- 오메가(Ω) 표기법
  - 하한선 : 최상의 경우
- 세타(θ) 표기법
  - 상한선과 하한선의 교집합 : 평균의 경우



#### References

- [점근적 표기법](https://ledgku.tistory.com/31)

---

## #2-4

### Merge Sort

+ 분할 단계와 병합 단계로 나눌 수 있으며, 중간인덱스를 찾아야하는 분할 비용보다 각 단계마다 값들을 모두 비교해서 병합해야 하는 비용이 크다.

+ 각 단계에서 모든 값을 비교해야 하므로 N*단계의 수 logN시간이 필요하다. 비교 = NlogN

  각 단계에서 임시배열에 복사했다가 다시 가져와야 하므로 이동 연산 2N

  이동 = 2NlogN (연결리스트로 구성하면 링크 인덱스만 변경되므로 데이터의 이동은 무시할 수 있을 정도로 작아진다.)

  총 시간 복잡도는 O(NlogN)

**References**

+ [병합 정렬](https://www.daleseo.com/sort-merge/)
+ [합병 정렬](https://gmlwjd9405.github.io/2018/05/08/algorithm-merge-sort.html)

## #2-6

### Quick Sort

<div align='center'>
    <img src='./images/' height='400px'>
</div>
<br>

#### References

- []()

## #4

### Dynamic Programming

큰 문제에 대한 답을 얻기 위해 동일한 문제이지만 크기가 더 작은 문제들을 먼저 해결한 뒤, 그 결과들을 이용해 큰 문제를 비교적 간단하게 해결하는 기법

Top down with Memoization

Bottom up with Tabulation

#### References

+ [Dynamic Programming](https://www.interviewbit.com/courses/programming/topics/dynamic-programming/)