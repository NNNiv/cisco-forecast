## 1. Seasonality Analysis

### Products with Strong Seasonality (Strength > 0.7)

|Product|Seasonality Strength|Dominant Quarter|Q1 Index|Q2 Index|Q3 Index|Q4 Index|
|---|---|---|---|---|---|---|
|SWITCH Enterprise High 2|1.0000|Q4|-21.03|15.84|-20.78|25.97|
|SWITCH Enterprise High 1|0.9338|Q4|1348.05|-3713.64|-4124.83|6490.42|
|TRANSCEIVER MODULE Mid 1|0.7984|Q4|-13010.48|-2080.73|-4548.05|19639.27|
|SWITCH Enterprise Ultra High 2|0.7833|Q4|-1004.97|23.53|-91.53|1072.97|
|MEMORY|0.7561|Q4|-7654.23|-7540.23|-2360.92|17555.39|
|SWITCH Enterprise Ultra High 1|0.7199|Q4|-916.33|-479.33|-393.95|1789.61|

### Products with Moderate Seasonality (0.5 ≤ Strength < 0.7)

|Product|Seasonality Strength|Dominant Quarter|Q1 Index|Q2 Index|Q3 Index|Q4 Index|
|---|---|---|---|---|---|---|
|POWER SUPPLY Mid|0.6992|Q4|870.59|-7196.78|-10666.59|16992.78|
|ROUTER Enterprise Mid 1|0.6924|Q4|-389.80|-1936.55|-185.30|2511.64|
|POWER SUPPLY High|0.6482|Q4|-3826.36|-5093.80|-8175.36|17095.52|
|TRANSCEIVER MODULE High|0.5970|Q3|-995.06|-855.81|4171.94|-2321.06|
|SERVER|0.5870|Q4|-160.11|-328.67|-1204.48|1693.27|

### Products with Weak Seasonality (Strength < 0.5)

|Product|Seasonality Strength|Dominant Quarter|Q1 Index|Q2 Index|Q3 Index|Q4 Index|
|---|---|---|---|---|---|---|
|ACCESS POINT Mid|0.4967|Q4|-6191.05|-139.86|-384.11|6715.02|
|ROUTER Enterprise Low|0.4690|Q2|-629.19|3167.50|-3423.06|884.75|
|SWITCH Data Center High|0.4571|Q2|-53.00|295.81|-160.94|-81.88|
|TRANSCEIVER MODULE Mid 2|0.3752|Q3|-3457.67|-1755.23|4304.70|908.20|
|SWITCH Data Center Mid 2|0.3004|Q1|250.31|-317.69|141.00|-73.63|
|ROUTER Enterprise Mid 2|0.2978|Q4|-152.03|-237.28|-79.84|469.16|
|SWITCH Enterprise Low|0.2075|Q1|4472.83|-1583.80|234.27|-3123.30|
|SWITCH Data Center Mid 1|0.2085|Q2|-241.88|164.31|128.63|-51.06|

### Insufficient Data

- PROCESSOR: Fewer than 8 data points available

## 2. Outlier Detection (Threshold: 2.5 Z-score)

|Product|Quarter|Demand|Z-score|
|---|---|---|---|
|TRANSCEIVER MODULE Mid 1|FY22 Q2|208,760|2.71|
|SWITCH Data Center Mid 1|FY22 Q3|6,513|2.76|
|SWITCH Data Center Mid 2|FY22 Q2|6,629|2.82|

## 3. Autocorrelation Analysis

### Products with Significant Lag-1 Autocorrelation

- SWITCH Enterprise High 1
- SWITCH Enterprise Ultra High 1
- SWITCH Enterprise Ultra High 2
- POWER SUPPLY High
- ACCESS POINT Mid
- POWER SUPPLY Mid
- SERVER
- TRANSCEIVER MODULE Mid 2
- ROUTER Enterprise Mid 2

### Products with No Significant Autocorrelation

- SWITCH Enterprise Low
- TRANSCEIVER MODULE Mid 1
- TRANSCEIVER MODULE High
- PROCESSOR
- SWITCH Data Center High
- ROUTER Enterprise Mid 1
- MEMORY
- SWITCH Data Center Mid 1
- ROUTER Enterprise Low
- SWITCH Data Center Mid 2
- SWITCH Enterprise High 2

