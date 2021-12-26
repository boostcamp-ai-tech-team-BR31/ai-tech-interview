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

#### 메모리 관리 전략에는 무엇이 있는지 간략히 설명해주세요.

메모리 관리는 메모리 location을 추적하여 얼마나 많은 메모리가 할당되었는지를 확인하고, 어느 시정에 어떤 process가 메모리가 필요한지를 결정한다. Anallocated 되거나 자유로운 메모리가 발생하면 그것의 상태를 업데이트한다.

#### Swapping

Swapping은 Profcess를 일시적으로 main memory에서 second storage(disk)로 swap(swap out)하는 메카니즘입니다. 잠시후에 시스템은 다시 해당 process를 secondary storage로 부터 main memeory로 swap back(swap in) 합니다. 

Performance(성능?)은 보통 swapping process에 영향을 받지만 다양하고 큰 process를 병렬적으로 처리할 수 있다. 이 때문에 swapping은 메모리압축기술로도 알려져있답니다.



<div align='center'>
     <img src=".\images\OS_9_1.JPG">
   </div>

- 스와핑 프로세스에 걸리는 총 시간에는 전체 프로세스를 보조 디스크로 이동한 다음 프로세스를 다시 메모리로 복사하는 데 걸리는 시간과 프로세스가 주 메모리를 다시 얻는 데 걸리는 시간이 포함

#### Fragmentation(단편화)

프로세스들이 메모리에 적재되고 제거되는 일이 반복되다보면 프로세스들이 차지하는 메모리 틈 사이에 사용하지 못할 만큼의 작은 자유공간들이 늘어가게 되는데, 이것이 **단편화**이다. 단편화는 2가지 종류로 나뉜다.

- **External fragmentation(외부 단편화)**

  메모리 공간 중 사용하지 못하게 되는 일부분. 물리 메모리(RAM)에서 사이사이 남는 공간들을 모두 합치면 충분히 공간이 되는 부분들이 분상되어 있을 때 발생한다고 볼 수 있다.

- **Internal fragmentation(내부 단편화)**
  프로세스가 사용하는 메모리 공간에 포함된 남는 부분. 예를 들어 메모리 분할 자유 공간이 10,000B 있고 Process A가 9,998B 사용하게 되면 2B 라는 차이가 존재하고, 이를 내부 단편화라 칭한다.

<div align='center'>
     <img src=".\images\OS_9_2.JPG">
   </div>

외부 단편화는 compaction(압축) 또는 shuffle memory 내용을 통해 모든 여유 메모리를 하나의 큰 블록에 함께 배치함으로써 줄일 수 있습니다. ~~압축이 가능하도록 하려면 dynamic relocation 이어야 합니다.~~

내부 단편화는 프로세스를 처리기에는 충분히 큰 것중에 가장 작은 파티션을 효율적으로 할당함으로써 줄일 수 있습니다.

#### paging(페이징)

paging은 process address space을 page라고 하는 동일한 크기의 블록으로 나누는 메모리 관리 기술입니다.(크기는 2의 거듭제곱, 512바이트에서 8192바이트 사이). 프로세스의 크기는 페이지 수로 측정됩니다.

마찬가지로 main memory는 frame이라는 작은 고정 크기의 (물리적) 메모리 블록으로 나뉘며 frame의 크기는 page의 크기와 동일하게 유지되어 main memory를 최적으로 활용하고 external fragmentation(외부 단편화)를 방지합니다.



<div align='center'>
     <img src=".\images\OS_9_3.JPG">
   </div>

- Frame에서 page로 system을 할당할 때 address translation과정(logical -> physical) 추가적으로 있는데 참고 자료 첨부합니다

**장점**

- paging 은 구현하기 쉽고 효율적인 메모리 관리 기술 
- page와 frame의 크기가 동일하기 때문에 swapping이 매우 쉬움
- 논리 메모리는 물리 메모리에 저장될 때, 연속되어 저장될 필요가 없음

**단점**

- 물리 메모리의 남는 프레임에 적절히 배치됨으로 외부 단편화를 해결할 수 있으나 내부 단편화 문제점 여전히 존재.
- Page table(Address translation 과정에서 사용됨)이 추가적인 메모리 공간을 필요로 하기 때문에 작은 크기의 RAM에서는 좋은 방법이 아닐 수 있다.

#### Segmentation(세그멘테이션)

한 Process를 페이징에서처럼 논리메모리와 물리메모리를 같은 크기의 블록이 아닌 서로 다른 크기의 **논리적 단위**인 세그먼트(Segment)로 분할. 각 segemetntaion은 **연관된 기능**을 수행하고, 프로그램에 **다른 logical address(논리적 주소)**를 갖고있다.

Segmentation Memory management는 paging과 매우 유사하만 segmentation은 가변 길이를 갖고 있고 paging page는 고정된 크기를 갖고있다.

<div align='center'>
     <img src=".\images\OS_9_4.JPG">
   </div>

#### Reference

- [Operating System - Memory Management](!https://www.tutorialspoint.com/operating_system/os_memory_management.htm)
- [[CS 기초 - 운영체제] 메모리 관리 전략](!https://velog.io/@deannn/CS-%EA%B8%B0%EC%B4%88-%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C-%EB%A9%94%EB%AA%A8%EB%A6%AC-%EA%B4%80%EB%A6%AC-%EC%A0%84%EB%9E%B5)

