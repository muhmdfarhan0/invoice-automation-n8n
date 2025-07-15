# 📬 Invoice Automation Workflow (n8n)

This repository contains an intelligent invoice processing system built with [n8n](https://n8n.io/). It monitors a Google Drive folder for new invoices, extracts key invoice details using AI, logs the data into a Google Sheet, and sends email notifications to internal billing teams.

---

## 🚀 Features

- 🔁 **Google Drive Trigger**: Watches a folder for new PDF invoices
- 📥 **Auto Downloads PDF** and extracts the content
- 🧠 **AI-Powered Data Extraction**: Uses OpenAI + LangChain's Information Extractor to extract fields:
  - Invoice Number
  - Client Name
  - Client Email
  - Client Address
  - Client Phone
  - Total Amount
  - Invoice Date
  - Due Date
- 📊 **Logs to Google Sheet**: Automatically updates the "Invoice DB"
- ✉️ **Sends Email Alerts**: Summarizes invoice info in an email to notify the finance team

---

## 📂 Included Files

| File | Description |
|------|-------------|
| `invoice-workflow.json` | The n8n workflow export |
| `invoice_db.xlsx` | Sample Google Sheet with extracted invoice entries |
| `invoice_sample.pdf` | Sample invoice used for testing the automation |

---

## 🧠 Technologies Used

- **n8n** – Workflow automation
- **Google Drive** – Trigger + file download
- **LangChain Information Extractor** – AI-powered structured data extraction
- **Google Sheets** – Invoice database
- **OpenAI GPT-4** – Natural language processing
- **Gmail API** – Send automated notifications

---

## 🛠️ Setup Instructions

1. Clone the repo and import the `invoice-workflow.json` into n8n.
2. Configure the following credentials inside n8n:
   - Google Drive OAuth2
   - Google Sheets OAuth2
   - OpenAI API Key (GPT-4)
   - Gmail OAuth2 (for email sending)
3. Ensure the **Google Sheet** and **Google Drive Folder** used in the workflow are accessible and mapped correctly.
4. Upload a sample invoice (PDF) into the Drive folder to trigger the flow.
5. Watch the magic happen! 🎉

---

## 📸 Screenshot

<img width="1739" height="439" alt="image" src="https://github.com/user-attachments/assets/d0ac08f5-4dce-4500-a622-db744fd20a6d" />


---

## 🤝 Contributing

Feel free to fork and extend the workflow for:
- Multi-page invoice parsing
- Vendor classification
- Line item extraction

---

## 📩 Contact

Created by **Muhammad Farhan**  
Feel free to connect on [LinkedIn](www.linkedin.com/in/muhammad-farhan-55a05a251) or email at `Muhammadfarhan03333@gmail.com`.

---

