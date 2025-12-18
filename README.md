# 🚢 HMM 주가 데이터 분석(HMM Stock Price Analysis)
**프로젝트 기간 (Duration)**:  2025.11.28 ~ 2025.12.02 (5일간)


**분석 대상 (Analysis target)** : HMM(011200)


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## ✏️ 프로젝트 요약(Description)
1. 한국거래소(KRX)에 등록되어 있는 기업을 선정하고, 해당 기업의 주식 거래량이 큰 폭으로 상승한 구간을 워드클라우드를 시각화
   - Select a company registered on the Korea Exchange (KRX) and visualize the section where the stock trading volume of the company has risen significantly
2. 주가에 영향을 줄 것으로 예상한 요소가 워드클라우드에 포함되어있는지 확인
   - Ensure WordCloud includes what you expect to impact the stock price
3. 주가 데이터와 요소 데이터를 피어슨 상관분석
   - Pearson correlation analysis of stock price and factor data
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
### 🔍 분석 배경(Analysis Background)
- 2025년 들어서 보호무역주의가 전세계적으로 나타나는 만큼, 국제믈동량이 감소할 것으로 예상함. 이러한 물동량 하락이 HMM 주가에 영향을 주었는 지, 이번 분석을 통해서 도출하고자 함
    - As protectionism appears worldwide in 2025, the amount of international trade is expected to decrease. Whether this decline in volume has affected HMM's stock price, we intend to derive it through this analysis
- HMM 주가에 영향을 줄 것으로 예상되는 요소 (Factors expected to affect HMM Stock Price)
    - SCFI (Shanghai Containerized Freight Index) : 상하이 컨테이너 지수 
    - WTI (West Texas Intermediate) : 서부 텍사스산 원유 지수
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
### 🚩 분석 목표(Goal)
- 주가에 영향을 줄 것으로 예상한 요소가 실제로 주가에 영향을 주었을 지 워드클라우드를 통해 확인하고, 피어슨 상관분석을 통해서 수치화
  - Using WordCloud to see if the factors we expected to affect the stock price actually affected the stock price, and analysis it through Pearson correlation analysis
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
|Tools|Skills|
|---|---|
|**Language**|Python|
|**Processing**|Pandas, NumPy|
|**Data Collection**|FinanceDataReader, yFinanace, Selenium|
|**Visualization**|Matplotlib, WordCloud|
