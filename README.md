# n8n Automation Projects Portfolio

A collection of practical n8n workflows demonstrating AI-powered automation, integrations, and intelligent agents built to solve real-world business problems.

## 📋 Table of Contents

- [n8n Automation Projects Portfolio](#n8n-automation-projects-portfolio)
  - [📋 Table of Contents](#-table-of-contents)
  - [🎯 Overview](#-overview)
  - [🚀 Projects](#-projects)
    - [1. WhatsApp Agent](#1-whatsapp-agent)
    - [2. Vector Database](#2-vector-database)
    - [3. Sentiment Analysis](#3-sentiment-analysis)
    - [4. Respond to Sponsorship](#4-respond-to-sponsorship)
    - [5. RAG Chatbot](#5-rag-chatbot)
    - [6. Google Sheets](#6-google-sheets)
    - [7. Form Submission to Airtable](#7-form-submission-to-airtable)
    - [8. Customer Service Assistant](#8-customer-service-assistant)
    - [9. AI-Powered Email Automation System](#9-ai-powered-email-automation-system)
      - [9.1 Emails to Pinecone](#91-emails-to-pinecone)
      - [9.2 Email Sender Agent](#92-email-sender-agent)
      - [9.3 Email Agent Pinecone](#93-email-agent-pinecone)
  - [🛠️ Technologies Used](#️-technologies-used)
    - [AI \& ML](#ai--ml)
    - [Vector Databases](#vector-databases)
    - [Integrations](#integrations)
    - [n8n Features](#n8n-features)
  - [📦 Setup Instructions](#-setup-instructions)
    - [Prerequisites](#prerequisites)
    - [Installation Steps](#installation-steps)
  - [🔑 Prerequisites](#-prerequisites)
    - [Technical Requirements](#technical-requirements)
    - [Account Requirements](#account-requirements)
    - [Knowledge Requirements](#knowledge-requirements)
  - [🤝 Contributing](#-contributing)
  - [📝 License](#-license)
  - [🙏 Acknowledgments](#-acknowledgments)
  - [📧 Contact](#-contact)

---

## 🎯 Overview

This repository contains 9 sophisticated n8n automation workflows that showcase:

- **AI Agent Development** using OpenAI GPT-4
- **Multi-modal Processing** (text, voice, documents)
- **Vector Database Integration** with Pinecone
- **RAG (Retrieval-Augmented Generation)** implementations
- **Business Process Automation**
- **Natural Language Processing**
- **Multi-platform Integrations** (WhatsApp, Gmail, Google Drive, Airtable, etc.)

---

## 🚀 Projects

### 1. WhatsApp Agent

**Description:** A comprehensive multimodal AI assistant that operates through WhatsApp, capable of handling both text and voice inputs, managing emails, calendars, and accessing team information.

**Key Features:**

- 📱 WhatsApp integration with text and voice message support
- 🎤 Audio transcription using OpenAI Whisper
- 🔊 Text-to-speech response generation
- 📧 Email management (Gmail Tool)
- 📅 Calendar operations (Google Calendar Tool)
- 📊 Google Sheets integration for team data
- 🧠 Conversation memory with context window management
- 🔄 Multi-agent architecture with sub-workflows

**Components:**

- WhatsApp Trigger
- Switch nodes for message type routing
- Audio transcription & generation
- AI Agent with multiple tools
  ![WhatsApp Agent](./WhatsApp%20Agent/WhatsApp%20Agent.png)
- Sub-workflows:
  - Email Agent
    ![WhatsApp Agent](.\WhatsApp%20Agent\Email%20Agent.png)
  - Calendar Agent
    ![WhatsApp Agent](.\WhatsApp%20Agent\Calender%20Agent.png)
- Memory management (20 message window)

**Use Cases:**

- Personal assistant via WhatsApp
- Voice-controlled email and calendar management
- Team information lookup
- Hands-free workflow automation

---

### 2. Vector Database

**Description:** Automated document ingestion pipeline that monitors Google Drive and stores document embeddings in Pinecone for semantic search capabilities.

**Key Features:**

- 🔍 Automatic Google Drive monitoring
- 📄 Multi-format document processing
- ✂️ Intelligent text chunking (900 chars, 50 overlap)
- 🧮 OpenAI embeddings generation
- 💾 Pinecone vector storage
- ⚡ Real-time document indexing

**Components:**

- Google Drive Trigger (monitors specific folder)
- Document download
- Text splitting with recursive character splitter
- OpenAI embeddings
- Pinecone vector store
  ![Vector Database](.\Vector%20Database\Vector%20Database.jpg)

**Use Cases:**

- Building searchable knowledge bases
- Document Q&A systems
- Semantic search implementations
- RAG system data preparation

---

### 3. Sentiment Analysis

**Description:** Web form-based feedback collection system with AI-powered sentiment analysis that automatically categorizes responses and stores them in Google Sheets.

**Key Features:**

- 📝 Custom web form for feedback collection
- 🤖 AI sentiment classification (Positive\Negative\Neutral)
- 📊 Automatic Google Sheets logging
- 🔄 Real-time analysis
- 📈 Structured data output

**Components:**

- Form Trigger (public web form)
- OpenAI GPT-4.1-mini for sentiment analysis
- Data merging
- Google Sheets integration
  ![Sentiment Analysis](.\Sentiment%20Analysis\Sentiment%20Analysis.jpg)

**Use Cases:**

- Customer feedback analysis
- Product review categorization
- Survey response processing
- Customer satisfaction tracking

---

### 4. Respond to Sponsorship

**Description:** Intelligent email automation system that detects sponsorship inquiries and generates professional responses with pricing and channel details.

**Key Features:**

- 📬 Gmail monitoring (every minute)
- 🤖 AI-powered sponsorship detection
- 📋 Structured output parsing
- ✉️ Automated professional responses
- 💰 Custom pricing information inclusion
- 🎯 Conditional workflow execution

**Components:**

- Gmail Trigger
- AI Agent with structured output parser
- Conditional logic (If node)
- OpenAI for email generation
- Gmail send integration

  ![Respond to Sponsorship](.\Respond%20to%20Sponsership\Respond%20to%20Sponsership.png)

**Channel Details:**

- Channel: TubeNotes (By Ayoub Youhad)
- Subscribers: 15,000+
- Average Views: 3,000 – 10,000
- Focus: Artificial Intelligence
- Pricing: €600 – €1,300 per sponsorship

**Use Cases:**

- Automated sponsorship inquiry handling
- Professional brand communication
- Lead qualification
- Time-saving for content creators

---

### 5. RAG Chatbot

**Description:** Public-facing chatbot specialized in answering questions about Tesla's quarterly financial reports using Retrieval-Augmented Generation.

**Key Features:**

- 💬 Public chat interface
- 🔍 Vector database retrieval (Pinecone)
- 📊 Financial data expertise
- 🧠 Conversation memory
- ⚡ Accurate, source-attributed responses
- 🎯 Domain-specific knowledge

**Components:**

- Chat Trigger (public webhook)
- AI Agent with custom system prompt
- Pinecone vector store retrieval
- OpenAI embeddings and GPT-4
- Memory management

  ![RAG Chatbot](.\RAG%20Chatbot\RAG%20Chatbot.png)

**Use Cases:**

- Financial report Q&A
- Investment research automation
- Corporate data accessibility
- Specialized knowledge chatbots

---

### 6. Google Sheets

**Description:** Simple utility workflow for programmatically creating Google Sheets spreadsheets.

**Key Features:**

- 📊 Automated spreadsheet creation
- 🖱️ Manual trigger activation
- ⚡ Quick setup template

**Components:**

- Manual Trigger
- Google Sheets create operation
  ![Google Sheets](.\Google%20Sheets\google%20sheets.jpg)

**Use Cases:**

- Template generation
- Automated report initialization
- Batch spreadsheet creation
- Workflow testing

---

### 7. Form Submission to Airtable

**Description:** Hotel room booking system with web form submission, Airtable database storage, and local file backup.

**Key Features:**

- 🏨 Room type selection (Deluxe, Standard, Studio, Double, Suite)
- 📋 Airtable database integration
- 💾 Local file backup (text format)
- 🔄 Multi-step data processing
- 📝 Form validation
- ![Form Submission to Airtable](.\Form%20Submission%20to%20Airtable\Form%20Submission.jpg)

**Components:**

- Form Trigger (public web form)
- Airtable record creation
- File conversion
- Local disk write
  ![Form Submission to Airtable](.\Form%20Submission%20to%20Airtable\Form%20Submission%20Workflow.jpg)

**Use Cases:**

- Hotel booking systems
- Registration forms
- Data collection with backup
- Multi-destination data flow

---

### 8. Customer Service Assistant

**Description:** Automated order notification system that monitors Airtable for new orders and sends formatted email notifications to the team.

**Key Features:**

- 🔔 Real-time Airtable monitoring
- 🤖 AI-generated professional emails
- 📧 Automatic team notifications
- 📋 Structured order details
- ⚡ Instant processing

**Components:**

- Airtable Trigger
- OpenAI for email generation
- Gmail send integration

  ![Customer Service Assistant](.\Customer%20Service%20Assitance\Customer%20Service%20Assitance.jpg)

**Order Information Included:**

- Order Number
- Customer details
- Product information
- Quantity & Price
- Order Date & Status

**Use Cases:**

- E-commerce order processing
- Team communication automation
- Order tracking systems
- Customer service workflows

---

### 9. AI-Powered Email Automation System

**Description:** A comprehensive three-workflow system for intelligent email management with vector database integration for contact lookup and AI-powered email composition.

#### 9.1 Emails to Pinecone

**Features:**

- 📄 Google Docs fetching
- ✂️ Document chunking (300 chars, 50 overlap)
- 🧮 Embedding generation
- 💾 Pinecone storage for email addresses

  ![Emails to Pinecone](.\AI-powered%20email%20automation%20system\Emails%20to%20Pincone.png)

#### 9.2 Email Sender Agent

**Features:**

- ✉️ HTML email formatting
- 🎨 Professional email templates
- 📧 Gmail integration
- 🤖 AI-powered composition

  ![Email Sender Agent](.\AI-powered%20email%20automation%20system\Email%20Sender%20Agent.png)

#### 9.3 Email Agent Pinecone

**Features:**

- 💬 Public chat interface
- 🔍 Contact lookup via vector search
- 🤖 Personalized email generation
- 🔄 Multi-tool orchestration
- 🎯 Automatic email sending

**Components:**

- Chat Trigger
- Vector store retrieval tool
- Email sender workflow tool
- OpenAI GPT-4
- Pinecone integration

  ![Email Agent Pinecone](.\AI-powered%20email%20automation%20system\Email%20Agent%20Pincone.png)

**Use Cases:**

- Automated email campaigns
- Personalized outreach at scale
- Contact database management
- Conversational email interface

---

## 🛠️ Technologies Used

### AI & ML

- **OpenAI GPT-4** - Language model for intelligent responses
- **OpenAI GPT-4.1-mini** - Efficient model for lightweight tasks
- **OpenAI Whisper** - Audio transcription
- **OpenAI TTS** - Text-to-speech generation
- **OpenAI Embeddings** - Vector representations

### Vector Databases

- **Pinecone** - Vector storage and similarity search

### Integrations

- **WhatsApp Business API** - Messaging platform
- **Gmail \ Google Workspace** - Email management
- **Google Calendar** - Calendar operations
- **Google Drive** - Document storage
- **Google Sheets** - Spreadsheet operations
- **Google Docs** - Document processing
- **Airtable** - Database and CRM

### n8n Features

- AI Agents
- LangChain integration
- Memory management
- Vector stores
- Sub-workflows
- Form triggers
- Chat triggers
- Webhook automation

---

## 📦 Setup Instructions

### Prerequisites

1. **n8n Installation**

   ```bash
   npm install -g n8n
   # or
   docker run -it --rm --name n8n -p 5678:5678 n8nio\n8n
   ```

2. **Required API Keys**
   - OpenAI API Key
   - Pinecone API Key
   - WhatsApp Business API credentials
   - Google Cloud Platform credentials (OAuth2)
   - Airtable Personal Access Token

### Installation Steps

1. **Clone or Download Workflows**

   - Import each `.json` workflow file into n8n
   - Go to n8n → Workflows → Import from File

2. **Configure Credentials**

   - Set up each integration in n8n credentials panel:
     - OpenAI API
     - Pinecone API
     - WhatsApp OAuth
     - Gmail OAuth2
     - Google Calendar OAuth2
     - Google Drive OAuth2
     - Google Sheets OAuth2
     - Airtable Token API

3. **Update Workflow-Specific Settings**

   **WhatsApp Agent:**

   - Replace `YOUR_WEBHOOK_ID` with your webhook
   - Replace `YOUR_PHONE_NUMBER_ID`
   - Update system prompt with your name\details
   - Configure sub-workflow IDs

   **Vector Database:**

   - Update Google Drive folder ID
   - Configure Pinecone index name and namespace

   **Sentiment Analysis:**

   - Update Google Sheets document ID

   **Respond to Sponsorship:**

   - Update channel details in system prompt
   - Modify pricing structure as needed

   **RAG Chatbot:**

   - Configure Pinecone index and namespace
   - Customize system prompt for your use case

   **Customer Service Assistant:**

   - Update Airtable base and table IDs
   - Configure recipient email address

   **Email Automation System:**

   - Update Google Docs URL
   - Configure Pinecone index
   - Link sub-workflows correctly

4. **Test Each Workflow**

   - Use manual triggers for testing
   - Verify all connections work
   - Check data flow between nodes

5. **Activate Workflows**
   - Enable production workflows
   - Monitor execution logs
   - Set up error notifications

---

## 🔑 Prerequisites

### Technical Requirements

- n8n instance (cloud or self-hosted)
- Node.js 16+ (for self-hosted)
- Stable internet connection
- Webhook endpoints (for triggers)

### Account Requirements

- OpenAI account with API access
- Pinecone account (free tier available)
- Google Cloud Platform project
- WhatsApp Business account
- Gmail account
- Airtable account
- Google Workspace (for Drive, Sheets, Calendar, Docs)

### Knowledge Requirements

- Basic n8n workflow understanding
- API concepts
- JSON data structures
- OAuth2 authentication
- Vector databases (basic understanding)
- LangChain concepts (helpful)

---

## 🤝 Contributing

Contributions, improvements, and feedback are welcome!

---

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🙏 Acknowledgments

- n8n community for excellent automation platform
- OpenAI for powerful AI models
- Pinecone for vector database solution
- All integration providers

---

## 📧 Contact

For questions, suggestions, or collaboration:

- **Email:** ayoubyouhad79@gmail.com

---
