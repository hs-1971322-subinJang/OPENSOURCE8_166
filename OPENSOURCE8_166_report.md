# 오픈소스 소프트웨어 시스템 설계서

#### 8반 16_6조 | 장수빈이현승, 임종혁, 김지훈,김진호,김태하



#### 프로젝트 개요



#### 서비스 설명


#### 유사서비스 분석

##### 유사점

현재 시중에 출시되고 있는 '스마트홈트', '하우핏' 등 수 많은 모션인식 PT App들이 있다. 
이 중 국내에서 출시 중이고 평점 수가 높은 '하우핏'과 Kakao에서 만든 '스마트홈트'를 유사서비스 분석 대상으로 선정하였다. 
두 App들은 모션인식을 기반으로 일정 수치 이상의 동작 이상이 없을 경우 동작의 일치함을 인정한다. 
또한, 유명 트레이너 및 강사들을 엽입하여 운동의 진입장벽을 낮추고 있다. 
운동을 마친 이후 개인 정보 탭에서 소모한 kcal를 알려주고, 운동을 한 분기점 전과 비교하여 감소율을 알려준다. 
기존 오프라인 시장에서의 PT는 운동을 하는데 있어 동작의 일치율을 본다. 
즉, 현 시장에서의 모션인식은 오프라인과 똑같은 형태의 서비스를 제공하고있다. 
다만, 대면에서와는 달리 모션인식은 전면으로만 보기에 각도에 있어서는 정확한 충고를 주기는 어렵다. 
온라인 상에서의 제공되는 서비스로는 동작의 일치율을 확인하는 모션인식, 식단을 촬영 시 해당하는 kcal를 알려주는 
식단 계산기가 있다. 우리가 제공하는 서비스 또한 모션인식 및 식단 계산을 한다는 점에 있어 타사들과 유사하다고 할 수 있다.

##### 차별점
=======
현재 시중에 출시되고 있는 '스마트홈트', '하우핏' 등 수 많은 모션인식 PT App들이 있다. 

이 중 국내에서 출시 중이고 평점 수가 높은 '하우핏'과 Kakao에서 만든 '스마트홈트'를 유사서비스 분석 대상으로 선정하였다. 

두 App들은 모션인식을 기반으로 일정 수치 이상의 동작 이상이 없을 경우 동작의 일치함을 인정한다. 

또한, 유명 트레이너 및 강사들을 엽입하여 운동의 진입장벽을 낮추고 있다. 

운동을 마친 이후 개인 정보 탭에서 소모한 kcal를 알려주고, 운동을 한 분기점 전과 비교하여 감소율을 알려준다. 

기존 오프라인 시장에서의 PT는 운동을 하는데 있어 동작의 일치율을 본다. 

즉, 현 시장에서의 모션인식은 오프라인과 똑같은 형태의 서비스를 제공하고있다. 

다만, 대면에서와는 달리 모션인식은 전면으로만 보기에 각도에 있어서는 정확한 충고를 주기는 어렵다. 

온라인 상에서의 제공되는 서비스로는 동작의 일치율을 확인하는 모션인식, 식단을 촬영 시 해당하는 kcal를 알려주는 

식단 계산기가 있다. 우리가 제공하는 서비스 또한 모션인식 및 식단 계산을 한다는 점에 있어 타사들과 유사하다고 할 수 있다.

동일한 서비스 형태는 타사들과의 경쟁 요소가 될 수 없다. 
현재 사용중인 PT의 핵심인 모션인식에서는 차별점을 크게 둘 수는 없다. 

현 시점에서 PT 앱을 이용 시 해당 서비스에서 제작한 영상을 보여주고, 
이에 사용자가 따라하는 형태를 취한다.  만약 운동에 대해 지식이 조금이나 있는 
사용자가 어깨 부위와 등 부위를 운동을 병행하고자 할 때, 각각의 영상을 따로 틀고, 
정해진 방식의 운동 루틴을 해야만 한다. 이러한 애로사항을 해결하기 위해 모션을 
인식만 하는 화면을 심플하게 만들고, 동작을 취함에 따라 해당하는 동작 이름을 아래에 기제해주고, 
동작의 일치율을 확인해줌으로 사용자의 니즈를 충족하고자 한다. 
만일 운동을 처음하는 사용자의 경우는 화면에 자신이 운동을 하고 싶은 부위를 손바닥으로 
짚어 확인 또는 직접 입력을 하게 되면 서비스는 해당 부위의 적절한 운동 동작을 알려준다.

