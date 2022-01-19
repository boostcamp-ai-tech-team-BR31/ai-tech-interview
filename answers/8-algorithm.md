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



## #2-2

#### Selection Sort

**선택 정렬**(selection sort)은 정렬 알고리즘의 하나로, 다음과 같은 순서로 이루어진다.

1. 주어진 리스트 중에 최소값을 찾는다.
2. 그 값을 맨 앞에 위치한 값과 교체한다(패스(pass)).
3. 맨 처음 위치를 뺀 나머지 리스트를 같은 방법으로 교체한다.

- n개의 주어진 리스트를 이와 같은 방법으로 정렬하는 데에는 $Θ(n^2) $만큼의 시간 복잡도를 갖는다.(n개의 원소  n-1번 비교)

- 선택 정렬은 알고리즘이 단순하며 사용할 수 있는 메모리가 제한적인 경우에 사용시 성능 상의 이점이 있다.
- 입력 배열이 이미 정렬되어 있건 말건 관계없이 동일한 연산량을 가지고 있기 때문에 최적화 여자가 적어서 다른 `O(N^2)` 대비해도 성능이 떨어지는 편으로 실전에서 거의 쓰이지 않는다.

<div align='center'>
    <img src='./images/algo-2-2.png' width='500px'>
</div>



**Python Code**

```python
def selection_sort(arr):
    for i in range(len(arr) - 1):
        min_idx = i
        for j in range(i + 1, len(arr)):
            if arr[j] < arr[min_idx]:
                min_idx = j
        arr[i], arr[min_idx] = arr[min_idx], arr[i]
```

#### References

