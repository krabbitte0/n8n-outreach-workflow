# n8n-outreach-workflow

An n8n Workflow That Automates SMS Outreach, Handles Incoming Replies, And Stores Conversation Memory In Google Sheets.

## What It Does
1) Reads Prospects From A Google Sheet And Sends Batched SMS Messages (Twilio).
2) Logs Success/Failure + Timestamp Back To Sheets.
3) Receives Replies On A Webhook, Routes By Intent (E.G., "MYSPOT"), Or Uses An LLM To Draft Short, Helpful Replies.
4) Stores Lightweight Memory In Sheets And Avoids Sending Follow-Ups Too Quickly.

## Files
- `workflows/Outreach_Workflow_2_0_sanitized.json` — Import Into n8n.
- `.env.example` — Environment Variables/Placeholders.

## How To Use
1) Import The JSON Into Your n8n Instance.
2) Configure Credentials (Twilio, Google Sheets, OpenAI) In n8n.
3) Replace Placeholders Using Your Own Values From `.env.example`.
4) Set Your Webhook Path (E.G., `/incoming-replies`) And Test.

## Privacy
All IDs, Links, And Phone Numbers Are Redacted And Replaced With Placeholders. No Real Data Is Included.