운동을 시작하는 사람에게 운동만큼의 중요한 요소는 식단 관리이다. 
아무리 운동을 열심히해도 일일섭취량 및 영양 성분을 챙기지 않을 경우 효과는 미미하다. 
식단 계산에 있어서는 각 회원에 맞는 하루 섭취량을 추가적으로 알려주고자 한다. 
사람마다 체형을 천차만별이다. 평균적인 남성, 여성의 하루 섭취량만 존재하고, 
평균적이기에 모두에게는 맞을 수 없다는 단점이 있다. 식단 계산에 해당 회원이 자신의 인바디를 
아는 경우는 직접 기제를 하고, 혹여 인바디를 모르는 경우 자신의 몸무게, 키를 입력하고, 
상체 및 하체의 대략적인 체형을 기제한다. 예를 들어 상체의 경우 배가 약간 나오고, 
하체에 살집이 많은 경우 상체 체형을 약간 비만, 하체 체형을 비만으로 체크시 각 회원에 
비슷한 데이터의 kcal를 추천을 해주고, 식단을 하는데 있어 필수적으로 챙겨주면 좋은 식재료 및 음식들을 추천한다.
=======
https://patterns-wipe-635163.framer.app/ (어플 UI 예시)

#### 오픈소스 설명

### FoodLens 오픈소스

개요 : 기존(''다이어트신'' 등)의 어플에서는 사용자가 직접 먹은 음식을 입력해야하는 번거로움이 있었다. 다음 오픈소스는 사용자로부터 사진데이터를 입력받으면 해당 사진의 음식데이터를 보내주는 기능을 수행한다. 사용자는 사진만으로 자신이 먹은 음식의 종류를 볼 수 있으며, 최종적으로 해당 음식의 정보가 맞는지 확인한 후 영양 정보또한 얻을 수 있다. 해당 데이터는 DoingLab DB를 기반으로 제공되며, MIT라이센스를 제공한다.

오픈소스 라이센스 : MIT라이센스

오픈소스 기능 : 입력된 사진데이터를 바탕으로 음식정보를 추천하고 제공한다.  두잉랩(SDK제공사)에서 제공하는 DoingLab DB를 기반으로 음식의 이름, 칼로리, 탄수화물, 단백질, 지방, 비타민 등의 데이터 값을 리턴받는다. 



(섭취한 영양정보 산출 계산식 [FoodLens 오픈소스 Readme.md에서 발췌])

`for(int i = 0; i < recognitionResult.getFoodPositions().size(); i++) {
	FoodPosition foodPosition = foodPositions.get(i);
	float eatAmount = foodPosition.getEatAmount(); // 사용자가 설정한 1회 섭취량
	Nutrition nutrition = foodPosition.getUserSelectedFood().getNutrition(); `

`// 선택한 음식에 대한 Raw 영양정보 데이터
	eatAmount * nutrition.getCarbonHydrate(); // 1회 섭취한 음식에 대한 탄수화물 섭취량
	eatAmount * nutrition.getProtein(); // 1회 섭취한 음식에 대한 단백질 섭취량
	eatAmount * nutrition.getFat(); // 1회 섭취한 음식에 대한 지방 섭취량
	...
}`

해당 코드를 사용하여 사용자가 섭취한 음식의 **총 칼로리 데이터**를 얻을 수 있다.



