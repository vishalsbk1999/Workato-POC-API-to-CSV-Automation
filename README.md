The goal of this POC is to showcase:
API integration using Workato’s HTTP connector
Data transformation from JSON → CSV
File handling and automated email delivery

🔹 Workflow Steps
Trigger: Scheduled trigger (runs daily/weekly as configured).
HTTP GET: Fetches user data from https://reqres.in/api/users?page=2.
CSV Composer: Transforms the API response (data[]) into a structured CSV file.
Email Sender: Sends the generated CSV as an email attachment.

🔹 Tech Stack
Workato iPaaS
HTTP Connector
Utilities (CSV Composer)
Workato Email Connector

🔹 Use Cases
Automating report generation from APIs
Sending daily user activity exports
emonstrating API → CSV → Email workflows in Workato

🔹 Future Enhancements
Add support for pagination (fetch multiple pages of API results).
Store CSV files in cloud storage (S3, GDrive, OneDrive) instead of email only.
Include error handling and logging with alerts (e.g., Slack).
