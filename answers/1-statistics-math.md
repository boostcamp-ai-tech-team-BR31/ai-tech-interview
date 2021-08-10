<div align='center'>
  <h1>📈 Statistics/Math 📈</h1>
</div>

> 질문은 <strong>[zzsza님의 Datascience-Interview-Questions](https://github.com/zzsza/Datascience-Interview-Questions)</strong>를 참고하였습니다.

## Table of Contents

- [xxx는 왜 yyy 일까요?](#1)
- [샘플링(Sampling)과 리샘플링(Resampling)에 대해 설명해주세요. 리샘플링은 무슨 장점이 있을까요?](#2)



## #4

### 확률 모형이란?

확률 분포를 보다 단순하게 묘사하기 위해 고안한 것이 **확률 모형(probability model)**이다.

확률 모형은 **분포 함수(distribution function)** 또는 **밀도 함수(density function)**라고 불리우는 미리 정해진 함수의 수식을 사용하여 분포의 모양을 정의(define)하는 방법이다. 이 때 분포의 모양을 결정하는 함수의 계수를 분포의 **모수(parameter)**라고 부른다.

예를 들어 가장 널리 쓰이는 정규 분포(Normal distribution)는 다음과 같은 수식으로 정의된다. 이 수식 자체의 이름은 $N$이고 함수의 독립 변수는 자료의 값을 의미하는 변수 $x$이다. 식에서 사용된 문자 $\mu$와 $\sigma$는 평균(mean)과 표준편차(standard deviation)이라는 이름의 모수이다.

$$ N(x; \mu, \sigma) = \frac{1}{\sigma\sqrt{2\pi}}\, e^{-\frac{(x - \mu)^2}{2 \sigma^2}} $$



### 확률 변수란?

어떤 자료의 값이 분포가 특정한 확률 모형과 일치하는 경우 그 자료를 **확률 변수(random variable)**라고 하고 해당 확률 모형을 따른다고 말한다.

확률 변수는 보통 $X$, $Y$와 같이 알파벳 대문자로 표시하며 확률 변수 $X$가 정규 분포를 따른 경우 수학적으로 다음과 같이 표기한다.

$$ X \sim N(\mu, \sigma) $$

중요한 점은 확률 모형은 사람에 의해 정의된 분포일 뿐이라는 점이다. 어떤 자료의 확률 분포가 특정한 확률 모형을 따르리라는 것은 어디까지나 여러가지 편의를 위해 그렇게 가정(assumption)한 것인 뿐인 경우가 많다.









