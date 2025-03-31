# Seasonality Analysis

|Product|Seasonal Strength|Q1 Index|Q2 Index|Q3 Index|Q4 Index|
|---|---|---|---|---|---|
|SWITCH Enterprise High 1|0.9338|1348.05|-3713.64|-4124.83|6490.42|
|SWITCH Enterprise Ultra High 1|0.7199|-916.33|-479.33|-393.95|1789.61|
|SWITCH Enterprise Ultra High 2|0.7833|-1004.97|23.53|-91.53|1072.97|
|SWITCH Enterprise Low|0.2075|4472.83|-1583.80|234.27|-3123.30|
|TRANSCEIVER MODULE Mid|0.5130|-1646.80|6925.18|-7583.90|1646.80|
|POWER SUPPLY High|0.6482|-3826.36|-5093.80|-8175.36|17095.52|
|TRANSCEIVER MODULE High|0.5970|-995.06|-855.81|4171.94|-2321.06|
|ACCESS POINT Mid|0.4967|-6191.05|-139.86|-384.11|6715.02|
|POWER SUPPLY Mid|0.6992|870.59|-7196.78|-10666.59|16992.78|
|SERVER|0.5870|-160.11|-328.67|-1204.48|1693.27|
|PROCESSOR|Insufficient data (need 8 points, have 7)|-|-|-|-|
|SWITCH Data Center High|0.4571|-53.00|295.81|-160.94|-81.88|
|TRANSCEIVER MODULE Mid (duplicate)|0.5130|-1646.80|6925.18|-7583.90|1646.80|
|ROUTER Enterprise Mid 1|0.6924|-389.80|-1936.55|-185.30|2511.64|
|MEMORY|0.7561|-7654.23|-7540.23|-2360.92|17555.39|
|ROUTER Enterprise Mid 2|0.2978|-152.03|-237.28|-79.84|469.16|
|SWITCH Data Center Mid 1|0.2085|-241.88|164.31|128.63|-51.06|
|ROUTER Enterprise Low|0.4690|-629.19|3167.50|-3423.06|884.75|
|SWITCH Data Center Mid 2|0.3004|250.31|-317.69|141.00|-73.63|
|SWITCH Enterprise High 2|1.0000|-21.03|15.84|-20.78|25.97|

## Key Seasonal Patterns

### Strong Seasonality (Strength > 0.7)

- **SWITCH Enterprise High 2**: Perfect seasonality (1.0000)
- **SWITCH Enterprise High 1**: Very strong seasonality (0.9338)
- **SWITCH Enterprise Ultra High 2**: Strong seasonality (0.7833)
- **MEMORY**: Strong seasonality (0.7561)
- **SWITCH Enterprise Ultra High 1**: Strong seasonality (0.7199)
- **POWER SUPPLY Mid**: Strong seasonality (0.6992)

### Q4 Dominant Products

- **MEMORY**: Strongest Q4 index (17555.39)
- **POWER SUPPLY High**: Strong Q4 index (17095.52)
- **POWER SUPPLY Mid**: Strong Q4 index (16992.78)

### Q1 Dominant Products

- **SWITCH Enterprise Low**: Strong Q1 index (4472.83)

### Q2 Dominant Products

- **TRANSCEIVER MODULE Mid**: Strong Q2 index (6925.18)
- **ROUTER Enterprise Low**: Moderate Q2 index (3167.50)

### Q3 Dominant Products

- **TRANSCEIVER MODULE High**: Strong Q3 index (4171.94)

# Outlier Detection (Threshold: 2.5 Z-score)

|Product|Quarter|Demand|Z-score|
|---|---|---|---|
|TRANSCEIVER MODULE Mid|FY22 Q2|208,760.0|2.90|
|SWITCH Data Center Mid 1|FY22 Q3|6,513.0|2.76|
|SWITCH Data Center Mid 2|FY22 Q2|6,629.0|2.82|

## Products with No Detected Outliers

- SWITCH Enterprise High 1
- SWITCH Enterprise Ultra High 1
- SWITCH Enterprise Ultra High 2
- SWITCH Enterprise Low
- POWER SUPPLY High
- TRANSCEIVER MODULE High
- ACCESS POINT Mid
- POWER SUPPLY Mid
- SERVER
- PROCESSOR
- SWITCH Data Center High
- ROUTER Enterprise Mid 1
- MEMORY
- ROUTER Enterprise Mid 2
- ROUTER Enterprise Low
- SWITCH Enterprise High 2


# Autocorrelation Analysis

|Product|Significant Autocorrelation Lags|
|---|---|
|SWITCH Enterprise High 1|[1]|
|SWITCH Enterprise Ultra High 1|[1]|
|SWITCH Enterprise Ultra High 2|[1]|
|SWITCH Enterprise Low|None|
|TRANSCEIVER MODULE Mid|None|
|POWER SUPPLY High|[1]|
|TRANSCEIVER MODULE High|None|
|ACCESS POINT Mid|[1]|
|POWER SUPPLY Mid|[1]|
|SERVER|[1]|
|PROCESSOR|None|
|SWITCH Data Center High|None|
|TRANSCEIVER MODULE Mid (duplicate)|None|
|ROUTER Enterprise Mid 1|None|
|MEMORY|None|
|ROUTER Enterprise Mid 2|[1]|
|SWITCH Data Center Mid 1|None|
|ROUTER Enterprise Low|None|
|SWITCH Data Center Mid 2|None|
|SWITCH Enterprise High 2|None|

## Seasonality Heatmap

