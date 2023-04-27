# Stochastic Control & HFT

<img src="https://img.shields.io/static/v1?label=Range&message=Academic project&color=007bff"/>&nbsp;&nbsp;<img src="https://img.shields.io/static/v1?label=Languages&message=Python&color=ff0000"/> 


**Workflows**: ![](https://img.shields.io/badge/Dependabot-enabled-blue)


## Overview

This project aims at studying a research article involving high-frequency trading & stochastic control applications. One also attempts to reproduce the numerical results shown in this paper.


- Original paper: *Optimal high frequency trading with limit and market orders*, Fabien GUILBAUD, Huyên PHAM (2011)
    - Link: [arxiv (1106.5040)](https://arxiv.org/abs/1106.5040) [(PDF)](https://arxiv.org/pdf/1106.5040.pdf) [(HTML via ar5iv)](https://ar5iv.labs.arxiv.org/html/1106.5040)
- Keywords: *Market making, limit order book, inventory risk, point process, stochastic control*

## Data description

This article's using Level 1 (L1) data from **`SOGCGEN.PA`** (intraday data) for only one day: *April 18, 2011* between 9:30 and 16:30 in Paris local time (UTC+1).

To reproduce the method introduced in this article, one applies it to L1 (tick data) sample dataset available on [TickHistory](https://tickhistory.com/)'s website.

**Dataset description**:
- **GOOG**: `trades` and `quotes` data
- **MSFT**: `trades` and `quotes` data

```
.
├── tickhistory_sample
│   ├── GOOG_Quote_2022_01_03.txt
│   ├── GOOG_Trade_2022_01_03.txt
│   ├── MSFT_Quote_2022_01_03.txt
│   ├── MSFT_Trade_2022_01_03.txt
│   ├── file_format_details.txt
│   └── tick_history_ticker_coverage.txt
└── tickhistory_sample.zip
```

Data from:
- https://tickhistory.com/
- https://firstratedata.com/tick-data

## Getting started

1. Install required modules:
```
pip3 install -r requirements.txt
```

2. Launch a Jupyter instance
```
jupyter-notebook .
```

## License

Adrien NAVARRO - Lucas RODRIGUEZ