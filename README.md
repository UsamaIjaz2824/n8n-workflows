# 🔄 n8n AI-Powered Automation Workflows  
A collection of production-ready n8n workflows integrating **AI**, **LLMs**, **Gmail**, **Airtable**, **Fireflies**, **Forms**, and **RAG pipelines**.  
Each workflow is exportable, customizable, and designed for real automation use-cases.

---

# 📌 Workflows Included

## 1️⃣ Handling Job Application Submissions with AI & n8n Forms  
This workflow creates a **two-step job application system** with automated CV extraction, validation, and pre-filled forms using AI.  
### 🔥 Features
- Applicant uploads a PDF CV via n8n form  
- AI checks if uploaded document is a valid CV  
- Extracts Name, Email, Address, Skills, Experience, Cover Letter, etc.  
- Auto-prefills step-2 application form  
- Saves structured applicant data to Airtable  
- Re-uploads document to Airtable record  
- Provides success confirmation  

### 🧠 Key AI Components
- OpenAI-powered extraction  
- AI text classification for document validation  
- Uses **Structured Output Parser** for clean JSON results  
- Airtable integration for an ATS-like flow  

---

## 2️⃣ AI-Powered RAG Workflow for Stock Earnings Report Analysis   
A complete **Retrieval-Augmented Generation (RAG)** pipeline for analyzing Google/Alphabet quarterly earnings reports.

### 🔥 Features
- Loads earnings PDFs from Google Drive  
- Splits, embeds, and indexes chunks into **Pinecone vector store**  
- AI Agent retrieves relevant financial data  
- Gemini embeddings + OpenAI LLM for analysis  
- Generates a full structured financial report  
- Saves the final output to Google Docs  

### 🧠 Ideal For
- Automated financial analysis  
- Document intelligence use cases  
- Corporate report summarization  
- AI research assistants  

---

## 3️⃣ Gmail Automation – AI Label Assignment  
This workflow auto-tags incoming Gmail messages with intelligent AI-generated categories.

### 🔥 Features
- Polls Gmail inbox every minute  
- Fetches email content  
- Runs email text through an LLM  
- Assigns labels such as:  
  - **Partnership**  
  - **Inquiry**  
  - **Notification**  
- Adds labels to Gmail message programmatically  
- Fully customizable labels and schema  

🧠 Uses a JSON schema validator to ensure clean AI output.

---

## 4️⃣ Compose Reply Draft in Gmail with OpenAI Assistant    
Automatically drafts high-quality replies to emails and inserts them into Gmail as a **draft response**.

### 🔥 Features
- Scans threads with a specific AI label  
- Extracts last message in the thread  
- Sends it to OpenAI Assistant  
- Converts AI response Markdown → HTML  
- Builds RFC-compliant raw email  
- Inserts draft directly into Gmail  
- Removes the AI label after processing  

### 🧠 Perfect For:
- Customer support  
- Sales teams  
- Automated cold outreach replies  

---

## 5️⃣ AI Agent for Project Management & Meeting Automation   
A full AI agent workflow integrating **Fireflies**, **Airtable**, and **Google Calendar** for complete meeting → tasks → notifications automation.

### 🔥 Features
- Webhook receives Fireflies meeting transcript  
- Agent checks if meeting is project-related  
- AI analyzes transcript & extracts tasks  
- Creates tasks in Airtable via “Create Tasks” tool  
- Sends task summaries to clients via Gmail  
- Creates Google Calendar events for follow-up calls  
- Supports multi-participant workflows  

### 🧠 Example Use Cases
- Automated project meeting action item extraction  
- Client follow-up automation  
- Smart PM assistant for large teams  

---


---

# 🚀 How to Import These Workflows in n8n

1. Open your **n8n dashboard**  
2. Click **Workflows → Import from File**  
3. Upload any workflow JSON  
4. Configure credentials (Gmail, Airtable, OpenAI, Pinecone, Fireflies, Google API)  
5. Activate workflow  

---

# 🔧 Requirements

These workflows may require credentials for:  
- OpenAI  
- Google Gemini  
- Gmail OAuth2  
- Airtable API  
- Pinecone  
- Fireflies API  
- Google Drive/Sheets/Docs  
- Google Calendar  

Each workflow contains sticky notes inside n8n explaining exactly what to configure.

