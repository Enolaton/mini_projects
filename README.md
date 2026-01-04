# 🚢 HMM 주가 데이터 분석(HMM Stock Price Analysis)
**프로젝트 기간 (Duration)**:  2025.11.28. ~ 2025.12.02. (5일간)
**분석 대상 (Analysis target)** : HMM(011200)

---

## ✏️ 프로젝트 요약(Description)
1. 한국거래소(KRX)에 등록되어 있는 기업을 선정하고, 해당 기업의 주식 거래량이 큰 폭으로 변화한 시기를 분석 구간으로 설정
   - Select a company registered on the Korea Exchange (KRX) and Set the period when the company's stock trading volume increased(or decreased) significantly as the analysis period
2. 해당 분석 구간의 뉴스 기사 제목을 웹 크롤링하고, 워드클라우드로 시각화
   -  Web-crawling the titles of the news of the specific duration and visualized it in WordCloud
4. 주가에 영향을 줄 것으로 예상한 요소가 워드클라우드에 포함되어있는지 확인
   - Ensure WordCloud includes what we expect to impact the HMM stock price
5. 주가 데이터와 요소 데이터를 피어슨 상관분석
   - Pearson correlation analysis of stock price and factor data
  
---

### 🔍 배경(Introduction: Analysis Background)
- 2025년 들어서 보호무역주의가 전세계적으로 나타나는 만큼, 국제믈동량이 감소할 것으로 예상함. 이러한 물동량 하락이 해운사 HMM의 주가에 영향을 주었는 지, 이번 분석을 통해서 도출하고자 함
    - As protectionism appears worldwide in 2025, the amount of international trade is expected to decrease. We would like to derive whether this decline in volume affected the stock price of HMM, a shipping company in Korea, through this analysis 
- HMM 주가에 영향을 줄 것으로 예상되는 요소 (Factors expected to affect HMM Stock Price)
   1. 상하이 컨테이너 지수 : 상하이 수출컨테이너 운송시장의 15개 항로의 스팟 운임을 반영한 운임지수
      - SCFI (Shanghai Containerized Freight Index) : spot freight rates for containerized cargo leaving Shanghai to major global ports
   2. 서부 텍사스산 원유 지수 : 미국 서부 텍사스 중간지역에서 생산되는 원유로, 세계 3대 유종 중 하나
      - WTI (West Texas Intermediate) : WTI is a light, sweet crude oil primarily sourced from Texas, known for its high quality and ease of refining

---

### 🚩 목적(Analysis Objective)
- 주가에 영향을 줄 것으로 예상한 요소가 실제로 주가에 영향을 주었을 지 워드클라우드를 통해 확인하고, 피어슨 상관분석을 통해서 수치화
  - Using WordCloud to see if the factors we expected to affect the stock price actually affected the stock price, and analysis it through Pearson correlation analysis
    
---

### 📊 결과(Results)
- 주식 거래량이 변화한 시기를 시각화한 결과, 주가에 영향을 줄 것으로 판단한 요소가 포함된 시기는 일부에 불과했고, 대부분 특정 시기에 발생한 이슈들로 인해서 거래량이 증가했음을 확인함
  - As a result of visualizing the timing of changes in stock trading volume, only a part of the time was included that it was determined to affect stock prices, and most of them confirmed that trading volume increased due to issues that occurred at certain times
    
---

### 📋 한계점 및 앞으로의 분석 방향 (Limitations & Future analysis directions)
- HMM 주가와 SCFI와 WTI가 강한 양의 상관관계가 있을 것으로 예상했지만, 분석결과 SCFI는 양의 상관관계에 있었고, WTI는 약한 양의 상관관계에 있었음
  - HMM stock price and SCFI and WTI were expected to have a strong positive correlation, but the analysis showed that SCFI was positively correlated and WTI was weakly correlated
- 앞으로 회귀분석이나 시계열 분석을 통해서 더욱 정밀한 결과를 도출 할 수 있을 것으로 판단
  - We expect that more precise results can be derived through regression or time series analysis
- 지수 데이터의 변동이 바로 주가 데이터에 영향을 미치지 않을 수 있으니, 시차를 두고 두 데이터를 분석해볼 수 있음
  - Set time-lag between stock price data and index data because the effects of index fluctuations may not affect immediately
    
---

### 📌 기술 스택 (Stacks)

|Tools|Skills|
|---|---|
|**Language**|Python|
|**Processing**|Pandas, NumPy|
|**Data Collection**|FinanceDataReader, yFinanace, Selenium|
|**Visualization**|Matplotlib, WordCloud|

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

