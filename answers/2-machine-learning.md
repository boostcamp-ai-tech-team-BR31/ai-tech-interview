<div align='center'>
  <h1>🏃‍♀️ Machine Learning 🏃‍♂️</h1>

</div>

> 질문은 <strong>[zzsza님의 Datascience-Interview-Questions](https://github.com/zzsza/Datascience-Interview-Questions)</strong>를 참고하였습니다.

---

## Table of Contents

- [알고 있는 metric에 대해 설명해주세요. (ex. RMSE, MAE, recall, precision ...)](#1)
- [정규화를 왜 해야할까요? 정규화의 방법은 무엇이 있나요?](#2)
- [Local Minima와 Global Minima에 대해 설명해주세요.](#3)
- [차원의 저주에 대해 설명해주세요.](#4)
- [dimension reduction 기법으로 보통 어떤 것들이 있나요?](#5)
- [PCA는 차원 축소 기법이면서, 데이터 압축 기법이기도 하고, 노이즈 제거기법이기도 합니다. 왜 그런지 설명해주실 수 있나요?](#6)
- [LSA, LDA, SVD 등의 약자들이 어떤 뜻이고 서로 어떤 관계를 가지는지 설명할 수 있나요?](#7)
- [Markov Chain을 고등학생에게 설명하려면 어떤 방식이 제일 좋을까요?](#8)
- [텍스트 더미에서 주제를 추출해야 합니다. 어떤 방식으로 접근해 나가시겠나요?](#9)
- [SVM은 왜 반대로 차원을 확장시키는 방식으로 동작할까요? SVM은 왜 좋을까요?](#10)
- [다른 좋은 머신 러닝 대비, 오래된 기법인 나이브 베이즈(naive bayes)의 장점을 옹호해보세요.](#11)
- [회귀 / 분류시 알맞은 metric은 무엇일까?](#12)
- [Association Rule의 Support, Confidence, Lift에 대해 설명해주세요.](#13)
- [최적화 기법중 Newton’s Method와 Gradient Descent 방법에 대해 알고 있나요?](#14)
- [머신러닝(machine)적 접근방법과 통계(statistics)적 접근방법의 둘간에 차이에 대한 견해가 있나요?](#15)
- [인공신경망(deep learning이전의 전통적인)이 가지는 일반적인 문제점은 무엇일까요?](#16)
- [지금 나오고 있는 deep learning 계열의 혁신의 근간은 무엇이라고 생각하시나요?](#17)
- [ROC 커브에 대해 설명해주실 수 있으신가요?](#18)
- [여러분이 서버를 100대 가지고 있습니다. 이때 인공신경망보다 Random Forest를 써야하는 이유는 뭘까요?](#19)
- [K-means의 대표적 의미론적 단점은 무엇인가요? (계산량 많다는것 말고)](#20)
- [L1, L2 정규화에 대해 설명해주세요.](#21)
- [Cross Validation은 무엇이고 어떻게 해야하나요?](#22)
- [XGBoost을 아시나요? 왜 이 모델이 캐글에서 유명할까요?](#23)
- [앙상블 방법엔 어떤 것들이 있나요?](#24)
- [feature vector란 무엇일까요?](#25)
- [좋은 모델의 정의는 무엇일까요?](#26)
- [50개의 작은 의사결정 나무는 큰 의사결정 나무보다 괜찮을까요? 왜 그렇게 생각하나요?](#27)
- [스팸 필터에 로지스틱 리그레션을 많이 사용하는 이유는 무엇일까요?](#28)
- [OLS(ordinary least squre) regression의 공식은 무엇인가요?](#29)

---

## #1

### 알고 있는 metric에 대해 설명해주세요. (ex. RMSE, MAE, recall, precision ...)

week4 민규님

## #2

### 정규화를 왜 해야할까요? 정규화의 방법은 무엇이 있나요?

normalization, regularization, standardization. 세 용어가 모두 정규화로 번역됩니다. 여기서는 normalization을 집고 넘고 넘어가겠습니다.

#### Normalization

ML 알고리즘의 목적 중 하나는 feature들을 비교하여 데이터의 패턴을 찾는 것입니다. 하지만 feature의 scale이 심하게 차이나는 경우 문제가 발생합니다. 그래서 **모든 데이터가 동일한 정도의 sclae(중요도)로 반영되도록 해주는 게 normalization의 목표**입니다.

1. **Min - Max normalization**

   <div align='center'>
     <img src="https://render.githubusercontent.com/render/math?math=\frac{x - min}{max-min}">
   </div>

   - 최소값과 최대값을 이용해 값의 범위를 0~1 사이 값으로 바꿉니다.
   - 하지만 outlier(이상치)에 너무 많은 영향을 받습니다.

2. **Z-score normalization**

   <div align='center'>
     <img src="https://render.githubusercontent.com/render/math?math=\frac{x - m}{\sigma}">
   </div>

   - standartdization을 활용해 outlier 문제를 어느정도 해결합니다.
   - 하지만 동일한 척도로 정규화된 데이터를 생성하지 않는다는 문제가 있습니다.

##### References

- [정규화 : normalization, standardization, regularization](https://realblack0.github.io/2020/03/29/normalization-standardization-regularization.html)
- [normalization 쉽게 이해하기](https://hleecaster.com/ml-normalization-concept/)

## #3

### Local Minima와 Global Minima에 대해 설명해주세요.

오차를 줄이기 위해 경사하강법을 이용하는데, 이는 오차를 계산하는 함수의 최소값을 찾기 위함이다. 이 때 경사하강법은 초기화된 위치에서부터 기울기를 구해 더 아래로 아래로 내려가려 한다.

<img src="images/ml_3.PNG" width="30%" height="30%">

<img src="images/ml_3_g.PNG" width="30%" >

이구간에서 최소값을 찾기위해 아래로 내려간다면 global minima에 도달하겠지만

<img src="images/ml_3_m.PNG" width="30%">

이부분에서 내려간다면 localminimum에 빠져 gradient가 0이 되어도, 오차를 최대로 줄일 수 없다.

##### References

- [Wikipedia](https://en.wikipedia.org/wiki/Maxima_and_minima)

## #4

### 차원의 저주에 대해 설명해주세요.

**차원의 저주(Curse of dimensionality)** 란, 데이터 학습을 위해 차원이 증가하면서 고차원 데이터 공간에서 데이터 표본이 희박해지는 것을 의미한다. 즉, 차원이 증가함에 따라(=변수의 수 증가) 모델의 성능이 안좋아지는 현상을 의미한다.

무조건 변수의 수가 증가한다고 해서 차원의 저주 문제가 있는 것이 아니라, 관측치 수보다 변수의 수가 많아지면 발생한다.

<img src="./images/ml_4_1.png" width="60%">

예를 들어 아래의 그래프을 봤을 때 **8** 을 표현하기 위해서는 1차원에서는 (8), 2차원에서는 (8,0), 3차원에서는 (8,0,0) 으로 표현해야한다.

<img src="./images/ml_4_2.png" width="60%">

따라서 차원이 커질수록, 설명 공간이 지수적으로 늘어나게 된다. 이는 Feature가 많아질수록 동일한 데이터를 설명하는 빈공간이 늘어난다는 것을 의미하며 이는 차원의 저주로 인해 알고리즘 모델링 과정에서 저장 공간과 처리 시간이 불필요하게 증가됨에 따라 결국 성능이 저하되는 것을 의미한다.

##### References

- [차원의 저주(Curse of dimensionality)](https://bioinformaticsandme.tistory.com/197)
- [[빅데이터] 차원의 저주](https://datapedia.tistory.com/15)
- [빅데이터: 큰 용량의 역습 – 차원의 저주 (Curse of dimensionality)](https://thesciencelife.com/archives/1001)

## #5

### dimension reduction기법으로 보통 어떤 것들이 있나요?

week4 민규님

## #6

### PCA는 차원 축소 기법이면서, 데이터 압축 기법이기도 하고, 노이즈 제거기법이기도 합니다. 왜 그런지 설명해주실 수 있나요?

PCA(Pricipal Component Analysis: 주성분 분석)는 고차원의 데이터를, 데이터들의 분산을 잘 유지하는 주성분(데이터들의 선형결합으로 이뤄짐)들을 구하고, 이 주성분을 이용해 저차원으로 데이터들을 표현하는 방법이다. 여기서 주성분들은 서로 직교한다.

주성분 분석은 기존의 고차원 데이터들을, 더 적은 차원의 주성분으로 데이터를 표현하므로 차원 축소 기법이라 할 수 있다. 주성분을 구할 때 데이터의 기존의 분산을 전체 다 이용하는 것이 아닌 분산을 설명하는 정도가 큰 몇개의 주성분만을 이용하므로 데이터를 압축한다고 할 수 있고, 이 과정에서 어느정도의 분산이 제거되므로 노이즈가 감소할 수 있다.

##### References

- [공돌이의 수학 노트 PCA](https://angeloyeo.github.io/2019/07/27/PCA.html)
- [주성분분석(PCA)의 이해와 활용-다크 프로그래머 블로그](https://darkpgmr.tistory.com/110)
- [PCA Eliminate noise in the data - stackExchange](https://stats.stackexchange.com/questions/247260/principal-component-analysis-eliminate-noise-in-the-data/247271)

## #7

### LSA, LDA, SVD 등의 약자들이 어떤 뜻이고 서로 어떤 관계를 가지는지 설명할 수 있나요?

week4 재욱님

## #10

### SVM은 왜 반대로 차원을 확장시키는 방식으로 동작할까요? SVM은 왜 좋을까요?

SVM(Support Vector Machine)은 데이터를 사상된 공간으로 표현하여, 이 공간에서 데이터간 가장 큰 폭을 갖는 경계(초평면: Hyperplane)를 찾는 알고리즘입니다. 분류와 회귀에 둘 다 적용 가능합니다.

기존의 데이터 차원에서는 적절한 데이터 간의 경계를 구할 수 없기 때문에 kernel trick을 이용해 고차원의 특징 공간으로 사상하여 데이터간 가장 먼 거리를 갖는 초평면(Hyperplane)을 찾습니다.

![img](https://t1.daumcdn.net/cfile/tistory/246E9C3A5852B48931)

왼쪽 문제의 경우 선으로 분리 될 수 없기에 가운데의 mapping 함수를 이용해 고차원의 특징공간으로 사상하여 선형으로 분리 될 수있는 초평면을 구합니다. 여기서 주목할 점은 사실 고차원의 공간으로 직접 이동하는것은 많은 연산을 요구하기에 이 점이 실제로 이동하기 보다는 kernel trick을 이용해 문제를 단순화하여 문제를 해결한다.

SVM은 고차원 데이터에서 잘 작동한다는 장점이 있지만 데이터 수가 많아지면 연산이 느려지고 Cross-Validation을 통해 kernel 함수를 정해야 한다는 단점이 있습니다.

#### Reference

- [statquest Youtube SVM](https://www.youtube.com/watch?v=efR1C6CvhmE&t=1028s)
- [커널과 커널트릭](https://sanghyu.tistory.com/14)
- [SVM 설명 블로그](https://excelsior-cjh.tistory.com/66)
- [SVM 장단점](https://www.analyticsvidhya.com/blog/2017/09/understaing-support-vector-machine-example-code/)

## #16

### 인공신경망(deep learning 이전의 전통적인)이 가지는 일반적인 문제점은 무엇일까요?

기존 단일 신경망(single layer perceptron)의 경우 xor과 같은 비선형 문제를 해결하지 못하는 문제점이 있었다. 그러나 비선형 활성화 함수와 Multi Layer Perceptron을 통해 xor 문제를 해결 할 수 있게 됬고 MLP를 학습시킬 수 있는 Backpropagation의 등장과 컴퓨팅 파워로 인해 지금의 deeplearning이 가능해졌다.

#### Reference

- [Solving XOR Problem with MLP](https://ynebula.tistory.com/22)

- [Multi Layer Perceptron 설명](http://users.ics.aalto.fi/harri/thesis/valpola_thesis/node43.html)

  