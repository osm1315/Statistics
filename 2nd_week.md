# 통계학 2주차 정규과제
## Statistics_2nd_TIL

### 1부. 데이터 기초체력 기르기
### 06. 확률분포
### 07. 가설검정

## Study Schedule

|주차 | 공부 범위     | 완료 여부 |
|----|----------------|----------|
|1주차| 1부 p.2~56     | ✅      |
|2주차| 1부 p.57~79    | ✅      | 
|3주차| 2부 p.82~120   | 🍽️      | 
|4주차| 2부 p.121~202  | 🍽️      | 
|5주차| 2부 p.203~254  | 🍽️      | 
|6주차| 3부 p.300~356  | 🍽️      | 
|7주차| 3부 p.357~615  | 🍽️      |

<!-- 여기까진 그대로 둬 주세요-->

# 06. 확률분포

```
✅ 학습 목표 :
* 이산확률분포의 종류와 특징을 설명할 수 있다.
* 연속확률분포의 종류와 특징을 설명할 수 있다. 
* 중심극한정리(CLT)의 개념을 이해하고 설명 할 수 있다.
```
![확률분포의 종류에 따른 형태](./images/study2/스크린샷%202025-03-27%20오후%207.18.38.png)
![이산형과 연속형](./images/study2/스크린샷%202025-03-27%20오후%207.19.06.png)

## 6.2. 이산확률분포

### 균등분포
### 이항분포
0과1의 값만 갖는 분포
### 초기하분포
이항분포와 달리 각 시행이 독립적이지 않아 시행마다 확률이 달라짐(비복원추출)
### 포아송분포
일정한 관측공간에서 특정 사건이 발생하는 횟수를 나타내는 분포
- 품질관리, 포험상품 개발 등에 사용
- 일정한 시공간 안에서 발생하는 사건의 횟수
- 성공과 실패,표본의 크기라는 개념이 존재하지 않음
- 조건
    - 발생하는 사건 모두 양의 정수 형태
    - 모든 사건 독립적 발생
    - 해당 시공간에서 사건의 발생 비율이 항상 같음(시공간 두배 -> 사건도 두배)
    - 한번에 둘 이상의 사건이 발생하지 않음
    
## 6.3. 연속확률분포
연속확률분포 
- 확률밀도곡선
- 확률밀도함수 사용

이상확률분포
- 확률질량함수 사용

### 정규분포(가우스분포)
평균을 중심으로 좌우 대칭의 종 모양 형태
- 표준화된 정규분포: 표준정규분포
    - 각기 다른 정규분포간 비교의 동질성을 만들기 위해 변환 

### 지수분포
특정 사건이 발생한 시점으로부터 다음 사건이 발생할때까지의 시간을 확률변숫값으로 하는 분포 
- 시간이 증가할수록 사건이 발생할 확률이 지수적으로 감소
- 포아송분포에서 사건의 횟수를 뜻하는 람다에 역수 -> 하나의 사건이 발생한 후 다음 사건이 발생하기까지의 평균 소요 시간 

## 6.4. 중심극한정리
데이터의 크기가 일정한 양을 넘으면 평균의 분포가 정규분포에 근사하다는 이론

모집단으로부터 무작위로 표본을 여러번 추출한 다음 추출된 각각의 표본들의 평균을 분포로 그려보면 정규분포의 형태를 가짐

- 일반적으로 30개 이상 


# 07. 가설검정

```
✅ 학습 목표 :
* 귀무가설과 대립가설의 개념을 정의하고, 주어진 연구 질문에 적절한 가설을 설정할 수 있다.
* 가설검정의 유의수준과 p값의 개념을 설명하고, p값을 해석하여 귀무가설을 기각할지 여부를 판단할 수 있다.
* 1종 오류와 2종 오류의 차이를 설명하고, 실제 사례에서 어떤 오류를 더 중요하게 고려해야 하는지 판별할 수 있다.
```
![가트너 분석 단계 모델](./images/study2/스크린샷%202025-03-27%20오후%207.32.58.png)

기술적 분석을 제외하고는 모두 가설설정이 필요 

## 귀무가설과 대립가설

귀무가설
- 증명하고자 하는 가설과 반대되는 가설로써 효과와 차이가 없는 가설

대립가설
- 귀무가설이 기각됐을때 대안적으로 채택되는 가설

자신이 옳다고 주장하는 내용과 정반대의 귀무가설을 세우고 잘못된 것임을 밝히기

## 가설검정 절차
![가설검정 절차](./images/study2/스크린샷%202025-03-27%20오후%207.36.00.png)

## 유의수준과 p값
귀무가설에 대한 p값이 유의수준안에 들어오는지에 따라 가설의 기각과 채택을 판별 
![유의수준과 p값](./images/study2/스크린샷%202025-03-27%20오후%207.38.40.png)

- 단측 검정
    - 왼쪽 꼬리 검정
    - 오른쪽 꼬리 검정
- 양측 검정

## 1종오류와 2종오류
1종오류
- 귀무가설이 참임에도 불구하고 귀무가설을 기각하는 오류
- 실제로 효과가 없는데 효과가 있다고 판단


2종오류
- 귀무가설이 거짓임에도 불구하고 귀무가설을 채택하는 오류 
- 실제로 효과가 있는데 효과가 없다고 판단 
- 가설의 검정력이 커질수록 감소 
- 유의수준이 주어지면 표본이 늘어나지 않는 이상 자동으로 결정 

트레이드오프 관계 
![1종오류,2종오류](./images/study2/스크린샷%202025-03-27%20오후%207.43.56.png)


<br>
<br>

# 확인 문제

## 문제 1.

> **🧚Q. 다음 중 귀무가설(H₀)을 기각해야 하는 경우는 언제인가요? 정답을 고르고, 그 이유를 간단히 설명해주세요.**

> **1️⃣ 유의수준(α)이 0.05이고, p값이 0.03일 때   
2️⃣ 유의수준(α)이 0.01이고, p값이 0.02일 때**

```
1번, p값이 유의수준보다 작아야하기 때문
```

