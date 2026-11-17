# Gmail-AI-Assistant
# Gmail AI Assistant (LangGraph + Groq)

An AI agent that reads an email, decides what kind it is, and handles it for me.

## What it does
1. **Classifies** each email as spam, needs a reply, or just FYI.
2. **Spam:** ignores it.
3. **FYI:** summarizes it in one line.
4. **Needs a reply:** drafts three replies (normal, a polite no, and professional), then lets me pick one before anything is "sent."

The approval step keeps a human in the loop. Replies are only printed, not actually sent. <!-- If yours really sends via Gmail, change this line -->

## How it works
- **LangGraph** controls the flow with nodes, edges, and a conditional step that picks the path.
- **Groq API** (open-source LLM) classifies emails and writes the replies.
- Built in **Python** on Google Colab.

## How to run
1. Open the notebook in Google Colab.
2. Get a free Gemini API key and save it in Colab Secrets as 'Gemini_Api_Key`.
3. Run the two cells in order.
4. Change the `email` text to test spam, FYI, and reply emails.

## What I learned
- Conditional routing in LangGraph
- Human-in-the-loop approval before an action
- Handling API rate limits and keeping keys in Colab Secrets

## Next steps
- Connect the Gmail API to read and send real email
- Add more categories, like urgent or newsletter
<img width="1499" height="645" alt="Capture" src="https://github.com/user-attachments/assets/fa956bba-147f-4ee0-9f1b-be8ec2d8bacb" />
<img width="1702" height="432" alt="Capture" src="https://github.com/user-attachments/assets/d1d90be2-b7ab-435f-9293-b0e9201d5fdd" />
