📌 Description

This project contains an automated email classification workflow built using n8n. The workflow is triggered by incoming emails from Gmail and processes each message to determine whether it is an order or an enquiry using AI (Google Gemini / OpenAI).

It includes batching and rate-limit handling to ensure stable API usage and prevent request throttling. Each email is processed individually with controlled delays, and the output is structured in a strict JSON format for easy integration with downstream systems.

⚙️ Features
Gmail Trigger integration
AI-based text classification (order vs enquiry)
Handles multiple emails safely using batching
Rate-limit protection with delays
Structured JSON output
Easy to import and reuse in n8n
🚀 Use Cases
Automated email sorting
Order management systems
Customer support workflows
CRM integrations
🧩 Tech Stack
n8n (workflow automation)
Google Gemini API / OpenAI API
Gmail API
