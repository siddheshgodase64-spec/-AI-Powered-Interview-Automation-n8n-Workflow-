🤖 AI-Powered Interview Automation (n8n Workflow)

This workflow demonstrates an end-to-end AI-powered interview automation system built using n8n, Google Workspace, and OpenAI.

It automatically schedules interviews and sends personalized emails when candidate data is updated in Google Sheets.

🔄 Workflow Overview

The automation follows this sequence:

1️⃣ Google Sheets Trigger

Trigger Type: anyUpdate

Listens for any update in a connected Google Sheet.

Typically used when a candidate is shortlisted or added.

📌 Example: Candidate email, name, role, and interview date added to the sheet.

2️⃣ Code in JavaScript (Data Processing)

Cleans and structures sheet data.

Extracts required fields like:

Candidate Name

Email

Interview Date & Time

Job Role

🛠 Used for data validation and formatting.

3️⃣ Create an Event (Google Calendar)

Automatically creates a Google Calendar interview event.

Adds interview schedule with correct date and time.

Ensures proper interview tracking.

📅 Eliminates manual scheduling.

4️⃣ Basic LLM Chain (AI Logic)

Connected to OpenAI Chat Model.

Generates:

Personalized interview invitation message

Professional tone and structured content

🧠 This is where AI personalization happens.

5️⃣ Code in JavaScript (Post-Processing)

Formats the AI-generated response.

Converts content into email-ready format.

Handles subject/body separation.

6️⃣ Send a Message (Gmail)

Sends the final interview email to the candidate.

Fully automated Gmail integration.

📧 Result: Candidate receives a professional AI-generated interview email instantly.

🚀 Key Features

✅ Fully automated interview scheduling

✅ AI-generated personalized emails

✅ Google Sheets → Calendar → Gmail integration

✅ No manual effort after data entry

✅ Scalable HR / recruitment automation

🧩 Tech Stack

n8n – Workflow automation

Google Sheets – Candidate data source

Google Calendar – Interview scheduling

Gmail – Email delivery

OpenAI Chat Model – AI message generation

JavaScript – Data processing

📌 Use Cases

HR Interview Scheduling

Recruitment Automation

AI-Driven Candidate Communication

Smart Calendar Management
