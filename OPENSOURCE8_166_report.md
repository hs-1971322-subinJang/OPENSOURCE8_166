# 오픈소스 소프트웨어 시스템 설계서

#### 8반 16_6조 | 장수빈, 이현승, 임종혁, 김지훈, 김진호, 김태하



### 프로젝트 개요

---

 자기 관리에 대한 관심이 계속해서 증가하고 있는 현재, 운동 그중에서도 헬스에 대한 관심은 그 어느때보다도 높다고 볼 수 있다. 과거에는 몸이 좋은 사람들을 보기가 쉽지 않았다. TV에서 연예인이나 운동 선수들을 보거나 길거리에서 지나가는 사람들 정도였다면 지금은 각종 SNS와 유튜브 등의 사용량이 증가하면서 몸이 좋은 사람들에 대한 접근이 쉬워졌고 자연스럽게 운동에 대한 관심도 늘어가게 되었다. 

 헬스를 시작하는 사람이 늘어난 것이 단순히 몸 좋은 사람들을 많이 접한 것 만으로 일어난 것은 아니다. SNS에는 사람들뿐만 아니라 운동 방법이나 식단, 영양성분에 대한 얘기들도 늘어나게 되었고, 과거 운동을 배우려면 돈을 더내고 PT를 받거나 어깨너머로 다른 사람을 흉내내는 것보다 더 훌륭한 교육 자료를 볼 수 있게 되었다. 덕분에 헬스를 시작하는 진입장벽이 많이 낮아지게 되었다.

 그러나 넘치는 정보의 홍수 속에서 어떤 정보가 나한테 맞는 정보인지, 내 몸상태에 어떠한 운동을 해주어야 하는지, 어떠한 음식을 먹어야하는지는 개인이 시간을 들여 찾아보아야하고 수많은 시행착오가 있어야한다. 아니면 개인 PT를 받아야하는데 금전적으로 여유가 있지않다면 차마 선뜻 시도하지 못한다. 이러한 어려움들이 운동을 다시 시작하는 부담을 높이게 되고 이러한 문제를 해결하기 위해 인공지능을 이용한 PT 서비스를 생각하게 되었다.

### 서비스 설명

---

 크게 3가지의 기능으로 나눌 수 있다. 

1. 체형분석 및 운동 루틴 추천

   일명 "눈바디"라고 부르는 사용자의 체형 사진을 찍어 체형분석을 한다. 그 후 사용자의 개개인의 체형과 목표에 맞는 운동을 추천을 해준다. 예를 들어 다이어트를 원한다면 칼로리 소모가 좀 더 높거나 유산소 비중을 높인 운동 루틴들을 추천해서 사용자가 선택, 이용하게 한다.

2. 운동 자세 교정 

   단순히 운동 방법을 알려주는 것이 아닌 사용자가 운동하는 모습을 영상으로 찍으면 사용자의 자세를 분석해서 교정을 해준다. 또한 따라하기 쉽도록 골격을 화면에 보여줘서 사용자 스스로 자신의 자세가 어떠한지 평가 할 수 있게 해준다.

3. 식단 추천 및 성분 분석 

   사용자가 원하는 체중이나 목표를 설정하면 그에 맞는 식단을 추천해준다. 항상 같은 메뉴가 아닌 비슷한 영양성분의 다른 메뉴들을 추천해줘서 질리지 않고 식단을 이어나갈 수 있도록 도와준다. 앱에서 추천해준 음식이 아닌 경우 음식의 사진을 찍으면 사진을 분석해서 그 음식의 칼로리, 성분들을 표시해준다. 

### 유사서비스 분석

---

 국내에서 출시 중인 App으로는 Kakao에서 만든 '스마트홈트', '하우핏' 2개가 다운로드 수도 많고, 평점수가 높아 유사서비스 분석 대상으로 선정하였다. 두 App들은 모션인식을 기반으로, 일정 수치 이상의 동작 이상이 없을 경우 동작의 일치함을 인정한다. 또한, 유명 트레이너 및 강사들을 영입하여 운동의 진입장벽을 낮추고 있다. 운동을 마친 이후 소모한 kcal를 알려주며, 운동을 한 분기점 전과 비교하여 감소율을 알려준다. 그렇지만, 운동을 마치고 해당 부위의 다른 운동법 추천이 없는 점이 꽤나 아쉬웠다.
'스마트홈트'의 경우는 자체적인 Ai 인식을 통한 kcal 계산을 할 수 있는 식단 시스템이 있다. 사진을 찍거나, 앨범에 있는 사진을 가져올 시 자체적인 딥러닝을 마춘 Ai가 유사 음식들과 비교하여 kcal를 알려준다. 하지만 음식의 분별력에 있어 한참 부족한 면이 있었고, 이를 보완했으면 더욱 좋다는 생각을 가졌다.

'스마트홈트'의 경우 오픈소스 라이선스를 지니고 있다.
[사용된 오픈소스 목록 및 URL]
firebase : https://github.com/firebase/firebase-android-sdk
facebook sdk : https://github.com/facebook/facebook-android-sdk
kotlinx.coroutines : https://github.com/Kotlin/kotlinx.coroutines
retrofit2-kotlin-coroutines-adapter : https://github.com/JakeWharton/retrofit2-kotlin-coroutines-adapter
RxJava : https://github.com/ReactiveX/RxJava
RxAndroid : https://github.com/ReactiveX/RxAndroid
RxKotlin : https://github.com/ReactiveX/RxKotlin
RxBinding : https://github.com/JakeWharton/RxBinding
Dagger : https://github.com/google/dagger
Retrofit2 : https://github.com/square/retrofit
OkHttp3 : https://github.com/square/okhttp
Glide :https://github.com/bumptech/glide
Exo Player : https://github.com/google/ExoPlayer
Gson : https://github.com/google/gson
Simple XML : http://simple.sourceforge.net
Anko : https://github.com/Kotlin/anko
stetho : https://github.com/facebook/stetho
leakcanary : https://github.com/square/leakcanary
material-calendarview : https://github.com/prolificinteractive/material-calendarview
AutoScrollViewPager : https://github.com/angeldevil/AutoScrollViewPager
ViewPagerIndicator : https://github.com/JakeWharton/ViewPagerIndicator
ExpandableTextView : https://github.com/Manabu-GT/ExpandableTextView
Skeleton : https://github.com/ethanhua/Skeleton
ShimmerLayout : https://github.com/team-supercharge/ShimmerLayout
jglm : https://github.com/jroyalty/jglm
Kakao Open SDK : https://developers.kakao.com/docs/sdk
mace : https://github.com/XiaoMi/mace
tensorflow : https://github.com/tensorflow/tensorflow
FlycoTabLayout : https://github.com/H07000223/FlycoTabLayout
Flurry : https://github.com/flurry/flurry-android-sdk
RealtimeBlurView : https://github.com/mmin18/RealtimeBlurView
CircularProgressView : https://github.com/rahatarmanahmed/CircularProgressView
CircleProgressBar :https://github.com/dinuscxj/CircleProgressBar
Subsampling Scale Image View : https://github.com/davemorrissey/subsampling-scale-image-view
ARCore : https://developers.google.com/ar/reference



### 오픈소스 설명

---

운동이 끝난 직후, 추천 영상을 소개해주는 오픈소스를 가져오고자 한다.

Algorithm : 운동 영상이 끝난 직후 적절한 영상감을 찾는 과정을 알려준다.
https://github.com/TheAlgorithms/C-Plus-Plus

Recommend : 'Algorithm'의 결과 값을 바탕으로 '추천'을 하는 소스이다.
https://github.com/hongleizhang/RSPapers.git

---

### Open Pose를 이용한 모션인식  

#### 개요

 현재 PT 관리 서비스를 통해 사용자에게 제공하려는 것은 카메라를 통해 사용자의 몸과 움직임을 인식하여 운동 동작이 제대로 되었는지 체크를 하고 교정해주는 것이다. 사용자와의 상호작용을 통해 잘못된 동작을 지적해주고 직접 헬스장을 가지 않더라도 디지털 기술을 활용해 현장에서 트레이너의 지도를 직접 받지 못한다는 한계를 극복하여 집에서도 편하게 이용할 수 있다. 뿐만 아니라 개인이 원하는 운동을 선택할 수 있고 추천해주는 서비스를 통해 개인 맞춤형을 제공한다. 이러한 서비스를 제공하기 위해 제일 핵심적인 부분은 카메라를 통해 사용자를 인식하는 것이다. 이를 위한 오픈소스로 Open Pose를 알아보았다.

### OpenPose란?

<b>OpenPose</b>는 인간 자세 예측 (Human Pose Estimation)의 한 분야로 오로지 카메라 한대로만 가지고 사람의 몸, 얼굴, 손가락마디를 정확하게 예측하는 <b>real-time multi-person 오픈소스 라이브러리</b>이다. 기존 키넥트 센서를 사용해서 사람의 스켈레톤 데이터를 따오는 과거의 현실에 비해 Open Pose는 일반 카메라로도 사람의 스켈레톤 데이터를 따올 수 있게 만든 딥러닝 네트워크이다.

