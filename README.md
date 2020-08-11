# Datamining Project - 그거 맞아?
#### -피싱 사이트 탐지-

--------------------------------
## 프로젝트 계획 및 목표
본 프로젝트의 주제는 ‘기계학습을 이용한 피싱 사이트의 탐지’ 로 다음과 같은 세 가지의 목표를 가지고 프로젝트를 진행하였다.

+ 피싱 사이트의 특징파악 및 Data Feature 선정

+ 알고리즘별 평가를 통한 가장 적합한 알고리즘 판단

+ URL 기반의 피싱 사이트와 정상사이트 구별

위 목표를 이루기 위해 우선 수집한 URL 데이터 셋으로부터 피싱 사이트의 특징을 파악하고
사이트 구분을 위한 Feature 선정을 우선적으로 진행하였다. 이후 선정된 Feature를 분류 알고리즘인
KNN, SVM, RF와 회귀 알고리즘인 Logistic Regression에 적용하고 Accuracy와 ROC 커브 분석을
거쳐 가장 성능이 좋은 알고리즘을 선택하였다. 최종적으로 알고리즘이 적용된 피싱 사이트 분류기에
임의 데이터를 넣어 유의미한 성능을 가지는지에 대해 평가하였다. 

-----------------------------------
## 파일 설명

### /Algorithm/Algorithm.ipynb
+ 최종적으로 학습을 진행할 Dataset을 각각 KNN, Logistic Regression, Random Forest, SVM에 적용하여 정확도를 분석한 파일

### /Algorithm/Dataset.csv
+ 학습을 진행할 Dataset 파일

### /Data/get_url.ipynb
+ teamdata.csv 파일을 통해 lastdata.csv 파일을 출력하는 데이터 전처리 과정을 담당하는 파일 

### /Data/lastdata.csv
+ 학습에 사용될 feature data를 만들기 위한 raw url dataset 파일

### /Documents
+ 초기 제안서, 최종 보고서와 PPT 파일이 포함된 폴더 

### /EDA/countplot.ipynb
+ 데이터 전처리를 위한 countplot을 그린 파일 

### /Feature/get_feautre.ipynb
+ 최종 학습을 진행할 Dataset 파일을 출력하는 알고리즘이 포함된 파일 

### /Feature/Features.csv
+ 학습에 진행되는 Dataset 파일 
