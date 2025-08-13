**SK네트웍스 Family AI 캠프 17기 2차 프로젝트**

---

# 1. 팀소개

###  ` ⭐️ 6조 Guardians of Health ⭐️ `

      
## 👥 팀 멤버 (개인 GitHub)
<br>
<table align="center">
  <tr>
    <td align="center" valign="top" style="padding: 10px;">
      <strong>김민균</strong><br/>
      <img alt="민균" src="https://github.com/user-attachments/assets/d9659893-0432-4261-a73a-97f51efa97db" width="150px" />
</td>
    <td align="center" valign="top" style="padding: 10px;">
      <strong>성기혁</strong><br/>
      <img alt="기혁님" src="https://github.com/user-attachments/assets/d57a5fb6-e897-40d9-9a91-fb3db9615ce2" width="150px" />
    </td>
    <td align="center" valign="top" style="padding: 1px;">
      <strong>이가은</strong><br/>
          <img alt="가은님" src="https://github.com/user-attachments/assets/46cf92d9-55d3-4ab8-b642-bc1b0c0a0fe5" width="150px"/>
<br/>
    </td>
    <td align="center" valign="top" style="padding: 800px;">
      <strong>이재은</strong><br/>
          <img alt="재은님" src="https://github.com/user-attachments/assets/bc902cc2-8379-4857-b2d3-581c90f38277"  width="150px"/>
<br/>
    </td>
    <td align="center" valign="top" style="padding: 500px;">
      <strong>홍문봉</strong><br/>
          <img height="1536" alt="문봉님" src="https://github.com/user-attachments/assets/d3f7a149-181f-472a-be6a-636380dfb4df" width="150px"/>
<br/>
    </td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/alswhitetiger">@alswhitetiger</a></td>
    <td align="center"><a href=https://github.com/venus241004>@venus241004</a></td>
    <td align="center"><a href=https://github.com/Leegaeune>@Leegaeune</a></td>
    <td align="center"><a href=https://github.com/JAEEUN0129>@JAEEUN0129</a></td>
    <td align="center"><a href=https://github.com/Glowcloudy>@Glowcloudy</a></td>
  </tr>
</table>


# 2. 프로젝트개요

## 💡 프로젝트 명

### ` 인공지능 기반 민간 건강보험 이탈 예측 프로젝트  `
<br>

## 🗓️ 프로젝트 기간

### 2025.08.12 ~ 2025.08.13

<br>

## 🌟 프로젝트 소개
#### 본 프로젝트는 **미국 인구조사국(Census Bureau)과 노동통계국(BLS)**이 공동으로 수집하는 **CPS-ASEC(Annual Social and Economic Supplement)** 데이터를 활용하여 **민간 보험(Private Health Insurance) 이탈 여부**를 예측하는 것을 목표로 한다.  
미국 거주자의 인구통계학적 정보(나이, 인종, 교육 수준 등)와 경제·고용 상태, 과거 및 현재 보험 가입 상태를 비교하여 **나이 변화, 소득 변화율** 등의 변화량 특징을 생성하였다.  
이후 범주형 변수 처리, 하이퍼파라미터 최적화(Optuna, GridSearchCV), 교차 검증(Stratified K-Fold), Early Stopping 등의 절차를 거쳐 XGBoost, CatBoost, LightGBM, RandomForest, Logistic Regression 등 다양한 머신러닝 모델을 학습 및 평가하였다.  
최종적으로 ROC AUC 등 여러 성능 지표를 활용하여 모델을 비교하고, 아티팩트 저장을 통해 재사용 가능하도록 구성하였다.
 
<br>

## 🚀 프로젝트 필요성(배경)
 #### 민간 보험 시장은 **고용 상태 변화**, **소득 수준 변화**, **주별 정책 차이**, **재난 발생 여부** 등에 따라 가입과 해지(이탈) 변동이 빈번하다.  
보험사는 이러한 이탈 가능성을 사전에 예측함으로써,  
- **고객 유지율 향상**을 위한 사전 대응  
- **맞춤형 상품 추천** 및 리마케팅  
- **보험 리스크 관리**를 통한 손실 최소화  
등의 전략을 수립할 수 있다.

