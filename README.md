# ❤ Check Point
## 🧡 01. 데이터셋 준비
- 임포트 (iris기준)
    - from sklearn.datasets import load_iris
- 준비할 데이터
    - iris_data = iris.data -> 학습데이터
    - iris_label = iris.target  -> 정답지

## 🧡 02. 학습할 데이터와 테스트 데스트 데이터 분리
- 임포트
    - from sklearn.model_selection import train_test_split
- 형식
    - X_train, X_test, y_train, y_test = train_test_split(학습데이터,  
                                                    정답지, 
                                                    테스트 데이터 비율, 
                                                    랜덤)

## 🧡 03. 학습 모델 선정 및 학습과 예측
- 임포트 
    - 모델별로 임포트 방식이 상이함.

- 학습 모델 종류
    1) DecisionTreeClassifier
    2) RandomForestClassifier
    3) SGDClassifier
    4) LogisticRegression

- 형식
    - model = 모델명()
    - model.fit(학습데이터, 정답 데이터)
    - y_pred = model.predict(테스트 데이터)
    - X_train : 학습할 데이터 , y_train : 학습할 데이터의 정답지
    - X_test : 테스트할 데이터 
    - y_pred : 테스트한 데이터의 답지 , y_test : 테스트한 답지랑 비교할 실제 정답지
    
## 🧡 04. 성능 평가
- 임포트
    - from sklearn.metrics import classification_report
    - 여러가지 성능평가(metrics)방식이 존재함.
- 형식 
    - classification_report(y_test, y_pred) 
    - 테스트데이터를통해 얻은 답과 실제 답을 비교하여 정확도 측정
    


