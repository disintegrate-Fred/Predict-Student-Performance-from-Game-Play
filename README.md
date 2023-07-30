# Predict-Student-Performance-from-Game-Play
1. It's suggested to install the necessary packages for running: 
polars 
sklearn 
catboost 
lightgbm

2. First, run step1_train_fe_fs.ipynb. 
The main functions of this code are:
(1) Feature engineering, save the generated feature files as df1.pkl, df2.pkl, df3.pkl
(2) Feature selection

3. Run step2_train_stage1.ipynb, save the model file to the 'savedata' folder. 
The main function of this code is to train the LGB model using the feature importance from the feature selection.

4. Run step3_train_stage2.ipynb, also save the model file to the 'savedata' folder. 
The main function of this code is to correct subsequent questions using the level of other questions.
The principle of this step is:
If the correctness of the previous question is high, the correctness of the subsequent questions will also become high.

5. Finally, run step4_infer.ipynb. This part of the code is used for submission and inference.
