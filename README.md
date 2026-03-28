# 🤖 Autonomous SQL Agent for Supply Chain Risk Detection

## 📌 Overview
This project builds an **AI-powered SQL agent** that can automatically analyze supply chain data and detect potential risks using natural language queries.

By leveraging **LLMs (Google Gemini)** and **relational data modeling**, the system translates user questions into SQL queries, retrieves relevant data, and generates **business-oriented insights**.

---

## 🎯 Objective
To automate **supply chain risk detection** by:
- Converting natural language queries into SQL
- Extracting insights from structured datasets
- Providing actionable, business-level conclusions

---

## ⚙️ How It Works

1. User asks a question (e.g., *"Which suppliers have the highest delay risk?"*)
2. The AI agent:
   - Understands the query
   - Generates an optimized SQL query
3. SQL query is executed on the database
4. Results are analyzed by the model
5. Final output includes:
   - 📊 Data results
   - 🧠 Business insights & recommendations

---

## 🧠 Example Workflow

**User Input:**
**Generated SQL:**
```sql
SELECT region, COUNT(*) AS disruption_count
FROM supply_chain_data
WHERE disruption_flag = 1
GROUP BY region
ORDER BY disruption_count DESC;

##Output Insight:

Regions like Asia-Pacific show higher disruption counts, indicating potential logistical inefficiencies or supplier instability. Businesses should consider diversifying suppliers or strengthening inventory buffers in these regions.