[오픈소스 github : https://github.com/doinglab/FoodLensSDK]
=======
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

  	이미지에서 joint들을 먼저 찾고, joint들의 상관관계를 분석하여 이들을 연결하여 자세를 추정

  - 정확도는 Top-down 방식에 비해 떨어지지만, Object Detection 과정이 없기 때문에 속도가 빨라 실시간 처리에 사용 가능

<hr>


### Realtime, Multi-Person ( Runtime Analsis )

Openpose의 저자는 Openpose 모델이 Realtime, Multi-Person 환경에서도 우수한 성능을 보여준다는 점을 논문의 제목에서부터 강조하고 있다. 저자는 다른 Human Pose Estimation 모델인 AlphaPose와 Mask R-CNN과 성능을 비교하여 이를 근거로 들었다. 자료는 아래와 같습니다.

![Realtime, Multi-Person](https://velog.velcdn.com/images%2Fmarkany%2Fpost%2F6e11738e-80be-4bf4-871e-199220d1dfff%2Fimage.png)

Openpose(아래쪽 평평한 두 개의 선)의 추론 시간은 이미지 내의 사람이 몇명이든 일정한 것이 가장 큰 특징이다. 위에서 설명했듯이 Bottom-up방식의 장점중 하나라고 할 수 있다. 반면 AlphaPose와 Mask R-CNN의 경우 이미지에 등장하는 사람 수에 비례해서 추론 시간이 늘어나는 것을 확인할 수 있다. 이를 통해 Openpose가 Realtime, Multi-Person 환경에서 유리하다는 것을 알 수 있다.

<hr>


### OpenPose의 딥러닝 네트워크 구조

![Realtime, Multi-Person](https://post-phinf.pstatic.net/MjAyMDAzMjBfMzQg/MDAxNTg0Njg3MzE5NDY5.6IwpJitMU6uSdP4RS_vuKaAGaVglQArkZ8WESZh3pfQg.c1fMTKvu_L5NOcJk4qTYjtwYtfV_EkDff5aqz1k5uJog.JPEG/humanpose_03.jpg?type=w1200)

=======
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

#### License

- ACADEMIC OR NON-PROFIT ORGANIZATION NONCOMMERCIAL RESEARCH USE ONLY

- 주소 : https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/LICENSE

=======

##### Recommders : 내부 탑재된 알고리즘을 통해 유저에게 추천을 해주는 오픈소스

##### 원리

1.  데이터 준비 : 각 추천 알고리즘에 대한 데이터 준비 및 로드

2.  모델 : 다양한 고전 및 딥 러닝 추천 알고리즘을 사용하여 모델을 구축

   Ex) 교대 최소 제곱 (ALS), eXtreme Deep Factorization Machines (xDeepFM)

3.  평가 : 오프라인 메트릭을 사용하여 자체적인 알고리즘 평가

4.  모델 선택 및 최적화 : 추천 모델에 대한 하이퍼 파라미터 값 조정 및 최적화

##### 소스 구현

내부에 탑재된 알고리즘을 활용하여 동일한 부위 및 운동 기구에 해당하는 영상을 찾는다.

너비 또는 깊이에 따른 적절한 탐색 방법을 활용하여 우선적으로 해당 부위의 운동 영상을 탐색한다.

동일한 운동 기구를 찾아 일치 여부를 확인한 후 요청한 회원에게 지원할 준비를 마친다.

이때, 알고리즘은 1순위로 동일한 운동 부위 및 운동 기구, 2순위로 동일한 운동 부위, 
3순위로 동일한 운동 기구의 순서를 지니고 있게 된다.

또한, 운동 뿐만 각기 다른 체형의 회원들마다 권장되는 일일 섭취량 및 식자재, 음식들 또한 지원한다.

##### 소스 구현 시뮬레이션

Ex1) A는 어깨 부위를 덤벨이라는 운동 기구를 통해 진행한다. 이때, 덤벨 숄더 프레스를 5세트

진행하였고, 시스템에서는 어깨 부위의 영상감을 알고리즘을 통해 찾아내고, 회원이 이용한

운동 기구를 체크하여 비슷 또는 동일한 기구와의 유사함을 확인한다. 이후 요청자에게 지원할 준비를

마친다.

Ex2) B는 체지방률이 많이 높고, 운동을 막 시작한 새싹 회원이다. 이때, 자신의 kcal 계산을 하였다.

시스템은 B의 계산 값을 확인하여 인바디 값에 대입하고, 동일한 체형의 일일 섭취량을 확인한다.

이후 점진적으로 체지방을 감량을 도울 수 있게 몸에 좋은 식자재 및 음식들을 추천한다.
##### 출처 및 언어, 라이선스

출처 : https://github.com/microsoft/recommenders.git

언어 : Python

라이선스 : MIT license
=====

## **Talend Open Studio for Data Integration**

#### Talend Open Studio란?

Talend는 오픈소스 ETL 데이터 통합 솔루션으로 온프레미스와 클라우드 모두에서 호환된다. 데이터 통합, 데이터 프로파일링, 클라우드 통합 및 빅데이터 등을 위한 개방형 아키텍쳐이다. Apache License를 사용하며 Oracle, Microsoft SQL server, MySQL 등 다양한 데이터베이스와 연결되어 이용 가능하다. 

#### **ETL** 

ETL은 추출(Extract), 변환(Transform), 적재(Load)로 여러 데이터 소스에서 데이터를 추출하여 사용자가 원하는 형태로 변환 후 데이터 웨어하우스, 데이터베이스 등에 적재하는 것을 말한다. 처리해야하는 데이터의 양의 폭발적으로 늘어나면서 데이터 분석에 많은 비용이 들게 되었는데 ETL 툴을 이용하여 데이터를 효율적으로 활용할 수 있다.

![image-20221112231455901](C:\Users\eltm5\AppData\Roaming\Typora\typora-user-images\image-20221112231455901.png)

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


MediaPipe 포즈 감지(Pose)

Licence
Apache License Version 2.0, January 2004

