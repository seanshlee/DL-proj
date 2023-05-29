# DL-proj

# 1. 프로젝트 주제 
: Kaggle에서 찾은 FER(Facial Expression Recognition)2013 데이터셋을 활용하여 간단한 딥러닝 모델 적용 서비스 만들기 

# 2. 데이터셋 설명 
: Angry, Disgusted, Fearful, Happy, Neutral, Sad, Surprised 까지 총 7가지의 표정 레이블로 분류된 35,887 개의 48x48 사람 얼굴 이미지 데이터셋

# 3. 모델 개발 및 적용 
- CNN 모델 개발 : LEARNING RATE, EPOCHS, Activation Functions, Convolution layer 개수 등을 조정하여 CNN 모델을 직접 개발, 68%의 정확도 달성 
- 전이학습(Transfer Learning) : 데이터셋에 적합한 ResNet-18, EfficientNet_b0, VGG16 모델로 전이학습 실시
(결과적으로 ResNet18과 EfficientNet은 각각 70.51%, 70.75% 의 정확도를, VGG16 모델은 73.88% 의 정확도를 달성함)

# 4. 개발된 모델을 적용한 웹캠 표정인식 서비스 개발 
- Colab : 로컬 PC에 GPU가 없는 경우, GPU 사용이 제공되는 코랩 환경에서 웹캠을 켜고 서비스를 적용할 수 있도록 JavaScript와 OpenCV에 모델을 적용한 코드 작성
- 로컬 PC : 로컬 PC에 GPU가 있거나, 그냥 CPU 환경에서 구동할 경우에 사용 가능한 OpenCV + 딥러닝 모델 코드 작성
