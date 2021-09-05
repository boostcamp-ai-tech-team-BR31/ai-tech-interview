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

#### Classification Metrics

1. Accuracy

   분류기의 성능을 측정할 때 가장 간단히 사용할 수 있다. (예측결과가 동일한 데이터 수)/(전체 예측 데이터 수)로 계산한다. 라벨 불균형이 있는 데이터에서는 accurcy를 사용하는 것은 바람직하지 않다.

2. Logloss

   분류 모델 평가시 사용한다. 확률 값을 음의 log함수에 넣어 변환을 시킨 값으로 평가하는데, 이는 잘못 예측할 수록, 패널티를 부여하기 위함이다. 모델 전체의 Logloss를 구하려면 확률 값을 음의 로그를 취해 모두 더하고 1/n해서 평균을 내면된다.

3. Confusion Matrix

   <img src="images/ml_1_1.PNG" width="50%">

   confusion matrixs는 모델이 예측을 하면서 얼마나 헷갈리고 있는지를 보여주는 지표이다. 주로 이진 분류에서 많이 사용하며 이진 분류에 대한 오차 행렬은 위의 그림처럼 같이 나타낼 수 있다. True Positive는 긍정으로 예측을 했는데 실제로 긍정인 경우를, False Negative는 긍정으로 예측했는데 실제로 부정인 경우를, False Negative는 부정으로 예측했는데 실제로 긍정인 경우를, True Negative는 부정으로 예측했는데 실제로 부정인 경우를 말한다. 위의 값을 바탕으로 모델이 어떤 오류를 발생시켰는지를 살펴볼 수 있다.

4. precision, recall

   precisionrhk recall은 긍정 데이터 예측 성능에 초점을 맞춘 평가지표이다. precision은 예측을 긍정으로 한 데이터 중 실제로 긍정인 비율을 말하며, recall은 실제로 긍정인 데이터 중 긍정으로 예측한 비율을 말한다. 오차 행렬을 기준으로 precission =  TP / (FP + TP), recall = TP / (FN + TP)으로 계산할 수 있다.

   precision과 recall은 trade-off 관계를 갖는다. 정밀도는 FP를, 재현율은 FN을 낮춤으로써 긍정 예측의 성능을 높인다. 이 같은 특성 때문에 정밀도가 높아지면 재현율은 낮아지고 재현율이 높아지면 정밀도는 낮아진다. 가장 좋은 경우는 두 지표 다 적절히 높은 경우이다.

5. F1-score

   정밀도와 재현율 한 쪽에 치우치지 않고 둘 다 균형을 이루는 것을 나타낸 것이 **F1-Score**이다. F1-Score는 정밀도와 재현율의 조화평균으로 계산할 수 있다.

6. Area Under Curve(AUC, ROC)

   <img src="images/ml_1_2.PNG" width="45%">

   ROC는 FPR(False Positive Rate)가 변할 때 TPR(True Positive Rate)가 어떻게 변하는지를 나타내는 곡선을 말한다. 여기서 FPR이란 FP / (FP + TN)이고, TPR은 TP / (FN + TP)으로 재현율을 말한다. 그럼 어떻게 FPR을 움직일까? 바로 분류 결정 임계값을 변경함으로써 움직일 수 있다. FPR이 0이 되려면 임계값을 1로 설정하면 된다. 그럼 긍정의 기준이 높으니 모두 부정으로 예측될 것이다. 반대로 1이 되려면 임계값을 0으로 설정하여 모두 긍정으로 예측시키면 된다. 이렇게 임계값을 움직이면서 나오는 FPR과 TPR을 각각 x와 y 좌표로 두고 그린 곡선이 ROC이다.

   AUC는 ROC 곡선의 넓이를 말한다. AUC가 높을수록 즉, AUC가 왼쪽 위로 휘어질수록 좋은 성능이 나온다고 판단한다. 즉, TPR이 높고 FPR이 낮을수록 예측 오류는 낮아지기 때문에 성능이 잘 나온다 볼 수 있다.

#### Regression Metrics

1. MSE

   예측값과 정답값 사이의 차이의 제곱의 평균으로 정의한다. 제곱을 했기 때문에 특이치(아웃라이어)에 민감하다.

   <img src="images/ml_1_3.PNG" width="25%">

2. RMSE

   MSE에 루트를 씌운 값을 말한다. 오류 지표를 실제 값과 유사한 단위로 다시 변환하기에 해석이 다소 용이해진다.

   <img src="images/ml_1_5.PNG" width="25%">

3. R-squared

   분산을 기반으로 예측 성능을 평가하는 지표를 말한다. 정답값의 분산 대비 예측값의 분산 비율을 지표로 하며, 1에 가까울수록 정확도가 높다.

4. MAE

    예측값과 정답값 사이의 차이의 절대값의 평균을 말한다.
    
    <img src="images/ml_1_4.PNG" width="25%">

