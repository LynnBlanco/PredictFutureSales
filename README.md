# Predict Future Sales
DSAI Final Project - [Predict Future Sales (Kaggle)](https://www.kaggle.com/competitions/competitive-data-science-predict-future-sales/overview)

Provided with daily historical sales data. The task is to forecast the total amount of products sold in every shop for the test set. Note that the list of shops and products slightly changes every month. Creating a robust model that can handle such situations is part of the challenge.

## Data Analyze
- Code: [Predict_Future_Sales_Data_Analyze.ipynb](https://github.com/LynnBlanco/PredictFutureSales/blob/bb07c70f281e595f33e7b295f32dc1180464874f/Predict_Future_Sales_Data_Analyze.ipynb)
<img src="https://github.com/LynnBlanco/PredictFutureSales/blob/faf3745352fedbfe4340d5836125f2b136f9229b/images/DSAI%20Final%20Project%20Presentation%20II%20-%20Predict%20Future%20Sales_page-0003.jpg" width="800px"/>
<img src="https://github.com/LynnBlanco/PredictFutureSales/blob/faf3745352fedbfe4340d5836125f2b136f9229b/images/DSAI%20Final%20Project%20Presentation%20II%20-%20Predict%20Future%20Sales_page-0004.jpg" width="800px"/>
<img src="https://github.com/LynnBlanco/PredictFutureSales/blob/faf3745352fedbfe4340d5836125f2b136f9229b/images/DSAI%20Final%20Project%20Presentation%20II%20-%20Predict%20Future%20Sales_page-0005.jpg" width="800px"/>
<img src="https://github.com/LynnBlanco/PredictFutureSales/blob/faf3745352fedbfe4340d5836125f2b136f9229b/images/DSAI%20Final%20Project%20Presentation%20II%20-%20Predict%20Future%20Sales_page-0006.jpg" width="800px"/>

## Data Processing
- Code: [Feature.py](https://github.com/LynnBlanco/PredictFutureSales/blob/bb07c70f281e595f33e7b295f32dc1180464874f/Feature.py)
<img src="https://github.com/LynnBlanco/PredictFutureSales/blob/faf3745352fedbfe4340d5836125f2b136f9229b/images/DSAI%20Final%20Project%20Presentation%20II%20-%20Predict%20Future%20Sales_page-0008.jpg" width="800px"/>
<img src="https://github.com/LynnBlanco/PredictFutureSales/blob/faf3745352fedbfe4340d5836125f2b136f9229b/images/DSAI%20Final%20Project%20Presentation%20II%20-%20Predict%20Future%20Sales_page-0009.jpg" width="800px"/>
<img src="https://github.com/LynnBlanco/PredictFutureSales/blob/faf3745352fedbfe4340d5836125f2b136f9229b/images/DSAI%20Final%20Project%20Presentation%20II%20-%20Predict%20Future%20Sales_page-0010.jpg" width="800px"/>

## Model Training
- Code: [XGBModel.py](https://github.com/LynnBlanco/PredictFutureSales/blob/bb07c70f281e595f33e7b295f32dc1180464874f/XGBModel.py)

### XGBoost
```
XGBRegressor(max_depth=8, n_estimators=1000, min_child_weight=400, colsample_bytree=0.8, subsample=0.8, eta=0.04, seed=42, objective="reg:squarederror")
```

## Code Execution
Environment: ```Python 3.7.0``` </br>

- Install ```requirements.txt```
```
$ pip install -r requirements.txt
```
- Execute ```Feature.py```
```
$ python Feature.py
```
- Because the data feature is too big, you can download ```new_train.pkl``` in [here](https://drive.google.com/file/d/1-fF89c8yZ2Ty3whWeZ4lTgnl_zr-tBcU/view?usp=sharing). Execute ```XGBModel.py```
```
$ python XGBModel.py
```
