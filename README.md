**Overview**
By collecting, processing, and analyzing author data from top OR journals, this study investigates how gender representation has evolved over time and across different venues. Machine learning models are applied to classify author genders based on their first names, and the results are visualized to highlight trends and disparities.

**Tools & Methodologies**
- Tools: Python, Google Colab
- Key Libraries: pandas, scikit-learn, TensorFlow/Keras, SMOTE, matplotlib
- Data Sources:
Author data from Scopus

Gender-labeled first names from Kaggle Dataset (https://www.kaggle.com/datasets/monukhan/gender-prediction-by-using-name)

**The Process**
1. Data Collection
Author names were extracted from article metadata across 10 journals (2013–2022). First names were compared with a gender-labeled dataset to prepare for model training.

- Challenge: Gender name dataset showed imbalance (63% female vs 37% male).
- Solution: Applied SMOTE to oversample minority class and balance training data.

2. Data Preprocessing
- Extracted non-abbreviated first names
- Parsed publication year and journal from file names
- Saved as structured .csv for modeling

3. Gender Classification
Two machine learning models were trained:
- Naive Bayes
- Artificial Neural Networks (ANNs)

4. Model Evaluation
![Screen Shot 2025-04-23 at 20 37 47](https://github.com/user-attachments/assets/ddd2a972-276c-41a1-ada5-0098669be53a)

Result: ANN significantly outperforms Naive Bayes on all key metrics.

5. Analysis & Visualizations
- Year-over-Year Gender Trends
- Gender Distribution Across Journals
- Female Representation Over Time (by Journal)

Conclusion
- Gender trends fluctuated from 2013–2022, with a peak in 2018 and decline post-2019 (likely pandemic-related).
- Female authorship ranged from 16% to 27%, with IJOPM showing the highest representation.
- No statistically significant trends (P > 0.05) were detected in any journal—indicating that observed changes may be due to randomness rather than systemic shifts.