Products ranked by seasonal intensity (high to low):

|Product|Peak|Low|Ratio|
|---|---|---|---|
|TRANSCEIVER MODULE High|Q1|Q4|2.76|
|SERVER|Q4|Q3|2.64|
|ROUTER Enterprise Mid 1|Q4|Q2|2.00|
|SWITCH Enterprise Ultra High 1|Q4|Q2|1.96|
|TRANSCEIVER MODULE Mid|Q3|Q2|1.93|
|SWITCH Enterprise High 2|Q4|Q2|1.85|
|PROCESSOR|Q2|Q3|1.83|
|SWITCH Enterprise Low|Q1|Q4|1.79|
|TRANSCEIVER MODULE Mid (duplicate)|Q2|Q1|1.79|
|SWITCH Data Center Mid 1|Q3|Q1|1.74|
|ROUTER Enterprise Mid 2|Q4|Q2|1.54|
|ROUTER Enterprise Low|Q2|Q3|1.52|
|SWITCH Enterprise Ultra High 2|Q2|Q1|1.47|
|SWITCH Data Center Mid 2|Q2|Q1|1.40|
|MEMORY|Q4|Q1|1.35|
|SWITCH Enterprise High 1|Q4|Q1|1.26|
|ACCESS POINT Mid|Q3|Q1|1.25|
|POWER SUPPLY High|Q4|Q1|1.25|
|POWER SUPPLY Mid|Q4|Q1|1.21|
|SWITCH Data Center High|Q2|Q3|1.21|

# Long-Term Cycle Analysis

### Annual Cycles (365-366 days)

Products with clear annual cycles (peak-to-peak or trough-to-trough):

- SWITCH Enterprise High 1: 366 days (~4.1 quarters) both peak-to-peak and trough-to-trough
- SWITCH Enterprise Ultra High 1: 366 days (~4.1 quarters) peak-to-peak
- SWITCH Enterprise Ultra High 2: 366 days (~4.1 quarters) peak-to-peak
- POWER SUPPLY High: 366 days (~4.1 quarters) peak-to-peak
- TRANSCEIVER MODULE High: 366 days (~4.1 quarters) both peak-to-peak and trough-to-trough
- ACCESS POINT Mid: 366 days (~4.1 quarters) peak-to-peak
- POWER SUPPLY Mid: 366 days (~4.1 quarters) peak-to-peak
- SWITCH Data Center High: 366 days (~4.1 quarters) trough-to-trough
- ROUTER Enterprise Mid 1: 366 days (~4.1 quarters) trough-to-trough
- MEMORY: 365 days (~4.1 quarters) peak-to-peak
- ROUTER Enterprise Mid 2: 366 days (~4.1 quarters) peak-to-peak
- SWITCH Data Center Mid 2: 366 days (~4.1 quarters) peak-to-peak

### Semi-Annual Cycles (~180-184 days)

Products with clear semi-annual cycles (peak-to-peak or trough-to-trough):

- SWITCH Enterprise Ultra High 2: 184 days (~2.0 quarters) trough-to-trough
- SWITCH Enterprise Low: 183 days (~2.0 quarters) peak-to-peak
- TRANSCEIVER MODULE High: 181 days (~2.0 quarters) peak-to-peak and 183 days (~2.0 quarters) trough-to-trough
- SERVER: 183 days (~2.0 quarters) peak-to-peak and 182 days (~2.0 quarters) trough-to-trough
- SWITCH Data Center High: 184 days (~2.0 quarters) peak-to-peak and 183 days (~2.0 quarters) peak-to-peak
- ROUTER Enterprise Mid 2: Multiple cycles around 182-184 days (~2.0 quarters)
- SWITCH Data Center Mid 1: 183 days (~2.0 quarters) peak-to-peak
- ROUTER Enterprise Low: 182 days (~2.0 quarters) peak-to-peak and 181 days (~2.0 quarters) trough-to-trough
- SWITCH Enterprise High 2: Multiple cycles around 182-183 days (~2.0 quarters)

### Three-Quarter Cycles (~270-275 days)

Products with clear three-quarter cycles (peak-to-peak or trough-to-trough):

- SWITCH Enterprise Low: Multiple cycles around 273-275 days (~3.0-3.1 quarters)
- POWER SUPPLY High: 275 days (~3.1 quarters) trough-to-trough
- TRANSCEIVER MODULE High: 274 days (~3.0 quarters) trough-to-trough
- POWER SUPPLY Mid: 275 days (~3.1 quarters) trough-to-trough
- SWITCH Data Center High: 273 days (~3.0 quarters) trough-to-trough
- ROUTER Enterprise Mid 1: 274 days (~3.0 quarters) peak-to-peak
- SWITCH Data Center Mid 1: 275 days (~3.1 quarters) trough-to-trough
- ROUTER Enterprise Low: 275 days (~3.1 quarters) both peak-to-peak and trough-to-trough
- SWITCH Data Center Mid 2: 275 days (~3.1 quarters) trough-to-trough

### Extended Cycles (>366 days)

Products with cycles longer than a year:

- POWER SUPPLY Mid: 457 days (~5.1 quarters) peak-to-peak
- SWITCH Data Center High: 456 days (~5.1 quarters) peak-to-peak
- ROUTER Enterprise Mid 1: 457 days (~5.1 quarters) peak-to-peak
- SWITCH Data Center Mid 1: 457 days (~5.1 quarters) peak-to-peak

### Products with No Clear Cycles

- TRANSCEIVER MODULE Mid
- PROCESSOR (insufficient data)