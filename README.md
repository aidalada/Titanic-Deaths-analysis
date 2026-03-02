**Overview**
This project predicts which passengers survived the Titanic shipwreck. It uses the Kaggle Titanic dataset and tests different machine learning models to find the highest accuracy.

**Data Processing**

* Filled missing data in columns like Fare and Age.
* Extracted ticket letters and grouped rare tickets into a single 'Rare' category.
* Used Label Encoding to change text columns like Embarked and Deck into simple numbers.
* Created a new Family Size column by adding the sibling and parent columns together.
* Scaled the numbers using StandardScaler so models like SVM could read them correctly. The scaler was saved using joblib to use on the test data.

**Models Tested**

* Support Vector Machine (SVM)
* AdaBoost

**Results**

* The best Kaggle public score was 0.75837 using the AdaBoost model.
* The SVM model achieved a score of 0.73444 after fixing the data scaling step.
* Creating the Family Size column was tested, but the AdaBoost model without it kept the highest score.

**How to Run**
The code is written in a Jupyter Notebook. It requires the train.csv and test.csv files from Kaggle. Run the data cleaning steps first, then run the model training cells to create the final submission.csv file.

---

**Kaggle scorings**:

<img width="1329" height="434" alt="Screenshot_20260302_164206" src="https://github.com/user-attachments/assets/6f1478ad-7890-4dfb-86d0-a00576f6ed79" />
