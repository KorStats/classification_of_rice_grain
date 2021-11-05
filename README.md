# classification_of_rice_grain

## Today
#### #scenario 파일에 다시 업데이트중.... (epoch수 적어도300으로 해야된다그래가지고 ㅠㅠ) 가중치는 용량 너무 커서 업로드 안됨. 별도 파일에 보관

## 과제
###### 1. 154장 epoch30 설정 -> yolov5의 다섯가지 모델 결과 출력 --> 모델 선택 (아마도 yolov5x가 되지 않을까)
###### 2. 데이터 증분하여 epoch 30 + yolov5x 모델 적용 (정확도 얼마나 증가하는지) https://lee-mandu.tistory.com/520?category=838684
###### 3. class 불균형 -> juk 이미지 증분 -> epoch 30 + yolov5x 모델 적용 (juk에 대한 인식률 얼마나 증가하는지)
###### 4. 하이퍼파라미터 조정 (epoch 수, batch_size, momentum 등등) //이 과정이 정말 많은 시간이 걸릴듯... 
###### 5. (시간 남으면) 모델 구조 수정
###### 6. 최종 모델 선택해서 평가지표 시연영상 녹화

###### Question 7 관련. yolov5x 자체가 이미 crop 인식률이 매우 높아 데이터 전처리과정을 진행한다 해도 효과가 두드러지게 안나타날 수도 있음. 
###### 속도가 가장 빠르지만 정확도는 떨어지는 yolov5s모델, epoch30 설정해서 데이터 증분/불균형을 이 모델로 테스트하면 효과가 더 눈에띄게 나타나지않을까? 하는 고민...

###### yolo 이론 https://deepbaksuvision.github.io/Modu_ObjectDetection/

## Question
###### 1. juk의 학습이 제대로 이루어지지않음. 평가지표를 count로 계산하는 것은 이론상 오류가 있는 것인지. juk의 이미지를 늘릴수는 없는지
###### 2. 정확도 향상에 대한 아이디어 수집
###### 3. 겹치는 데이터 많은 경우 yolo모델이 과연 옳은가 (오버랩 모델에서는 faster-RNN이 더 효과적)
###### 4. object detection은 mAP로 성능을 평가한다는데 어느정도로 높아야 사용할 수 있는가.. (현재 0.5도 안되서...)
###### 5. object detection의 파라미터 조정 방법이 있는지 (GridSearchCV, RandomSearchCV라던지...)
###### 6. cross validation 방안 (cross_val_score(lr_clf, X_data, Y_data, scoring='accuracy', cv=3) 같은...?)
###### 7. 발표 순서에 대한 질문.. 보통 전처리를 완료하고 다양한 모델들의 정확도를 구해서 가장 높은 모델을 선택하고 예측값에 대해 발표를 하지 않나. 

## 발표 구상
###### 1. 왜 yolo인가? (기존 프로그램과의 차이점 보여주기: real time으로 하기 위해) //1분
###### 2. 이미지라벨링 과정 및 model 선택 (epoch30, batch_size=16으로 한 yolov5 s/m/l/x 결과 이미지 비교 ) //1분
###### 3. 데이터 부족함에 대한 해결 방안 -> 증분을 이용하여서 정확도 XX % 향상됨 //1분
###### 4. class 불균형에 대한 해결 방안 -> juk 이미지 증분해봄 -> juk 에 대한 인식률 OO % 향상됨 //1분
###### 5. 하이퍼파라미터 조정 (batch_size 조정, epoch 조정, momentum 조정) //2분
###### 6. 모델 구조 수정 --> OO% 향상 //1분
###### 8. 최종 모델의 평가지표 및 시연 영상 //2분
###### 9. 앞으로 나아가야할 방향 : juk 정확도 향상을 위한 방법 추가 설명 //1분
###### 10. 끝

