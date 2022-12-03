# ✨목차

1. [소개](#Plants-Image-Classification-Project)
2. [제작기간 및 참여인원](#제작기간-및-참여인원)
3. [사용기술 & 개발환경](#사용기술-&-개발환경)
4. [제작과정 및 기능](#제작과정-및-기능)

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
- Google colaboratory
- Yolov5
- Tesnsorflow
<br>

[목차🔺](#목차)

<br>

# 식물 데이터셋
### 1. Class : 17
  - Golden_pothos, Muehlenbeckia_complexa, Happy_plant, Bunnyearscactus, Rosmarinus, Dracaena, Chlorophytum
  - Monstera, Chamaedorea_elegans, Bengal_Fig, Stuckyi, Pachira, Ardisia_crenata, Zamia, Staghorn
  - Birkin, Wilma

2. Images : 6800
3. Train/Vaild (100%)
  - Train : 5440(80%)
  - Valid : 1360(20%)



Data set Download : https://drive.google.com/file/d/18gkiKTJwl_FO99dnqbxyCCDyFQdo6hpY/view?usp=sharing

# 모델 트레이닝

1. yolov5 설치
```bash
!git clone https://github.com/ultralytics/yolov5.git
```

<br>

2. requirements.txt 설치
```bash
%cd /content/yolov5/
pip install -r requirements.txt
```

<br>

3. Model 학습
```bash
!python train.py --img 416 --batch 16 --epochs 20 --data /content/dataset/data.yaml --cfg ./models/yolov5s.yaml --weights yolov5s.pt --name yolov5s_result
```

<br>

4. Model 테스트
``` bash
!python detect.py --weights /content/yolov5/runs/train/yolov5s_result/weights/best.pt --img 416 --conf 0.5 --source /content/dataset/export/testimg/테스트할 이미지.jpg
```

<br>

### 4. 학습 결과

학습된 가중치 파일(best.pt) 

<br>

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
