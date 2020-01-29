# DSC2019_Final
> 네이버 DSC 본선 과제

## 1. 폴더 설명

### 1.1 foreign_lunage/
- 해외 주식 데이터분석에 사용한 csv 파일들의 모음

### 1.2 data/
- 제공 받은 데이터 파일(비어 있음)


## 2. 월령 수집 관련 파일

### 2.1 all_lunage.py
- 한국 천문 연구원에서 제공하는 월령 데이터(공공데이터)를 api를 이용하여 수집
- 링크: https://www.data.go.kr/dataset/15012689/openapi.do
- return으로 DataFrame을 반환

### 2.2 save_lunage.ipynb
- all_lunage.py를 이용하여 dt_lunage.csv파일로 월령 정보를 저장. 

### 2.3 dt_lunage.csv
- 20090101 ~ 20190531 까지의 월령 정보를 담고 있음


## 3. 데이터 전처리 관련 파일

### 3.1 add_lunage_changerate.ipynb 
- 기존의 주식 데이터에 로그변동률 추가
- 기존의 주식 데이터에 저장해놓은 월령 값 파일(dt_lunage.csv)을 이용하여 컬럼 추가


## 4. 데이터 분석 파일

### 4.1 foreign_analysis.ipynb
- 해외 주식 시장데이터를 이용한 데이터 분석


## 5. 데이터 검정 파일

### 5.1 Verification.ipynb
- 분석한 데이터를 검정(test)하기 위한 파일