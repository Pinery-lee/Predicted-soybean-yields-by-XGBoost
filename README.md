# Predicted-soybean-yields-by-XGBoost
 Repository of "[A county-level soybean yield prediction framework coupled with XGBoost and multidimensional feature engineering](https://doi.org/10.1016/j.jag.2023.103269)" and the paper of "Investigating how yield trends affect machine-learned crop yield predictions: Comparing detrending approaches using XGBoost" (under review). These two papers make up [my graduation thesis](https://github.com/Pinery-lee/Predicted-soybean-yields-by-XGBoost/blob/main/thesis/李远超_机器学习和多维特征耦合的县级尺度作物单产预测方法和框架.pdf).

------

"[A county-level soybean yield prediction framework coupled with XGBoost and multidimensional feature engineering](https://doi.org/10.1016/j.jag.2023.103269)" is my first paper mainly conducted some experimental work, including selection of predictor variables, machine model comparisons and explorations in feature engineering. So at that time, the code was experimental. Therefore, I used Jupyter Notebook to ensure that I could run and output the parts I wanted anytime, anywhere. Of course, the code is somewhat messy and dirty, please forgive me. The code can be categorized into two types: data preprocessing and model prediction. The code for the first paper is unavailable here (It has been improved and used for the second paper and my graduation thesis, and at that time, I was not proficient in using version control software). But The first ten rows of data from the soy input data can be viewed [here](https://github.com/Pinery-lee/Predicted-soybean-yields-by-XGBoost/tree/main/data/first_paper), showing what features (columns) were used and it only involves soybean yield data in the first data. The full soybean input data is available here: [all-data.csv in aliyundrive](https://www.aliyundrive.com/s/BWngaLBpLbL) or [all-data.csv in google drive](https://drive.google.com/file/d/1sN88IUqi8iH0fuI5kNcRyG_zR0UYQhuL/view?usp=sharing).

"Investigating how yield trends affect machine-learned crop yield predictions: Comparing detrending approaches using XGBoost" (under review) is the second paper, which specifically explores yield trends based on the first paper. The data in this paper involves both soybean and maize yields data. Many modifications have been made to the code, which can be found here. Additionally, you can access all the processed data here and here (later).

The graduation thesis systematically integrates both of them and conducts some additional explorations, such as examining the difference between single-factor and multi-factor predictions. The data is available [input_soybean_rename.csv](https://www.aliyundrive.com/s/Qu5ipe717D6) and [input_maize_rename.csv](https://www.aliyundrive.com/s/6ve7iodqS1s).



---Prediction Process---(Taking the code from the graduation thesis as an example, you need to generate feature importance first before starting training and prediction.)

1. Read data in .../graduation_thesis/model.ipynb.
2. Generate feature importance.
3. In .../graduation_thesis/average_feature_importance.ipynb, consolidate multi-year feature importance into one table/average_feature_importance.csv.
4. Read data again in .../graduation_thesis/model.ipynb and read /average_feature_importance.csv.
5. Make predictions.



