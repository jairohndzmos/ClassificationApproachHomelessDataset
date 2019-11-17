# Classification Approach using Bogota-Colombia homeless survey dataset

# Introduction

This repository shows a training model that applying four supervised classification algorithms, using 14 features and one binary label, testing a dataset publicated in National Colombian Data Archive '(ANDI)'

# Dataset

The dataset, provide by the study named as COLOMBIA-Censo de Habitantes de Calle - CHC 2017 - Bogotá, D.C', from this one, has been selected  14 predictive features (source: [http://microdatos.dane.gov.co/index.php/catalog/548/study-description](http://microdatos.dane.gov.co/index.php/catalog/548/study-description)):

 

 - P22: Principal reason that started living as homeless (Discrete-Nominal)
 - P26_1: Recived helped by (Discrete-Nominal)
 - P30_1: Consumed drugs (Discrete-Nominal)
 - P9R: Gender (Discrete-Binary)
 - P17S3: strugglin Mental and emotional issues? (Discrete-Binary)
 - P16S9: strugglin Respiratory and cardiac issues on daily activities? (Discrete-Ordinal)
 - P17S7: Sexually transmitted disease? (Discrete-Binary)
 - P28R: Education (Discrete-Ordinal)
 - P16S6: Learn, remind, handle decision? (Discrete-Ordinal)
 - P8: Age (Discrete-Numeric)
 - P29: Money source (Discrete-Nominal)
 - P31: There's some understanding about government rehab programs? (Discrete-Binary)
 - P33_1: Fear for one's life  (Discrete-Binary)
 - P24: Which reason do you still living on the streets? (Discrete-Nominal)

There's one target:

 - P32: Do you use goverments rehab programs? (Discrete-Binary)


## Approach
Has been employing four models for classification target:

 - K-Nearest Neighbor
 - Decision Tree
 - Logistic Regression
 - Support Vector Machine
 
Testing in some parameters that could improve particular model's final accuracy

## Results

Taking as indicator f1 weighted average score, might said SVM approach with linear kernel parameter shows better results, introduced by following table:
      

              precision    recall  f1-score   support

           1       0.73      0.80      0.76       361
           2       0.75      0.68      0.72       329
    accuracy                           0.74       690
    macro avg       0.74     0.74      0.74       690
    weighted avg    0.74     0.74      0.74       690


