### Approach
1. Imported the required modules for the task.
2. Uploaded the provided dataset
3. Created a Pandas Dataframe from the dataset for easier handling of the data
4. Checked the head and tail (top and bottom 5 rows) of the dataframe to get an initial raw idea about the data
5. Checked the info to uderstand the non-null count and Data Type of the columns
6. Since the info shows difference in null count for different columns, removed the rows (data) having NAN value i.e. removed the incomplete data
7. Rechecked the info to confirm the change
8. Checked the Data Description to understand the distribution of the data in the columns
9. Checked for existing correlations and plotted a heatmap to better visualize the correlation data. Also used pairplot to chek the realtions between the columns
10. Extracted the target dataseries ad features dataframe from the given data
11. Split the data into testing and training sets (3:7, which is good considering the size of the data provided)
12. Used Linear Regression Model
13. Checked for the model score for the training dataset. There was 63.6% accuracy. Not very promising
14. But still proceeded to use the model for prediciting the values of the testing dataset. Checked the score and the errors. Plotted the errors for easier analysis. The error curve showed a bell curve centered around 0, making the model acceptable. A scatter plot between the actual values and the prediciton also confirmed the same by showing acceptabe linear behaviour. But the model score, showed that the model wasn't very promising as there was only a 63.8% accuracy.
15. To create a better model, proceded to use Random-Forest Regressor Algorithm. I could've used Decision Tree, but Random Forest being an ensemble algorithm would provide better results and prevent overfitting of the data.
16. Used Random Forest Regression with 100 Decision Trees (Larger number might have been better, but considering the large size of the dataset, it could lead to high training time)
17. Repated the same procedure as Linear-Regression for evaluating the model. The results were much better. Narrow peaked bell curve of error and better linear scatter plot of target vs predicition were the inital indicators of the same. The R2 score of 82.4% was achieved which is considered very good. The Mean Errors observed were also lesser than that of LR. 
18. I could have further optimized the model by tuning the hyper-paramters using gridsearchcv, but since the accuracy seemed pretty good, stopped with the model. It was a trade-off between the accuracy and time for training 

### Interest in ML
Considering amount of data generated on a daily basis in various fields, it is very effective and interesting to have the computer analyze and make data-driven recommendations and decisions. Finding relationships between data and using it for predictions is very exciting. But for better results, larger datasets are required and processing it becomes humanly impossible. Also it is fascinating to build data-driven models that simulate the real world. Considering these I have been exploring the field for some time now and would love to go deeper. 
