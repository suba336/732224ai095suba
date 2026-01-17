1. **Create a new workflow in n8n**
   You’re working in **Personal → My workflow 4**.

2. **Add the “On form submission” trigger**
   This node fires whenever someone submits the connected n8n form.

3. **User submits the form**
   The form data (name, email, answers, etc.) is captured as **1 item**.

4. **Trigger passes form data forward**
   All submitted fields are sent to the next node.

5. **Add “Append row in sheet” (Google Sheets)**
   This node is configured to insert a new row into a specific spreadsheet.

6. **Map form fields to sheet columns**
   Each form field is matched to its corresponding Google Sheets column.

7. **Row is successfully added to Google Sheets**
   The submission is now stored permanently in the sheet.

8. **Google Sheets Trigger detects a new row**
   The **rowAdded** event fires when the new row appears.

9. **Send a Gmail message**
   The Gmail node sends an email using the data from the new row (confirmation, alert, etc.).

10. **Workflow completes successfully ✅**
    Logs show each step executed with no errors.

<img width="1919" height="907" alt="Screenshot 2026-01-17 122928" src="https://github.com/user-attachments/assets/9ff655f6-08c0-4ee7-b4eb-fb5450e91a03" />