CPS-ASEC 데이터는 전국 규모의 표본을 기반으로 하여, 인구통계학적 특성과 보험 상태를 함께 분석할 수 있다는 장점이 있어,  
민간 보험사의 **이탈 위험 예측 모델** 개발에 매우 적합한 데이터이다.
 
<br>

## ✅ 프로젝트 목표

- 민간 건강보험 이탈 여부를 예측할 수 있는 인공지능 모델 개발

- 다양한 알고리즘(XGBoost, LGBM, CatBoost, Logistic Regression, RandomForest)의 성능 비교 및 최적 모델 선정

- 주요 영향 요인 분석을 통해 고객 이탈의 핵심 변수 도출

- 보험사 맞춤형 고객 관리 및 마케팅 전략 수립을 위한 데이터 기반 의사결정 지원

<br>

---

## 📦 데이터 출처 목록

| 데이터 이름                           | 파일 형식 / 수집 방법 | 출처 URL |
|--------------------------------------|------------------------|----------|
| IPUMS CPS     |     직접 다운로드 / CSV       | [바로가기](https://cps.ipums.org/cps/index.shtml) |


---

# 3. 기술스택
| 분류 | 기술/도구 |
|---|---|
| 언어 | [![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/) |
| 개발 환경 | [![Jupyter Notebook](https://img.shields.io/badge/Jupyter%20Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/) |
| 라이브러리 | [![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/) [![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/) [![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white)](https://matplotlib.org/) [![Seaborn](https://img.shields.io/badge/Seaborn-4EABC0?style=for-the-badge&logo=seaborn&logoColor=white)](https://seaborn.pydata.org/) [![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/) |
| 협업 툴 | [![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/) |


---

# 4. WBS
![WBS 시각화 이미지](image/wbs_2nd.png)


---
# 5. 데이터 전처리 결과서
## 데이터 전처리 과정

1. **데이터 로드 및 컬럼 분석**
   
      <img width="761" height="216" alt="1 컬럼명" src="https://github.com/user-attachments/assets/701942e6-0f29-4c29-9f67-e3eb14ecaa92" />
   
      YEAR: Survey year, CPSIDP: person record, PHINSUR: Reported covered by private health insurance last year									

      AGE: Age, NCHILD:	Number of own children in household, EARNWEEK: Weekly earnings
				
	  EMPSTAT: Employment status, LABFORCE: Labor force status, HICHAMP: Covered by military health insurance last year, CAIDLY: Covered by Medicaid last year, MARST: Marital status

      RACE: Race, EDUC: Educational attainment recode

 - 상관관계 히트맵: 선택된 수치형 변수 간 상관 분석
   - Pairplot: AGE, NCHILD, ASECWT의 분포와 고용 상태별 관계 시각화
   - Boxplot, Barplot: 인종별/혼인 상태별 평균 나이 비교
     
	<p align="center">
  	<img src="image/p_1.png" width="45%">
	</p>
									  		  <p align='center'>나이에 따른 인구수와 평균주당수입</p>
	<p align="center">
  	<img src="image/p_2.png" width="45%">
	</p>
	       								  	 <p align='center'>결혼 상태에 따른 인구수와 평균 자녀수</p>
	<p align="center">
 	 <img src="image/p_3.png" width="45%">
	</p>
	      								    <p align='center'>교육수준에 따른 평균 주당 분포</p>

SERIAL — 가구 일련번호 (5자리 숫자), PERNUM — 가구 내 개인 번호 (2자리), CPSIDV — 검증된 종단 식별자 (15자리 숫자), ASECWT — ASEC 개인 가중치 (소수 4자리 암시)

추가적인 개인 식별용 변수, YEAR, CPSIDP로 한 사람을 추정할 수 있기 때문에 무의미

HFLAG - 데이터 수집 방식, ASECFLAG - 조사 유형, ASECWTH - 가중치 스케일, Month - 월 정보

위는 분석 대상의 실제 특성과는 직접적인 연관이 없고,
모델 입력 변수로 활용할 경우 의미 있는 설명력이나 예측력을 제공하지 않는 보조·메타 정보이기 때문에 제외
   
   - 주요 분석 컬럼(`YEAR`, `AGE`, `RACE`, `MARST`, `EDUC`, `EARNWEEK`, `PHINSUR` 등)
   - 사용되지 않는 컬럼 (`SERIAL`, `ASECFLAG`, `ASECWTH`, `PERNUM`, `CPSIDV`, `ASECWT`, `Month` 등) 
     
3. **사용할 샘플과 타겟데이터 설정**
   
   <img width="517.5" height="450" alt="2 사용할 샘플과 타겟데이터 설정" src="https://github.com/user-attachments/assets/e71e20bf-fb52-48bd-a090-0089e9fe8029" />

   - PHINSUR 변화를 target으로 설정, YEAR: Survey year, CPSIDP: person record를 Private Key로 사용해 한 사람 추적
   - 샘플 수 확인

4. **변화량으로 피쳐엔지니어링**
   <img width="832" height="122" alt="수치형" src="https://github.com/user-attachments/assets/9a832b92-2fde-43ee-877d-f7e59fe784a4" />

   <img width="465" height="453" alt="EDUC 그룹화" src="https://github.com/user-attachments/assets/b1a2e66a-48ec-4b42-bc89-ab529bf8f989" />

   <img width="376" height="372" alt="RACE 그룹화" src="https://github.com/user-attachments/assets/e278dc11-0cd2-4c5c-a9f9-f805d70fb319" />

   <img width="683" height="65" alt="범주형 변화여부 EDUC RACE빼야함" src="https://github.com/user-attachments/assets/d46d1982-4ef2-4a91-b2dc-2de3adbafcf9" />


   - AGE, NCHILD의 변화량은 절대값으로 사용, EARNWEEK는 퍼센트 변화량으로 사용
   - RACE와 EDUC을 제외한 범주형은 동일하게 변화여부 확인
   - RACE와 EDUC은 모델별로 원핫인코딩, 그룹화 등 진행

---

# 6. 인공지능 학습 결과서

## 모델별 처리 및 학습 과정

### 1. XGBoost
- **특징 생성**: 고객의 과거·현재 데이터를 비교하여 나이 변화, 소득 변화율 등의 변화량 특징 생성  
- **범주형 처리**: EDUC, RACE 등 범주형 변수는 원-핫 인코딩 또는 레이블 인코딩 적용  
- **하이퍼파라미터 탐색**: Optuna를 이용하여 최적 파라미터 탐색  
- **검증 방법**: Stratified K-Fold 교차 검증 + Early Stopping  
- **모델 학습**: 최적 파라미터로 전체 데이터 학습  
- **평가 지표**: ROC AUC  
- **아티팩트 저장**: 모델, 파라미터, 특징 중요도 저장 → 재사용/분석 가능


### 2. CatBoost
- **특징 생성**: 과거·현재 데이터 비교 후 변화량 특징 생성  
- **범주형 처리**: EDUC, RACE 등 범주형 변수는 원-핫 인코딩 없이 `cat_features`로 직접 처리  
- **하이퍼파라미터 탐색**: Optuna로 최적 파라미터 탐색  
- **검증 방법**: Stratified K-Fold 교차 검증 + Early Stopping  
- **모델 학습**: 최적 파라미터로 전체 데이터 학습  
- **평가 지표**: ROC AUC  
- **아티팩트 저장**: 모델, 파라미터, 특징 중요도 저장

### 3. LightGBM
- **특징 생성**: 과거·현재 데이터 비교 후 변화량 특징 생성  
- **범주형 처리**: EDUC, RACE 등 범주형 변수는 원-핫 인코딩 적용  
- **하이퍼파라미터 탐색**: Optuna로 최적 파라미터 탐색  
- **검증 방법**: 교차 검증  
- **모델 학습**: 최적 파라미터로 전체 데이터 학습  
- **평가 지표**: ROC AUC, Precision, Recall, F1-Score  
- **아티팩트 저장**: 모델, 파라미터, 특징 중요도 저장

### 4. RandomForest
- **특징 생성**: 과거·현재 데이터 비교 후 변화량 특징 생성  
- **범주형 처리**: EDUC, RACE 등 범주형 변수는 원-핫 인코딩 또는 레이블 인코딩  
- **하이퍼파라미터 탐색**: Optuna를 이용해 트리 개수, 최대 깊이 등 최적 파라미터 탐색  
- **검증 방법**: Stratified K-Fold 교차 검증  
- **모델 학습**: 최적 파라미터로 전체 데이터 학습  
- **평가 지표**: ROC AUC, Accuracy 등  
- **아티팩트 저장**: 모델, 파라미터, 특징 중요도 저장


### 5. Logistic Regression
- **특징 생성**: 과거·현재 데이터 비교 후 변화량 특징 생성  
- **전처리**: 수치형 변수의 NCHILD, AGE는 절대값 그대로 EARNWEEK는 퍼센트 변화로, 범주형 변수는 원-핫 인코딩 및 그룹화
- **하이퍼파라미터 탐색**: Optuna로 최적 파라미터 탐색  
- **검증 방법**: Stratified K-Fold 교차 검증  
- **모델 학습**: 최적 파라미터로 전체 데이터 학습  
- **평가 지표**: ROC AUC, Accuracy, Precision, Recall  
- **아티팩트 저장**: 모델(계수 포함), 파라미터, 스케일러 저장

### 1. 프로젝트 개요
주제: 머신러닝 기반 민간보험 고객이탈 예측

목적: 고객 이탈 가능성을 사전에 예측하여 마케팅 전략 및 유지 비용 최적화

데이터 개요: 데이터 건수, 피처 개수, 주요 변수 설명   ( -> 좀이따가 넣기 ) 


### 2. 모델링 과정
사용한 모델들: Logistic Regression, XGBoost, CatBoost, Random Forest

버린 모델:

Logistic Regression → 데이터가 선형성이 낮아 성능 저하

성능이 떨어진 CatBoost 모델은 사용 제외

채택한 방법: XGBoost + Random Forest + LGBM 앙상블 합치기


### 3. 평가지표 선택과 이유
Recall을 0.7까지 끌어올림

Precision은 하락했지만, 보험 업종 특성상 실제 이탈 고객을 놓치지 않는 것이 더 중요하다고 판단

이유:

Recall↑ → 실제 이탈 고객을 많이 잡음

Precision↓ → 오탐이 늘어 마케팅 비용 증가 → 저비용 유지 전략 필요


### 4. 인사이트
Recall을 높이기 위해 Precision 일부 포기 → 저비용 마케팅 전략 필요

Precision 보완 방안 → 고객군 세분화, 고위험군 집중 마케팅

TP, FP, FN, TN 기반 가상 비용 산정 → 마케팅 예산 계획 반영 가능

가상 비용 분석 예시: 
| 구분 | 의미       | 단가    | 효과/손실 |
| -- | -------- | ----- | ----- |
| TP | 이탈 방지 성공 | 100만원 | 매출 유지 |
| FP | 불필요 마케팅  | 5만원   | 비용 증가 |
| FN | 이탈 방치    | 100만원 | 매출 손실 |
| TN | 정상 유지    | 0원    | 영향 없음 |


### 5. 추가 분석 계획
TP/TN/FP/FN 기반 가상 비용 계산 후 유의미하면 포함

Feature importance 분석 후 마케팅 타겟 선정 기준 제시

하이퍼파라미터 튜닝으로 모델 최적화 예정

---

# 7. 수행결과(테스트 결과 화면 또는 시연 페이지)

<img width="1142" height="163" alt="8 최종 선정된 다섯가지 모델들과 지표들" src="https://github.com/user-attachments/assets/d1dcf395-56be-423a-a40f-e6712111f036" />
다섯가지 모델 별 평가

<img width="702" height="165" alt="9 catboost의 경우 진행하다보니 precision과 recall의 값이 너무 크게 변화하는 걸 확인해서 버림" src="https://github.com/user-attachments/assets/4c0b018e-2e2e-42e9-8ff3-dabe2b403650" />
CatBoost의 경우 진행하다보니 precision과 recall의 값이 너무 크게 변화하는 걸 확인해서 사용하지 않기로 결정.
logistic regression의 경우 변수간의 관계가 선형적이지 않고 값도 다른 모델에 비해 좋지 않기 때문에 사용하지 않기로 결정.

<img width="1105" height="136" alt="10 RF XGB LGBM + 세가지 합 친SOFTVOTE 로진행" src="https://github.com/user-attachments/assets/916c4652-67c7-4dd9-81ea-328d1668faea" />
최종적으로 선정된 XGB, LGBM, RandomForest를
지표 향상을 위해 softvoting방식으로 사용

<img width="1050" height="750" alt="softvote_confusion_counts_vs_target_recall" src="https://github.com/user-attachments/assets/c20fab20-02f7-4e92-b9ff-1a7535b33157" />
<img width="1050" height="750" alt="softvote_threshold_vs_target_recall" src="https://github.com/user-attachments/assets/cf12e6f6-1e27-408a-ad28-61862685d24c" />

보험 이탈 예측이 주 목적이기 때문에 recall을 가장 중요한 지표라고 판단

<img width="753" height="103" alt="12 recall 이0 7, 0 8인 경우 다 른값들 을비교" src="https://github.com/user-attachments/assets/edea85a2-f4d2-4ba6-93c7-265af3a8b9c8" />
softvote방식에서 recall값에 따른 precision과 confusion matrix값을 확인

recall에 따른 요약
Recall ↑ 0.70 → 0.80로 올리면 놓치는 이탈(FN)이 5,001 → 3,389 (32% 감소)
즉, 더 많은 이탈자를 잡아냄. Precision ↓
0.1400 → 0.1299 (약 7% 감소)
잡아낸 사람 중 실제 이탈자가 아닐 확률이 조금 더 높아짐.
FP(오탐) 증가
73,707 → 91,159 (약 23% 증가)
불필요하게 '이탈'로 분류되는 고객 수가 크게 늘어남.
F1 Score ↓
0.2337 → 0.2236 (약 4% 감소)
Precision 하락 폭이 Recall 상승 효과보다 커서 F1은 떨어짐.
선택 가이드
Recall 0.70 → 균형형. Precision과 F1이 조금 더 높음.
⇒ "이탈자 놓침도 줄이고, 오탐 부담도 너무 크지 않게" 하려면 적합.
Recall 0.80 → 공격형. 놓치는 이탈자를 최소화하려고 FP 증가 감수.
⇒ "이탈을 놓치는 게 훨씬 큰 손실"인 상황(예: 보험 해약 방지 캠페인)이라면 적합.

최종 결론 : 0.7 > 0.8로 늘릴경우 
FP(오탐)가 73,707 → 91,159 (약 23% 증가) 매우 많이 증가하기 때문에 (불필요하게 '이탈'로 분류되는 고객 수가 크게 늘어남.)
이탈을 놓치는 게 훨씬 큰 손실인 특별한 상황이 아닐경우 0.7로 해야함

<img width="241" height="100" alt="13 최종적으로 0 7recall로 설정했을 때 precision과의 관계" src="https://github.com/user-attachments/assets/523ffd52-69bd-4383-931f-99401cddcce6" />
<img width="137" height="47" alt="Confusion Matrix" src="https://github.com/user-attachments/assets/6e720bb7-7028-4047-aa02-a01ab2264f78" />
최종적으로 recall을 0.7로 설정했을 때 precision과의 관계와 confusion matrix

<img width="1200" height="750" alt="per1000_net_profit" src="https://github.com/user-attachments/assets/ec91c9c8-e334-4d34-ae18-b5d21f90085a" />
<img width="1350" height="900" alt="stack_components_by_scenario" src="https://github.com/user-attachments/assets/d1d27e52-0ed5-4228-b1e9-645722b4d70c" />

1. 각 confusion matrix가 보험 이탈 예측에서 갖는 의미
TP 1명당 절감되는 손실 금액
이탈할 고객을 붙잡았을 때 막을 수 있는 평균 손실.
예: 보험 해지로 잃는 고객 LTV(고객 생애 가치)가 평균 200만원이면, TP 1명당 +200만원 효과.

FP 1명당 대응 비용
오탐 고객에게 제공한 혜택·마케팅·상담 비용.
예: 전화 상담·혜택 제공에 평균 5만원.

FN 1명당 손실 금액
실제 이탈했는데 놓친 고객의 손실 = TP 절감액과 같은 수치로 볼 수 있음.
예: 200만원.

현재 모델의 혼동행렬(Confusion Matrix)
TP, FP, TN, FN을 이용 손익 계산

2. 계산 방식
손익 = (TP × 절감액) - (FP × 대응비) - (FN × 손실액)

Recall을 높이면 TP가 늘고 FN이 줄지만, FP도 늘어납니다.

Precision을 높이면 FP가 줄지만, FN이 늘어납니다.

3. 왜 상황 따라 다른가?
고객당 LTV가 높은 보험(고액 종신보험)일수록 Recall 극대화 전략이 압도적으로 유리.

반대로 대응 비용이 매우 높은 경우(예: 대면 고급 상담, 고가의 혜택)는 FP가 늘면 부담이 커짐.

따라서 회사의 단가 구조를 알아야 정확한 최적 threshold를 찾을 수 있음.

SoftVote(Recall=0.7) 결과로,
TP·FP·FN을 이용해서 단가를 가정한 2~3가지 시나리오별 손익 비교표
threshold 선택에 훨씬 설득력이 붙어요.

1. TP 절감액 (고객 LTV)
200만 원: 국내 장기보험(예: 자동차, 건강보험)에서 중형급 고객의 평균 잔여 LTV 수준과 비슷
예: 월 10만 원 보험료 × 잔여기간 20개월 = 200만 원
120만 원: 단기 계약이거나 보험료가 낮은 상품군에 해당
300만 원: 고액 장기보험(LTV 높은 고객), 특히 종신보험·고액 건강보험의 경우 현실적

2. FP 1명당 대응 비용
5만 원: 전화 상담 + 소액 혜택(상품권, 포인트, 할인 등) 수준
8만 원: 콜센터 + 맞춤형 혜택 + 추가 마케팅 비용이 포함된 경우
3만 원: 자동화 메시지·저비용 리마케팅 정도일 때 현실적

3. FN 손실액
대부분 TP 절감액과 동일하게 잡는 게 일반적
이유: 놓친 고객(FN)은 그대로 해지하므로 LTV 손실 = TP로 막을 수 있었던 금액과 같음

결론적으로,

A (200만 / 5만 / 200만) → 현실적
B (120만 / 8만 / 120만) → 저가 보험·FP 대응 비용 큰 경우, 충분히 현실적
C (300만 / 3만 / 300만) → 고가 보험·대응비 낮은 경우, 특히 VIP 고객군 타겟 시 적합


LTV(고객 생애 가치, Lifetime Value)란?
정의: 고객이 우리 회사와 관계를 유지하는 동안 가져다 줄 총이익의 현재가치.
보험에서는 LTV가 특히 크다. 왜냐하면:
장기간 계약(5~20년) 동안 매년 보험료를 납부.
초기 가입 시점에 마케팅·설계사 비용이 크지만, 유지 시 추가비용 적음.
계약 유지가 곧 안정적인 현금 흐름을 보장.
LTV가 높다는 말은:
고객 한 명이 평생(또는 계약 기간) 동안 회사에 기여하는 이익이 크다는 뜻.
고액·장기보험일수록 LTV가 높아짐.
이런 경우 **Recall(재가입·유지율)**을 높이는 전략이 훨씬 수익성 있음.

## 한계점 (Limitations)

### 1. 데이터 구조상의 한계
- CPS-ASEC 자료는 **연 1회 스냅샷 데이터**이므로,  
  - 연중 몇 번이나 보험 상태가 변경되었는지  
  - 무보험 기간이 얼마나 지속되었는지  
  를 파악할 수 없음.
- 시점 간격이 불규칙하며, 동일 개인이 2개 이상의 시점에 나타날 경우 이상치처럼 보이는 사례 발생.
- 관측 시점이 제한되어 **중간 churn(이탈) 발생 시점**을 정확히 추적하기 어려움.


### 2. 변수 및 범위 제한
- **주별 민간보험사 수, 보험 상품 개수** 등의 시장 구조 정보가 반영되지 않음.
- **재난별 보험료 인상률**(예: 플로리다 허리케인, 중부 토네이도 등 상습 재난지역 요율 변화) 고려 불가.
- **고용자보험 vs 마켓플레이스 보험 구분 불가** → 민간보험 이탈의 성격을 명확히 구분하기 어려움.
- 연방정부 지원 사보험(보조금 등)은 민간보험으로 처리되어, 민간↔공보험 전환 분석 시 혼동 가능.
- 공보험 변수에 Medicaid·군보험만 포함되어, Medicare(노인), CHIP(아동) 등이 제외됨 → 전환 분류 오류 가능.


### 3. 데이터 품질 문제
- **PHINSUR / CAIDLY / HICHAMP** 등 주요 보험 여부 변수는 **자가보고(self-report)**이므로,  
  - 기억 오류  
  - 응답 오류  
  가능성 존재.
- CPS-ASEC 특유의 **Seam Bias**(연도 경계에서 상태 변화 과대/과소 추정)로 인해 전환 횟수 추정이 왜곡될 수 있음.
- 가구·가족 구조 변화(피부양 전환, 가구 재구성 등)를 정밀 추적하기 어려움.


### 4. 분석 모델 한계
- 일부 머신러닝 모델(CatBoost)에서 **특정 변수 값의 분포가 비정상적으로 튀는 현상**이 발견되어 모델에서 제외하였으나,  
  원인 분석이 완전히 이루어지지 않음.
- 잠재 이탈 고객(예: 보험 유지 중이지만 곧 해지 가능성이 높은 고객) 식별에는 한계가 있음.


### 5. 현재 결과로 말할 수 없는 것
- **이탈 시점의 정확한 원인** (몇 월에 왜 해지했는지)  
- 중간에 몇 번 상태가 변경되었는지, 무보험 기간의 길이  
- 고용자보험과 마켓플레이스 보험 간 차이  
- 보험료 보조금·프리미엄 변동, 주별 정책 변화의 인과효과





---

# 8. 한 줄 회고

김민균: 많은 양의 데이터를 확인 하고 그걸 전처리와 이상치등을 제거 하는데 많은 시간이 걸린다는  것을 알았고 그래프를 각각 그렸을 때 그래프의 모양이 좋지 않았고 그래프를 합치고 하는 과정이 너무 나도 힘들다는 것을 알게 되었습니다. 또한 머신러닝을 돌렸을 때에도 점수가 이상하게 나와서 그것을 다시 정비하는 것에 어려움을 느끼게 되어서 다음 부터는 더욱더 많은 것을 습득하여서 완벽하게 하고 싶습니다.


성기혁: 주제에 알맞은 데이터를 구하는 과정과, 정제되지 않은 데이터를 사용해볼 수 있었다. 어떤 모델을 사용해야하는지, 또 모델의 방식에 따라 어떻게 데이터를 넣어야하는지 확인할 수 있었다.


이가은: 전처리 전·후 데이터의 비교 시각화를 통해 데이터 품질 개선 효과를 확인하였으며, 분석의 신뢰성을 높였습니다. 향후에는 변수 선정과 이상치 기준 설정에 더 체계적인 근거를 마련하고, 하이퍼파라미터 최적화 및 추가 데이터 활용을 통해 모델의 예측력을 향상시키고자 합니다.


이재은: 해외에서 수집한, 구조가 정제되지 않고 생소한 칼럼을 포함한 데이터셋을 전처리하고 EDA를 수행하는 과정이 쉽지 않았다. 데이터 구조를 이해하고 불필요하거나 불명확한 정보를 정리하는 데 많은 시간이 소요되었지만, 다양한 형태의 데이터를 다루는 역량을 쌓을 수 있었다는 점에서 의미 있는 경험이었다.


홍문봉: 데이터 자체 크기가 이전 프로젝트보다 크고, 비 정제된 데이터로 인해 데이터 전처리와 이탈률 관련 그래프를 그림에 있어서 여러 변수들간에 상관관계를 생각하며 그리기에는 너무 복잡성이 높았습니다. 이로 인해 상관관계간에 그래프를 나타냄으로써 데이터이해의 도움이 되었습니다.