> 전통적인 방식의 Human Pose Estimation

기존 전통적인 방식은 사람 몸에 무언가를 부착하고 하기에 돈이 많이 들고 공간의 제약, 사람 체형에 따라 달라지는 장비로 많은 불편함이 있었다.

하지만 컴퓨터 성능의 발전으로 인해 컴퓨터비전(Computer Vision)에 딥러닝(Deep Learning) 기술이 사용되었고. 이러한 기술을 조합하여 영상으로만 이 Human Pose Estimation을 정확하게 할수 있게 되었다.

> 업그레이드 된 Human Pose Estimation -> OpenPose

OpenPose 전에도 이렇게 인간의 스켈레톤을 찾는 방법은 연구가 되었지만 그 전에는 사람을 검출하고, 검출된 사람에 대한 자세를 찾도록 반복 수행하는 Top-Down 방식을 사용 하였지만 OpenPose는 Bottom-Up 방식으로 반복처리 없이 수행을 한다.

<hr>
### 자세 추정 방식

- <em>Top-Down</em>

  - 이미지에서 사람을 먼저 찾고, 찾은 사람의 Bounding Box에서 자세를 추정
  - 사람을 먼저 찾고, 사람안에서 joint들을 찾기 때문에 정확도가 Bottom-up방식보다 높다
  - 검출된 사람들을 순회하며 joint들을 찾기 때문에 속도가 Bottom-up방식보다 느리다

- <em>Bottom-up</em>

  Bottom-up 방식은 이미지 상에서 모든 신체 부위를 먼저 찾아내고, 이후에 찾아낸 신체 부위가 어떻게 연결되는지 추론 하는 방법을 말한다.

  		- 이미지에서 joint들을 먼저 찾고, joint들의 상관관계를 분석하여 이들을 연결하여 자세를 추정

  - 정확도는 Top-down 방식에 비해 떨어지지만, Object Detection 과정이 없기 때문에 속도가 빨라 실시간 처리에 사용 가능

<hr>
### Realtime, Multi-Person ( Runtime Analsis )

Openpose의 저자는 Openpose 모델이 Realtime, Multi-Person 환경에서도 우수한 성능을 보여준다는 점을 논문의 제목에서부터 강조하고 있다. 저자는 다른 Human Pose Estimation 모델인 AlphaPose와 Mask R-CNN과 성능을 비교하여 이를 근거로 들었다. 자료는 아래와 같습니다.

