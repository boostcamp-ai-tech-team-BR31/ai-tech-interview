# 라이엇게임즈 CTO 특강

## Unit Test

unit test를 하지 않으면 사소한 버그가 쌓여서 걷잡을 수 없는 버그에 봉착한다.

디버깅을 잘 하는 게 개발을 잘 하는 것인가? 

ㄴㄴ 제일 중요한 것은 내가 오류를 만들었을 때, 오류가 바로 눈에 보이는 것. 이것이 바로 TTD Unit Test.

Regression: 하나의 버그를 고쳤는데, 다른 곳에서 여러 오류가 더 발생하는 것.

unit test : method 하나하나 테스트 함. 내가 작성한 부분에서 다른 dependency를 다 끊어내고 테스트.

- Manual Testting
  - 변화가 생길때 마다 다른곳이 깨짐. 사람이 손으로 하는 것. 반복하기 어려움. 시간낭비.
- Automated testing
  - 위의 방법과 비슷하지만 자동
- Test-first development
  - 
- Test-driven development (이것부터하면 장점 많음)
  - 테스트를 먼저 작성함
  - 디자인을 같이 함.



test fixture

- test에 도움이 되는 준비를 하는 과정

test case

- 실제 테스트

test suite

- 테스트를 별개의 묶음으로 묶음, 목적에 따라?

test runner

- 자동화된 테스트 돌려주는 것