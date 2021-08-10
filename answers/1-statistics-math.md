<div align='center'>
  <h1>📈 Statistics/Math 📈</h1>
</div>

> 질문은 <strong>[zzsza님의 Datascience-Interview-Questions](https://github.com/zzsza/Datascience-Interview-Questions)</strong>를 참고하였습니다.

## Table of Contents

- [xxx는 왜 yyy 일까요?](#1)
- [샘플링(Sampling)과 리샘플링(Resampling)에 대해 설명해주세요. 리샘플링은 무슨 장점이 있을까요?](#2)
- [누적 분포 함수와 확률 밀도 함수는 무엇일까요? 수식과 함께 표현해주세요!](#3)



## #1

#### xxx는 왜 yyy 일까요?

Hello World

## #2

#### 샘플링(Sampling)과 리샘플링(Resampling)에 대해 설명해주세요. 리샘플링은 무슨 장점이 있을까요?

## #3

#### 누적 분포 함수와 확률 밀도 함수는 무엇일까요? 수식과 함께 표현해주세요!

누적 분포 함수(cumulative distribution function, cdf)를 알기 위해서는 먼저 확률 밀도 함수(probability density function, pdf)를 집고 넘어가야 합니다.

확률 밀도 함수  <!--$ f(x) $--> 와 구간 $$[a, b]$$​에 대해서 확률 변수 $$X$$​가 구간에 포함될 확률 $$P(a\leq X \leq B)$$​는 아래의 수식으로 정의합니다.
$$
P(a \leq X \leq b) = \int_{a}^{b}{f(x)dx}
$$

확률 밀도 함수는 확률변수 $X$가 **연속 확률 변수** 라는 점에서 확률 질량 함수와 큰 차이점을 갖습니다.

확률 질량 함수의 확률 변수는 이산 확률 변수로 이산 확률 변수 $X$에 대하여 $X=x$일 사건이 일어날 확률 $P(X=x)$​​​에 대응하는 함수로 정의합니다. 확률을 가능성의 크기로 생각하는 질량으로 간주하면, 그 확률(질량)을 나타내기 때문에 확률 질량 함수라고 부릅니다.

하지만 확률 밀도 함수의 확률변수 $X$는 연속 확률 변수이기 때문에 구간이 정의되어야 확률을 의미할 수 있습니다. 그래서 확률 $f(x)dx$를 구간 $[a, b]$에서 연속적으로 더해줍니다. 따라서 확률 밀도 함수 $f(x)$​는 그 자체로 확률을 의미하지 않고, 특정 구간에 대한 정의가 필요합니다.

통계학에서 확률 밀도 함수를 $f(x) = \dfrac{확률(질량)}{구간길이(부피)} = \dfrac{f(x)dx}{dx}$​​로 파악하고​​​​​​​​, 이는 물리학에서 밀도의 개념과 비슷하기에 확률 밀도 함수라고 부릅니다.

누적 분포 함수는 말 그대로 확률 밀도 함수를 특정 값 a까지 누적한 함수입니다. 누적 분포 함수 $F(a)$​는 아래와 같이 정의합니다.
$$
F(a) = P(X\le a) = \int_{-\infty}^{a}{f(x)dx}
$$
확률 밀도 함수와 누적 분포 함수는 서로 미분과 적분의 관계를 갖습니다. 

##### References

- [확률 밀도 함수의 정의 in 위키백과](https://ko.wikipedia.org/wiki/%ED%99%95%EB%A5%A0_%EB%B0%80%EB%8F%84_%ED%95%A8%EC%88%98)

- [확률 분포 함수와 확률 밀도 함수의 의미](https://velog.io/@groovallstar/%ED%99%95%EB%A5%A0-%EB%B6%84%ED%8F%AC-%ED%95%A8%EC%88%98%EC%99%80-%ED%99%95%EB%A5%A0-%EB%B0%80%EB%8F%84-%ED%95%A8%EC%88%98%EC%9D%98-%EC%9D%98%EB%AF%B8)

