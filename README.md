# SMS Spam Classifier
This is a Machine Learning project that classifies SMS messages as either **Ham** (Legitimate) or **Spam**. The project involves data preprocessing, exploratory data analysis (EDA), text vectorization, and model evaluation to achieve high accuracy and precision.
## 🚀 Features
- **Data Cleaning**: Handled missing values and duplicates.
- **EDA**: Visualized the distribution of Ham vs Spam using Pie charts and Histograms.
- **Text Preprocessing**: 
    - Tokenization
    - Removing special characters
    - Removing stop words and punctuation
    - Stemming (using PorterStemmer)
- **Word Cloud**: Visualized the most frequent words in Spam and Ham messages.
- **Model Building**: Trained and compared multiple algorithms like Naive Bayes and Random Forest.
- **High Performance**: Achieved excellent precision and accuracy scores.

## 🛠️ Tech Stack
- **Language**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, NLTK, Matplotlib, Seaborn
- **Environment**: Jupyter Notebook

## 📊 Project Workflow

### 1. Data Cleaning
Initially, the dataset contained some unnecessary columns. We kept the target (`v1`) and the message (`v2`) and renamed them to `target` and `text`. Labels were encoded (Ham: 0, Spam: 1).

### 2. Exploratory Data Analysis (EDA)
Analysis showed that the dataset is imbalanced (more Ham than Spam). We also engineered features like:
- Number of characters
- Number of words
- Number of sentences

### 3. Data Preprocessing
Text data was transformed through:
- Lowercasing
- Tokenization
- Removing Stop words
- Stemming

### 4. Model Building & Evaluation
We converted the text into vectors using **TF-IDF Vectorization**. Various models were tested, with **Multinomial Naive Bayes** performing the best in terms of precision.

## 📈 Results
The model ensures that legitimate messages are not wrongly classified as spam, which is crucial for this use case.

| Model | Accuracy | Precision |
| :--- | :--- | :--- |
| MultinomialNB | ~97% | 100% |

## 📁 File Structure
- `spam.csv`: The raw dataset.
- `sms-spam-detection.ipynb`: The complete Jupyter Notebook with code and analysis.
- `README.md`: Project documentation.

## ⚙️ How to Run
1. Clone the repository.
2. Install dependencies: `pip install pandas numpy scikit-learn nltk matplotlib seaborn`.
3. Run the Jupyter Notebook.
