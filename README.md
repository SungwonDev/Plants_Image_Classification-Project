# ✨목차

1. [소개](#Plants-Image-Classification-Project)
2. [제작기간 및 참여인원](#제작기간-및-참여인원)
3. [사용기술 & 개발환경](#사용기술-&-개발환경)
4. [데이터 수집, 가공 및 라벨링](#데이터-수집,-가공-및-라벨링)

<br><br>

# Plants Image Classification Project
### 입력 받은 식물 이미지를 인식한다
Yolov5를 기반으로 제작한 식물 분류 인공지능<br>

<br>

[목차🔺](#목차)

<br><br>

# 제작기간 및 참여인원
### 데이터 수집, 가공 및 라벨링
2022-09-4 ~ 2022-9-20
### 데이터 학습 및 오류 수정
2022-09-20 ~ 2022-9-30
### 참여인원
팀 프로젝트 (총 6명)<br>

<br>

[목차🔺](#목차)

<br><br>

# 사용기술 & 개발환경
### 
<img src="https://img.shields.io/badge/Yolov5-black?style=for-the-badge&logo=Yolov5#&logoColor=white">&nbsp;<br>
<img src="https://img.shields.io/badge/colab-black?style=for-the-badge&logo=&logoColor=white">&nbsp;
<img src="https://img.shields.io/badge/make sense-black?style=for-the-badge&logo=make sense&logoColor=white">&nbsp;
<br>

[목차🔺](#목차)

<br>

# 제작과정 및 기능

### 1. 데이터 수집, 가공
Yolov5 모델에 학습시킬 이미지를 크롤링하여 각각 400장씩 수집합니다. <br>
수집한 이미지를 416 * 416 리사이즈한 뒤 ardisia_crenata_001부터 시작하여 400 순으로 이름을 정렬시킵니다.

<br>

### 2. 라벨링

Make Sense 사이트에서 400장씩 17종 총 6800장의 이미지를 라벨링 해줍니다.
라벨링이 끝나면 이미지와 바운딩박스의 정보가 담긴 txt파일을 받을 수 있습니다.

### 3. 데이터 학습


<br><br>

# 트러블 슈팅
<details>
<summary>프로젝트 진행과정의 분업과 효율성에 대한 고민</summary>
<br>
- 네 명의 인원이 각각의 파트를 맡아 개발을 진행하였을 때, 서로의 개발 코드에 대한 이해도가 떨어질 수 있다는 문제점이 있다.
- 반대로 네 명의 인원이 함께 모든 파트를 구현하기에는 시간적으로 효율성이 떨어진다는 판단을 하였다.
- 따라서 프로젝트 파트를 두개로 나눠 함께 구현함으로써 효율성과 원활한 개발코드 공유를 도모하였다. </br></br>
---
</details>

<br>
[목차🔺](#목차)
