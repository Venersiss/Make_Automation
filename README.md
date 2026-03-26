# Make.com Automation Blueprints

My first automation projects built with [Make.com](https://www.make.com), created while learning workflow automation.

---

## Scenario 1: Gmail Email Logger

**File:** `Integration_Gmail_blueprint.json`

Automatically logs all incoming Gmail emails into Google Sheets, separated by sender.

**How it works:**

1. **Trigger** — Watches for new unread emails in Gmail inbox
2. **Router** — Checks who sent the email
   - **If sent by me** — Logs to a "Sent Emails" Google Sheet
   - **If sent by someone else** — Logs to a "Received Emails" Google Sheet

**Data logged per email:** Sender, Receiver, Subject, Snippet/Body, Category Folder, Has Media, Date

**Tools used:** Gmail, Google Sheets, Make.com Router + Filter

---

## Scenario 2: Cookie Order Automation

**File:** `Integration_Google_Forms_blueprint.json`

Automates the entire order flow for a cookie shop — from form submission to confirmation email to team notification.

**How it works:**

1. **Trigger** — Customer submits a cookie order through Google Forms (name, email, address, cookie type, quantity, delivery option)
2. **Log to Sheets** — Order details are saved to a Google Sheet for tracking
3. **Router** splits into two actions:
   - **Send confirmation email** — Customer receives a Gmail confirmation with their order details
   - **Notify the team on Discord** — A message is posted to a Discord channel with the order info and "Please Ship ASAP!"

**Tools used:** Google Forms, Google Sheets, Gmail, Discord, Make.com Router

---

## How to Use These Blueprints

1. Go to [Make.com](https://www.make.com) and create a free account
2. Create a new scenario
3. Click the three dots menu (bottom of the editor) and select **Import Blueprint**
4. Upload the `.json` file
5. Reconnect your own Google, Gmail, and Discord accounts in each module
6. Turn on the scenario

---

## Built With

![Make](https://img.shields.io/badge/Make.com-6D00CC?style=for-the-badge&logo=make&logoColor=white)
![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white)
![Google Forms](https://img.shields.io/badge/Google%20Forms-7A1FA2?style=for-the-badge&logo=googleforms&logoColor=white)
![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)
