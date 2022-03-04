# All-About-TimeSeries-Analysis

> @jhbale11

**시계열 데이터**란 일정한 시간동안 수집된, 일련의 순차적인 순서를 가지는 데이터셋의 집합으로 시간에 관해 순서가 매겨져 있으며 연속한 관측치는 서로 상관관계를 가지고 있다는 특징을 가지고 있습니다.

POS(Point Of Sales) 구매 자료, 일일 코스피 주식 가격, 월별/분기별/연도별 특정 사건의 수치 등 일상의 많은 데이터가 시계열 데이터이기에 **"시계열 데이터에 대한 End-To-End 분석 방법론"**을 알고 이를 적용하는 것은 그것이 어떤 도메인의 데이터든 상관없이 분석의 가장 기초적인 단계가 될 것입니다.

이 프로젝트에서는 Pandas, Matploblib, Plotly, Statsmodels 라이브러리를 사용하여 시계열 데이터를 분석하는 모든 방법을 정리하고 실습해보고자 합니다. 시계열 데이터를 처음 접하는 초심자와 어느 정도 pandas, visualization library, statsmodel을 사용할 줄 아는 중급자들에게 좋은 가이드가 되었으면 좋겠습니다.

## Table Of Contents
- <a href='#1'>1. Date와 Time의 이해</a>
    - <a href='#1.1'>1.1 시계열 데이터 불러오기</a>
    - <a href='#1.2'>1.2 시계열 데이터 전처리</a>
    - <a href='#1.3'>1.3 데이터 시각화</a>
    - <a href='#1.4'>1.4 Shifting과 Lagging</a>
    - <a href='#1.5'>1.5 Resampling</a>
- <a href='#2'>2. 금융데이터와 통계학</a>
    - <a href='#2.1'>2.1 비율 변화(Percent change)</a>
    - <a href='#2.2'>2.2 주식 수익률(Stock returns)</a>
    - <a href='#2.3'>2.3 절댓값 변화(Absolute change in successive rows)</a>
    - <a href='#2.4'>2.4 두 시계열 데이터 비교</a>
    - <a href='#2.5'>2.5 윈도우 함수(Window functions)</a>
    - <a href='#2.6'>2.6 OHLC 차트</a>
    - <a href='#2.7'>2.7 Candlestick 차트</a>
    - <a href='#2.8'>2.8 자기상관과 편자기상관(Autocorrelation and Partial Autocorrelation)</a>
- <a href='#3'>3. 시계열 데이터 분해(ecomposition)와 랜덤 워크(Random Walks)</a>
    - <a href='#3.1'>3.1 트렌드(Trends), 계절성(Seasonality)과 노이즈(Noise)</a>
    - <a href='#3.2'>3.2 화이트 노이즈(White Noise)</a>
    - <a href='#3.3'>3.3 랜덤 워크(Random Walk)</a>
    - <a href='#3.4'>3.4 정상성(Stationarity)</a>
- <a href='#4'>4. statsmodels 사용하기</a>
    - <a href='#4.1'>4.1 AR models</a>
    - <a href='#4.2'>4.2 MA models</a>
    - <a href='#4.3'>4.3 ARMA models</a>
    - <a href='#4.4'>4.4 ARIMA models</a>
    - <a href='#4.5'>4.5 VAR models</a>
    - <a href='#4.6'>4.6 State space methods</a>
        - <a href='#4.6.1'>4.6.1 SARIMA models</a>
        - <a href='#4.6.2'>4.6.2 Unobserved components</a>
        - <a href='#4.6.3'>4.6.3 Dynamic Factor models</a>