## 4. Seasonality Heatmap - Peak-to-Low Ratio

|Product|Peak Quarter|Low Quarter|Ratio|
|---|---|---|---|
|TRANSCEIVER MODULE High|Q1|Q4|2.76|
|SERVER|Q4|Q3|2.64|
|ROUTER Enterprise Mid 1|Q4|Q2|2.00|
|SWITCH Enterprise Ultra High 1|Q4|Q2|1.96|
|TRANSCEIVER MODULE Mid 2|Q3|Q2|1.93|
|SWITCH Enterprise High 2|Q4|Q2|1.85|
|PROCESSOR|Q2|Q3|1.83|
|SWITCH Enterprise Low|Q1|Q4|1.79|
|TRANSCEIVER MODULE Mid 1|Q2|Q1|1.79|
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

## 5. Long-Term Cycle Analysis

### Annual Cycles (4 Quarters)

|Product|Cycle Type|Duration (Days)|Quarters|
|---|---|---|---|
|SWITCH Enterprise High 1|Peak-to-peak & Trough-to-trough|366|~4.1|
|SWITCH Enterprise Ultra High 1|Peak-to-peak|366|~4.1|
|SWITCH Enterprise Ultra High 2|Peak-to-peak|366|~4.1|
|POWER SUPPLY High|Peak-to-peak|366|~4.1|
|TRANSCEIVER MODULE High|Peak-to-peak & Trough-to-trough|366|~4.1|
|ACCESS POINT Mid|Peak-to-peak|366|~4.1|
|POWER SUPPLY Mid|Peak-to-peak|366|~4.1|
|SWITCH Data Center High|Trough-to-trough|366|~4.1|
|ROUTER Enterprise Mid 1|Trough-to-trough|366|~4.1|
|MEMORY|Peak-to-peak|365|~4.1|
|ROUTER Enterprise Mid 2|Peak-to-peak|366|~4.1|
|SWITCH Data Center Mid 2|Peak-to-peak|366|~4.1|

### Semi-Annual Cycles (2 Quarters)

|Product|Cycle Type|Duration (Days)|Quarters|
|---|---|---|---|
|SWITCH Enterprise Ultra High 2|Trough-to-trough|184|~2.0|
|TRANSCEIVER MODULE Mid 1|Multiple cycles|181-184|~2.0|
|TRANSCEIVER MODULE High|Peak-to-peak & Trough-to-trough|181-183|~2.0|
|SERVER|Multiple cycles|182-183|~2.0|
|SWITCH Data Center High|Peak-to-peak|183-184|~2.0|
|TRANSCEIVER MODULE Mid 2|Trough-to-trough|181|~2.0|
|ROUTER Enterprise Mid 2|Multiple cycles|181-184|~2.0|
|SWITCH Data Center Mid 1|Peak-to-peak|183|~2.0|
|ROUTER Enterprise Low|Multiple cycles|181-182|~2.0|
|SWITCH Enterprise High 2|Multiple cycles|182-183|~2.0|

### Other Cycles (3 or 5 Quarters)

|Product|Cycle Type|Duration (Days)|Quarters|
|---|---|---|---|
|SWITCH Enterprise Low|Multiple cycles|273-275|~3.0|
|POWER SUPPLY High|Trough-to-trough|275|~3.1|
|TRANSCEIVER MODULE High|Trough-to-trough|274|~3.0|
|POWER SUPPLY Mid|Peak-to-peak & Trough-to-trough|275-457|~3.1-5.1|
|SWITCH Data Center High|Multiple cycles|273-456|~3.0-5.1|
|TRANSCEIVER MODULE Mid 2|Peak-to-peak & Trough-to-trough|457-458|~5.1|
|ROUTER Enterprise Mid 1|Peak-to-peak|274-457|~3.0-5.1|
|SWITCH Data Center Mid 1|Peak-to-peak & Trough-to-trough|275-457|~3.1-5.1|
|ROUTER Enterprise Low|Multiple cycles|275|~3.1|
|SWITCH Data Center Mid 2|Trough-to-trough|275|~3.1|