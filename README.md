# AI Office Assistant — n8n Workflow

An AI-powered office assistant built using **n8n, OpenRouter, Gmail, and Google Drive** to classify employee requests, identify their priority, recommend next steps, and route requests to the appropriate department.

## Features

- **AI-Powered Chat:** Responds naturally to greetings and general questions.
- **Request Classification:** Classifies employee requests into Leave, IT Support, Payroll, HR, or Other.
- **Priority Detection:** Assigns Low, Medium, or High priority based on the request.
- **Suggested Next Steps:** Generates reasons for classification and practical recommendations for the receiving department.
- **Department-Based Routing:** Routes requests according to their categories using workflow logic.
- **Automated Email Notifications:** Sends formatted Gmail notifications containing employee request details.
- **Calculator Integration:** Supports mathematical and arithmetic questions.
- **Google Drive Integration:** Includes file-processing nodes for additional document-related tasks.
- **AI Agent Integration:** Uses OpenRouter as the language model provider.

## Technologies Used

- n8n
- OpenRouter API
- AI Agent
- Gmail
- Google Drive
- JavaScript Expressions
- Workflow Automation

## Workflow Architecture

1. **Chat Trigger:** Receives messages from users.
2. **AI Agent:** Handles general conversation and classifies actionable employee requests.
3. **OpenRouter Chat Model:** Processes messages and generates AI responses.
4. **Calculator Tool:** Supports calculations when required.
5. **Switch Node:** Routes requests based on the predicted category.
6. **Data Preparation:** Extracts the category, priority, reason, original message, and suggested next step.
7. **Gmail Nodes:** Send formatted notifications to the appropriate recipients.

## Example Use Cases

- Requesting sick leave or vacation.
- Reporting laptop or network problems.
- Asking about salary or payslip discrepancies.
- Requesting HR assistance or employee documents.
- Routing other office-related requests to the appropriate team.

## Setup Instructions

### Prerequisites

- A running n8n instance.
- An OpenRouter API key.
- Gmail OAuth2 credentials.
- Google Drive credentials if using the file-processing functionality.

### Import the Workflow

1. Download `AI_Office_Assistant_GitHub_Safe.json` from this repository.
2. Open your n8n instance.
3. Import the JSON workflow file.
4. Configure your OpenRouter, Gmail, and Google Drive credentials as required.
5. Review the email recipients and update the example addresses.
6. Test each workflow branch using sample messages.
7. Activate the workflow only after verifying the configuration.

**Note:** Credentials are not included in the exported workflow. You must configure your own credentials after importing it.

## Security Considerations

- Never upload API keys, passwords, OAuth tokens, or `.env` files.
- Use sample data when demonstrating the workflow publicly.
- Protect the n8n editor and webhook endpoints.
- Review AI-generated classifications and recommendations before making important employment-related decisions.
- The assistant recommends next steps; it does not independently approve leave or resolve employee requests.

## Resume Description

**AI Office Assistant Automation | n8n, OpenRouter, Gmail, Google Drive**

Developed an AI-powered office assistant workflow using n8n to classify employee requests by department and priority, generate actionable recommendations, and automate email notifications. Integrated OpenRouter-based AI agents, calculator functionality, and Google Drive file-processing nodes.

## Project Purpose

This project demonstrates practical skills in AI integration, workflow automation, API integrations, conditional routing, and business process automation.
