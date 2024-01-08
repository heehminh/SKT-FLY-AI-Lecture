# Transfer Learning

종류

- Fine-tuned ConvNet: 미리 학습된 ConvNet의 마지막 Fully Connected Layer만 변경해 분류 실행
- Pre-trained Model: 미리 학습된 모델의 가중치를 새로운 모델에 적용
- Domain Adaptation: 풍부한 데이터를 바탕으로 훈련 시 도메인 구분 능력은 약하게 학습하여 Target Data를 분류가능하도록 모델 구축
- Layer Re-use: 기존 모델의 일부 Layer를 재사용하여 부족 Data Domain 모델 구축에 활용항목 추가 <br />

```
VGG16(.., include_top=False, ..)
```

-> feature extractor 용도로만 사용하고 그렇게 추출한 feature를 가지고 다른 모델을 학습하는 것을 의미
