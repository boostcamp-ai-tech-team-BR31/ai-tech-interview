<div align='center'>
  <h1>🌐 Network 🌐</h1>
</div>

> 질문 중 일부는 <strong>[WeareSoft님의 tech-interview](https://github.com/WeareSoft/tech-interview)</strong>를 참고하였습니다.

---

## Table of Contents

- [TCP/IP의 각 계층을 설명해주세요.](#1)
- [OSI 7계층와 TCP/IP 계층의 차이를 설명해주세요.](#2)
- [Frame, Packet, Segment, Datagram을 비교해주세요.](#3)
- [TCP와 UDP의 차이를 설명해주세요.](#4)
- [TCP와 UDP의 헤더를 비교해주세요.](#5)
- [TCP의 3-way-handshake와 4-way-handshake를 비교 설명해주세요.](#6)
- [TCP의 연결 설정 과정(3단계)과 연결 종료 과정(4단계)이 단계가 차이나는 이유가 무엇인가요?](#7)
- [만약 Server에서 FIN 플래그를 전송하기 전에 전송한 패킷이 Routing 지연이나 패킷 유실로 인한 재전송 등으로 인해 FIN 패킷보다 늦게 도착하는 상황이 발생하면 어떻게 될까요?](#8)
- [초기 Sequence Number인 ISN을 0부터 시작하지 않고 난수를 생성해서 설정하는 이유가 무엇인가요?](#9)
- [HTTP와 HTTPS에 대해서 설명하고 차이점에 대해 설명해주세요.](#10)
- [HTTP 요청/응답 헤더의 구조를 설명해주세요.](#11)
- [HTTP와 HTTPS 동작 과정을 비교해주세요.](#12)
- [CORS가 무엇인가요?](#13)
- [HTTP GET과 POST 메서드를 비교/설명해주세요.](#14)
- [쿠키(Cookie)와 세션(Session)을 설명해주세요.](#15)
- [DNS가 무엇인가요?](#16)
- [REST와 RESTful의 개념을 설명하고 차이를 말해주세요.](#17)
- [소켓(Socket)이 무엇인가요? 자신 있는 언어로 간단히 소켓 생성 예시를 보여주세요.](#18)
- [Socket.io와 WebSocket의 차이를 설명해주세요.](#19)
- [IPv4와 IPv6 차이를 설명해주세요.](#20)
- [MAC Address가 무엇인가요?](#21)
- [라우터와 스위치, 허브의 차이를 설명해주세요.](#22)
- [SMTP가 무엇인가요?](#23)
- [노트북으로 `www.google.com`에 접속을 했습니다. 요청을 보내고 받기까지의 과정을 자세히 설명해주세요.](#24)
- [여러 네트워크 topology에 대해 간단히 소개해주세요.](#25)
- [subnet mask에 대해서 설명해주세요.](#26)
- [data encapsulation이 무엇인가요?](#27)
- [DHCP를 설명해주세요.](#28)
- [routing protocol을 몇 가지 설명해주세요. (ex. link state, distance vector)](#29)
- [이더넷(ethernet)이 무엇인가요?](#30)
- [client와 server의 차이점을 설명해주세요.](#31)
- [delay, timing(jitter), throughput 차이를 설명해주세요.](#32)

---


## #1

### TCP/IP 각 계층을 설명해주세요.

데이터 전송을 담당하는 

1. 네트워크 인터페이스 계층

2. 인터넷 계층

3. 전송계층

전송된 데이터의 내용을 보고 사용자가 이용할 수 있는 서비스를 제공하는

4. 응용계층



 응용계층은 애플리케이션이 제공하는 서비스마다 개별적인 기능을 구현하기 때문에 다른 계층과 달리 하나의 계층으로서 두드러진 특징이 있다기보다 애플리케이션마다 별개로 존재하는 프로토콜들이 독자적인 특징을 갖고있음.

 수많은 컴퓨터와 네트워크 장비가 연결된 인터넷에서 네트워크 인터페이스 계층이 ① 물리적으로 직접 연결된 기기 간의 데이터 통신을 제어하고, 인터넷 계층이②직접 연결되지 않은 컴퓨터까지 데이터를 전송하기 위해 네트워크 간의 데이터 통신을 구현하며, 전송 계층이 ③송신지에서 수신지까지 데이터의 흐름을 제어하고 수신지 컴퓨터에 도착한 데이터가 어떤 애플리케이션에서 사용하는 것인지 판단해서 데이터를 배분함으로써 데이터 통신 기능이 구현됨.

#### Reference

- [TCP/IP 계층의 특징과 역할 및 프로토콜](https://better-together.tistory.com/82)

## #2

### OSI 7계층과 TCP/IP 계층의 차이를 설명해주세요.

<div align='center'>
     <img src="./images/network_2.png">
   </div>

### OSI 7계층

1. **물리계층 (Physical Layer)**
   - **전기적, 기계적, 기능적인 특성을 이용하여 통신 케이블로 데이터를 전송**한다.
2. **데이터 링크계층 (DataLink Layer)**
   - **물리 계층을 통해 송수신되는 정보의 오류와 흐름을 관리하여 안전한 정보의 수행을 도와주는 역할**을 한다.
3. **네트워크 계층 (Network Layer)**
   - 데이터를 목적지까지 가장 안전하고 빠르게 전달하는 기능을 한다.
   - **경로를 선택하고 주소를 정하고 경로에 따라 패킷을 전달해주는 역할**을 한다.
   - 대표적인 장비로 라우터, (라우팅 기능이 포함된)스위치가 있으며, **IP 주소를 사용**한다.
4. **전송 계층 (Transport Layer)**
   - **통신을 활성화하기 위한 계층**이다. 보통 **TCP 프로토콜을 사용**하며, 포트를 열어서 응용 프로그램을 전송한다.
5. **세션 계층 (Session Layer)**
   - **데이터가 통신하기 위한 논리적인 연결**을 한다.
   - **세션 설정, 유지, 종료, 전송 중단시 복구 등의 기능**이 있다.
6. **표현 계층 (Presentation Layer)**
   - **데이터 표현이 상이한 응용 프로세스의 독립성을 제공하고, 암호화**한다.
   - 해당 데이터가 텍스트인지, 그림인지, GIF인지, JPG인지의 구분 등의 역할을 한다.
7. **응용 계층 (Application Layer)**
   - 최종 목적지로서 HTTP, FTP, SMTP, Telnet 등과 같은 프로토콜이 있다.
   - **응용 프로세스와 직접 관계하여 일반적인 응용 서비스를 수행**한다.
   - 네트워크 소프트웨어의 UI 부분, 사용자의 입출력 부분을 담당한다.



OSI 계층은 TCP/IP 계층의 응용 계층을 더 세분화한 것이다. 

네트워크 전송시 **테이터 표준을 정리**한 것이 **OSI계층**이라면, 이 이론을 실제로 사용하는 **인터넷 표준**이 **TCP/IP**계층이다.

#### Reference

- [OSI 7계층, TCP/IP 4계층 모델](https://devowen.com/344)


## #3

### Frame, Packet, Segment, Datagram을 비교해주세요.
(❊ TCP/IP 5계층 기준으로 설명한다.)

Frame, Packet, Segment, Datagram은 데이터를 송수신할 때, TCP/IP 5계층에서 각각 만들어지는 데이터 입니다.

**Packet**은 pack과 bucket의 합친 말입니다. 우체국에서 화물을 적당한 덩어리로 나눠 행선지를 표시하는 꼬리를 붙이는데, 이 과정을 데이터 통신에 접목한 것입니다.

큰 데이터는 대역폭을 너무 많이 차지하기 때문에 쪼개서 트래픽이 많아집니다. 그래서 데이터를 Packet들로 분할하게 됩니다. 이러한 교환 방식을 **패킷 교환 방식**이라고 합니다.

#### #데이터 송신

<div align='center'>
     <img src="./images/network_#3_1.png">
   </div>
1. 응용 계층에서 요청 데이터가 만들어진다.

2. 전송 계층에서 신뢰할 수 있는 통신을 구현하기 위한 헤더를 데이터에 붙인다. 이렇게 만들어진 데이터를 **세그먼트**라고 한다.

3. 네트워크 계층에서 다른 네트워크와 통신하기 위한 헤더를 세그먼트에 붙인다. 이렇게 만들어진 데이터를 **패킷** 또는 **데이터그램**이라고 한다.

4. 데이터 링크 계층에서 물리적인 통신 채널을 열기 위해 패킷에 헤더와 트레일러를 붙인다. 여기서 트레일러는 데이터를 전달할 때 데이터 끝부분에 붙이는 정보로, 주로 에러 검출에 쓰인다. 이렇게 만들어진 데이터를 **프레임**이라고 한다.

5. 이렇게 만들어진 프레임을 최종적으로 물리 계층에서 0, 1의 비트로 구성된 전기 신호로 변환해 수신 컴퓨터 쪽에 전송한다.

- 이 단계를 **캡슐화**라고 합니다

#### #데이터 수신

<div align='center'>
     <img src="./images/network_#3_2.png">
   </div>

- 데이터 수신할 땐, 반대로 헤더를 제거하며 데이터를 전달하는 **역캡슐화** 과정을 거칩니다.


### References

- [패킷이란 무엇일까? 패킷의 정의와 구조 - Jay's Blog](https://enlqn1010.tistory.com/9)
- [[네트워크] TCP/IP 5계층에서 일어나는 일 (1) - 코알라일락's BLOG](https://zion830.tistory.com/104)

## #4

### TCP와 UDP의 차이를 설명해주세요

**TCP(Transmission Control Protocol)** 

> 인터넷상에서 데이터를 메세지의 형태로 보내기 위해 IP와 함께 사용하는 프로토콜

**UDP(User Datagram Protocol)**

> IP를 사용하는 네트워크 내에서 컴퓨터들 간에 메시지들이 교환될 때 제한된 서비스만을 제공하는 통신 프로토콜

<div align='center'>
     <img src="./images/Network_5.JPG">
   </div>

UDP는 TCP에 비해 일방적인 프로토콜이다.

**신뢰성이 요구되는 애플리케이션에서는 TCP를 사용하고** **간단한 데이터를 빠른 속도로 전송하고자하는 애플리케이션에서는 UDP를 사용한다.**

## #5

#### TCP와 UDP의 헤더를 비교해주세요.

TCP(Transmission Control Protocol) Vs UDP(User Datagram Protocol)

두 프로토콜은 모두 [패킷](https://velog.io/@hidaehyunlee/TCP-와-UDP-의-차이)을 한 컴퓨터에서 다른 컴퓨터로 전달해주는 `IP 프로토콜`을 기반으로 구현되어 있지만, 서로 다른 특징을 갖는다.

<div align='center'>
     <img src="./images/Network_5.JPG">
   </div>

TCP는 데이터를 확실히 송 수신 했는지 확인하고 송 수신 속도를 조절한다면 UDP는 일방적으로 데이터를 송신하기만 한다.

따라서  **신뢰성이 요구되는 애플리케이션에서는 TCP를 사용**하고 **간단한 데이터를 빠른 속도로 전송하고자 하는 애플리케이션에서는 UDP를 사용**한다.

<div align='center'>
     <img src="./images/network_5-2.JPG">
   </div>



### TCP 헤더 정보

| **필드**                      | **크기** | **내용**                                                     |
| ----------------------------- | -------- | ------------------------------------------------------------ |
| 송수신자의 포트 번호          | 16       | TCP로 연결되는 가상 회선 양단의 송수신 프로세스에 할당되는 포트 주소 |
| 시퀀스 번호 (Sequence Number) | 32       | 송신자가 지정하는 순서 번호, 전송되는 바이트 수를 기준으로 증가 SYN = 1 : 초기 시퀀스 번호가 된다. ACK 번호는 이 값에 1을 더한값 SYN = 0 : 현재 세션의 이 세그먼트 데이터의 최초 바이트 값의 누적 시퀀스 번호 |
| 응답 번호 (ACK Number)        | 32       | 수신 프로세스가 제대로 수신한 바이트 수를 응답하기 위해 사용 |
| 데이터 오프셋 (Data Offset)   | 4        | TCP 세그먼트의 시작 위치를 기준으로 데이터의 시작 위치를 표현(TCP 헤더의 크기) |
| 예약 필드(Reserved)           | 6        | 사용을 하지 않지만 나중을 위한 예약 필드이며 0으로 채워져야한다. |
| 제어 비트(Flag Bit)           | 6        | SYN, ACK, FIN 등의 제어 번호                                 |
| 윈도우 크기(Window)           | 16       | 수신 윈도우의 버퍼 크기를 지정할 때 사용. 0이면 송신 프로세스의 전송 중지 |
| 체크섬(Checksum)              | 16       | TCP 세그먼트에 포함되는 프로토콜 헤더와 데이터에 대한 오류 검출 용도 |
| 긴급 위치(Urgent Pointer)     | 16       | 긴급 데이터를 처리하기 위함, URG 플래그 비트가 지정된 경우에만 유효 |

### UDP의 헤더정보

| **필드**           | **크기** | **내용**                                 |
| ------------------ | -------- | ---------------------------------------- |
| 송신자의 포트 번호 | 16       | 데이터를 보내는 어플리케이션의 포트 번호 |
| 수신자의 포트 번호 | 16       | 데이터를 받을 어플리케이션의 포트 번호   |
| 데이터의 길이      | 16       | UDP 헤더와 데이터의 총 길이              |
| 체크섬(Checksum)   | 16       | 데이터 오류 검사에 사용                  |

- UDP 헤더는 8B(바이트)이고 TCP 헤더는 20B이다. 

- 두 헤더 모두 첫 2B가 Source Port Number(SP)이고, 다음 2B가 Destination Port Number(DP)이다. 
- 데이터에 대한 오류를 체크한다.
- TCP헤더의 경우 송수신(연결)을 통해 데이터를 전달하기 때문에 더 많은 정보를 필요로 한다.(뇌피셜..)
- 또한 TCP는 순서를 보장하기 때문에 시퀀스 정보가 필요



#### Reference

- [TCP 와 UDP 차이를 자세히 알아보자](https://velog.io/@hidaehyunlee/TCP-%EC%99%80-UDP-%EC%9D%98-%EC%B0%A8%EC%9D%B4)

- [Ethernet, IP, TCP/UDP 헤더 소개](https://www.netmanias.com/ko/post/blog/5372/ethernet-ip-ip-routing-network-protocol/packet-header-ethernet-ip-tcp-ip)

## #7

#### TCP의 연결 설정 과정(3단계)과 연결 종료 과정(4단계)이 단계가 차이나는 이유가 무엇인가요?

<div align='center'>
     <img src="./images/nt_7_3sh.JPG">
   </div>

<div align='center'>
     <img src="./images/nt_7_4sh.JPG">
   </div>

서버에서 TCP 구현할 때 클라이언트의 SYN 플래그를 승인해야 하기 때문에 두가지 일이 동일한 세그먼트에서 수행될 수 있다.

종료시에도 TCP가 세 개의 세그먼트(FIN, FIN-ACK, ACK)만 사용하여 "4방향" 종료를 수행하는 것도 가능하다.

그러나 일반적으로 4단계로 일어나는 이유는 클라이언트가 FIN을 보냈을때, 응답은 바로 해야하지만, 서버가 언제 종료할 지는 클라이언트 종료가 조건이 아니고 애플리케이션에 의해 결정된다. FIN을 수신하면 애플리케이션에 이를 알리고(예: EOF 사용)  애플리케이션은 자체 바이트 스트림을 종료하게 되는데( 예: shutdown() 또는 close()) 이 결정이 매우 빠르지 않는 한 TCP는 이미 FIN에 대한 ACK을 보냈을 것이다. 따라서 애플리케이션이 종료될 때 TCP는 FIN과 함께 두번째 세그먼트를 보내야 한다. 

근본적으로 TCP 연결과 종료과정은 모두 4방향 교환이나, 이를 4개의 세그먼트를 사용하거나 3개로 압축할 수 있다. 

#### Reference

- [Quora](https://www.quora.com/Why-is-the-TCP-connection-terminated-in-a-4-way-handshake)
- [TCP 연결 종료](http://www.ktword.co.kr/test/view/view.php?no=2436)

## #8

### 만약 Server에서 FIN 플래그를 전송하기 전에 전송한 패킷이 Routing 지연이나 패킷 유실로 인한 재전송 등으로 인해 FIN 패킷보다 늦게 도착하는 상황이 발생하면 어떻게 될까요?

Client에서 세션을 종료시킨 후 뒤늦게 도착하는 패킷이 있다면 이 패킷은 Drop되고 **데이터는 유실**될 것이다.

이러한 현상에 대비하여 Client는 Server로부터 **FIN**을 수신하더라도 일정시간동안 세션을 남겨놓고 잉여 패킷을 기다리는 과정을 거치게 되는데 이 과정을 **TIME_WAIT** 라고 한다. 일정 시간이 지나면, 세션을 만료하고 연결을 종료시킨다.

#### References

- [[네트워크\] 3-way / 4-way Handshake 란? - 방구의 개발냄새](https://bangu4.tistory.com/74)

## #9

### 초기 Sequence Number인 ISN을 0부터 시작하지 않고 난수를 생성해서 설정하는 이유가 무엇인가요?

- SYN : SYnchronize sequence Number
  - TCP 연결의 포트 번호로 이해하면 됩니다!

#### #첫번째 이유

Connection을 맺을 때 사용하는 포트는 유한 범위 내에서 사용하고 시간이 지남에 따라 재사용됩니다.

따라서 두 통신 호스트가 과거에 사용된 포트 번호 쌍을 사용하는 가능성이 존재합니다.

서버 측에서는 패킷의 SYN을 보고 패킷을 구분하게 되는데 난수가 아닌 순차적인 number가 전송된다면 이전의 connection으로부터 오는 패킷으로 인식할 수 있습니다.

이러한 문제가 발생할 가능성을 줄이기 위해서 난수로 ISN을 설정하는 것입니다.

#### #두번째 이유

0에서 시작하는 ISN은 이어지는 Sequence number를 쉽게 예측할 수 있게 되어 보안에 취약하게 됩니다. 이를 방지하기 위해 난수의 ISN을 사용하는 것입니다.

### References

- [[Network] (TCP) 3-way-handshake & 4-way-handshake - 어제보다 한 걸음 더](https://k39335.tistory.com/21)
- [TCP - Connection Establishment/Termination](https://nogan.tistory.com/22)


## #10 

### HTTP와 HTTPS에 대해서 설명하고 차이점에 대해 설명해주세요.

**HTTP(Hyper Text Transfer Protocol)**

> 서버/클라이언트 모델을 따라 데이터를 주고 받기 위한 프로토콜

즉, HTTP는 인터넷에서 하이퍼텍스트를 교환하기 위한 통신 규약으로, 80번 포트를 사용하고 있다. 따라서 HTTP 서버가 80번 포트에서 요청을 기다리고 있으며, 클라이언트는 80번 포트로 요청을 보내게 된다.

HTTP의 구조

- HTTP는 애플리케이션 레벨의 프로토콜로 **TCP/IP 위에서 작동**한다. HTTP는 상태를 가지고 있지 않는 Stateless 프로토콜이며 Method, Path, Version, Headers, Body 등으로 구성된다.

하지만 HTTP는 암호화가 되지 않은 평문 데이터를 전송하는 프로토콜이였기 때문에, HTTP로 비밀번호나 주민등록번호 등을 주고 받으면 제3자가 정보를 조회할 수 있었다. 그리고 이러한 문제를 해결하기 위해 HTTPS가 등장하게 되었다.



**HTTPS(Hyper Text Transfer Protocol Secure)**

> HTTP에 데이터 암호화가 추가된 프로토콜

HTTPS는 HTTP와 다르게 443번 포트를 사용하며, 네트워크 상에서 중간에 제3자가 정보를 볼 수 없도록 공개키 암호화를 지원하고 있다.



**HTTP와 HTTPS**

HTTP는 암호화가 추가되지 않았기 때문에 보안에 취약한 반면, HTTPS는 안전하게 데이터를 주고받을 수 있다. 하지만 HTTPS를 이용하면 암호화/복호화의 과정이 필요하기 때문에 HTTP보다 속도가 느리다.(오늘날에는 거의 차이를 못느낄 정도이다.) 또한 HTTPS는 인증서를 발급하고 유지하기 위한 추가 비용이 발생하다.

***그렇다면 언제 HTTP를 쓰고, 언제 HTTPS를 쓰는 것이 좋겠는가?***

개인 정보와 같은 민감한 데이터를 주고 받아야 한다면 HTTPS를 이용해야 하지만, 단순한 정보 조회 등만을 처리하고 있다면 HTTP를 이용하면 된다.



**Reference**

- [망나니개발자](https://mangkyu.tistory.com/98)

## #11

#### HTTP 요청/응답 헤더의 구조를 설명해주세요.



HTTP 메시지는 서버와 클라이언트 간에 데이터가 교환되는 방식입니다. 메시지 타입은 두 가지가 있습니다. 요청(*request)은* 클라이언트가 서버로 전달해서 서버의 액션이 일어나게끔 하는 메시지고, 응답(*response)은 요청*에 대한 서버의 답변입니다. 두 메시지는 공통 포맷을 가지고 있고 HTTP 헤더와 HTTP 본문을 포함합니다.

**HTTP 요청/응답 메시지**

<div align='center'>
     <img src="./images/network_11.png">
   </div>

- 스타트라인(Start Line): 실행되어야 할 요청, 또은 요청 수행에 대한 성공 또는 실패가 기록되어 있습니다. 이 줄은 항상 한 줄로 끝납니다. 요청 메시지일 때 요청라인(request line)이라고 하고, 응답 메시지일 때 상태라인(status line)이라고 합니다.

- 헤더(Header): 여기에는 요청에 대한 설명, 혹은 메시지 본문에 대한 설명이 들어갑니다. 각 행의 끝에 줄 바꿈 문자인 CRLF(Carriage Return Line Feed)가 있으며, 헤더와 바디는 빈 줄로 구분합니다.
- 빈 줄(blank line): 요청에 대한 모든 메타 정보가 전송되었음을 알리는 줄

- 헤더와 바디(Body): 생략할 수 있고, 바디에는 텍스트뿐만 아니라 바이너리 데이터도 들어갈 수 있습니다. 요청과 관련된 내용(HTML 폼 콘텐츠 등)이 옵션으로 들어가거나, 응답과 관련된 문서(document)가 들어갑니다. 본문의 존재 유무 및 크기는 첫 줄과 HTTP 헤더에 명시
<div align='center'>
     <img src="./images/network_11-2.png">
</div>

Header는 General Header, Request/Response Header, Entity Header

#### **HTTP Requests**

**start line** 

- 첫번째는 HTTP 메서드로, 영어 동사([`GET`](https://developer.mozilla.org/ko/docs/Web/HTTP/Methods/GET), [`PUT`](https://developer.mozilla.org/ko/docs/Web/HTTP/Methods/PUT),[`POST`](https://developer.mozilla.org/ko/docs/Web/HTTP/Methods/POST)) 혹은 명사([`HEAD`](https://developer.mozilla.org/ko/docs/Web/HTTP/Methods/HEAD), [`OPTIONS`](https://developer.mozilla.org/ko/docs/Web/HTTP/Methods/OPTIONS))를 사용해 서버가 수행해야 할 동작을 나타냄

- 두번째로 오는 요청 타겟은 주로 [URL](https://developer.mozilla.org/ko/docs/Glossary/URL), 또는 프로토콜, 포트, 도메인의 절대 경로로 나타낼 수도 있으며 이들은 요청 컨텍스트에 의해 특정지어 집니다. 요청 타겟 포맷은 HTTP 메소드에 따라 달라집니다.
- 마지막으로 HTTP 버전이 들어갑니다.

**Header**

요청 헤더는 요청한 URL, 메소드 (GET, POST, HEAD), 요처

요청에 들어가는 [HTTP 헤더](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers)는 HTTP 헤더의 기본 구조를 따릅니다. 대소문자 구분없는 문자열 다음에 콜론(`':'`)이 붙으며, 그 뒤에 오는 값은 헤더에 따라 달라집니다. 헤더는 값까지 포함해 한 줄로 구성되지만 꽤 길어질 수 있습니다.

다양한 종류의 요청 헤더가 있는데, 이들은 다음과 같이 몇몇 그룹으로 나눌 수 있습니다.


<div align='center'>
     <img src="./images/HTTP_Request_Headers2.png">
   </div>

- General 헤더: 전송되는 HTTP 본문 컨텐츠와 관련없고, HTTP 통신에 대한 일반적인 정보 포함(ex: 날짜, 메세지 전송시 보안 적용 )
- Request 헤더: 요청헤더는 요청한 URL, 메소드(GET, POST, HEAD), 요청 생성에 사용 된 브라우저 및 기타 정보와 같은 요청에 대한 정보 포함
- Entity 헤더: 실제 메시지 또는 전송중인 HTTP 본문에 대한 정보를 포함 (ex: 콘텐츠 길이,  만료날짜 ...) 

**body**

해당 reqeust의 실제 메세지/내용. Body가 없는 request도 많다.

**HTTP Response**

**start line** 

1. *프로토콜 버전:* 보통 `HTTP/1.1`입니다.
2. 상태 코드: 요청의 성공 여부를 나타냅니다. 2xx, 3xx, 4xx
3. 상태 텍스트: 짧고 간결하게 상태 코드에 대한 설명을 글로 나타내어 사람들이 HTTP 메시지를 이해할 때 도움이 됩니다.

**Header**

구성 요소는 request header와 동일

응답 헤더는 사용자가 특정 페이지 또는 리소스에 대한 요청을 보낸 후 서버에서 브라우저에 의해 수신되며 컨텐츠에 사용 된 인코딩, 서버 시스템에서 응답을 생성하는 데 사용되는 서버소프트웨어 및 기타정보를 포함한합니다.


<div align='center'>
     <img src="./images/HTTP_Response_Headers2.png">
   </div>
**body**

- Response의 body와 일반적으로 동일, 모든 response가 body가 있지는 않다. 데이터를 전송할 필요가 없을경우 body가 비어있게 된다.

**한줄 정리**

> 헤더엔 General 헤더, request/response header, entity header 존재 제너럴은 일반적인 정보(날짜) 포함 request/response는 요청/반응에 대한 브라우저 정보, 인코딩 정보 포함, Entity는반응/요청에 따른 본문에 대한 내용(콘텐츠 길이) 포함

#### Reference

- [메시지 구조와 함께 HTTP 프로토콜 이해하기](https://deepwelloper.tistory.com/entry/HTTP-%EB%A9%94%EC%8B%9C%EC%A7%80-%EA%B5%AC%EC%A1%B0%EC%99%80-%ED%95%A8%EA%BB%98-HTTP-%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0)
- [HTTP-구조-및-핵심-요소](https://velog.io/@teddybearjung/HTTP-%EA%B5%AC%EC%A1%B0-%EB%B0%8F-%ED%95%B5%EC%8B%AC-%EC%9A%94%EC%86%8C)
- [HTTP 구조 헤더와 본문](https://blueyikim.tistory.com/1999)

- [HTTP 메시지](



## #13

#### CORS가 무엇인가요?

<div align='center'>
     <img src="./images/nt_13_CORS.JPG">
   </div>

url에서 다른 서비스에 api로 정보를 받아오기 위해 프론트에서 http요청을 보냈을 때, 미리 어떤 설정을 해주지 않으면 CORS에 막힌다.

사실 SOP(Same-Origin Policy)가 동일 출처에서만 api등의 데이터 접근이 가능하도록 막는 거고, CORS(Cross-Origin Resource Sharing)이 다른 출처간에 리소스를 공유할 수 있도록 하는 것이다.

미리 해야하는 어떤 설정이라는 것은 요청을 받는 백엔드쪽에서 이걸 허락한 다른 출처들을 미리 명시해두면 된다. 각 백엔드 프레임워크의 문서에서 CORS 옵션을 넣는 방법을 알 수 있다.

#### Reference

- [ERROR](https://ichi.pro/ko/gandanhan-lokeol-cors-teseuteu-dogu-92698556174789)
- [CORS](youtube.com/watch?v=bW31xiNB8Nc)

## #14

### HTTP GET과 POST 메서드를 비교/설명해주세요.

### GET 

- 클라이언트에서 서버로 어떠한 리소스로 부터 정보를 요청하기 위해 사용되는 method
- 요청을 전송할 때 URL 주소 끝에 파라미터로 포함되어 전송되며, 이 부분을 **쿼리 스트링**이라고 한다. 

```
www.example-url.com/resources?name1=성민&name2=동진
```

위 예는 쿼리 스트링을 포함한 URL이다. 파라미터인 name1과 name2를 통해 값을 전달받고 &로 연결한다.

- GET은 데이터를 읽을때만 사요하고 수정할 때는 사용하지 않는다.



### POST

- 리소스를 생성/업데이트하기 위해 서버에 데이터를 보낼때 사용
- 전송할 데이터를 HTTP 메세지의 Body에 담아서 전송
- HTTP 메세지의 Body는 길이의 제한없이 데이터를 전송할 수 있다. 그래서 `POST` 요청은 `GET`과 달리 대용량 데이터를 전송할 수 있다.



<div align='center'>
     <img src="./images/network14.png">
   </div>

#### References

- [Get과 Post의 차이를 아시나요?](https://velog.io/@songyouhyun/Get%EA%B3%BC-Post%EC%9D%98-%EC%B0%A8%EC%9D%B4%EB%A5%BC-%EC%95%84%EC%8B%9C%EB%82%98%EC%9A%94)


## #15

### 쿠키(Cookie)와 세션(Session)을 설명해주세요.

**쿠키(Cookie)**

쿠키는 **클라이언트(브라우저) 로컬에 저장되는 키와 값이 들어있는 작은 데이터 파일**입니다.

사용자 인증이 유효한 시간을 명시할 수 있으며, 유효 시간이 정해지면 브라우저가 종료되어도 인증이 유지된다는 특징이 있습니다.

쿠키는 클라이언트의 상태 정보를 로컬에 저장했다가 참조합니다.

Response Header에 Set-Cookie 속성을 사용하면 클라이언트에 쿠키를 만들 수 있습니다.

쿠키는 사용자가 따로 요청하지 않아도 브라우저가 Request 시에 Request Header를 넣어서 자동으로 서버에 전송합니다.

- 쿠키의 구성 요소
  - 이름 : 각각의 쿠키를 구별하는 데 사용되는 이름
  - 값 : 쿠키의 이름과 관련된 값
  - 유효시간 : 쿠키의 유지시간
  - 도메인 : 쿠키를 전송할 도메인
  - 경로 : 쿠키를 전송할 요청 경로


- 쿠키의 동작 방식
    1. 클라이언트가 페이지를 요청
    2. 서버에서 쿠키를 생성
    3. HTTP 헤더에 쿠키를 포함 시켜 응답
    4. 브라우저가 종료되어도 쿠키 만료 기간이 있다면 클라이언트에서 보관
    5. 같은 요청을 할 경우 HTTP 헤더에 쿠키를 함께 보냄
    6. 서버에서 쿠키를 읽어 이전 상태 정보를 변경할 필요가 있을 때 쿠키를 업데이트하여 변경된 쿠키를 HTTP 헤더에 포함시켜 응답

- 쿠키의 사용 예
  - 방문 사이트에서 로그인 시, "아이디와 비밀번호를 저장하시겠습니까?"
  - 쇼핑몰의 장바구니 기능
  - 자동로그인, 팝업에서 "오늘 더 이상 이 창을 보지 않음" 체크, 쇼핑몰의 장바구니

**세션(Session)**

세션은 쿠키를 기반하고 있지만, 사용자 정보 파일을 브라우저에 저장하는 쿠키와 달리 세션은 **서버 측에서 관리**합니다.

서버에서는 클라이언트를 구분하기 위해 세션 ID를 부여하며 웹 브라우저가 서버에 접속해서 브라우저를 종료할 때까지 인증 상태를 유지합니다.

접속 시간에 제한을 두어 일정 시간 응답이 없다면 정보가 유지되지 않게 설정이 가능하다.

사용자에 대한 정보를 서버에 두기 때문에 쿠키보다 보안에 좋지만, 사용자가 많아질수록 서버 메모리를 많이 차지하게 된다.

즉 동접자 수가 많은 웹 사이트인 경우 서버에 과부하를 주게 되므로 성능 저하의 요인이 된다.

클라이언트가 Request를 보내면, 해당 서버의 엔진이 클라이언트에게 유일한 ID를 부여하는 데 이것이 세션 ID다.

- 세션의 동작 방식
    1. 클라이언트가 서버에 접속 시 세션 ID를 발급
    2. 클라이언트는 세션 ID에 대해 쿠키를 사용해서 저장하고 가지고 있음
    3. 클라이언트는 서버에 요청할 때, 이 쿠키의 세션 ID를 서버에 전달해서 사용
    4. 서버는 세션 ID를 전달받아서 별다른 작업 없이 세션 ID로 세션에 있는 클라언트 정보를 가져옴
    5. 클라이언트 정보를 가지고 서버 요청을 처리하여 클라이언트에게 응답

- 세션의 사용 예
  - 로그인 같이 보안상 중요한 작업을 수행할 때 사용

- **차이점**
    - 사용자의 정보가 저장되는 위치
        - 쿠키는 서버의 자원을 전혀 사용하지 않으며, 세션은 서버의 자원을 사용한다.
    - 보안
        - 쿠키는 클라이언트 로컬에 저장되기 때문에 변질되거나 request에서 스니핑 당할 우려가 있어서 보안에 취약하다.
        - 세션은 쿠키를 이용해서 세션 ID만 저장하고 그것으로 구분해서 서버에서 처리하기 때문에 비교적 보안성이 좋다.
    - 라이프 사이클
        - 쿠키는 만료시간이 있지만 파일로 저장되기 때문에 브라우저를 종료해도 계속해서 정보가 남아 있을 수 있다. 또한 만료 기간을 넉넉하게 잡아두면 쿠키 삭제를 할 때까지 유지될 수도 있다.
        - 반면에 세션도 만료시간을 정할 수 있지만 브라우저가 종료되면 만료시간에 상관없이 삭제된다.
    - 속도
        - 쿠키에 정보가 있기 때문에 서버에 요청 시 속도가 빠르다.
        - 세션은 정보가 서버에 있기 때문에 처리가 요구되어 비교적 느린 속도를 낸다.

세션은 서버의 자원을 사용하기 때문에 무분별하게 만들다 보면 서버의 메모리가 감당할 수 없어질 수가 있고 속도가 느려질 수 있기 때문에 쿠키를 함께 사용한다.

### References

- [쿠키와 세션 개념 - 라이언 서버](https://interconnection.tistory.com/74)


## #16

### DNS가 무엇인가요?

**DNS(Domain Name System)** 은 사람이 읽을 수 있는 도메인 이름(e.g. www.amazon.com)을 머신이 읽을 수 있는 IP 주소(e.g. 192.0.2.44)로 변환한다.

#### DNS 기본 사항

스마트폰이나 노트북부터 대규모 소매 웹 사이트의 콘텐츠를 서비스하는 서버에 이르기까지 인터넷상의 모든 컴퓨터는 숫자를 사용하여 서로를 찾고 통신합니다. 이러한 숫자를 **IP 주소**라고 합니다. 웹 브라우저를 열고 웹 사이트로 이동할 때는 긴 숫자를 기억해 입력할 필요가 없습니다. 그 대신 example.com과 같은 **도메인 이름**을 입력해도 원하는 웹 사이트로 갈 수 있습니다.

Amazon Route 53과 같은 DNS 서비스는 전 세계에 배포된 서비스로서, www.example.com과 같이 사람이 읽을 수 있는 이름을 192.0.2.1과 같은 숫자 IP 주소로 변환하여 컴퓨터가 서로 통신할 수 있도록 합니다. 인터넷의 DNS 시스템은 이름과 숫자 간의 매핑을 관리하여 마치 전화번호부와 같은 기능을 합니다. DNS 서버는 이름을 IP 주소로 변환하여 도메인 이름을 웹 브라우저에 입력할 때 최종 사용자를 어떤 서버에 연결할 것인지를 제어합니다. 이 요청을 **쿼리**라고 부릅니다.

#### Reference

- [AWS](https://aws.amazon.com/ko/route53/what-is-dns/)

## #17

#### REST와 RESTful의 개념을 설명하고 차이를 말해주세요.

#### REST(REpresentational State Transfer)

자원을 이름(자원의 표현)으로 구분해 해당 자원의 상태(정보)를 주고 받는 모든 것을 의미합니다.

즉, 자원(resource)의 표현(representation)에 의한 상태 전달을 뜻한다.

**REST 구성요소**

- 자원(Resource)-URI: 
  - 해당 소프트웨어가 관리하는 모든 것(문서, 그림, 데이터, 해당 소프트웨어 자체 등).  at server
  - URI라는 고유한 ID 존재
  - Client는 URI를 통해 해당 자원의 상태(정보)에 대한 조작 server에 요청 
- 행위(Verb) - MeTHOD
  - HTTP 프로토콜의 method를 사용
  - HTTP 프로토콜은 GET, POST, PUT, PATCH, DELETE의 Method를 제공합니다.
- 표현 ( Representation of Resource ) 
  - Client와 Server가 데이터를 주고받는 형태로 JSON, XML, TEXT, RSS 등이 있습니다.
  - JSON, XML을 통해 데이터를 주고 받는 것이 일반적입니다.

REST는 기본적으로 웹의 기존 기술과 HTTP 프로토콜을 그대로 활용하기 때문에, 웹의 장점을 최대한 활용할 수 있는 아키텍처 스타일. 즉 REST는 네트워크 상에서 Client와 Server 사이의 통신 방식 중 하나이다.

특징: **Server-Client (서버-클라이언트 구조)**, **Stateless (무상태)**, **Cacheable (캐시 처리 기능)**, **Layered System (계층 구조)**, **Uniform Interface (인터페이스 일관성)**, **Self-Descriptiveness (자체 표현)**

#### REST API

- API(Application Programming Interface)란?
  -  데이터와 기능의 집합을 제공하여 컴퓨터 프로그램간 상호작용을 촉진하며, 서로 정보를 교환가능 하도록 하는 것
- REST API란?
  REST 기반으로 서비스 API를 구현한 것

**REST API 설계 규칙**

- **첫 번째,** URI는 정보의 자원을 표현해야 한다.
- **두 번째,** 자원에 대한 행위는 HTTP Method(GET, POST, PUT, PATCH, DELETE)로 표현한다.
  - 행위(Method)는 URI에 포함하지 않는다.

**추가 규칙**

1. URI는 명사를 사용한다.(리소스명은 동사가 아닌 명사를 사용해야 한다.)
2. 슬래시( / )로 계층 관계를 표현한다. 

3. URI 마지막 문자로 슬래시 ( / )를 포함하지 않는다.

4. 밑줄( _ )을 사용하지 않고, 하이픈( - )을 사용한다.

5. URI는 소문자로만 구성한다.

6. HTTP 응답 상태 코드 사용

- 클라이언트는 해당 요청에 대한 실패, 처리완료 또는 잘못된 요청 등에 대한 피드백을 받아야 한다.

7. 파일확장자는 URI에 포함하지 않는다.

#### RESTful이란?

- RESTful은 일반적으로 REST라는 아키텍처를 구현하는 웹 서비스를 나타내기 위해 사용되는 용어이다.
- ‘REST API’를 제공하는 웹 서비스를 ‘RESTful’하다고 할 수 있다.
- RESTful은 REST를 REST답게 쓰기 위한 방법으로, 누군가가 공식적으로 발표한 것이 아니다.
  즉, REST 원리를 따르는 시스템은 RESTful이란 용어로 지칭된다.(API도제공)

**한줄 정리**

> RESTful은 기존 REST에서 API를 제공하는 웹서비스

#### Reference

- [REST란? REST API 와 RESTful API의 차이점?](https://dev-coco.tistory.com/m/97)
- [[Network] REST란? REST API란? RESTful이란?](https://gmlwjd9405.github.io/2018/09/21/rest-and-restful.html)
- [REST API란? (RESTful,REST)](https://www.lostcatbox.com/2021/01/19/basic-api/)



## #19

#### Socket.io와 WebSocket의 차이를 설명해주세요.

**WebSocket**

- HTML5 웹 표준 기술
- 매우 빠르게 작동하며 통신할 때 아주 적은 데이터를 이용함
- 이벤트를 단순히 듣고, 보내는 것만 가능함

**Socket.io**

- 표준 기술이 아니며, 라이브러리임
- 소켓 연결 실패 시 fallback을 통해 다른 방식으로 알아서 해당 클라이언트와 연결을 시도함
- 방 개념을 이용해 일부 클라이언트에게만 데이터를 전송하는 브로드캐스팅이 가능함



서버에서 연결된 소켓(사용자)들을 세밀하게 관리해야하는 서비스인 경우에는 Broadcasting 기능이 있는 socket.io을 쓰는게 유지보수 측면에서 훨씬 이점이 많다.

반면 가상화폐 거래소같이 데이터 전송이 많은 경우에는 빠르고 비용이 적은 표준 WebSocket을 이용하는게 바람직하다. 실제로 업비트나 바이낸스 소켓 API를 사용해보면 정말 엄청나게 많은 데이터가 들어온다.

#### Reference

- [웹소켓과 socket.io](https://www.peterkimzz.com/websocket-vs-socket-io/)
