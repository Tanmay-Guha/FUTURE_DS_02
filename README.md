# 📩 Customer Support Ticket Analysis
This project analyzes customer support ticket data to extract common issues, visualize trends, and provide actionable suggestions for improving support efficiency.

---

## 📄 Description

The script performs the following steps:

1. Loads support ticket data from a CSV file.
2. Cleans and preprocesses ticket descriptions.
3. Identifies frequently occurring issues using word frequency.
4. Visualizes common problems and ticket categories.
5. Provides a summary report with key recommendations.

---

## 🛠️ Technologies & Libraries Used

* Python
* Pandas
* NLTK
* Matplotlib
* Regex
* Collections (Counter)
* Google Colab (for development)

---

## 📂 Input

* **CSV File**: `customer_support_tickets.csv`

  * Required columns:

    * `Ticket Description` (for text analysis)
    * `Category` *(optional but used for grouped visualizations)*

---

## 🔍 Features

### ✅ Text Cleaning & Preprocessing

* Converts to lowercase
* Removes digits and punctuation
* Tokenizes text and removes stop words using NLTK

### ✅ Common Issue Identification

* Uses word frequency (`Counter`) to extract top 20 common words
* Helpful for understanding major customer concerns

### ✅ Visualizations

* Bar chart of top 20 frequent words in tickets
* Horizontal bar chart of ticket volume per category (if `Category` column exists)

### ✅ Summary Report

Includes:

* Total ticket count
* Most frequent words
* Suggestions for improving support handling

---

## ▶️ How to Run

1. Upload your dataset as `customer_support_tickets.csv`.
2. Run the notebook in Jupyter or Google Colab.
3. The output will include:

   * Cleaned text column
   * Top issues visualization
   * Optional category-wise ticket plot
   * Summary report with insights and recommendations

---

## 📈 Output

* Bar plot of most common support issues
* Category-wise ticket distribution (if available)
* Printed summary report:

  ```json
  {
    "Total Tickets": ...,
    "Most Common Words": [...],
    "Top Suggestions": [
      "Automate replies for frequent issues...",
      "Improve knowledge base articles...",
      "Use categorization to assign tickets..."
    ]
  }
  ```

---

## ⚠️ Notes

* Ensure NLTK data is downloaded:

  ```python
  nltk.download('stopwords')
  nltk.download('punkt')
  ```

* Adjust the column name if your dataset uses a different name for ticket descriptions.

---

## ✍️ Author

* **Name**: *TANMAY GUHA*
* **Contact**: *tanmayguha15@gmail.com*
