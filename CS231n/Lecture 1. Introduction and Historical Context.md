# 📝 Lecture 1. Introduction and Historical Context
<br></br>
## 🔎 Computer Vision이란?
 시각적 데이터들을 효과적으로 이해하고 분석해서, 컴퓨터가 인간의 시각적인 인식 능력을 가질 수 있도록 알고리즘을 개발하기 시작한 것이다. 
<br></br>

## 🔎 Vision의 역사
 약 5억 4천만 년 전, 천 만 년이라는 짧은 시간 동안 생물의 종이 폭발적으로 늘어나게 된 시기가 있다.
진화 생물 학자에 의하면 이 현상을 Evolution's Big Bang이라고 부른다.
이러한 현상이 발생한 원인의 가설 중 가장 설득력 있는 가설을 세운 Andrew Parker는 약 5억 4천만 년 전 최초의 눈이 생겨났다고 말했다.
그렇게 눈이 생김으로써 생물들은 훨씬 더 능동적이게 바뀌었고, 살아남기 위해서는 빠른 진화가 필요해졌다고 한다. 
<br></br>

## 🔎 Computer Vision의 역사


### 💡1950s
<b>[Hubel & Wiesel]</b>
 - 이들은 생물의 시각적 메커니즘을 알고 싶어 하였고, 이를 위해 그들은 고양이 두뇌 뒷면에 전극을 꽂았다.
그리고 어떤 자극을 줘야 1차 시각 피질 뉴런들이 격렬히 반응하는지 관찰했고, 이로써 1차 시각 피질에는 다양한 종류의 세포가 있다는 것을 알게 됐다.
이 중 시각적 input의 edges가 움직일 때 반응하는 단순한 세포에 초점을 맞추었고, 그들은 "시각 처리는 edge와 같은 단순한 구조로 시작되어 점점 복잡한 요소들을 처리하고, 궁극적으로 실제 시각적 input을 인지할 수 있게 된다"는 결론을 내렸다.
<br></br>

