# AmazonSentimentAI 🔍📢  

**Analyzing customer sentiment through Amazon reviews** helps businesses understand **customer satisfaction trends, product feedback, and areas of improvement**. This project applies **natural language processing (NLP) and machine learning** to classify customer reviews as **positive or negative**, providing valuable insights into consumer behavior.

---

## 🚀 Project Overview

Sentiment analysis is essential for monitoring **customer feedback** and improving **product quality and service**. This project aims to:
- **Classify Amazon reviews** into **positive** and **negative** sentiments.
- **Leverage NLP techniques** for text preprocessing and feature extraction.
- **Compare classification models** to determine the best-performing approach.

The model is trained using **Naïve Bayes and Logistic Regression** to predict whether a review expresses **satisfaction or dissatisfaction**.

---

## 📊 Dataset Overview

The dataset includes **3,150 customer reviews** for Amazon's **Alexa** product. Each record contains:
- **Review text** (customer feedback)
- **Rating** (1-5 stars)
- **Feedback** (1 = positive, 0 = negative)

### 🔍 Sample Data
| Rating  | Date | Variation | Verified Review | Feedback |
|---------|------------|------------|------------------|----------|
| 5       | 31-Jul-18  | Charcoal Fabric | Love my Echo! | 1        |
| 5       | 31-Jul-18  | Charcoal Fabric | Loved it!      | 1        |

📌 **Source:** Kaggle – Amazon Alexa Reviews Dataset  

---

## 🛠️ Setting Up the Project

1️⃣ **Clone the Repository**
```sh
git clone https://github.com/FazilMammadli/AmazonSentimentAI.git
cd AmazonSentimentAI
```

2️⃣ **Create and Activate a Virtual Environment**
```sh
python -m venv .venv
.venv\Scripts\activate  # Windows
source .venv/bin/activate  # Mac/Linux
```

3️⃣ **Install Required Libraries**
```sh
pip install -r requirements.txt
```

4️⃣ **Run the Jupyter Notebook**
```sh
jupyter notebook
```
Open and execute `Sentiment_Analysis.ipynb` to explore the dataset and train models.

---

## 🔬 Data Preprocessing & Cleaning

### **1️⃣ Handling Missing & Unnecessary Data**
- Checked for **missing values** (none found).
- Removed **unnecessary columns** (`rating` and `date`) as they **do not contribute to sentiment analysis**.

### **2️⃣ Data Visualization**
- **Sentiment distribution in dataset**  
  ![Sentiment Distribution](https://user-images.githubusercontent.com/107464383/196098503-7cf65ccb-6191-4548-b76c-6e30a4ed8e7f.PNG)

- **Review ratings breakdown**
  ![Ratings Breakdown](https://user-images.githubusercontent.com/107464383/196098624-adbc3729-e75c-42e3-87b3-d217afbfe5f2.PNG)

- **Product variation analysis**
  ![Product Variations](https://user-images.githubusercontent.com/107464383/196098752-3dd27916-7bc1-4d85-a57f-a77cda472f66.PNG)

### **3️⃣ Text Processing Steps**
We cleaned the review text by:
✅ **Removing punctuation** (`,`, `.`, `!`, `?` etc.)  
✅ **Eliminating stopwords** (e.g., _the, is, and, I, you, etc._)  
✅ **Applying tokenization and stemming**  

✅ **Example of cleaned text:**  
**Original:** "_I absolutely love this product! It’s amazing!_"  
**Processed:** "_absolut love product amaz_"  

---

## 🤖 Machine Learning Models Used

### **1️⃣ Naïve Bayes Classifier**
✅ **Fast and effective for text classification**  
✅ **Good performance on small datasets**  
✅ **Used MultinomialNB for sentiment analysis**

📌 **Confusion Matrix**
  ![Naive Bayes Confusion Matrix](https://user-images.githubusercontent.com/107464383/196121222-1ff69d37-e720-40fa-87a5-a0ca4c035abe.PNG)  

📌 **F1 Score**
  ![Naive Bayes F1 Score](https://user-images.githubusercontent.com/107464383/196122894-1a50c563-3716-4469-8ddc-9026be737db5.PNG)  
🔹 **Accuracy: 93%**  

---

### **2️⃣ Logistic Regression**
✅ **Handles large feature sets well**  
✅ **Provides slightly higher accuracy than Naïve Bayes**  

📌 **Confusion Matrix**
  ![Logistic Regression CM](https://user-images.githubusercontent.com/107464383/196125764-51041d6f-c65f-4ff4-a4c1-8fe51155ca3f.PNG)  

📌 **F1 Score**
  ![Logistic Regression F1 Score](https://user-images.githubusercontent.com/107464383/196126152-9dc15fef-5577-4d1d-a729-04d9fccab31a.PNG)  
🔹 **Accuracy: 94%**  

---

## 🔑 Key Insights

📌 **Customer sentiment is overwhelmingly positive** – most reviews have **5-star ratings**.  
📌 **Logistic Regression outperforms Naïve Bayes** in this dataset, achieving **94% accuracy**.  
📌 **Word clouds** provide insights into common themes in **positive vs. negative reviews**.  

💬 **Common words in positive reviews:** “love,” “great,” “amazing,” “works.”  
💬 **Common words in negative reviews:** “disappointed,” “bad,” “waste,” “return.”  

---

## 📌 Business Applications

💡 **Product Feedback Analysis**  
- Identify **common complaints** and improve product features.  
- Track **customer sentiment over time** for **product development**.  

💡 **Marketing Insights**  
- Highlight **positive reviews** in **advertisements and promotions**.  
- Address **negative sentiment trends** to improve **brand reputation**.  

💡 **Automated Customer Support**  
- Use sentiment classification to **prioritize urgent customer issues**.  
- Implement AI-driven **chatbots for handling common complaints**.  

---

## 🎯 Conclusion

This project successfully demonstrated how **machine learning and NLP** can classify Amazon reviews into **positive and negative sentiments**. 

🚀 **Key Takeaways:**  
✅ **Text preprocessing is crucial** for sentiment analysis.  
✅ **Logistic Regression performed best** with **94% accuracy**.  
✅ **Machine learning models can enhance customer feedback analysis** in E-commerce.  

---

## ⭐ Support & Contributions

If this project was useful, **drop a ⭐ on GitHub**!  
For feedback or contributions, **submit a pull request**! 🚀  
