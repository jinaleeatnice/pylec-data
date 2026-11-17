# pylec-data

"파이썬을 활용한 금융데이터 분석" 강의 실습용 공개 데이터입니다. 노트북에서 아래 raw 링크로 바로 읽습니다.

| 파일 | 내용 | 링크 |
|------|------|------|
| `etf_prices.csv` | 미국 ETF 7종(SPY, QQQ, TQQQ, QLD, GLD, SCHD, VTI) 일별 가격, 2021-08-23 ~ 2026-08-20. 출처: Twelve Data API | https://raw.githubusercontent.com/jinaleeatnice/pylec-data/main/etf_prices.csv |

컬럼: `symbol, datetime, open, high, low, close, volume`

```python
import pandas as pd
etf = pd.read_csv('https://raw.githubusercontent.com/jinaleeatnice/pylec-data/main/etf_prices.csv',
                  parse_dates=['datetime'])
```
