## Dataset is large, please download it from kaggle:
 https://www.kaggle.com/c/msk-redefining-cancer-treatment/
 
 Download training_variants.zip and training_text.zip 
 unzip and put both the unziped files in training folder of same folder.

# Project overview
## It is multiclass(9-class) classification problem, cost of misclassification is very high.
### KPI(Key performance indicator) : Multiclass Log Loss  and Confusion matrix.

## There were 3 features:
<ul>
  <li>Gene : categorical</li>
  <li>Variation : categorical</li>
  <li>Text : text</li>
</ul>
## Categorical features are transformed using 2 technique:
<ul>
  <li>OneHot Encoding: high dim</li>
  <li>Response coding: low dim</li>
  <li>Text : text</li>
</ul>
## Univariate analysis
Univariate analysis using only gene, only variation, only text</br>
text was the best among these three.</br>
## I have tried many models, models are listed bellow:
<ul>
 <li>1. MultinomialNB Naive Bayes </li>
 <li>2. KNN</li>
 <li>3. Logistic regression with class balancing</li>
 <li>4. Logistic regression without class balancing</li>
 <li>5. Linear Support vector machine</li>
 <li>6. Random forest + response coded data </li>
 <li>7. Random forest + OneHotEncoded data </li>
 <li>8. Stacked classifier (LR+SVC+NaiveBayes) </li>
 <li>9. Majority voting classifier</li> 
</ul>

# I got the best result using Logistic regression with class balancing.
