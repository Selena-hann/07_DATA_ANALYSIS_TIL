# 데이터분석 6주차 정규과제

📌데이터분석 정규과제는 매주 정해진 분량의 『*혼자 공부하는 데이터 분석 with 파이썬*』 을 읽고 학습하는 것입니다. 이번 주는 아래의 **DataAnalysis_6th_TIL**에 나열된 분량을 읽고 공부하시면 됩니다.

아래의 문제를 풀어보며 학습 내용을 점검하세요. 문제를 해결하는 과정에서 개념을 스스로 정리하고, 필요한 경우 제시된 강의를 참고하여 보완하는 것이 좋습니다.

<!-- 강의 링크는 아래와 같습니다.
https://www.youtube.com/watch?v=XD65UhBMOiI&list=PLVsNizTWUw7FGzSRCkQrPEEe-ljVXgS7k&index=12
https://www.youtube.com/watch?v=NTQ5NXelOfw&list=PLVsNizTWUw7FGzSRCkQrPEEe-ljVXgS7k&index=13
-->


## DataAnalysis_6th_TIL

### 6장 복잡한 데이터 표현하기
#### 01. 객체지향 API로 그래프 꾸미기
#### 02. 맷플롯립의 고급 기능 배우기


## Study Schedule

| 주차  | 공부 범위     | 완료 여부 |
| ----- | ------------- | --------- |
| 1주차 | p.24~81    | ✅         |
| 2주차 | p.84~151   | ✅         |
| 3주차 | p.154~219  | ✅         |
| 4주차 | p.222~279 | ✅         |
| 5주차 | p.282~325 | ✅         |
| 6주차 | p.328~379 | ✅         |
| 7주차 | p.382~430 | 🍽️         |

<br>

<!-- 여기까진 그대로 둬 주세요-->


# 1️⃣ 개념 정리 

## 01. 객체지향 API로 그래프 꾸미기

- 객체지향 API: 명시적으로 피겨 객체와 서브플롯 객체를 만들고 이 객체의 메서드를 사용하여 맷플롯립 그래프를 그리는 방법
- 컬러맵: 맷플롯립에서 그래프를 그리는 데 사용하기 위해 사전에 정의한 색상 리스트. 기본 컬러맵은 진녹색에서 노란색으로 변화하는 viridis이다. 파란색에서 노란색에서 빨간색으로 변하는 jet 컬러맵도 많이 사용한다.
- 컬러 막대: 데이터 포인트에 적용된 색상의 범위를 보여주는 막대이다. 보통 그래프의 오른쪽에 나란히 놓이며 색깔이 의미하는 실제 값을 참조하는데 사용된다.

~~~
matplotlib.pyplot.rc(): rcParams 객체의 값을 설정함
Figure.colorbar(): 그래프에 컬러 막대를 추가함
~~~

## 02. 맷플롯립의 고급 기능 배우기

- 범례: 그래프에 그려진 데이터의 이름과 색상을 요약한 표
- 피벗 테이블: 테이블 형태의 데이터를 평균, 합 등의 방식으로 집계하여 만든 요약표
- 스택 영역 그래프: 여러 개의 선 그래프를 y축 방향으로 쌓은 그래프. 선 아래로 색상이 채워진 영역 형태로 표현됨. 마찬가지로 여러 개의 막대 그래프를 y축 방향으로 쌓으면 스택 막대 그래프가 됨. 막대 위에 막대가 누적되듯이 표현됨.
- 원 그래프: 데이터의 비율을 부채꼴 모양으로 나타낸 그래프. 다만 그래프에 비율이 표시되어 있지 않으면 크기를 비교하기 어려우므로 autopct 매개변수를 사용하여 명확하게 비율을 표시해 주는 것이 좋음

|함수.매서드|기능|
|---------|---|
|Axes.legend()|그래프에 범례를 추가함|
|Axes.set_xlim()|x축의 출력 범위를 지정함|
|DataFrame.pivot_table()|피벗 테이블 기능을 제공함|
|Axes.stackplot()|스택 영역 그래프를 그림|
|DataFrame.plot.area()|스택 영역 그래프를 그림|
|DataFrame.plot.bar()|막대 그래프를 그림|
|DataFrame.cumsum()|행이나 열 방향으로 누적 합을 계산함|
|Axes.pie()|원 그래프를 그림|

# 2️⃣ 수행 인증

<img width="1710" height="1069" alt="image" src="https://github.com/user-attachments/assets/d51b8961-0f10-4769-a966-b48b7ea22095" />
<img width="1710" height="1069" alt="image" src="https://github.com/user-attachments/assets/9402db15-3742-4a7d-a9b7-54c061561f27" />
<img width="1710" height="1069" alt="image" src="https://github.com/user-attachments/assets/bb29de0d-8dee-44b6-b55a-b91a3298f62e" />
<img width="1710" height="1069" alt="image" src="https://github.com/user-attachments/assets/13050e41-3ae7-413b-8303-0b10570ffa45" />
<img width="1710" height="1069" alt="image" src="https://github.com/user-attachments/assets/ae136e81-2a11-40a4-bc84-1de66e611b57" />
<img width="1710" height="1069" alt="image" src="https://github.com/user-attachments/assets/ceeca413-57b5-47f0-973c-a4689741a665" />



<br>
<br>

# 3️⃣ 확인 문제

## 문제 1.

> **🧚Q. 이번 주차에는 확인문제 대신 그래프 그리기 실습을 진행합니다.
4주차에서 사용했던 캐글 데이터셋을 활용하여, 다양한 요소를 포함한 복잡한 그래프를 직접 작성해주세요.**

```
여기에 코랩 링크를 첨부해주세요!
(제출 전, 코랩의 공유 설정을 ‘링크가 있는 모든 사용자가 보기 가능’으로 변경했는지 반드시 확인해주세요.)
```



### 🎉 수고하셨습니다.
