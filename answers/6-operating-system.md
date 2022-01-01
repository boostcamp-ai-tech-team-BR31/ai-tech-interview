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



## #5

#### 뮤텍스와 세마포어의 차이를 설명해주세요.

Mutex = Mutual + Exclusion (상호 배제)

여러 스레드를 실행하는 환경에서 자원에 대한 접근에 제한을 강제하기 위한 메커니즘 

lock, blocking, sleep

## #9

#### 메모리 관리 전략에는 무엇이 있는지 간략히 설명해주세요



## #11

#### 교착상태(데드락, Deadlock)의 개념과 조건을 설명해주세요.

교착상태  -  두 가지 이상의 작업이 서로 상대방의 작업이 끝나기만을 하염없이 기다리는 상태. 서로 자원을 놓아줄 생각은 없고 자원 요청을 무한정 대기하고 있는 상태

네 가지 조건

상호 배제 - 프로세스들이 필요로 하는 자원에 대해 배타적인 통제권을 요구하는 것. 하나의 프로세스가 공유 자원을 사용할 때, 다른 프로세스가 동일한 공유자원에 접근할 수 없도록 통제하는 것.
