# Kannada 이미지 분석

> Kaggle의 Kannada MNIST 컴피티션 참여 : https://www.kaggle.com/c/Kannada-MNIST

> 사용 알고리즘 : CNN(Convolutional Neural Network), SVM(Support Vector Machine)

> SVM - Baseline

- 차원의 저주를 피하기 위해 주성분 분석(PCA)로 차원 축소 후 커널 트릭으로 가우시안 커널 사용

> CNN - SOTA

- VGG Net 사용하려 했는데 문제가 있었음
- 기존 VGG Net 모델의 사용 이미지는 224 x 224인 반면에 Kannada 이미지는 28 x 28
- 또한 Pooling을 5번 사용하여 이미지가 너무 작아질 것이 우려되었음
- 그래서 모델 크기와 필터 수 조정

> 결과 : CNN 정확도 98.46%로 1214팀 중 438등 (참고로 SVM은 정확도 95.56%)
