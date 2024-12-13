[![](Image.jpg)](https://unsplash.com/photos/black-android-smartphone-on-black-textile-3PyBkxgTiL0)
## Phone Price Prediction

### Overview
The Phone Price Prediction project aims to classify mobile phones into different price ranges based on their technical specifications. Using machine learning algorithms, the project evaluates features like battery power, RAM, processor cores, and more to predict the price category of a phone. This repository demonstrates data preprocessing, feature selection, and model optimization techniques to achieve accurate predictions.

<br>

### Process Workflow

#### Data Collection & Cleaning
- **Dataset:** A dataset of mobile phone specifications and their respective price ranges is used.
- **Preprocessing:**
  - Removed irrelevant columns such as pixel dimensions and screen dimensions (`px_width`, `px_height`, `sc_w`, `sc_h`, `m_dep`).
  - Ensured the data quality by handling missing or inconsistent values.

#### Feature Engineering
- Selected key features like battery power, processor cores (`n_cores`), RAM, and more to train the model.
- Performed data scaling using `StandardScaler` to normalize feature distributions.

#### Model Building
- Tested multiple machine learning models, including:
  - **Decision Tree Classifier (DT)**
  - **Random Forest Classifier (RF)**
  - **Support Vector Classifier (SVC)**
- Optimized hyperparameters using `GridSearchCV` and `RandomizedSearchCV` for better performance.

#### Model Evaluation
- Splitted the dataset into training and testing sets using an 80-20 ratio.
- Evaluated models using metrics such as:
  - **Accuracy Score**
  - **Classification Report**

<br>

### Results
The project achieved the following results:
- **Best Model:** Random Forest Classifier, providing the highest accuracy.
- **Performance Metrics:**
  - Accuracy scores for each model are reported in the notebook.
  - The classification report highlights precision, recall, and F1 scores for each price range.

<br>

### Repository Contents

- **Data:**
  - [Original dataset](https://www.kaggle.com/datasets/atefehmirnaseri/cell-phone-price) and cleaned data (in the file) are available.
- **Notebook:**
  - The main Jupyter Notebook (`Price Prediction.ipynb`) contains the complete workflow, from preprocessing to evaluation.
- **README.md:**
  - Documentation summarizing the project's objectives, methodology, and results.

<br>

### How to Contribute
We welcome contributions to enhance the project! Follow these steps:
1. Fork the repository.
2. Create a new branch for your changes.
3. Submit a pull request with a clear description of your modifications.

<br>
---

#### Additional Notes
This project demonstrates fundamental data science and machine learning techniques and serves as a learning tool for classification tasks.