### 💡1960s
<b>[Larry Roberts' Block World]</b>
 - 사물들을 기하학적 모양으로 단순화하고, 이를 통해 시각적 세상을 재구성하는 연구를 진행하였다.
<br></br>
### 💡1966
<b>[MIT Summer Project]</b>
 - 이 기간동안 대부분의 시각 체계를 구현하고자 했다.
<br></br>
### 💡1970s
<b>[David Marr's Vision]</b>
 - David Marr는 그가 비전을 무엇이라 생각하는지, 어떤 방향으로 컴퓨터 비전이 나아가야 하는지, 컴퓨터가 비전을 인식하기 위해 어떤 방향으로 알고리즘을 개발해야 하는지에 대해 책을 저술하였다.
그는 이 책에서 "최종적인 full 3D 표현"으로 만들려면 몇 단계의 과정을 거쳐야 한다고 하였다.
첫 단계는 "Primal Sketch"라고 하는 단계이다. 이 과정은 가장자리, 막대, 끝, 가상의 선, 커브, 경계가 표현되는 과정이고, 이는 신경 과학자들에게 영감을 받은 것이다. 이것은 Hubel&Wiesel의 말과도 비슷하다.
그리고 다음 단계는 "2.5D Sketch"라는 단계이며, 이 단계는 시각 장면을 구성하는 표면, 깊이, 레이어, 불연속 점등의 정보를 종합하는 것이다.
마지막으로 이것들을 한 곳에 모아 surface and volumetric primives 형태의 계층적으로 조직화된 최종 3D 모델을 만들어 내는 것이다.

<b>[Stanford & SRI]</b>
 - 과학자들이 "generalized cylinder", "pictorial structure" 아이디어를 제안했다. 이 두가지의 공통 기본 개념은 "모든 객체는 단순한 기하학적 형태로 표현할 수 있다"는 것이다. 
이 두 방법 모두 단순한 모양과 기하학적 구성을 이용하여 복잡한 객체를 단순화시켰다. 
<br></br>
### 💡1980s
<b>[David Lowe]</b>
 - David Lowe는 어떻게 하면 단순한 구조로 실제 세계를 재구성/인식할 수 있을 지 고민 했고, 이 연구에서 면도기를 인식하기 위해서 선, 경계, 직선을 조합하여 면도기를 구성해냈다.

<br></br>
✔️ 여기까지 아주 대담한 시도였지만 아주 단순한 수준에 그쳤다. 그래서 컴퓨터 비전 연구자들은 도대체 어떤 실수를 하고 있는지 고민을 하였고,
"객체 인식이 어렵다면 객체 분할(segmentation)이 먼저가 아니었을까"하는 질문을 떠올렸다.
여기서 말하는 객체 분할은 이미지의 각 픽셀을 의미 있는 방향으로 군집화하는 방법을 의미한다. 픽셀을 모았을 때 이것이 사람인지 인식할 수 없을지라도, 배경 픽셀과 사람이 속해 있을지도 모르는 픽셀을 가려낼 수 있었다.
이것을 "Image segmentation"이라고 하였고, 이 문제를 Jitendra Malik 교수와 Jianbo Shi가 연구하였다. 이 연구에서는 Image Segmentation 문제를 해결하기 위해 그래프 이론을 도입하였다.
<br></br>

### 💡1999/2000s
<b>[기계학습/통계적 기계학습]</b>

<b>["Support Vector Machine", "Boosting", "Graphical models", "Neural Network"]</b>

<b>[Paul Viola & AdaBoost]</b>
 - 실시간 얼굴 인식을 성공시켰다.

<b>[Fujifilm]</b>
 - 실시간 얼굴을 지원하는 최초 디지털 카메라를 선보였다.

<b>[David Lowe's SIFT feature]</b>
- 객체의 특징 중 일부는 다양한 변화에 좀 더 강인하고 불변한다는 점을 발견하고, 객체 인식은 객체에서 이와 같은 중요한 특징을 찾아 내어 그 특징들을 다른 객체에 매칭시키는 과제로 만들었다.
이미지에 존재하는 특징을 사용하게 되면서 컴퓨터 비전은 또 한 번의 도약을 하였고, 장면 전체를 인식하기에 이르렀다.

<b>[Spatial Pyramid Matching, Support Vector Algorithm]</b>


* 21세기에는 인터넷과 카메라의 발전으로 실험 데이터의 질이 급격히 상승했다. 이 때부터 양질의 데이터 셋을 모으기 위한 움직임이 이어졌다.

<b>[PASCAL Visual Object Challenge(VOC)]</b>
 - 이 데이터 셋에는 20개의 클래스가 있었고, 클래스 당 수천 수만 개의 이미지들이 있었으며 이것 알고리즘 테스트에 사용되었다.

<b>[ImageNet]</b>
 - 가장 큰 데이터 셋을 만들어 Overfitting을 방지하고 일반화 능력을 키워 이 세상 모든 객체들을 인식할 준비를 하였다. 
ILSVRC 대회를 열어 해당 데이터 셋으로 지속적인 알고리즘 테스트를 진행하였다. 여기서 낸 실험 결과에서 주목해야할 것은 2012년도의 CNN이다.
CNN이 오류율을 약 10% 초반으로 감소시킨 것을 확인할 수 있었다.
<br></br><br></br>

<b>
🗝️ 따라서, 이 수업에서는 CNN에 대하여 중점적으로 배울 것이다. 이 수업에서는 "image classification", "object detection", "image captioning"에 대해 다룰 것이다.
컴퓨터 비전의 최종적인 목표는 "사람처럼 볼 수 있는 기계를 만드는 것"이며, 앞으로 "Semantic Segmentation", "Perceptual Grouping", "3D understanding", "행동 인식"을 문제를 해결해 나가야할 것이다.</b>
