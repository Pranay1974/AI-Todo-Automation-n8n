# AI Agent To-Do List (n8n Workflow)

An AI-powered To-Do List automation built with **n8n**, **OpenAI**, and **Google Sheets**.

This workflow allows you to manage your tasks using natural language by chatting with an AI agent. The agent can create, list, update, and delete tasks while automatically storing them in Google Sheets.

---

## Overview

The **AI Agent To-Do List** workflow combines AI with automation to create a simple task manager. Instead of manually editing spreadsheets or apps, you can simply chat with the AI agent.

The AI understands your request and performs the appropriate action on your task list stored in Google Sheets.

Example commands:

- “Add a task to finish my project tomorrow”
- “Show my tasks”
- “Update task 3 as completed”
- “Delete task 2”

---

## Features

- Add new tasks using natural language
- View your task list
- Update task status
- Delete tasks
- Store tasks automatically in Google Sheets
- AI-powered interaction using OpenAI
- Built using n8n automation platform

---

## Tech Stack

- **n8n** – Workflow automation platform  
- **OpenAI** – AI agent for natural language understanding  
- **Google Sheets** – Task storage database  

---

## Workflow Architecture

The workflow starts when a user sends a chat message to the AI agent. The agent processes the request and uses tools connected to Google Sheets to perform the required action.

### Main Components

1. **Chat Trigger**
   - Starts the workflow when a chat message is received.

2. **AI Agent**
   - Understands user intent using OpenAI.

3. **Tools Connected to AI**
   - Add New Task (Google Sheets)
   - Get Task List
   - Update Task
   - Delete Task

4. **Memory**
   - Maintains context for the AI conversation.

---

## How It Works

1. User sends a message to the AI agent.
2. OpenAI processes the message.
3. The AI decides which tool to use.
4. The workflow interacts with Google Sheets.
5. The AI returns the result to the user.

---

## Google Sheets Structure

The tasks are stored in a Google Sheet.

Example structure:

| Task ID | Task              | Status    | Created At |
|---------|-------------------|-----------|------------|
|    1    | Finish assignment |  Pending  | 2025-03-09 |
|    2    |  Study AI agents  | Completed | 2025-03-09 |

---

## Setup Instructions

### 1. Import Workflow

1. Download the workflow JSON file.
2. Open **n8n**.
3. Click **Import Workflow**.
4. Upload the JSON file.

---

### 2. Configure OpenAI

1. Add your **OpenAI API key** in n8n credentials.
2. Connect the OpenAI node to the workflow.

---

### 3. Configure Google Sheets

1. Connect your **Google account** in n8n.
2. Select the correct spreadsheet.
3. Configure the Google Sheets node to store and manage tasks.

---

### 4. Run the Workflow

Start the workflow and interact with the AI agent through chat.

---

## Example Commands

Add a task
> Add a task to complete my homework tonight

Show tasks
> Show my to-do list

Update a task
> Mark task 2 as completed

Delete a task
> Delete task 3

---

## Future Improvements

- Add due dates
- Add task priorities
- Add reminders
- Integrate with WhatsApp or Telegram
- Add Notion or database support

---

## License

This project is open-source and available under the **MIT License**.
