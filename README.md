# classification_of_rice_grain

https://arxiv.org/pdf/1806.03891.pdf

## Today
#### 테스트 결과 좌표 추가 syntax 추가하기 (과제에 쓰이는 대표 코드 수정 예정)

## 과제1
###### 1. 150장 crop 데이터로 epoch20, batch 16 으로 yolov5s,m,l,x 각각 결과, 테스트 결과(이미지, 좌표), weight 지표 저장 (test_size=0.1)
###### 2. 1500장 crop 증분 데이터(90도 회전)로 epoch20, batch16으로 yolovx모델 결과, 테스트 결과(이미지, 좌표), weight 지표 저장 (test_size=0.1)
---------- 목요일까지
###### 3. 하이퍼파라미터 조정 (epoch : 30, 50, 100 -> batch 8, 32, 64 -> momentum, learning_rate조정)
###### 3-1. epoch 20 + batch 8 / epoch 20 + batch 16 / epoch 20 + batch 32 / epoch 20 + batch 64 => 최적의 batch 선택
###### 3-2. epoch 30 + batch / epoch 50 + batch / epoch 70 + batch / epoch 100 + batch => 최적의 epoch 선택
###### 3-3. 시간 남으면 momentum, learning_rate 조정하기

###### 4. 프로젝트 1의 최종 모델로 결과, 테스트결과(이미지, 좌표), weight지표 저장
###### 5. 시연영상 녹화

## 과제2
###### 1. 150장 crop/juk 데이터 1:1 비율로 맞추기
###### 2. 1500장 증분 데이터로 프로젝트1에서 나온 최종 모델을 적용해서 결과 저장
###### 3. 모델 코드 직접 수정하기 
###### 4. 쭉정이 인식 비율 개선 결과와 더 나아가야할 방향 제시

## 발표 구상
###### 1. 왜 yolo인가? (기존 프로그램과의 차이점 보여주기: real time으로 하기 위해) //1분
###### 2. 이미지라벨링 과정 및 model 선택 (epoch20, batch_size=16으로 한 yolov5 s/m/l/x 결과 이미지 비교 ) //1분
###### 3. 데이터 부족함에 대한 해결 방안 -> 증분을 이용하여서 정확도 XX % 향상됨 //1분
###### 4. 하이퍼파라미터 조정 (batch_size 조정, epoch 조정, momentum조정) // 1분
###### 5. 최종 모델의 평가지표 및 test결과 첨부 //2분
###### 6. 쭉정이 인식이 낮다는 한계 제시와 쭉정이 인식 향상을 위한 과정 발표 (1:1 비율, 모델 코드 직접 수정) //3분
###### 8. 앞으로 나아가야할 방향 : juk 정확도 향상을 위한 방법 추가 설명 및 count regression branch 추가 //1분
###### 10. 질문

