# mushroom-classifier
Asymmetric classification project to prioritize safety in mushroom foraging.


## 🎯 Goal
The goal of this project is to classify mushrooms as edible or poisonous. Because eating a poisonous mushroom is fatal, the model is optimized for **100% Recall** (Safety First).

## 🛠️ Tools Used
- **Python / Google Colab**
- **Scikit-Learn:** RandomForest, CalibratedClassifierCV
- **Pandas/Numpy:** Data manipulation

## 📈 Methodology
- **Calibration:** Used Sigmoid calibration to ensure probability scores were accurate.
- **Asymmetric Thresholding:** Instead of the standard 0.5 threshold, I implemented a dynamic threshold calculated to catch every poisonous sample (Recall = 1.0).
- **Categorical Handling:** Used OneHotEncoding and treated missing values as 'unknown' to capture hidden toxicity patterns.

## 🏆 Competition Results
- The final model was deployed on unlabeled foraged data for a classroom competition.
- Achieved high edibility rates while maintaining absolute safety.
