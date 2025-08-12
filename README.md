**SK네트웍스 Family AI 캠프 17기 2차 프로젝트**

---

# 1. 팀소개

###  ` ⭐️ 6조 Guardians of Health ⭐️ `

      
## 👥 팀 멤버 (개인 GitHub)

| 이름  | GitHub 계정                                    |
| ----- | ---------------------------------------------- |
| 김민균 | [@alswhitetiger](https://github.com/alswhitetiger)   |
| 성기혁 | [@venus241004](https://github.com/venus241004) |
| 이가은 | [@Leegaeune](https://github.com/Leegaeune)   |
| 이재은 | [@JAEEUN0129](https://github.com/JAEEUN0129)   |
| 홍문봉 | [@Glowcloudy](https://github.com/Glowcloudy)   |

<br>

---

# 2. 프로젝트개요

## 💡 프로젝트 명

### ` 인공지능 기반 민간 건강보험 이탈 예측 프로젝트  `
<br>

## 🗓️ 프로젝트 기간

### 2025.08.12 ~ 2025.08.13

<br>

## 🌟 프로젝트 소개
#### `본 프로젝트는 미국 CPS(Annual Social and Economic Supplement) 데이터를 활용하여, 고객의 인구통계학적 정보(연령, 교육 수준, 결혼 여부, 고용 상태 등)와 경제적 지표(주당 소득, 노동시장 참여 여부, 군·공공·민간 보험 가입 여부)를 종합적으로 분석하여 민간 건강보험 이탈 여부를 예측하는 인공지능 모델을 개발하는 것을 목표로 합니다.<br>데이터 전처리 및 EDA 과정을 통해 유의미한 변수들을 추출하고, CatBoost, Logistic Regression, XGBoost, Elastic Net 등 다양한 머신러닝 알고리즘을 적용하여 성능을 비교·평가했습니다.`
 
<br>

## 🚀 프로젝트 필요성(배경)
 #### 민간 건강보험 시장에서는 고객의 이탈을 사전에 예측하고 이를 방지하는 전략이 중요한 과제로 부각되고 있습니다. 특히 소득 변화, 직업 상태, 공공보험 가입 여부 등의 요인이 민간보험 유지 여부에 직접적인 영향을 미칠 수 있습니다. 본 프로젝트는 이러한 다양한 속성 데이터를 기반으로 고객의 이탈 가능성을 예측함으로써, 보험사들이 보다 효율적인 리텐션(고객 유지) 전략을 수립할 수 있도록 지원합니다.
 
<br>

## ✅ 프로젝트 목표

- 민간 건강보험 이탈 여부를 예측할 수 있는 인공지능 모델 개발

- 다양한 알고리즘(CatBoost, Logistic Regression, XGBoost, Elastic Net)의 성능 비교 및 최적 모델 선정

- 주요 영향 요인 분석을 통해 고객 이탈의 핵심 변수 도출

- 보험사 맞춤형 고객 관리 및 마케팅 전략 수립을 위한 데이터 기반 의사결정 지원

<br>

---

## 📦 데이터 출처 목록

| 데이터 이름                           | 파일 형식 / 수집 방법 | 출처 URL |
|--------------------------------------|------------------------|----------|
| IPUMS CPS     |             | [바로가기](https://cps.ipums.org/cps/index.shtml) |
| 지역, 월별 차량 등록 현황 (통계)      | 직접 다운로드 / CSV    | [바로가기](https://stat.molit.go.kr/portal/cate/statView.do?hRsId=58&hFormId=5498&hSelectId=1244&hPoint=00&hAppr=1&hDivEng=&oFileName=&rFileName=&midpath=&sFormId=5498&sStyleNum=562&settingRadio=xlsx) |
| 현대자동차 홈페이지 FAQ               | Selenium 라이브러리     | [바로가기](https://www.hyundai.co.kr/main/mainRecommend) |
| 포드자동차 홈페이지 FAQ              | Selenium 라이브러리     | [바로가기](https://www.frontierford.com/faq/ford-electric-lineup.htm?srsltid=AfmBOooBqN_a6WwQzWidD_fI7v7RV0FVtLepfbByBUO7VGRhPYe_fvdT) |
| 전기/하이브리드 자동차 종합정보 신규등록정보 (2024)   | API 수집 / MYSQL               | [바로가기](https://www.stgdata.co.kr/data/15059401/openapi.do?recommendDataYn=Y) |

---

# 3. 기술스택
<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Jupyter_Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white">
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white">
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white">
  <img src="https://img.shields.io/badge/Matplotlib-CB3B27?style=for-the-badge&logo=matplotlib&logoColor=white">
  <img src="https://img.shields.io/badge/Seaborn-98FB98?style=for-the-badge&logo=seaborn&logoColor=white">
  <img src="https://img.shields.io/badge/Scikit-learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white">
</p>


---

# 4. WBS
![WBS 시각화 이미지](image/wbs_2nd.png)


---
# 5. 전처리 결과서 
## 데이터 전처리 과정
1. **데이터 로드**
   ![전처리 코드 이미지](image/pre1.png)
   - 원본 데이터에서 필요한 컬럼만 선택 로드 (usecols 사용) -> 불필요한 변수는 초기에 제외하여 메모리 절약 및 분석 속도 향상
   - 주요 분석 컬럼(`YEAR`, `AGE`, `RACE`, `MARST`, `EDUC`, `EARNWEEK`, `PHINSUR` 등)만 추출
3. **결측치 처리**
   ![전처리 코드 이미지](image/pre2.png)
   - RACE, MARST, EMPSTAT를 코드형으로 변환하여 RACE_code, MARST_code, EMPSTAT_code 생성
   - 범주형 → 수치형 변환은 상관관계 분석, 모델 입력에 활용 가능

5. **이상치 처리**
   ![전처리 코드 이미지](image/pre3.png)
   - 

7. **카테고리 변수 인코딩**
   ![전처리 코드 이미지](image/pre4.png)
   - 
   - 

9. **데이터 샘플링**
   ![전처리 코드 이미지](image/pre5.png)
   - EDA 시 가독성 향상을 위해 10% 무작위 샘플링

11. **데이터 저장**
   - 전처리 완료 데이터를 CSV로 저장 (`insurance_clean.csv`)


# 6. EDA(데이터 전처리 결과서)

![EDA 시각화 이미지](image/1.png)
![EDA 시각화 이미지](image/2.png)

---

# 7. 수행결과(시연 페이지)
![수행결과 이미지](image/stm1.png)
![수행결과 이미지](image/stm2.png)
![수행결과 이미지](image/stm3.png)
![수행결과 이미지](image/stm4.png)
![수행결과 이미지](image/stm5.png)
![수행결과 이미지](image/stm6.png)
![수행결과 이미지](image/stm7.png)
![수행결과 이미지](image/stm8.png)
![수행결과 이미지](image/stm9.png)
![수행결과 이미지](image/stm10.png)
![수행결과 이미지](image/stm11.png)



---

# 8. 한 줄 회고

김민균:


성기혁:


이가은:


이재은:


홍문봉:




