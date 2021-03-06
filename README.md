

# TEAM 만원대왕 데이터 분석💸

[깃헙 주소](https://github.com/SuHae-Bae/Sejong-house)

### 

### 👤contributor

- [김지우](https://github.com/g-wooo)
- [배수혜](https://github.com/SuHae-Bae)

------

## TEAM 만원대왕

- COMPAS의 (세종시)주택 시장 특성분석 대회에 참여하기 위해 진행한 데이터 분석 프로젝트입니다.
- 세종시의 아파트 가격은 2020년 10개월간 39.22% 증가하여 전국 최고 수준의 집값 상승률을 보여주었고, 전셋값 또한 동일기간내 41.45%의 상승을 기록하며 가장 높은 상승률을 나타냈습니다. 이 상황에서, 세종시의 대대적인 주택 시장 실태 조사 요구가 증가하고 있습니다.
- 데이터 분석을 진행하고, 세종시 주택 시장 특성을 쉽고 명확히 보이도록 시각화 모델을 제시하는 것을 최종 목표로 합니다.

### 분석문항

📎 [**분석1.** 연도별 인구수와 주택 매매가(평균)의 상관관계](#분석1-연도별-인구수와-주택-매매가(평균)의-상관관계)

📎 [**분석2.** 읍면동 별 인구수와 주택 매매가(평균)의 상관관계](#분석2-읍면동-별-인구수와-주택-매매가(평균)의-상관관계)

📎 [**분석3.** 건물 유형별 거래건수 비교](#분석3-건물-유형별-거래건수-비교)

📎 [**분석4.** 세종시 연도별 총 인구수 변화와 업종별 상권 개수](#분석4-세종시-연도별-총-인구수-변화와-업종별-상권-개수)

📎 [**분석5.** QGIS 시각화 ](#분석5-QGIS-시각화)

📎 [**분석5-1.** 아파트, 연립다세대 매매거래 중 고가의 매매거래가 발생한 지역과 그 외 지역의 평균 매매가 비교 ](#분석5-1-아파트,-연립다세대-매매거래-중-고가의-매매거래가-발생한-지역과-그-외-지역의-평균-매매가-비교)

------

## 분석1. 연도별 인구수와 주택 매매가(평균)의 상관관계

👤contributor : [김지우](https://github.com/g-wooo)

- 연도별 인구수가 주택 매매가(평균)에 어떤 영향을 미치는지 알아보기 위한 분석을 진행했습니다.

### 📋활용한 데이터

- 세종시 아파트 매매 실거래가
- 세종시 연립다세대 매매 실거래가
- 세종시 단독다가구 매매 실거래가
- 세종시 오피스텔 매매 실거래가

- 세종시 연령별 인구현황
  - 출처: COMPAS 및 세종시 제공

### ✏️분석결과

1. **아파트와 연립다세대**

![image](https://user-images.githubusercontent.com/33304926/147364543-c253a841-162c-48aa-b7f9-ea3ce53cb559.png)

- 연도별 인구수는 모두 선형으로 증가하였습니다.
- 아파트 매매가의 상승세와 인구수 증가 추세가 일치함을 발견할 수 있었습니다.
- 연립다세대 매매가는 2019년, 전년대비 급격히 상승 후 2020년, 인구수 증가 추세와 비일치하는 것으로 나타났습니다.



**2. 단독다가구와 오피스텔**

![image](https://user-images.githubusercontent.com/33304926/147364430-2ff0f2f0-f3f7-4913-87c7-18919d1931d1.png)

- 마찬가지로 연도별 인구수는 둘 모두 선형으로 증가하였습니다.
- 단독다가구 매매가는 2018년 기점으로 하락세를 보였으며, 인구수 증가 추세와 비일치하였습니다.
- 오피스텔 매매가는 2019년, 전년대비 급격히 하락하였고 2020년에 인구수가 증가하자, 매매가도 약간의 상승세를 보였습니다.



**3. 연도별 인구수와 주택 매매가의 상관관계**

- 연도별 인구수(res), 아파트(apt), 연립다세대(multi), 단독다가구(single), 오피스텔(office) 매매가의 상관관계를 구하였습니다.

<img src="https://user-images.githubusercontent.com/33304926/147365045-ffc6c036-69d6-4b0a-9052-487f0378985e.png " width="600" height="370">

- 상관계수가 0.6 이상인 변수간의 관계를 유의미하다고 정의하였으며, 인구수와 주택 매매가, 주택 매매가간의 관계만 고려하였습니다.

<img src="https://user-images.githubusercontent.com/33304926/147365187-a98ed91b-67e6-4dcd-aa05-59dc99e26a3f.png" width="500" height="370">

------

## 분석2. 읍면동 별 인구수와 주택 매매가(평균)의 상관관계

👤contributor : [김지우](https://github.com/g-wooo)

- 읍면동 별 인구수가 주택 매매가(평균)에 어떤 영향을 미치는지 알아보기 위한 분석을 진행했습니다.

### 📋활용한 데이터

- 세종시 아파트 매매 실거래가
- 세종시 연립다세대 매매 실거래가
- 세종시 단독다가구 매매 실거래가
- 세종시 오피스텔 매매 실거래가

- 세종시 연령별 인구현황
  - 출처: COMPAS 및 세종시 제공

### ✏️분석결과

**1. 읍면동 별 인구수와 아파트 매매가의 상관관계**

![image](https://user-images.githubusercontent.com/33304926/147365390-d4d695da-85ac-4c26-825c-16be608da424.png)

- 읍면동 별 인구수와 아파트 매매가는 비슷한 흐름을 보였습니다.
- 하지만, **대평동**은 인<u>구수가 상대적으로 적은데도</u> 아파트 매매가의 평균이 "8억 1754만원"으로 높았습니다.

![image](https://user-images.githubusercontent.com/33304926/147365511-4475df7b-dc3f-4dd5-8842-97952925c832.png)

- 거래건수 또한 2020년에 <u>150건</u>으로 상승하여, 이유를 알아보기 위해 이후 QGIS로 주변 상권을 분석해보았습니다.

**2. 읍면동 별 인구수와 연립다세대 매매가의 상관관계**

![image](https://user-images.githubusercontent.com/33304926/147365553-b43142bf-fcc7-4712-8afe-61053fcc4fbd.png)

- 읍면동 별 인구수와 연립다세대 매매가는 비슷한 흐름을 보였습니다.
- 하지만, **장군면**은 <u>인구수가 상대적으로 적은데도</u> 연립다세대 매매가의 평균이 "1억 3천만원"으로 높았습니다.

![image](https://user-images.githubusercontent.com/33304926/147365656-b902da26-7ab3-4e43-9083-1e25a394a55b.png)

- 장군면의 매매가 평균 또한 18, 19, 20년 모두 세종특별시 전체의 매매가 평균보다 높아, 이유를 알아보기 위해 이후 QGIS로 주변 상권을 분석해보았습니다.

**3. 읍면동 별 인구수와 단독다가구 매매가의 상관관계**

![image](https://user-images.githubusercontent.com/33304926/147365704-56c249c9-7347-4fe4-bf38-2483d0c8d7d5.png)

- 읍면동 별 인구수와 단독다가구 매매가는 비슷한 흐름을 보였습니다.
- 하지만, **도담동, 아름동, 고운동**은 <u>타 지역에 비해</u> 연립다세대 매매가의 평균이 모두 "9천만원 이상"으로 높았습니다.

![image](https://user-images.githubusercontent.com/33304926/147365774-eb7bfa46-6082-44ec-94e7-3a5d869db221.png)

- 하지만 타 지역에 비해 도담동, 아름동, 고운동에서 <u>단독다가구의 거래 횟수가 현저히 적어</u>, 이유를 알아보기 위해 이후 QGIS로 세 지역의 특성을 시각화해보았습니다.

**4. 읍면동 별 인구수와 오피스텔 매매가의 상관관계**

![image](https://user-images.githubusercontent.com/33304926/147365805-ce1a7764-737e-4707-909f-c244b37c5f00.png)

- 읍면동 별 인구수와 오피스텔 매매가는 비슷한 흐름을 보였습니다.
- 도담동은 인구수와 매매가가 비례하는 반면, 부강면은 인구수가 적음에도 오피스텔 거래가가 높았습니다.
- 하지만, 세종시의 오피스텔 거래량이 매우 적기 때문에 <u>거래가 있었던 지역만의 매매건수</u>를 살펴보았습니다.

![image](https://user-images.githubusercontent.com/33304926/147365821-03af7abf-c66c-4337-a5a2-2da41f2aebbb.png)

- **조치원읍, 부강면, 도담동**에서만 거래가 발생하였습니다.
- 특히, **도담동**에서는 꾸준한 거래가 있어왔음을 확인하였습니다.
- 이에 이유를 알아보기 위해 QGIS로 세 지역의 특성을 분석하였습니다.

------

## 분석3. 건물 유형별 거래건수 비교

👤contributor : [배수혜](https://github.com/SuHae-Bae)

- 건물 유형(아파트, 연립다세대, 단독다가구, 오피스텔)별 거래건수를 python으로 그래프를 만들어 비교해 보았습니다.

### 📋활용한 데이터

- 세종시 아파트 매매 실거래가
- 세종시 연립다세대 매매 실거래가
- 세종시 단독다가구 매매 실거래가
- 세종시 오피스텔 매매 실거래가

- 세종시 연령별 인구현황
  - 출처: COMPAS 및 세종시 제공

### ✏️분석결과

**1. 아파트, 연립다세대, 단독다가구, 오피스텔 거래건수**

<img src="https://user-images.githubusercontent.com/33304926/147366094-ed5da4a6-0aaf-48a0-a7af-68972a4b103c.png" width="600" height="370">

- 아파트(Apart), 연립다세대(Multicomplex), 단독다가구(SingleHousehold), 오피스텔(Officetel)의 매매(meme, 분홍색), 전/월세(zeonwolsae, 하늘색)거래건수를 막대 그래프로 나타내 보았습니다.
- 아파트의 거래건수가 압도적으로 많아 다른 유형의 거래건수가 상대적으로 작게 표시되어, 연립다세대, 단독다가구, 오피스텔을 따로 떼어 거래건수 그래프를 그려보았습니다.

**2. 연립다세대, 단독다가구, 오피스텔 거래건수**

<img src="https://user-images.githubusercontent.com/33304926/147366188-d673c22f-1889-48a4-9c43-09fcb1cc67ce.png" width="600" height="370">

- 단독다가구(SingleHousehold)는 전/월세 거래건수가 매매보다 압도적으로 많았습니다.
- 연립다세대(Multicomplex)는 매매 거래건수가 전/월세보다 많았습니다.
- 오피스텔(Officetel)은 전/월세 거래건수가 매매 거래건수보다 많았습니다.

**3. 건물유형 별 연도 별 거래건수**

![image](https://user-images.githubusercontent.com/33304926/147366326-42d70553-5aec-47fa-b620-0c28b6f79e21.png)

- 아파트(Apart)의 경우, 2018년을 제외하면 매매(밝은 청록색), 전/월세(어두운 녹색) 모두 거래건수가 매년 증가하였습니다.
- 연립다세대(Multicomplex)는 2017, 2020년에 매매 거래가 특히 많았습니다.
- 단독다가구(SingleHousehold)는 매년 매매 거래가 적었지만 전/월세의 경우 매년 거래건수가 증가하였습니다.
- 오피스텔(Officetel)은 2019년까지 전월세 거래가 매매 거래보다 많았으나, 2020년의 경우 매매 거래가 전월세 거래보다 많았습니다. 이는 코로나로 인해 대학가의 원룸(오피스텔)의 거래가 감소한 것에 영향을 받은 것으로 보입니다.

------

## 분석4. 세종시 연도별 총 인구수 변화와 업종별 상권 개수

👤contributor : [배수혜](https://github.com/SuHae-Bae)

- 세종시 연도별 총 인구수 변화와 업종별 상권 개수를 python을 활용하여 비교해 보았습니다.

### 📋활용한 데이터

- 세종시 상권정보

- 세종시 연령별 인구현황
  - 출처: COMPAS 및 세종시 제공

### ✏️분석결과

**1. 세종시의 연도별 총 인구수 변화**

<img src="https://user-images.githubusercontent.com/33304926/147366596-9d68b85b-362f-4122-8014-5d4a7f3e2044.png" width="600" height="370">

- 세종시의 인구를 연도별로 나타낸 결과, 2017년부터 2020년까지 꾸준히 증가함을 알 수 있었습니다.

<img src="https://user-images.githubusercontent.com/33304926/147366684-a9733673-42f2-4a12-88c8-c62a70236f17.png" width="600" height="370">

- 세종시의 인구를 남성과 여성으로 구분하여 나타낸 결과, 매년 여성의 인구수가 남성의 인구수보다 근소하게 많음을 발견하였습니다.

**2. 세종시의 업종별 상권 개수**

![image](https://user-images.githubusercontent.com/33304926/147366728-2614b1eb-4642-47eb-9618-e66b8b93a2f6.png)



- 대분류명을 기준으로 음식 업종이 가장 많고, 스포츠 업종이 가장 적었습니다.
- 소분류명을 기준으로 한식/백반/한정식 업종이 가장 많은 것으로 나타났으며, 학원-제과기술, 유류판매 등이 가장 적은, 한 업종씩뿐인 것으로 나타났습니다.

------

## 분석5. QGIS 시각화

👤contributor

- [김지우](https://github.com/g-wooo)
- [배수혜](https://github.com/SuHae-Bae)
  - 세종시의 주택 시장 특성이 담긴 데이터를 QGIS를 이용해 다양한 방법으로 시각화하였습니다.

### 📋활용한 데이터

- 세종시 아파트 매매 실거래가
- 세종시 연립다세대 매매 실거래가
- 세종시 단독다가구 매매 실거래가
- 세종시 오피스텔 매매 실거래가
- 세종시 상권정보

- 세종시 연령별 인구현황
  - 출처: COMPAS 및 세종시 제공

### ✏️분석결과

**1. 세종시 총 인구수 현황**

![image](https://user-images.githubusercontent.com/33304926/147366978-e62d9c6a-61f6-49d3-9169-7172742563ad.png)

- 세종시의 총인구수 격자(100m)를 내추럴 브레이크를 이용해 5등급으로 나눈 뒤 표시하였습니다.
- 인구가 많은 지역: 조치원읍, 반곡동, 소담동, 보람동, 대평동, 한솔동, 나성동, 새롬동, 다정동, 어진동, 종촌동, 고운동, 아름동, 도담동

**2. 세종시 전체 상권 현황**

![image](https://user-images.githubusercontent.com/33304926/147367033-6e552de5-3438-4918-aaa8-2d33e67706b0.png)

- 세종시의 전체 상권을 지도에 표시한 결과입니다. 이를 구체적인 상권분류에 따라 나누어 표시한 결과는 다음과 같습니다.

![image](https://user-images.githubusercontent.com/33304926/147367056-37c1fe57-eb9f-44ab-bdad-39ae0962f35b.png)

- 약간의 차이는 있지만, 상권분류가 다르더라도 주로 상권이 밀집되어 있는 지역이 비슷함을 확인할 수 있었습니다. 이에, 읍면동 별 상권 개수를 시각화하였습니다.

**3. 읍면동 별 상권 개수**

![image](https://user-images.githubusercontent.com/33304926/147367142-0f63cd8f-5e14-4995-b6bb-5dde28186cce.png)

- 세종시의 법정경계(읍면동)을 기준으로 각 읍면동별 상권 개수를 COUNT한 다음, 이를 내추럴 브레이크로 5분위로 나누어 지도에 시각화하였습니다.
- 상권수가 가장 <u>많은</u> 지역은 **조치원읍(3553개)**로, 상권수가 가장 <u>적은</u> 지역은 **합강동(0개)**인 것으로 나타났습니다.

**4. 아파트 매매 실거래가, 거래건수**

![image](https://user-images.githubusercontent.com/33304926/147367220-791d128e-950c-4cd0-9bf3-872a236a9923.png)

- 세종시의 아파트 매매 실거래가 데이터를 매매가격(단위: 만원)을 기준으로 내추럴 브레이크를 통해 5등급으로 나누었습니다. 
- 매매가가 높은 지역으로는 반곡동, 소담동, 보람동, 대평동, 한솔동, 나성동, 새롬동, 다정동, 어진동, 종촌동, 고운동, 아름동, 도담동이 나타났습니다.

![image](https://user-images.githubusercontent.com/33304926/147367285-03eeb53c-9831-4648-b23d-09e6a7f33b46.png)

- 세종시의 법정경계(읍면동)을 기준으로 각 읍면동별 아파 매매 거래건수를 COUNT한 다음, 이를 내추럴 브레이크로 5분위로 나누어 지도에 시각화 하였습니다.
- 매매건수가 가장 <u>많은</u> 지역은 **조치원읍(3889건)**으로 나타났으며, 매매건수가 <u>적은</u> 지역은 **가람동(0건), 산울동(0건), 해밀동(0건), 합강동(0건), 집현동(0건), 연기면(0건)**인 것으로 나타났습니다.

**5. 연립다세대 매매 실거래가, 거래건수**

![image](https://user-images.githubusercontent.com/33304926/147367352-f1fdd26d-544a-45c7-927c-d82910fb082e.png)

- 세종시의 연립다세대 매매 실거래가 데이터를 매매가격(단위: 만원)을 기준으로 내추럴 브레이크를 통해 5등급으로 나누었습니다. 
- 연립다세대 매매가가 고가인 지역은 조치원읍, 금난면, 반곡동, 부강면인 것으로 나타났습니다.

![image](https://user-images.githubusercontent.com/33304926/147367385-df7a5027-4000-48bc-8767-c78e5b6331bb.png)

- 세종시의 법정경계(읍면동)을 기준으로 각 읍면동별 연립다세대 매매 거래건수를 COUNT한 다음, 이를 내추럴 브레이크로 5분위로 나누어 지도에 시각화하였습니다.
- 매매 거래건수가 가장 <u>많은</u> 지역은 **조치원읍(357건)**으로 나타났으며, 매매 거래건수가 <u>적은</u> 지역은 **반곡동(0), 대평동(0), 가람동(0), 한솔동(0), 나성동(0), 새롬동(0), 다정동(0), 어진동(0), 종촌동(0), 고운동(0), 아름동(0), 산울동(0), 해밀동(0), 합강동(0), 집현동(0), 연동면(0)**으로 나타났습니다.

------

## 분석5-1. 아파트, 연립다세대 매매거래 중 고가의 매매거래가 발생한 지역과 그 외 지역의 평균 매매가 비교

- QGIS 분석 결과, 고가의 매매거래가 발생한 지역과 아닌 지역이 두드러지게 구분되어, 이에 지역을 2가지로 구분하여 표를 그려보았습니다.

  ![image](https://user-images.githubusercontent.com/33304926/147367538-05412fe2-7d69-4a4e-b2ee-33bb1d15983a.png)

- **아파트**의 경우, 높은 매매가가 있는 지역인 **반곡동, 소담동, 보람동, 대평동, 한솔동, 나성동, 새롬동, 다정동, 어진동, 종촌동, 고운동, 아름동, 도담동**의 평균 매매가가 그 외의 지역의 평균 매매가보다 높았습니다.

- **연립다세대**의 경우, 높은 가격의 매매가가 있는 지역인 **조치원읍, 금난면, 반곡동, 부강면**의 평균 매매가가 그 외의 지역의 평균 매매가보다 낮았습니다. 이들 지역에서는 <u>높은 가격의 매매가가 있을 뿐 아니라, 낮은 가격의 매매가 또한 있어</u> 이러한 결과가 나온 것으로 추정됩니다.

------

## 결과 활용 방안 및 기대효과





![image](https://user-images.githubusercontent.com/33304926/147367628-29fcca07-5da4-4db0-a457-c61b69298c2b.png)



![image](https://user-images.githubusercontent.com/33304926/147367653-33fdaa80-fbf0-417a-b99d-84ad41a47d1e.png)

