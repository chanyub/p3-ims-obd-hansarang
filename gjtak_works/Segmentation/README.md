# P-stage3 Segmentation 한사랑개발회 탁금지 실험결과 정리

|Date|Model Name|Encoder|Arguments|WanDB Link|LB score|ETC|
|----|----------|-------|---------|----------|--------|---|
|2021-04-29|Unet|resnet50|loss function=CrossEntropyLoss<br>optimizer=adam(params=model.parameters() / learning rate=1e-4 / weight decay=1e-6)<br>pretrained=imagenet<br>batch size=10<br>epoch=10|[resnet50](https://wandb.ai/pstage12/gjtak/runs/3grmk6yo?workspace=user-atica)|efficientnet 계열보다 빠른 학습 시간을 보임|
|2021-04-29|Unet|resnext50_32x4d|loss function=CrossEntropyLoss<br>optimizer=adam(params=model.parameters() / learning rate=1e-4 / weight decay=1e-6)<br>pretrained=imagenet<br>batch size=10<br>epoch=10|[resnext50_32x4d](https://wandb.ai/pstage12/gjtak/runs/d2ts77ua?workspace=user-atica)|efficientnet 계열보다 빠른 학습 시간을 보임  validataion 상으로는 지금까지 진행한 테스트 결과 중 가장 좋은 결과를 보임|
|2021-04-29|Unet|resnet101|loss function=CrossEntropyLoss<br>optimizer=adam(params=model.parameters() / learning rate=1e-4 / weight decay=1e-6)<br>pretrained=imagenet<br>batch size=10<br>epoch=10|[resnet101](https://wandb.ai/pstage12/gjtak/runs/1zmluwoa?workspace=user-atica)|efficientnet 계열보다 빠른 학습 시간을 보임  validataion 상으로는 지금까지 진행한 테스트 결과 중 가장 좋은 결과를 보임|
