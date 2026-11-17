# Medical Appointment No-Show Prediction

Graduation project (B.Sc. Biomedical Informatics, Nile University, 2024).
This project predicts whether a patient will miss a medical appointment, using supervised machine learning.

## Team
Team of five students. My contribution (Farah Amro Mohamed Mahmoud):
- Data cleaning and preprocessing
- Logistic Regression model (tuned with GridSearchCV)
- Writing the project report

## Dataset
- Dataset: Medical-appointments-no-show-en.csv (not included in this repository; provided by the course instructor and contains patient-level records).
- Size: 49,593 appointments, 26 columns
- Target: no_show (4,832 yes = 9.7%, 44,761 no = 90.3%)

## Models (team notebook)
Logistic Regression, Random Forest, Gradient Boosting, Voting ensemble, KNN, Neural network (Keras), SVM, Decision Tree, Gaussian Naive Bayes, Multinomial Naive Bayes.

## Results (test accuracy)
| Model | Accuracy |
| Logistic Regression | 0.900 |
| Random Forest | 0.900 |
| Gradient Boosting | 0.900 |
| Voting ensemble | 0.900 |
| KNN | 0.899 |
| Neural network | 0.899 |
| SVM (linear) | 0.899 |
| Decision Tree | 0.898 |
| Gaussian Naive Bayes | 0.877 |
| Multinomial Naive Bayes | 0.803 |

Majority-class baseline (always predict "attended"): 0.903.

## Limitations
- The classes are imbalanced, so accuracy is close to the baseline. Precision and recall for no-shows should be reported.
- Some cells re-split the training data, so test sets are not identical across models.

## How to run
The dataset contains patient-level records and is not distributed with this repository, so the notebook cannot be run end to end without access to it. With the CSV obtained from the data owner (course instructor), upload it to the Colab working directory as `/content/Medical-appointments-no-show-en.csv`, install the libraries in `requirements.txt`, and run all cells.
