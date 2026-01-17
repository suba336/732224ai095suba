1. **Create a new workflow in n8n**
   You’re working inside **Personal → My workflow 2**.

2. **Add the “When chat message received” trigger**
   This node listens for messages typed into n8n’s built-in chat panel.

3. **User sends a chat message**
   Example shown: the user types **“hello”**.

4. **Trigger fires and outputs one item**
   It produces:

   * `sessionId`
   * `action` (sendMessage)
   * `chatInput` (“hello”)

5. **Connect the trigger to the AI Agent node**
   One item flows from the chat trigger into the AI Agent.

6. **Add a Chat Model to the AI Agent**
   You connect **Google Gemini Chat Model** as the agent’s model.

7. **AI Agent receives the chat input**
   The agent reads the user’s message and keeps the session context.

8. **AI Agent processes the message with Gemini**
   Gemini generates a response based on the agent’s instructions.

9. **Response is returned to the chat UI**
   The chat displays: *“Hello! How can I help you today?”*

10. **Workflow execution completes successfully ✅**
    Logs show **1 item processed** with no errors.

<img width="1919" height="902" alt="Screenshot 2026-01-17 120035" src="https://github.com/user-attachments/assets/716c3281-223a-4a92-856b-5a8ef1637ed7" />

