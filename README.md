# Sleep Quality Prediction with Machine Learning

A supervised machine learning project that predicts sleep quality based on lifestyle, health, and coffee consumption data.

## Dataset

**GlobalCoffeeHealth Dataset** - A synthetic dataset with 10,000 records from 20 countries containing information about coffee consumption, sleep, health, and lifestyle.

### Features
- **Age**: 18-80 years
- **Gender**: Male, Female, Other
- **Country**: 20 different countries
- **Coffee_Intake**: Daily cups (0-10)
- **Caffeine_mg**: Daily caffeine intake
- **Sleep_Hours**: Average sleep hours (3-10)
- **BMI**: Body Mass Index (15-40)
- **Heart_Rate**: Resting heart rate (50-110 bpm)
- **Stress_Level**: Low, Medium, High
- **Physical_Activity_Hours**: Weekly exercise (0-15 hours)
- **Health_Issues**: None, Mild, Moderate, Severe
- **Occupation**: Office, Healthcare, Student, Service, Other
- **Smoking**: Yes/No
- **Alcohol_Consumption**: Yes/No

### Target Variable
- **Sleep_Quality**: Poor, Fair, Good, Excellent

## Methodology

1. **Data Preprocessing**
   - Label encoding for categorical variables
   - Removed ID and Sleep_Hours columns
   - Train/test split with stratification

2. **Model Evaluation**
   - Tested 10 different algorithms
   - Compared performance with original, standardized, and normalized data
   - Used 10-fold cross-validation

3. **Hyperparameter Optimization**
   - GridSearch for KNN, Naive Bayes, SVM
   - RandomizedSearch for complex models

## Results

**Best Model**: Naive Bayes
- **Accuracy**: 86.5%
- **Configuration**: Original dataset (no scaling needed)

### Model Performance Comparison
- Naive Bayes: 86.5%
- SVM (standardized): 86.5% 
- Random Forest: 86.4%
- Gradient Boosting: 86.4%
- KNN (optimized): 86.3%

## Key Findings

- Naive Bayes performed best without data preprocessing
- Standardization improved KNN and SVM performance significantly
- Ensemble methods showed consistent good performance
- The model successfully identifies relationships between lifestyle factors and sleep quality

## Usage

The trained model can predict sleep quality for new individuals based on their:
- Demographics and health metrics
- Coffee/caffeine consumption patterns
- Physical activity levels
- Stress and lifestyle factors

## Tools & Libraries

- **Python 3.x**
- **Scikit-learn**: Machine learning algorithms
- **Pandas**: Data manipulation
- **NumPy**: Numerical computing
- **Matplotlib**: Data visualization

## Files

- `MVP_ML.ipynb`: Main notebook with complete analysis
- `coffee_health.csv`: Dataset file
- Model comparison and evaluation results

---

*Note: This dataset is synthetic and designed for educational and research purposes in machine learning and health analytics.*
