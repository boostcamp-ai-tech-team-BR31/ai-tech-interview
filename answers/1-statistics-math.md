<div align='center'>
  <h1>📈 Statistics/Math 📈</h1>
</div>

> 질문은 <strong>[zzsza님의 Datascience-Interview-Questions](https://github.com/zzsza/Datascience-Interview-Questions)</strong>를 참고하였습니다.

## Table of Contents

- [xxx는 왜 yyy 일까요?](#1)
- [샘플링(Sampling)과 리샘플링(Resampling)에 대해 설명해주세요. 리샘플링은 무슨 장점이 있을까요?](#2)



## #1

#### 고유값 (eigen value) 와 고유벡터 (eigen vector)에 대해 설명해주세요. 그리고 왜 중요할까요?

선형대수학에서, 선형 변환의 고유 벡터는 그 선형 변환이 일어난 후에도 방향이 변하지 않는, 영벡터가 아닌 벡터입니다. 

고유 벡터의 길이가 변하는 배수를 그 고유 벡터에 대응하는 고유값이라고 합니다.
$$
A\vec{x} = \lambda\vec{x}
$$
어떤 정방행렬 <!-- $$ A$$--> 는 임의의 <!-- $$ \vec{x}$$--> 에 곱해져서 <!-- $$ \vec{x}$$--> 의 위치나 방향을 변환시키는 역할을 합니다. 이 때, 어떤 특정 벡터들은 <!-- $$ A$$--> 에 곱해져도 자신과 평행한 방향을 갖는데, 이러한 벡터들을 고유벡터라고 합니다. 변환 전후의 크기 차이는 특정 상수를 곱한 정도로 존재하는데, 이 특정 상수가 고유값입니다.

