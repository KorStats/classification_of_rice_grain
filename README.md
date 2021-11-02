# classification_of_rice_grain

### 1번 시나리오
데이터 전처리 안함 + --img 640 --batch 16 --epochs 30 + yolov5s 적용
현재 최대 precision : 0.6 ,f1 socre : 0.5(crop만... juk은 거의 학습되지 않아 전체 모델의 f1 score는 0.2로 굉장히 낮음)

11/3-11/5
https://lynnshin.tistory.com/48 평가지표에 대해서 읽고 요약하기
2번 시나리오 : 데이터 스케일링 해보기 (줌인/줌아웃/회전 데이터 추가해서 학습) -- 전체적인 평가지표 수치가 개선되는지 봐야함
3번 시나리오 : 1번 시나리오에 cross-validation 적용하기

