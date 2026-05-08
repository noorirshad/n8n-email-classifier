📧 Gmail AI Email Automation Workflow (n8n + Google Gemini)

This project is an automated email processing workflow built using n8n, designed to intelligently handle incoming Gmail messages, classify them, and generate AI-powered responses using Google Gemini.

🚀 Workflow Overview

The system listens for new incoming emails in a Gmail account and processes them through a structured automation pipeline:

1. 📩 Email Trigger (Gmail)

When a new email is received in the connected Gmail account, the workflow is triggered automatically.

2. ⏳ Delay Handling

A 5-second wait node is applied to ensure email content is fully available and avoid partial or incomplete processing.

3. 🧠 Email Classification (Text Classifier)

A text classification step analyzes the email content and categorizes it into predefined types:

Order → If the email contains keywords like "order" or "new order"
Inquiry → If the email contains keywords like "inquiry"

This allows dynamic routing based on intent.

4. 🤖 AI Response Generation (Google Gemini)

The categorized email is then passed to Google Gemini, which generates a contextual and professional response based on the email content and category.

5. 📝 Message Structuring (Code Node)

Since Gemini returns the response in a single field, a Code node is used to:

Extract and structure the response
Split it into two clear attributes:
Subject
Body

This ensures compatibility with Gmail draft formatting requirements.

6. 📄 Gmail Draft Creation

Finally, the structured response is used to:

Create a Gmail draft email
Populate subject and body fields
Store it in the Gmail account for review or manual sending
⚙️ Tech Stack
n8n (Workflow Automation)
Gmail API
Google Gemini AI Model
JavaScript (Code Node processing)
🎯 Key Features
Automated email categorization (Order / Inquiry)
AI-generated email responses
Structured email formatting (Subject + Body separation)
Gmail draft creation for human approval
Fully no-code / low-code automation using n8n


<img width="1463" height="523" alt="image" src="https://github.com/user-attachments/assets/8a12aa03-6526-4b07-825e-4d17cb1d0033" />
