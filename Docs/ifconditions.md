1. **Create a new workflow in n8n**
   You’re working inside **Personal → My workflow 5**.

2. **Add the Manual Trigger**
   The node **“When clicking ‘Execute workflow’”** starts the workflow when clicked.

3. **Click “Execute workflow”**
   The trigger fires and outputs **1 item**.

4. **Get rows from Google Sheets**
   The **Get row(s) in sheet** node reads existing data from a spreadsheet.

5. **Multiple rows are returned**
   In your case, the sheet returns **5 items (rows)**.

6. **Pass rows into an If node**
   Each row is evaluated individually by the **If** condition.

7. **Evaluate the condition**
   The If node checks a rule (e.g., Age, Role, Hobby, or any field you defined).

8. **Split the data by condition**

   * **True branch:** 2 items
   * **False branch:** 3 items

9. **Append rows to different sheets**

   * **True → Append row in sheet**
   * **False → Append row in sheet1**

10. **Workflow completes successfully ✅**
    Logs confirm both append operations ran without errors, writing the data to the correct sheets.
<img width="1919" height="908" alt="Screenshot 2026-01-17 125254" src="https://github.com/user-attachments/assets/797e69f1-f99c-4f2c-920a-748ade04cf7d" />

