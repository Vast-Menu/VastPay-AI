# Sales Insight Generator for Merchants

## 📌 Overview
This Python script provides smart sales analytics for merchants by connecting to a MySQL database and using OpenAI to summarize and interpret sales data. It helps the store owner understand total sales, buyer count, and top-performing branches.

## 🧠 Features
- Retrieves and analyzes sales data.
- Calculates total sales, number of buyers, top-selling branches.
- Uses AI to summarize performance insights.
- Helps merchants improve strategic decisions.

## 🗃️ Data Sources
- Sales transactions from MySQL database.
- Buyer IDs, amounts, branch names.

## 🧹 Preprocessing
- Removal of incomplete or null sales entries.
- Grouping and aggregation by branch and date.
- Handling currency formats and date parsing.

## 🛠️ Tech Stack
- **Language**: Python
- **AI Model**: OpenAI GPT API
- **Database**: MySQL
- **Libraries**: `pymysql`, `pandas`, `openai`

## 🚀 How to Run
1. Install dependencies:
   ```bash
   pip install openai pymysql pandas
   ```
2. Configure your database credentials and OpenAI key.
3. Run the script:
   ```bash
   python sales_insights.py
   ```

## 📈 Output
- Printed or exported summary of:
  - Total sales
  - Number of unique buyers
  - Top-performing branches
  - AI-generated performance report