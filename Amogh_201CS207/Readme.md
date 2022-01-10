## Submission:
After going through dataset found there are null values\
Dropped rows with Null values.\
Checked for correlation among features.\
Would drop correlated features but since no improvement in model performance decided to keep all.\
Plotted all values to check for any significant imbalance in output(prices). None found.\
Did Train, val, test split in the ratio 8:1:1.\
Used Robust Scaler, Also tried Standard Scaler.\
Used Lazy Predict to see performance of some popular models.\
Found Boosted trees and Decision Trees to perform better.\
Tried Neural Networks.\
Neural network gave a result with a decent RMSE of 48,000.\
Went ahead with Decision Trees.\
Chose XGB regressor and optimized it.\
Gave a result with RMSE around 46,500.\
Tried Catboost Regressor.\
Catboost gave the best Score with RMSE around 45,000.\

## ML Interest
I have recently got into ML and I have a lot of interest in it. I want to go deeper into that field and explore more.
I learnt about many of these models through a kaggle contest that I looked into. I also want to explore RL and more. Looking forward to this Sub yantra.

PS. Sorry for the long Catboost output idk how to make it go away on github(was compressed and fine on my pc)
