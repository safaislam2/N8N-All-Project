# 🚀 WooCommerce E-Commerce Automation Engine with n8n, AI Agent & Google Sheets

An end-to-end, intelligent workflow automation architecture built with **n8n**, **WooCommerce API**, **Google Sheets**, and **Google Gemini AI Agent**. This system automates product lifecycle management, processes order invoices seamlessly from email triggers, and generates beautifully formatted weekly executive sales summary reports in BDT (৳) currency.

---

## 📌 Key Features

### 1. 📦 Automated Product Lifecycle Management (CRUD)
- **Create / Update / Delete Products**: Store managers can manage their WooCommerce catalog directly via Google Sheets without logging into the WordPress admin dashboard.
- Syncs product title, SKU, price, stock quantity, and status in real-time.

### 2. 🧾 Smart Order Parsing & Invoice Calculation
- **Email Order Triggering**: Automatically fetches incoming WooCommerce order notification emails via Gmail node.
- **AI-Powered Data Extraction**: Utilizes an **AI Agent (Google Gemini)** to parse unstructured email bodies into structured JSON data containing:
  - Customer Name
  - Order ID
  - Total Sales Amount
  - Total Tax Collected
  - Total Items Sold
- **Automated Ledger**: Automatically appends calculated transactions into a Google Sheets invoice ledger.

### 3. 📊 Scheduled Automated Sales Summary Reports
- **Periodic Triggering**: Runs on a configurable schedule (Daily / Weekly).
- **Data Aggregation**: Uses an `Aggregate` node to consolidate multiple sheet rows into a single batch item, preventing duplicate emails.
- **Executive AI Insights**: AI analyzes overall performance metrics, calculates grand totals, and formats a responsive, professional HTML email report including:
  - Total Unique Orders
  - Total Revenue Generated in Bangladeshi Taka (BDT ৳)
  - Total Tax & Items Sold
  - Executive Strategic Insights & Recommendations

---

## 🛠️ Tech Stack & Integrations

- **Workflow Engine**: [n8n](https://n8n.io/)
- **E-Commerce Platform**: WooCommerce / WordPress REST API
- **AI Engine**: Google Gemini Chat Model (LangChain Agent Architecture)
- **Google Services**: Google Sheets API, Gmail API
- **Templating**: HTML5 with inline CSS for responsive email rendering

 
