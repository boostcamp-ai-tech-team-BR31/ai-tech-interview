<div align='center'>
  <h1>🖥️ Operating System 🖥️</h1>
</div>

> 질문은 <strong>[WeareSoft님의 tech-interview](https://github.com/WeareSoft/tech-interview)</strong>를 참고하였습니다.

---

## Table of Contents

- [프로세스와 스레드의 차이(Process vs Thread)를 알려주세요.](#1)
- [멀티 프로세스 대신 멀티 스레드를 사용하는 이유를 설명해주세요.](#2)
- [캐시의 지역성에 대해 설명해주세요.](#3)
- [Thread-safe에 대해 설명해주세요. (hint: critical section)](#4)
- [뮤텍스와 세마포어의 차이를 설명해주세요.](#5)
- [스케줄러가 무엇이고, 단기/중기/장기로 나누는 기준에 대해 설명해주세요.](#6)
- [CPU 스케줄러인 FCFS, SJF, SRTF, RR, Priority Scheduling에 대해 간략히 설명해주세요.](#7)
- [동기와 비동기의 차이를 설명해주세요.](#8)
- [메모리 관리 전략에는 무엇이 있는지 간략히 설명해주세요.](#9)
- [가상 메모리에 대해 설명해주세요.](#10)
- [교착상태(데드락, Deadlock)의 개념과 조건을 설명해주세요.](#11)
- [사용자 수준 스레드와 커널 수준 스레드의 차이를 설명해주세요.](#12)
- [외부 단편화와 내부 단편화에 대해 설명해주세요.](#13)
- [Context Switching이 무엇인지 설명하고 과정을 나열해주세요.](#14)
- [Swapping에 대해 설명해주세요.](#15)

---

## #1
### 프로세스와 스레드의 차이(Process vs Thread)를 알려주세요.
#### 개념 정의
`
한줄요약: 프로그램 -> 프로세스 -> 스레드
`
- **프로그램(Program)**: 파일이 저장 장치에 저장되어 있지만 메모리에는 올라가 있지 않은 `정적`인 상태.
  - 아직 실행되지 않은 파일 그 자체를 가르킴.
- **프로세스(Process)**: 운영체제로부터 자원을 할당받은 `작업`의 단위.
  - 프로그램을 실행 -> 메모리에 올라감 -> 동적인 상태 -> 이 상태의 프로그램을 프로세스라고 함.
- **스레드(Thread)**: 프로세스가 할당받은 자원을 이용하는 `실행 흐름`의 단위.
  - 프로세스 내에서 실행되는 여러 흐름의 단위
    - 즉 프로세스는 최소 1개의 스레드를 갖고 있음

#### 프로세스와 스레드의 차이
가장 큰 특징은 메모리 공유.
OS가 **프로세스**에게 code/data/stack/heap 메모리 영역을 할당해 최소 작업 단위로 삼지만
**스레드**는 프로세스 내에서 stack 메모리 영역을 제외한 다른 메모리 영역을 같은 프로세스 내 다른 스레드와 공유.
이로 인한 각각의 장단점은 #2에서 다룸!
### Reference

- [프로세스와 스레드의 차이](https://velog.io/@raejoonee/%ED%94%84%EB%A1%9C%EC%84%B8%EC%8A%A4%EC%99%80-%EC%8A%A4%EB%A0%88%EB%93%9C%EC%9D%98-%EC%B0%A8%EC%9D%B4)

## #3

#### 캐시의 지역성에 대해 설명해주세요.

**캐시 메모리(Cash Memory)**

- CPU의 처리 속도와 메모리의 속도 차이로 인한 병목현상을 완화하기 위해 사용하는 고속 버퍼 메모리

- 주기억장치에서 자주 사용하는 프로그램과 데이터를 저장행두어 속도를 빠르게 하는 메모리
  - 주기억장치 보다 크기가 작다
- 주기억장치와 CPU사이에 위치
- 캐시 메모리에 먼저 접근후에 없으면 메인메모리로 접근



**지역성(Locality)**

- 어떻게 자주 사용하는 기준을 판단하여 정보를 캐시 메모리에 저장할까? 이때 사용하는 개념이 지역성(Locality)의 원리
- `지역성(Locality)`이란 기억 장치 내의 정보를 균일하게 액세스하는 것이 아닌 어느 한순간에 특정 부분을 집중적으로 참조하는 특성
- 지역성은 크게 2가지 시간적 지역성(Temporal Locality)`, `공간적 지역성(Spatial Locality) 존재
- 시간적 지역성(Temporal Locality): 현재 사용되는 데이터는 곧 다시 쓰일것이다.
- 공간적 지역성(Spatial Locality): 현재 사용되는 메모리 근처의 데이터는 곧 사용될 것이다.
- 그러나 지역성은 어디까지나 경향에 대한 것이므로 항상 캐시의 높은 적중률(캐시 메모리가 쓰이냐 안 쓰이냐)을 보장해 주지는 않는다.

#### Reference

- [[OS] 캐시 메모리(Cache Memory)란? 캐시의 지역성(Locality)이란?](https://chelseashin.tistory.com/43)
- [ 캐시가 동작하는 아주 구체적인 원리](https://parksb.github.io/article/29.html)

- [Locality of Reference and Cache Operation in Cache Memory](https://www.geeksforgeeks.org/locality-of-reference-and-cache-operation-in-cache-memory/)



## #9

#### 메모리 관리 전략에는 무엇이 있는지 간략히 설명해주세요

