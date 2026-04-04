# 데이터분석 5주차 정규과제

📌데이터분석 정규과제는 매주 정해진 분량의 『*혼자 공부하는 데이터 분석 with 파이썬*』 을 읽고 학습하는 것입니다. 이번 주는 아래의 **DataAnalysis_5th_TIL**에 나열된 분량을 읽고 공부하시면 됩니다.

아래의 문제를 풀어보며 학습 내용을 점검하세요. 문제를 해결하는 과정에서 개념을 스스로 정리하고, 필요한 경우 제시된 강의를 참고하여 보완하는 것이 좋습니다.

<!-- 강의 링크는 아래와 같습니다.
https://www.youtube.com/watch?v=ho0LZ6GWhtc&list=PLVsNizTWUw7FGzSRCkQrPEEe-ljVXgS7k&index=10
https://www.youtube.com/watch?v=deYY4xHsI0o&list=PLVsNizTWUw7FGzSRCkQrPEEe-ljVXgS7k&index=11
-->


## DataAnalysis_5th_TIL

### 5장 데이터 시각화하기
#### 01. 맷플롯립 기본 요소 알아보기
#### 02. 선 그래프와 막대 그래프 그리기


## Study Schedule

| 주차  | 공부 범위     | 완료 여부 |
| ----- | ------------- | --------- |
| 1주차 | p.24~81    | ✅         |
| 2주차 | p.84~151   | ✅         |
| 3주차 | p.154~219  | ✅         |
| 4주차 | p.222~279 | ✅         |
| 5주차 | p.282~325 | ✅         |
| 6주차 | p.328~379 | 🍽️         |
| 7주차 | p.382~430 | 🍽️         |

<br>

<!-- 여기까진 그대로 둬 주세요-->


# 1️⃣ 개념 정리 

## 01. 맷플롯립 기본 요소 알아보기

- 피겨

:맷플롯립의 그래프 요소를 모두 담고 있는 최상위 객체.
맷플롯립의 그래프를 그릴 때 자동으로 피겨가 생성되고, 그래프가 그려진 후 삭제됨.
명시적으로 피겨 객체를 만들면 다양한 옵션을 제어할 수 있음.

- rcParams

:맷플롯립 그래프의 기본값을 관리하는 객체.
객체에 담긴 값만 출력하는 것 뿐만 아니라 새로운 값으로 바꿀 수도 있음.
이후에 그려지는 모든 그래프에 바뀐 설정이 적용됨.

- 축

:그래프에서 데이터 좌표를 표현함.
2차원 그래프는 2개의 축을 가지며 3차원 그래프는 3개의 축을 가짐.
맷플롯립에서는 Axis 클래스로 축 객체를 다룸.
두 개 이상의 Axis 객체로 이루어진 Axes 객체는 그래프가 그려질 영역을 표현함.

- 마커

:그래프에 데이터 포인트를 표시하는 방법.
기본 마커는 동그라미를 나타내는 o임.

- 서브플롯

:피겨 안에 포함된 그래프 영역.
보통 Axes 객체를 말함.
subplots()함수로 여러개의 서브플롯과 서브플롯을 포함하는 피겨를 만들 수 있음.

## 02. 선 그래프와 막대 그래프 그리기

- 선 그래프
각 데이터 포인트를 직선으로 연결한 그래프.
- 막대 그래프
데이터 포인트의 크기를 막대 높이로 나타낸 그래프.

~~~
matplotlib.pyplot.annotate(): 지정한 좌표에 텍스트를 출력
matplotlib.pyplot.bar(): 세로 막대 그래프를 그림
matplotlib.pyplot.barh(): 가로 막대 그래프를 그림
matplotlib.pyplot.imread(): 이미지 파일을 넘파이 배열로 읽어들임
matplotlib.pyplot.imshow(): 이미지를 출력함
matplotlib.pyplot.imsave(): 넘파이 배열을 이미지 파일로 저장함
matplotlib.pyplot.savefig(): 그래프를 이미지로 저장함
~~~

# 2️⃣ 수행 인증

<img width="1710" height="1069" alt="image" src="https://github.com/user-attachments/assets/14a46ddb-69ea-4f28-a159-c9ac307c0659" />
<img width="1710" height="1069" alt="image" src="https://github.com/user-attachments/assets/f1bdde80-4efb-4970-8a8f-67249ed0c561" />
<img width="1710" height="1069" alt="image" src="https://github.com/user-attachments/assets/837f89df-5217-433b-b76b-cacd4488fd0f" />
<img width="1710" height="1069" alt="image" src="https://github.com/user-attachments/assets/c1adbf5a-2199-469c-9bd4-82259959b027" />




<br>
<br>

# 3️⃣ 확인 문제

## 문제 1.

> **🧚Q. 다음 데이터를 이용하여 matplotlib으로 선그래프를 그리는 코드를 작성해주세요.**
- x = [1, 2, 3, 4, 5]
- y = [2, 4, 6, 8, 10]
> 조건은 아래와 같습니다.
```
1️⃣ 제목은 "Linear Trend"로 설정해주세요.
2️⃣ x축 이름은 "X values"로 설정해주세요.
3️⃣ y축 이름은 "Y values"로 설정해주세요.
4️⃣ 마커(marker)를 포함하여 선그래프를 그려주세요.
```

```
import matplotlib.pyplot as plt

x=[1,2,3,4,5]
y=[2,4,6,8,10]

plt.plot(x,y,marker='o')

plt.title("Linear Trend")
plt.xlabel("X values")
plt.ylabel("Y values")

plt.show()
```



### 🎉 수고하셨습니다.
