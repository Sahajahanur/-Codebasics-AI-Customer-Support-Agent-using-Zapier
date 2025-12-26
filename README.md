# Codebasics-AI-Customer-Support-Agent-using-Zapier
An AI-powered customer support agent built with Zapier that automatically handles email inquiries for an e-learning platform. This agent reduces response time from 5 minutes to seconds by intelligently drafting responses and escalating complex queries.

## ✨ Features
* 📧 Automated Email Processing: Monitors support inbox and responds to common queries
* 🧠 Intelligent Knowledge Base: Searches through course brochures and FAQs for accurate answers
* 🎯 Confidence Scoring: Rates response accuracy (1-10) to determine automation level
* 📨 Smart Drafting: Creates email drafts for high-confidence answers (>7/10)
* ⚠️ Human Escalation: Sends WhatsApp alerts for low-confidence queries (<7/10)
* 🔄 Seamless Integration: Works with Gmail, Google Drive, and WhatsApp

## 🏗️ Architecture

<img width="1728" height="406" alt="image" src="https://github.com/user-attachments/assets/3c2fec70-e8bd-4c9e-b5c0-a058261f0d61" />

<img width="1906" height="866" alt="image" src="https://github.com/user-attachments/assets/e0762d61-ec4a-44ba-ae8a-43da7fe09716" />


## 📋 Prerequisites

* Zapier Account (Free trial available)
* Gmail Account (for support inbox)
* Google Drive (with course brochures/FAQs)
* WhatsApp Business API or similar for notifications

## 🚀 Quick Setup

### 1. Create AI Agent in Zapier
 * Log into Zapier
 * Navigate to Agents → Create New Agent
 * Select "Support Email Agent" template

### 2. Configure Agent Prompt

       You are an AI agent supporting the learner experience team at Codebasics.
     When you receive a customer query:
    1. Determine the intent and relevant bootcamp (Data Science or Data Analytics)
    2. Search the provided brochures for accurate information
    3. Respond in a friendly, professional tone aligned with our brand
    4. Assign a confidence score (1-10) based on answer quality
    5. If score >7: Draft email response in Gmail
    6. If score <7: Send WhatsApp notification to support team

### 3. Add Knowledge Sources

1. Click "Add Knowledge Source" in agent editor
2. Connect your Google Drive
3. Select relevant PDFs:
    
       * DS_Bootcamp_brochure_pdf.pdf
    
       * DA_Bootcamp_brochure_pdf.pdf

### 4. Integrate Tools

* Gmail: "Create Draft Reply" action
* WhatsApp: "Send Message" action for notifications

### 5. Test & Activate

1. Send test emails to your support address
2. Monitor agent activity in Zapier dashboard
3. Enable agent when testing is successful

## 🛠️ Configuration Details

     High Confidence (8-10):
      - Answer found directly in knowledge base
      - Clear, unambiguous information
      - Action: Auto-draft email for review
    
    Medium Confidence (4-7):
      - Partial information available
      - Requires interpretation
      - Action: WhatsApp alert for manual handling
    
    Low Confidence (1-3):
      - No relevant information found
      - Ambiguous or complex query
      - Action: Immediate WhatsApp escalation

## Email Trigger Settings

     {
      "trigger": "New Email in Gmail",
      "conditions": [
        "To: support@codebasics.io",
        "Exclude: Auto-generated emails",
        "Include: Customer inquiries only"
      ]
    }

<img width="1910" height="857" alt="image" src="https://github.com/user-attachments/assets/2d7d4087-47e0-44c8-83e5-38c533e205c3" />



## 🔧 Customization Options
### Add More Knowledge Sources

* Course syllabi
* Pricing information
* Technical requirements
* Student testimonials
* Refund policy documents

### Integrate Additional Tools

* Slack: For team notifications
* Trello/Asana: Create support tickets
* CRM: Update customer records
* Calendar: Schedule follow-ups

## Testing Checklist

* Test with simple FAQ questions
* Verify confidence scoring
* Check email drafting functionality
* Test WhatsApp notifications
* Validate response accuracy
* Ensure brand voice consistency

## 📈 Scaling & Evolution

### Phase 2: Enhanced Capabilities
   * Add voice call transcription
   * Integrate with learning management system
   * Implement customer feedback loop
   * Add proactive support (anticipate needs)

### Phase 3: Multi-Agent System

<img width="1727" height="401" alt="image" src="https://github.com/user-attachments/assets/f716c3e5-2b72-4346-b298-632b81559a6f" />

## 🙏 Acknowledgments

* Built following Codebasics YouTube Tutorial
* Inspired by real customer support challenges
* Powered by Zapier's no-code AI platform















































  























