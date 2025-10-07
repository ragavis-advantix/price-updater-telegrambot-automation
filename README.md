
# PriceUpdaterBot – Telegram Chatbot Workflow

A smart Telegram bot workflow to fetch product prices on demand.
PriceUpdaterBot interacts with users in a fun and friendly manner, processes SKU/product queries, retrieves product details from Supabase, and responds with accurate price information.

---

## 📖 Features

* 🤖 **Telegram Interaction** – Responds to user messages instantly
* 🌟 **Friendly AI Responses** – Distinguishes between greetings, product queries, and unrelated messages
* 🔍 **SKU/Product Lookup** – Searches Supabase database for matching products
* 💰 **Price Reporting** – Returns SKU, product name, and price to users
* ⚠️ **Error Handling** – Alerts users if a SKU is not found
* 📝 **Structured Data Handling** – Processes AI responses into structured workflow data

---

## 🛠️ Tech Stack

* **n8n** – Automation workflow engine
* **Google Gemini (PaLM)** – AI agent for message classification
* **Supabase** – Database for storing product information
* **Telegram API** – For chatbot interaction
* **JavaScript** – Workflow code for processing AI responses and logic

---

## ⚙️ Setup Instructions

### 1. Clone the Repo

```bash
git clone https://github.com/ragavis-advantix/PriceUpdaterBot.git
cd PriceUpdaterBot
```

### 2. Import Workflow into n8n

* Open the n8n dashboard
* Import the workflow JSON file
* Configure credentials for:

  * Telegram API
  * Google Gemini (PaLM) API
  * Supabase

### 3. Verify Workflow

* Send test messages in Telegram to check bot responses
* Ensure SKU/product queries return correct price information
* Confirm greetings and unrelated messages are correctly handled

---

## 📝 Development Notes

* **Customization**:

  * Update AI prompts in the “AI Agent” node for different response styles
  * Modify Supabase table references if database schema changes

* **Scaling**:

  * Additional features like Slack notifications or email reports can be added via n8n
  * Can be deployed behind NGINX or on a server for continuous operation

* **Testing**:

  * Use known SKU/product codes to test lookup functionality
  * Check logs in n8n for debugging workflow issues

---

## 👨‍💻 Author

**Ragavi**
📧 Email: [ragavis@advantixagi.com](mailto:ragavis@advantixagi.com)


