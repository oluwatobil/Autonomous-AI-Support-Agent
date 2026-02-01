# Autonomous AI Support Agent

An end-to-end automation built with **n8n** that uses **GPT-4o-mini** to autonomously resolve technical dashboard inquiries via Gmail.


## Description
This project solves the challenge of high-volume, repetitive support tickets. The system autonomously triages incoming emails, references a knowledge base in Google Sheets, and provides instant resolutions. 

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Tech Stack](#tech-stack)
- [Results and Impact](#results-and-impact)
- [License](#license)

## Installation
To set up this workflow:

1. **Download the JSON:** Get the `autonomous-ai-support-agent.json` file from this repo.
2. **Import to n8n:** Open n8n, go to the menu, and select **Import from file**.
3. **Configure Credentials:** * Connect **Gmail API** to the trigger and send nodes.
    * Add your **OpenAI API Key** to the AI Agent node.
    * Link the **Google Sheets** node to your FAQ spreadsheet.
4. **Activation:** Save the workflow and switch the **Active** toggle to **ON**.

## Usage
Once the workflow is active, it monitors the connected Gmail inbox. When an email regarding technical dashboard issues is received:

1. **The Gmail Trigger** captures the message snippet.
2. **The AI Agent** analyzes the intent and searches the Google Sheets FAQ tool.
3. **A professional response** is drafted based on the FAQ data and sent back to the customer automatically.

## Tech Stack
* **n8n:** Workflow orchestration and logic.
* **OpenAI (GPT-4o-mini):** Intent recognition and natural language processing.
* **Google Sheets:** Lightweight knowledge base/FAQ storage.
* **Gmail API:** Automated communication layer.

## Results and Impact
* **Efficiency:** Response time less than one minute for 100% of tested inquiries.
* **Consistency:** Standardized technical troubleshooting across all interactions.