- [선택 정렬(Selection Sort) 이란?](https://gmlwjd9405.github.io/2018/05/06/algorithm-selection-sort.html)
- [ 선택 정렬 - Selection Sort](https://www.daleseo.com/sort-selection/)
- [선택 정렬 from wikipedia](https://ko.wikipedia.org/wiki/%EC%84%A0%ED%83%9D_%EC%A0%95%EB%A0%AC)

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

## #2-8

#### Radix Sort(기수 정렬)

기수 정렬(Radix Sort)은 입력값의 자릿수(d) 각각에 대해 카운팅 정렬을 적용하여 입력 데이터의 최댓값인 k가 커질수록 효율이 떨어지는 카운팅 정렬의 단점을 보완한 정렬 알고리즘이다. 

Radix(기수)는 '자리수'를 의미하는 것으로 기수 정렬은 다음과 같은 순서로 이뤄진다.

**1. 1의 자릿수를 보면서 각각의 버킷에 알맞게 담아준다. 버킷에서 순차적으로 뺀다면 1의 자릿수에 맞게 정렬이된다.**

**2. 1)에 의해서 정렬된 배열에서, 10의 자릿수를 비교해서 버킷에 담고 순차적으로 빼준다.**

**3. 2)에 의해서 정렬된 배열에서, 100의 자릿수를 비교해서 버킷에 담고 순차적으로 빼준다.**

**4. 최대 자릿수까지 계속해서 반복한다..**

`[121, 432, 564, 23, 1, 45, 788]`가 주어졌을 때 radix sort를 적용한 과정과 결과는 다음과 같다.

<div align='center'>
    <img src='./images/Radix-sort-0_0.png' width='500px'>
</div>

위 예시의 과정

1. 주어진 리스트의 최대값을 찾고 최대값의 자리수(Radix)를 계산한다. 여기서는 788로 자리수는 3이다.

2. 각 자리수에 대해 counting sort를 적용한다. 첫번째는 1의 자리에 대해서 counting sort 적용

   <div align='center'>
       <img src='./images/Radix-sort-one.png' width='500px'>
   </div>

3. 2의 결과를 이용하여 10의 자리에 대해서 counting sort를 적용

<div align='center'>
    <img src='./images/Radix-sort-ten.png' width='500px'>
</div>

4. 3의 결과를 이용하여 100의 자리에 대해서 counting sort를 적용

   <div align='center'>
       <img src='./images/Radix-sort-hundred.png' width='500px'>
   </div>

Radix sort의 경우 중간에 counting sort를 사용하기 때문에 시간 복잡도는 `O(d(n+k))` 이다. 여기서 `d`는 최대값의 자리수(cycle의 횟수)이고 `n+k`는 counting sort에서 오는 시간 복잡도인데 Radix sort는 k = 10이다.

빠르고 counting sort을 개선한 방법이지만 여전히 추가적인 메모리가 필요하고 데이터 타입이 바뀌면 새로 정의해주어야 한다.(10진수 -> 16진수)

**Python Code**
Version 1
```python
from collections import deque

def radix_sort(nums):
    buckets = [deque() for _ in range(10)]

    max_val = max(nums)
    Q = deque(nums)
    cur_ten = 1

    while max_val >= cur_ten:
        while Q:
            num = Q.popleft()
            buckets[(num // cur_ten) % 10].append(num)

        for bucket in buckets:
            while bucket:
                Q.append(bucket.popleft())

        cur_ten *= 10
    return list(Q)

print(radix_sort([15, 27, 64, 25, 50, 17, 39, 28]))
```

Version 2
```python
# Radix sort in Python


# Using counting sort to sort the elements in the basis of significant places
def countingSort(array, place):
    size = len(array)
    output = [0] * size
    count = [0] * 10

    # Calculate count of elements
    for i in range(0, size):
        index = array[i] // place
        count[index % 10] += 1

    # Calculate cumulative count
    for i in range(1, 10):
        count[i] += count[i - 1]

    # Place the elements in sorted order
    i = size - 1
    while i >= 0:
        index = array[i] // place
        output[count[index % 10] - 1] = array[i]
        count[index % 10] -= 1
        i -= 1

    for i in range(0, size):
        array[i] = output[i]


# Main function to implement radix sort
def radixSort(array):
    # Get maximum element
    max_element = max(array)

    # Apply counting sort to sort elements based on place value.
    place = 1
    while max_element // place > 0:
        countingSort(array, place)
        place *= 10


data = [121, 432, 564, 23, 1, 45, 788]
radixSort(data)
print(data)
```





#### References

- [기수 정렬 설명 블로그 - 1](https://yabmoons.tistory.com/248l)
- [기수 정렬 설명 블로그 - 2](https://week-year.tistory.com/206)
- [Radix-sort Algorithm from programiz](https://www.programiz.com/dsa/radix-sort)

## #4

### Dynamic Programming

큰 문제에 대한 답을 얻기 위해 동일한 문제이지만 크기가 더 작은 문제들을 먼저 해결한 뒤, 그 결과들을 이용해 큰 문제를 비교적 간단하게 해결하는 기법

Top down with Memoization

Bottom up with Tabulation

#### References

+ [Dynamic Programming](https://www.interviewbit.com/courses/programming/topics/dynamic-programming/)

## #6

### Graph

- 그래프 관련 용어
    - 정점(node, vertex) : 자료
    - 간선(edge) : 정점 간의 관계
    - 가중치(weight) : 간선의 거리
    - 차수(degree) : 그래프와 연결된 간선의 개수
    - 단순경로(simple path) : 하나의 정점을 최대 한 번씩만 방문한 경로
    - cycle : 단순 경로의 출발점과 도착증이 같은 경우
- 그래프 종류
    - 양방향 그래프(=무방할 그래프)
    - 방향 그래프
    - 완전 그래프 : 각 정점에서 자신을 제외한 모든 정점과 연결된 그래프
        - 간선의 개수 : $\frac{V(V-1)}{2}$
    - 다중 그래프 : 두 정점 사이에 여러개의 간선이 있는 그래프
    - 사이클 없는 방향 그래프
    - 부분 그래프 : 정점이나 간선을 제외하여 만든 그래프
    - 이분 그래프 : 인접 정점까지 서로 다른 색으로 칠했을 때, 모든 정점을 두 가지 색으로 칠할 수 있는 그래프
- 그래프 표현
  - 인접 리스트
  - 인접 행렬
