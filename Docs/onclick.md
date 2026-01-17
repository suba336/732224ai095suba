1. Open n8n and create a new workflow
You’re in the Editor view under Personal → My workflow.

2. Add a Manual Trigger node
This is the node labeled “When clicking ‘Execute workflow’” — it starts everything.

3. Configure the Manual Trigger (no setup needed)
By default, it just emits one empty item when you click Execute.

4. Add a Gmail node
You added Gmail → Send a message right after the trigger.

5. Connect Manual Trigger → Gmail
The connection passes 1 item from the trigger into Gmail.

6. Authenticate your Gmail account
The Gmail node is already authorized (green checkmark = success).

7. Set the email fields in Gmail node
You configure:

To

Subject

Message body
(Static text or expressions — your choice)

8. Save the workflow
You hit Save in the top-right to keep changes.

9. Click “Execute workflow”
This manually fires the trigger node.

10. Email is sent successfully 
Gmail sends 1 message, and n8n confirms with “Workflow executed successfully”.

<img width="1913" height="881" alt="Screenshot 2026-01-17 113227" src="https://github.com/user-attachments/assets/60bd913d-a489-4da5-adc8-9ee12ab735da" />
