# Impute Missing Values

This is a Kaggle competition about imputing missing values, which won the first place.

The ability to effectively handle missing data is crucial in many data analysis tasks, as missingness can introduce bias and reduce the accuracy of statistical models. In this Kaggle competition, our goal is to develop robust methods for imputing missing values in a data set provided to us. All values in the dataset are numerical. Furthermore, the missing data in this data set is generated according to a specific mechanism, making it an interesting challenge to tackle.

To decoding the missing data generation process, understanding the missingness pattern is important. By doing the exploratory data analysis (EDA), we could observe that significant correlations are observed among neighboring variables (e.g., $V_i$ and $V_{i+1}$ for $i$ = 1, $\ldots$ , 50), while correlations between distant variables (e.g., $V_1$ and $V_50$) are relatively low. Deploying the imputation techniques which consider time series might be useful, since these missing values might be linked to time. In this case, we consider different imputation methods, including Multiple Imputation by Chained Equations (`MICE`) algorithm, Classification and Regression Tree (`CART`), Imputation on Univariate Time Series (`imputeTS`), and Gaussian Conditional Imputation.

The results of our imputation analysis, as evaluated through the mean square error (MSE) metric, provide valuable insights into the effectiveness of different imputation methods in handling missing data. The result shows that the imputation method based on Univariate Time Series outperforms other methods in terms of imputation accuracy. All in all, our results underscore the importance of selecting appropriate imputation methods tailored to the characteristics of the data set.

Please refer to 'Kaggle_Report.pdf' for a detailed overview of my written report.