##### References

- [Metric 종류](https://wooono.tistory.com/99)
- [Log loss란?](https://seoyoungh.github.io/machine-learning/ml-logloss/)
- [ROC curve와 AUC이해하기](https://dsdoris.medium.com/roc-curve%EC%99%80-auc-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0-126978d80a9e)
- [Regression - 모델 평가 : MSE, MAE, RMSE, RMSLE, R-Squared](https://steadiness-193.tistory.com/277)

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

차원 축소는 매우 많은 feature로 구성된 다차원 dataset의 차원을 축소해 새로운 차원의 dataset을 생성하는 것이다. 일반적으로 차원이 증가할수록 데이터 포인트 간의 거리가 기하급수적으로 멀어지게 되고, 희소(sparse)한 구조를 가지게 된다. 즉, 데이터가 넓게 분포되어 있어 지역적으로 밀도가 적게 분포되어 있는 구조를 말한다. 

차원 축소는 피처 선택(feature selection)과 피처 추출(feature extraction)으로 나눌 수 있다. 피처 선택이란 특정 feature에 종속성이 강한 불필요한 feature는 아예 제거하고, 데이터의 특성을 잘 나타내는 주요 feature만 선택하는 것이다. 피처 추출은 기존 feature를 저차원의 중요 feature로 압축해서 추출하는 것이다. 이렇게 새로 추출된 중요 특성은 기존 feature와는 완전히 다른 값이 된다.

 PCA, SVD, NMF는 잠재적인 요소를 찾는 대표적인 차원 축소 알고리즘이다. 매우 많은 의미를 가지는 이미지나 텍스트에서 차원 축소를 통해 잠재적인 의미를 찾아 주는 데 이러한 알고리즘들이 잘 활용되고 있다.



##### References

- [머신러닝 스터디 - 차원축소](https://blog.mathpresso.com/mathpresso-%EB%A8%B8%EC%8B%A0-%EB%9F%AC%EB%8B%9D-%EC%8A%A4%ED%84%B0%EB%94%94-15-%EC%B0%A8%EC%9B%90-%EC%B6%95%EC%86%8C-dimensionality-reduction-76b13460506f)
- [차원 축소 개요](https://velog.io/@sset2323/06-01.-%EC%B0%A8%EC%9B%90-%EC%B6%95%EC%86%8CDimension-Reduction-%EA%B0%9C%EC%9A%94)

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

## #8

#### Markov Chain을 고등학생에게 설명하려면 어떤 방식이 제일 좋을까요?

마르코프 체인이란 각 사건의 확률이 이전 사건에서 얻은 상태에 따라서만 달라지는 일련의 가능한 사건들을 설명하는 확률적 모델이다. 고등학생에게 설명하기 위해 쉽게 표현하자면, 오늘의 날씨가 맑을 때, 내일의 날씨가 맑을지 비가 내릴지를 확률적으로 표현하는 것이다. 

<img src="images/Markovkate_01.svg" width="30%">

위 그림을 풀어서 말하면 아래와 같다.

E가 연속적으로 발생할 확률 : 0.3

E다음에 A가 발생할 확률 : 0.7

A다음에 E가 발생할 확률 : 0.4

A가 연속적으로 발생할 확률 : 0.6

**간단한 날씨 예측 모델을 마르코프 체인으로 구현한다고 가정해보자**

| 오늘/내일 | 맑음 |  비  |
| :-------: | :--: | :--: |
|   맑음    | 0.7  | 0.3  |
|    비     | 0.5  | 0.5  |

*오늘 맑고 내일 맑고 모레 비가올 확률은?*

0.7 (오늘 맑고 내일 맑을 확률) * 0.3(맑은 다음 비올 확률) = 0.21

##### References

- https://en.wikipedia.org/wiki/Markov_chain
- https://www.puzzledata.com/blog190423/

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

## #11

### 다른 좋은 머신 러닝 대비, 오래된 기법인 나이브 베이즈(naive bayes)의 장점을 옹호해보세요.

> 기하학에 피타고라스 정리가 있다면 확률론에는 베이즈 정리가 있다
>
> -해럴드 제프리스 경

제프리스 경이 말한 것처럼 베이즈 정리는 AI와 통계학에 엄청난 영향을 끼친 이론입니다.
- Naive : 예측한 특징이 상호 독립적이라는 가정 하에 확률 계산을 단순화. naive의 순진하다라는 의미를 모든 변수들이 동등하다는 것으로 사용하고 있습니다.
- Bayes : 추론 대상의 사전 확률과 추가적인 정보를 기반으로 사후확률을 추론하는 방법입니다. Statistics/Math 카테고리의
[Bayesian Estimation](.\1-statistics-math.md\#14)에서 좀 더 자세히 알 수 있습니다.
나이브 베이지안에 대한 더 자세한 예시와 적용은 3번째 reference를 참고하면 됩니다.
> 나이브 베이지안 장점
>> 간단하고 빠르고 효율적인 알고리즘
>> 
>> 잡음과 누락 데이터를 잘 처리
>> 
>> 데이터 크기에 상관 없음
>> 
>> 예측을 위한 추정 확률을 쉽게 얻음

> 나이브 베이지안 단점
>> 모든 데이터가 독립이라는 가정이 전제 되어야 함
>> 
>> nummeric feature이 많은 dataset에는 이상적이지 않음
>> 
>> 추정된 확률이 예측된 클래스보다 덜 신뢰

이러한 나이브 베이지안의 단점을 보완하기 위해 Laplace Smoothing, Underflow 등 보정 방법을 활용하곤 한다.
##### References

- [나이브 베이즈 분류](https://needjarvis.tistory.com/621)
- [베이즈 추정](https://bkshin.tistory.com/entry/dd?category=1042793)
- [딥 러닝을 이용한 자연어 처리 입문 : 나이브 베이즈 분류기](https://wikidocs.net/22892)


## #16

### 인공신경망(deep learning 이전의 전통적인)이 가지는 일반적인 문제점은 무엇일까요?

기존 단일 신경망(single layer perceptron)의 경우 xor과 같은 비선형 문제를 해결하지 못하는 문제점이 있었다. 그러나 비선형 활성화 함수와 Multi Layer Perceptron을 통해 xor 문제를 해결 할 수 있게 됬고 MLP를 학습시킬 수 있는 Backpropagation의 등장과 컴퓨팅 파워로 인해 지금의 deeplearning이 가능해졌다.

#### Reference

- [Solving XOR Problem with MLP](https://ynebula.tistory.com/22)

- [Multi Layer Perceptron 설명](http://users.ics.aalto.fi/harri/thesis/valpola_thesis/node43.html)

## #18

#### ROC 커브에 대해 설명해주실 수 있으신가요?

ROC 커브(Receiver operating characteristic)란 **이진 분류기의 성능을 표현하는 방법**이다. 설명하기 앞서 TPR과 FPR의 개념에 대해 이해해야 한다. TPR은 True Positive Rate, FPR은 False Positive Rate을 의미한다. 쉽게 말하자면, 의사가 환자가 암에 걸렸는지 아닌지를 판별하는 상황을 이진분류라고 가정했을 때, 실제로 암에 걸린 환자를 암에 걸렸다고 진단하는 것이 True Postiive, 암에 걸리지 않은 환자를 암에 걸렸다고 오진하는 것이 False Postive이다. Postive는 암에 걸린 상태, 이것을 잘 예측하면 앞에 True가 붙는 것이다.

<img src="images/jaeuk_roc_curve.png" width="50%">

ROC Curve 를 나타낸 그래프이다. 위 그래프에서 그래프가 좌측 상단쪽으로 쏠려있을 수록 좋은 True Positive가 1에 수렴하므로 Classifier임을 의미한다.

gif로 보면 이해가 빠르니 아래 2번째 링크에서 확인하면 좋을 것 같다. (저작권 문제로 gif를 가져오지 못함)

##### References

- https://youtu.be/n7EoYT5kDO4
- https://angeloyeo.github.io/2020/08/05/ROC.html
- https://en.wikipedia.org/wiki/Receiver_operating_characteristic

## #19

### 여러분이 서버를 100대 가지고 있습니다. 이때 인공신경망보다 Random Forest를 써야하는 이유는 뭘까요?
   <div align='center'>
     <img src="images\ml_19_randomForest.png">
   </div>
Random Forest는 수많은 의사결정 트리(Decision Tree)로 만들어진 모델입니다. 새로운 데이터 포인트를 각 트리에 동시에 통과시키며 각 트리가 분류한 결과에서 가장 많이 결과를 최종 분류 결과로 선택합니다. 많은 Tree를 만들기 때문에 Forest라는 단어를 쓰기 시작한거죠. random이라는 요소 때문에 overfitting을 방지하는 ensemble효과를 가져옵니다. 수많은 Decision Tree를 만들기 위해 Bagging, Bagging Features 등의 과정을 거칩니다.
인공신경망(Neural Network)은 각 단계별로 의존적인 end-to-end 구조로 하나의 서버에서 이뤄져야 합니다.
서버수의 여유가 있다면 많은 Decision Tree 모델을 병렬적으로 처리하도록 하여 Random Forest를 활용하는 것이 효율적입니다. 
#### References
- [Random Forest : iris 데이터 예측](https://myjamong.tistory.com/79)
- [Random Forest 개념 정리](https://eunsukimme.github.io/ml/2019/11/26/Random-Forest/)
- [Interview Question & Answer: 출근 루틴, 하루 3문제](https://yongwookha.github.io/MachineLearning/2021-01-29-interview-question) : 다른 문항들도 보는 것을 추천!