![Realtime, Multi-Person](https://velog.velcdn.com/images%2Fmarkany%2Fpost%2F6e11738e-80be-4bf4-871e-199220d1dfff%2Fimage.png)

Openpose(아래쪽 평평한 두 개의 선)의 추론 시간은 이미지 내의 사람이 몇명이든 일정한 것이 가장 큰 특징이다. 위에서 설명했듯이 Bottom-up방식의 장점중 하나라고 할 수 있다. 반면 AlphaPose와 Mask R-CNN의 경우 이미지에 등장하는 사람 수에 비례해서 추론 시간이 늘어나는 것을 확인할 수 있다. 이를 통해 Openpose가 Realtime, Multi-Person 환경에서 유리하다는 것을 알 수 있다.

<hr>
### OpenPose의 딥러닝 네트워크 구조

![Realtime, Multi-Person](https://post-phinf.pstatic.net/MjAyMDAzMjBfMzQg/MDAxNTg0Njg3MzE5NDY5.6IwpJitMU6uSdP4RS_vuKaAGaVglQArkZ8WESZh3pfQg.c1fMTKvu_L5NOcJk4qTYjtwYtfV_EkDff5aqz1k5uJog.JPEG/humanpose_03.jpg?type=w1200)

네트워크의 입력은 높이(h) x 폭(w) 크기의 컬러 이미지이고 VGG-19 네트워크의 일부를 통과하게 된다. VGG 네트워크는 옥스포드대학교의 Visual Geometry Group에서 개발했다. 세계 최대 이미지 인식 경연대회인 ILSVRC(ImageNet Large Scale Visual Recognition Competition) 2014년 행사에서 GoogleNet과 함께 주목을 받으며 근소한 차이로 2위를 차지했지만, 구조가 간단하여 이해하기 쉽고 변형을 시켜가면서 테스트하기 용이한 장점이 있다.

이미지가 VGG-19 네트워크의 입력으로 들어가면, CNN의 Convolution Layer(C)와 Pooling Layer(P)를 거쳐서 특징맵(F)을 생성하게 된다. 특징맵(F)은 처음에는 큰 의미 없는 내용이 담겨 있지만, 그 내용을 학습 데이터와 비교하며 차이점을 점점 줄여나가는 방향으로 최적화를 하면 학습 데이터에 맞는 특징을 갖게 될 것이다. 그리고 이 특징맵(F)은 Stage 1의 입력으로 들어간다.

Stage 1은 2개의 브랜치로 나누어진다. 첫 번째 브랜치의 CNN(p1)은 모든 사람의 관절 위치를 결정하는 Confidence Map(S)을 생성한다. Confidence Map은 특정 신체부위가 위치할 가능성에 따라 높은 값(최저 0 ~ 최고 1)을 갖는 흑백 이미지라고 할 수 있다. 관절이 위치한 픽셀을 중심(중심 값은 1.0)으로 퍼지면서 값이 감소하는 Heatmap을 만든다. 예를 들어 아래 그림은 왼쪽 어깨에 대한 Confidence Map과 실제 데이터를 겹쳐서 표현한 이미지이다. 왼쪽 어깨에 해당하는 부분이 높은 값을 갖는 것을 볼 수 있다. 이 Confidence Map을 학습시켜서 사진으로부터 각 관절의 위치를 추정할 수 있다.

두 번째 브랜치의 CNN(ф)에서는 Part Affinity Fields(PAFs)를 예측하는데, PAFs(L)는 한 파트에서 다른 파트로 이어지는 방향(Position and Orientation)을 인코딩한 2D 벡터로 인체 부위 사이의 연관 정도를 나타낸다. 이 정보는 관절이 연결된 정보를 담고 있고 누구의 것인가를 파악하는 데 사용된다. 예를 들어 아래 [그림 5]는 왼쪽 어깨와 목의 Part affinity이다. 같은 사람의 인체 부위(목, 어깨)가 크게 연관되어 있는 것을 볼 수 있다.

이후 Stage 2부터는 Stage 1의 출력인 Confidence Map(S)과 PAFs(L), VGG Network의 출력인 특징맵(F)을 조합해서 CNN의 입력으로 사용한다. 네트워크가 깊어질수록 앞에 위치한 layer는 학습의 영향이 줄어들기 때문에 좀 더 나은 결과를 얻기 위해 매 Stage마다 특징맵(F)을 사용한다. 네트워크의 각 Stage에서는 예측한 수치와 실제 훈련 데이터에 있는 정답과 비교를 통해 오차값을 구하고 이를 최소화하는 방향으로 네트워크를 학습시킨다.

<hr>
### 한계

- 학습되지 않은 희귀한 자세 (추정은 어느정도 하지만 떨리는 현상)
- 몸의 일부가 잘 안보이게 될 시 (잘려서 나오거나 스켈레톤이 떨림)

- 사람 형태를 하고 있는 경우 (옷, 마네킹 등)

- 원거리 스켈레톤 검출 잘 안됨 (원거리의 기준은 카메라 해상도, FOV마다 다르다.)

<hr>
### 사용 결과 및 실행 결과

사람의 몸에 장비를 장착하지 않고 사진이나 영상으로 사람의 자세를 추출할 수 있다.

- #### Whole-body (Body, Foot, Face, and Hands) 2D Pose Estimation

![Result1](https://github.com/CMU-Perceptual-Computing-Lab/openpose/raw/master/.github/media/pose_hands.gif)

- #### Whole-body 3D Pose Reconstruction and Estimation

  ![Result2](https://github.com/CMU-Perceptual-Computing-Lab/openpose/raw/master/.github/media/openpose3d.gif)

- #### Google에 push up을 검색한 것 중 gif 파일을 Webcam에 비춘 모습

![Result](https://velog.velcdn.com/images%2Foneul1213%2Fpost%2Fd8e515b8-addd-41c5-968e-163b4704cfc8%2Fpushup-openpose.gif)

#### 오픈소스 출처

https://github.com/CMU-Perceptual-Computing-Lab/openpose

---

## **Talend Open Studio for Data Integration**

#### Talend Open Studio란?

Talend는 오픈소스 ETL 데이터 통합 솔루션으로 온프레미스와 클라우드 모두에서 호환된다. 데이터 통합, 데이터 프로파일링, 클라우드 통합 및 빅데이터 등을 위한 개방형 아키텍쳐이다. Apache License를 사용하며 Oracle, Microsoft SQL server, MySQL 등 다양한 데이터베이스와 연결되어 이용 가능하다. 

#### **ETL** 

ETL은 추출(Extract), 변환(Transform), 적재(Load)로 여러 데이터 소스에서 데이터를 추출하여 사용자가 원하는 형태로 변환 후 데이터 웨어하우스, 데이터베이스 등에 적재하는 것을 말한다. 처리해야하는 데이터의 양의 폭발적으로 늘어나면서 데이터 분석에 많은 비용이 들게 되었는데 ETL 툴을 이용하여 데이터를 효율적으로 활용할 수 있다.

![ETL(추출, 변환 및 로드) - Azure Architecture Center | Microsoft Learn](https://learn.microsoft.com/ko-kr/azure/architecture/data-guide/images/etl.png)

#### **장점**

\-   코딩을 하지않고 drag & drop으로 사용가능해 사용자 친화적인 GUI를 지원한다-

\-   이클립스 기반으로 구현되어서 JAVA코드와 매핑되고 jar파일을 생성 가능하다.

\-   1000개 이상의 사전 구축된 커넥터를 제공하여 파일 변환, 데이터 로드 등의 작업을 쉽게 수행가능하다.

\-   다양한 소스의 데이터를 쉽게 결합, 변환 및 업데이트 할 수 있다.

#### **용도**

본 서비스에서는 운동 정보나 음식의 영양 정보를 가지고 있는 데이터베이스에서 필요한 정보만을 추출해낸다. 그 후 운동 부위별, 음식은 영양소별(탄수화물, 단백질, 지방 등)으로 구분하여 새로이 데이터베이스에 저장하는 용도로 사용한다. 사용자가 운동이나 식단에 대해 물었을 때 미리 재구성한 데이터베이스에서 정보를 제공한다.

 #### 공식홈페이지

https://www.talend.com/

#### 소스코드

https://sourceforge.net/projects/talend-studio/

---

## MediaPipe 포즈 감지(Pose)

#### Licence
Apache License Version 2.0, January 2004

#### MediaPipe
MediaPipe란 구글에서 제공하는 AI 프레임워크로서, 비디오형식 데이터를 이용한 다양한 비전 AI 기능을 파이프라인 형태로 손쉽게 사용할 수 있도록 제공된다. AI 모델개발 및 수많은 데이터셋을 이용한 학습도 마친 상태로 제공되므로 간편하게 호출하여 사용하기만 하면 된다.
기본적인 얼굴인식 이외에도 Pose 인식 등 다양한 비전AI 기능들이 제공되는데 본 서비스에서는 Pose만 사용한다.

#### Pose Land Mark
포즈 랜드마크의 리스트이다.. 각 랜드마크는 다음과 같이 구성된다. 
x와 y : 랜드마크의 좌표는 각각 이미지의 너비와 높이로 [0.0, 1.0]로 표준화된다.
z : 엉덩이 중간 지점의 깊이를 원점으로 하여 랜드마크의 깊이를 나타내며, 랜드마크가 카메라에 가까울수록 값이 작아진다. z의 크기는 x와 거의 비슷한 척도를 사용한다.
Pose Land Mark를 통해 영상 속 사람의 Skeleton Model을 추출할 수 있다. 추출된 Skelton Model의 Pose Land Mark의 반복적인 움직임을 통해 올바른 동작 자세를 추출할 수 있다.

#### Pose Classification
MediaPipe를 활용하면 포즈 분류가 가능하다. 각 운동의 최종 상태( 팔굽혀 펴기를 예로 들면 위, 아래의 위치)에 대한 수백개의 샘플을 추출해낸다.
Pose Land Mark를 특징 벡터로 변환하기 위해 손목과 어깨, 두 손목 사이의 거리와 같이 미리 정의된 포즈 관절 목록 사이의 쌍별 거리를 사용한다. 알고리즘은 거리에 의존하기 때문에 모든 포즈는 변환 전에 동일한 몸통 크기와 수직 몸통 방향을 갖도록 정규화된다.

#### Repetition Counting
반복적인 움직임을 채크한다. 이를 통해 Pose Land Mark의 x,y,z 축의 움직임을 측정할 수 있다.

#### 활용방안
운동 영상을 통해 데이터를 구축한다.
Pose Classification를 통해 동작을 분류하고, Repetition Counting을 통해 반복적인 움직임을 관측한다. 그 후 Pose Land Mark을 통해 x,y,z,의 움직임을 수집한다.

#### Mediapipe 깃 허브 주소
https://github.com/google/mediapipe.git

출처
https://google.github.io/mediapipe/solutions/pose_classification.html
https://google.github.io/mediapipe/solutions/pose

---

### DFD

![DFD_오픈소스](https://user-images.githubusercontent.com/70803824/202886656-3e3a4d51-1360-4157-b3a9-210ad6fe2f08.png)

### 결론









