<img width="810" height="109" alt="image" src="https://github.com/user-attachments/assets/4250ad8c-eef6-4082-84e3-891438277f27" /># BengaluruAirQualityForecast
This is a GNN based multi modal forecasting of PM2.5 air quality parameter. It considers external events like festivals, harvesting, time of the day(peak, off-peak), season(summer, spring, winter) to derive useful insights. The dataset is derived from Central Control Room for Air Qualiry Management. It is multimodal as it contains meteirological parameters, sensor parameters(PM10, NO, SO2, CO, Ozone), traffic(traffic count, average speed, congestion level) and weather parameters(wind speed, wind direction, pressure, relative humidity)


## Tech Stack
- Python
- PyTorch / PyTorch Geometric
- Graph Neural Network
- Grok tunneling & Streamlit

## Problem Statement
I am trying to predict accurate PM2.5 values to judge the quality of air in the upcoming days.

## Approach
- Data preprocessing & feature Engineering
- Model / algorithm used are SARIMAX, GNN
- Training strategy used is I replaced the old daily dataset with new hourly records dataset to derive more insights.
- Evaluation is done using RMSE, MAE and Accuracy

## Results
- Accuracy with GNN was 0.9171. MSE was 0.083. MSE for SARIMAX was 231.03.
  

## How to Run
```bash
#pip install -r requirements.txt
jupyter notebook airqualityforecasting.ipynb
