#  Category Wise Profit Automation using n8n

##  Project Overview

This project automates category-wise profit analysis using **n8n**. It reads sales data from **Google Sheets**, processes the data using **JavaScript**, calculates the total profit for each category, and sends the final report to **Telegram**.

---

#  Workflow

```
Manual Trigger
      │
      ▼
Google Sheets
      │
      ▼
JavaScript Code
      │
      ▼
Telegram
```

---

#  Workflow Explanation

### 1️ Manual Trigger
- Starts the workflow manually.
- Used for testing and executing the workflow whenever required.

### 2️ Google Sheets
- Connects to Google Sheets using OAuth 2.0.
- Reads all sales records from the spreadsheet.
- Passes the data to the next node.

### 3️ JavaScript Code
- Processes all rows received from Google Sheets.
- Groups records by **Category**.
- Calculates the **total profit** for each category.
- Creates a formatted report message.

### 4 Telegram
- Receives the formatted report.
- Sends the Category Wise Profit report automatically to the configured Telegram chat.

---

#  Sample Output

```
 Category Wise Profit

Electronics : ₹518580
Furniture : ₹540542
Office Supplies : ₹551575
```

---

#  Technologies Used

- n8n
- Google Sheets API
- Google OAuth 2.0
- JavaScript
- Telegram Bot API

---

#  Features

- Reads live data from Google Sheets
- Calculates category-wise profit automatically
- Sends reports instantly to Telegram
- No manual calculation required
- Easy to schedule for daily or hourly execution

---

#  Future Improvements

- Schedule automatic daily reports
- Email notifications
- Dashboard integration
- Monthly and yearly profit analysis
- AI-powered business insights

---

#  Author

**Sowmiya M**

Learning Automation | Python | SQL | Power BI | n8n
