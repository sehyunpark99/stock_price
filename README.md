# 제2회 KRX 주식 투자 알고리즘 경진대회
한국거래소의 정보사업을 확대하고, 시장참가자들에게 더욱 유용한 투자 참고 정보를 제공하기 위해,   
제2회 KRX 주식 투자 알고리즘 경진대회를 개최합니다.   
자본시장 데이터 및 공공 데이터를 활용하여 높은 안정성과 수익률을 기대할 수 있는 주식 투자 알고리즘을 만들어주세요.   
&#8251;Read more : [제2회 KRX 주식 투자 알고리즘 경진대회](https://dacon.io/competitions/official/236117/overview/description)    

- 팀원 : 박선영, 박세현, 이명주, 이채은

## 1. Overview
### <Data>    
  <b>train.csv</b> : 일자 | 종목코드 | 종목명 | 거래량 | 시가 | 고가 | 저가 | 종가   
![스크린샷 2023-07-29 오후 9 37 56](https://github.com/sehyunpark99/stock_price/assets/85481704/7c9ec632-d268-416a-ba49-03ef5c0c4dd3)

### <예선>  
- Submission   
![1687332501266426](https://github.com/sehyunpark99/stock_price/assets/85481704/58c07445-7a6e-4304-835a-0675b52a1c1a)

- Evaluation Proces   
![1687506259750990](https://github.com/sehyunpark99/stock_price/assets/85481704/05b34792-5b5b-468d-a400-599655730561)    

- Evaluation Score   
<img width="668" alt="스크린샷 2023-07-29 오후 9 47 10" src="https://github.com/sehyunpark99/stock_price/assets/85481704/8dc4e0e2-961a-462e-8237-5f37adcb429d">

<b>Sharpe Index</b> : (연율화된 총자산 최종 수익률 - 무위험 수익률) / 총자산 일간 수익률 변동성    
  참고파일 : calculate_sharpe.ipynb

## 2. Model
### (1) ARIMA    
#간략한설명#
&#8251;Read more : [ARIMA_submission.ipynb](https://github.com/sehyunpark99/stock_price/blob/main/ARIMA_submission.ipynb)

### (2) LSTM
#간략한설명#
* Prediction Plot
![image](https://github.com/sehyunpark99/stock_price/assets/85481704/7a2349cf-cb44-49d2-9b58-a7cf4fb99cb2)

&#8251;Read more : [LSTM_submission.ipynb](https://github.com/sehyunpark99/stock_price/blob/main/LSTM_submission.ipynb)
### (3) Cosine similarity

### (4) Moving Average

## 3. Result

|Model|Sharpe Index|annualized return|
|:-|:-:|:-:|
|stock_MA|0.21|0.17|
|cosine sim|0.377|0.18|
|lstm|0.226|0.029|
|arima|0.28|0.83|
|cos & sharpe|0.61|0.26|
|stockMA&cos|0.71|0.26|
|lstm&cos|0.27|0.81|
|arima&cos|0.27|0.60|

### LSTM + Cos ensemble model 
** 수식 ** 

## 