Mediapipe 깃 허브 주소
https://github.com/google/mediapipe.git

MediaPipe
MediaPipe란 구글에서 제공하는 AI 프레임워크로서, 비디오형식 데이터를 이용한 다양한 비전 AI 기능을 파이프라인 형태로 손쉽게 사용할 수 있도록 제공된다. AI 모델개발 및 수많은 데이터셋을 이용한 학습도 마친 상태로 제공되므로 간편하게 호출하여 사용하기만 하면 된다.
기본적인 얼굴인식 이외에도 Pose 인식 등 다양한 비전AI 기능들이 제공되는데 본 서비스에서는 Pose만 사용한다.

Pose Land Mark
포즈 랜드마크의 리스트이다.. 각 랜드마크는 다음과 같이 구성된다. 
x와 y : 랜드마크의 좌표는 각각 이미지의 너비와 높이로 [0.0, 1.0]로 표준화된다.
z : 엉덩이 중간 지점의 깊이를 원점으로 하여 랜드마크의 깊이를 나타내며, 랜드마크가 카메라에 가까울수록 값이 작아진다. z의 크기는 x와 거의 비슷한 척도를 사용한다.
Pose Land Mark를 통해 영상 속 사람의 Skeleton Model을 추출할 수 있다. 추출된 Skelton Model의 Pose Land Mark의 반복적인 움직임을 통해 올바른 동작 자세를 추출할 수 있다.

Pose Classification
MediaPipe를 활용하면 포즈 분류가 가능하다. 각 운동의 최종 상태( 팔굽혀 펴기를 예로 들면 위, 아래의 위치)에 대한 수백개의 샘플을 추출해낸다.
Pose Land Mark를 특징 벡터로 변환하기 위해 손목과 어깨, 두 손목 사이의 거리와 같이 미리 정의된 포즈 관절 목록 사이의 쌍별 거리를 사용한다. 알고리즘은 거리에 의존하기 때문에 모든 포즈는 변환 전에 동일한 몸통 크기와 수직 몸통 방향을 갖도록 정규화된다.

Repetition Counting
반복적인 움직임을 채크한다. 이를 통해 Pose Land Mark의 x,y,z 축의 움직임을 측정할 수 있다.

활용방안
운동 영상을 통해 데이터를 구축한다.
Pose Classification를 통해 동작을 분류하고, Repetition Counting을 통해 반복적인 움직임을 관측한다. 그 후 Pose Land Mark을 통해 x,y,z,의 움직임을 수집한다.

출처
https://google.github.io/mediapipe/solutions/pose_classification.html
https://google.github.io/mediapipe/solutions/pose

---

#### DFD

![DFD_오픈소스](https://user-images.githubusercontent.com/70803824/203985749-e0714078-d210-4306-98da-4885645b5ec6.jpg)

<hr>

### <fitness_calculator>

#### github 주소   
https://github.com/manas3874/fitness-calculator      
#### 라이센스      
MIT License   

#### 개요
fitness calulator는 사용자의 BMI, BMR, 칼로리 필요량, 총 일일 에너지 소비량, 매크로 등을 계산하는 데 도움이 되는 오픈소스입니다.

#### 기능   
포함된 기능은 총 8가지로   
1.BMR(기초 대사율)   
2.BMI(체질량 지수)   
3.BFP(체지방률)   
4.이상체중   
5.칼로리 필요량   
6.TDEE(총 일일 에너지 소비량)   
7.매크로   
8.BAC(혈중 알코올 농도)   
가 있습니다.   


#### 활용 및 작동 방식
이 오픈 소스로 사용자에 현재 상태 및 알맞은 목표와 필요한 칼로리양을 쉽게 알 수 있습니다.   
이러한 기능 중 저희 어플에 사용하면 좋은 것들은 BMR, BMI, BFP, 칼로리 필요량, TDEE가 있습니다.   
이러한 기능들을 사용하기 위해서는 어플 초기, 성별, 나이, 신장, 체중, 목, 허리, 엉덩이, 활동량을 입력합니다.   
이후 변화 하는 변수들만 재입력하면 이후 계산을 통하여 원하는 값들의 반환이 가능합니다.   
이중 활동량이라는 변수는 5가지의  있습니다. sedentary, light, moderate, active, extreme 왼쪽부터 오른쪽 순으로 활동 강도를 나타내며,   
예를들어 직업이 계속 앉아있는 사무직이며, 운동을 주 1회 이하 하는 경우 sedentary, 자주 움직이는 직업에 매일 고강도의 운동을 하고있을경우 extreme, 식으로 선택하면 됩니다.


#### 결론









