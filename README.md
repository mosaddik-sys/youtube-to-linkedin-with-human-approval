# YouTube to LinkedIn Auto-Poster with Human Approval

This n8n workflow automates the entire process of turning YouTube videos into LinkedIn posts with built-in human approval.

##  Key Features

- Scheduled execution every 3 days
- Automatic YouTube video discovery and transcript extraction
- Dual AI processing using OpenAI (GPT-4o-mini) and Google Gemini for summaries
- Professional email sent for human review and approval
- AI-generated engaging LinkedIn posts with strong hooks and calls-to-action
- Automatic posting to LinkedIn with video thumbnail

##  Technologies Used

- n8n Workflow Automation Platform
- OpenAI GPT-4o-mini
- Google Gemini
- YouTube Data API
- Gmail API (Approval System)
- LinkedIn API

## How to Deploy

1. Download `workflow.json` from this repository
2. Import the workflow into your n8n instance
3. Configure the following credentials:
   - YouTube OAuth2
   - OpenAI API Key
   - Google Gemini API Key
   - Gmail OAuth2
   - LinkedIn OAuth2
4. Activate the workflow and test

## Workflow Flow

Schedule Trigger → Fetch Latest Videos → Extract Transcript → AI Summarization → Generate Approval Email → Wait for Human Response → If Approved → Generate LinkedIn Post → Post to LinkedIn
