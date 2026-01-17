1. **Create a new workflow in n8n**
   You’re in **Personal → My workflow 2** in the Editor view.

2. **Add the “When chat message received” trigger**
   This node listens for messages typed into n8n’s built-in chat panel.

3. **User sends a chat message**
   Example shown: the user types **“hello”** in the chat.

4. **Trigger fires and creates one item**
   The trigger outputs:

   * `sessionId`
   * `action`
   * `chatInput`

5. **Connect the trigger to an AI Agent node**
   One item flows from the chat trigger into the AI Agent.

6. **Add a Chat Model to the AI Agent**
   You connect **Google Gemini Chat Model** as the agent’s model.

7. **AI Agent receives the user message**
   The agent reads `chatInput` (“hello”) and keeps the `sessionId` for conversation context.

8. **AI Agent generates a response**
   Gemini processes the message using the agent’s system prompt and settings.

9. **Response is sent back to the chat UI**
   The agent replies: *“Hello! How can I help you today?”*

10. **Workflow execution completes successfully ✅**
    n8n logs show **1 item processed** and a successful execution.


<img width="1910" height="920" alt="Screenshot 2026-01-17 114315" src="https://github.com/user-attachments/assets/b5588ccc-36f1-4e0b-bab1-25ddd362da93" />

