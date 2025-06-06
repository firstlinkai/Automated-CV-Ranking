# Automated-CV-Ranking
Automated CV Ranking System for Recruitment Agencies – Using n8n


I’ve developed an intelligent recruitment automation that streamlines CV evaluation in just a few steps – saving time, reducing manual errors, and ensuring better candidate screening.

🔍 Here’s how it works:
1- CV Submission
 A custom form collects the candidate’s name, email, and CV (PDF).

2- CV Upload & Text Extraction
 The uploaded file is saved to Google Drive and parsed using n8n’s Extract From File node.

3- AI-Powered Information Extraction
 Using LangChain nodes, we extract key attributes:

4- Personal details (city, birthdate, phone)
Education, job history, and technical skills

5- Candidate Summary
 A short, conversational summary is generated using an LLM summarization chain.

6- Profile Matching
 The system compares the candidate’s summary to the desired job profile (e.g., data analyst with Power BI, Maximo, SQL, etc.).

7- Scoring Logic (1–10)
 An LLM prompt assesses the alignment and gives a score, along with HR-style reasoning (“consideration”).

8- Data Logging
 All outputs—summary, score, and insights—are automatically logged in Google Sheets for review.

💡 Built entirely in n8n with:
OpenAI (via LangChain)
Google Drive & Sheets integrations
Zero-code, scalable architecture

📈 This system helps recruitment teams pre-screen candidates efficiently—ranking talent at scale, with context-aware AI assistance.
