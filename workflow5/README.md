# 📅 AI-Powered Google Calendar & Sheets Automation
One of my first AI agent automations — simple idea, powerful workflow.

Hi everyone!
This project showcases one of my first automations built with AI agents. The idea behind it is simple, but the workflow itself relies on several nodes working together with careful setup. Here’s a clear breakdown of how everything works:

![screenshot](./)

🚀 What This Automation Does

You can ask the AI to create an event for you, and the workflow will:

Understand your request through an AI model

Store your conversation context using memory

Create the event automatically in Google Calendar

Log it inside Google Sheets for organization

Allow you to ask about specific dates

Update event details whenever needed

All of this is handled seamlessly through a single workflow powered by an AI agent.

🧠 AI Agent Setup

Working with an AI agent requires two key components:

AI Model – In this case, I used OpenRouter.
It’s free, has some limits, but works perfectly for learning and experimentation.

Memory – Stores your previous messages so the agent can stay consistent and understand context.

🛠️ Tools Used
Google Calendar

Used to:

Create new events

Update event times or descriptions

Store your scheduling data automatically

Google Sheets

Used to:

Log all created events

Retrieve events for a specific date

Update rows when details change

🔄 How the Workflow Works

Here’s the flow step-by-step:

Chat Trigger receives your message

The message is sent to the AI Agent

The AI model interprets what you want (e.g., “schedule a meeting tomorrow at 3 PM”)

Memory keeps track of past requests

The workflow creates the event in Google Calendar

The event is then logged in Google Sheets

You can also:

Ask about events on a certain day

Update details in the sheet

Keep using natural language to manage your schedule
