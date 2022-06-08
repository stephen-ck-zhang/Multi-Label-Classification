# Multi-Label-Classification

_This is the class project in New York University Natural Language Processing class during 2022 Spring. All rights reserved._

**A movie can embody multiple genres, and we create a system that can predict movie genres based on its plot overview.**

**The paper can be accessed at:** ([click here](https://drive.google.com/file/d/1Eh8ZDyB6aEgOvDdjTpPwRtkI3CpvSt9m/view?usp=sharing))

## 
The system is based on the existing movie dataset, The Movies Dataset, and it is publicly available on Kaggle. ([click here](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset?select=movies_metadata.csv)) And we have downloaded for our experiment, please check it in _movies_metadata.csv_, which includes metadata of over 45,000 movies.


There are four models built, including our final system, RoBERTa; two comparison models, GloVe+CNN & GloVe+BiLSTM; and our baseline, TF-IDF+LR.
##
**Data_Preprocessing.ipynb**
This is our data preprocessing & cleaning file. Data with non-English overviews or invalid overviews (NaN) aredropped. Raw genre labels, originally in JSON
format, are transformed into Python lists of strings and stored Pandas Dataframe form. Also, The dataset is split into 70% of training data, 15% of validation data, and 15% of test data. The split data is stored into 3 CSV files for our experiment, you can check it in _Data_ file.
##
**MovieClassification_Baseline.ipynb**
This is the implementation of our baseline, TF-IDF+Logistic Regression. Please make sure the envirnoment is set up and run the cells to check the results. Also, keeping the preprocessed dataset in the same directory.
##
**MovieClassification_BiLSTM.ipynb**
This is the implementation of our comparison models, GloVe+BiLSTM & GloVe+CNN. Please make sure the envirnoment is set up and run the cells to check the results. Also, keeping the preprocessed dataset in the same directory.
##
**MovieClassification_RoBERTa.ipynb**
This is the implementation of our final system, RoBERTa. Please make sure the envirnoment is set up and run the cells to check the results. Also, keeping the preprocessed dataset in the same directory.

Note, you can use our preprocessed data in the _Data_ file. This is the resulting data by runing our _Data_Preprocessing.ipynb_ file.

##
People who contribute this system: Andy Wang (gw1035@nyu.edu), Stephen Zhang (cz1906@nyu.edu), Koji Liu (ml7324@nyu.edu), Matthew Li (sl7029@nyu.edu)
