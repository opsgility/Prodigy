---
lab:
  title: 'Lab Setup'
  description: 'Prepare your Microsoft 365 Copilot (GCC) workspace and DWR resource files for the Everyday Productivity workshop, and learn the GCSE prompting framework used throughout.'
  duration: 10 minutes
  level: 200
  islab: true
---

# Lab Setup

In this morning workshop you apply Microsoft 365 Copilot to everyday California Department of Water Resources (DWR) work: catching up in Outlook and Teams, drafting documents and decks in Word and PowerPoint, and summarizing spreadsheets and notes with Excel and OneNote. You work entirely inside your organization's **GCC (Government Community Cloud)** tenant.

Because this is a GCC tenant, Copilot grounds on **your own files in OneDrive and SharePoint**, not the public web, and a few in-app Copilot features are not yet available. Setting up your files first, and knowing what works today, is what makes the exercises succeed.

> [!IMPORTANT]
> Two GCC realities to keep in mind all morning:
> 1. **Public-web grounding is off by default.** Copilot answers from your work content (files, email, chats), not the open web.
> 2. **"Edit with Copilot" (the in-canvas agent) is not available in GCC** for Word, Excel, PowerPoint, or OneNote, and Copilot's in-grid analysis of structured Excel data is limited in GCC today. Where an in-app step is unavailable, the exercise gives you a path through the **Copilot chat pane** that works in the tenant right now.

### Step 1: Get the DWR Resource Files

Your instructor will share the workshop resource pack (a folder named **DWR-Copilot-ResourceFiles**). Confirm it contains:

- `Duty_Statement_reference.md` (an approved duty statement, used as a structure reference)
- `Duty_Statement_DRAFT_rough.md` (rough notes for a new vacancy to turn into a clean duty statement)
- `Project_Accomplishments_List.md` (a bulleted list to turn into a narrative)
- `Alternatives_Analysis_source.md` (a source memo to summarize into a PowerPoint deck)
- `Permit_Conditions.csv` (a permit-conditions workbook to summarize)
- `Weekly_Project_Notes.md` (a week of rough notes to turn into a weekly summary)
- `Practice_Inbox_Pack.md` (four sample email threads for the optional Exercise 2b — you **email these to yourself**, see Step 5; do not upload this one to OneDrive)

> [!NOTE]
> The files ship as Markdown and CSV. If your instructor provided Word or Excel versions (`.docx`, `.xlsx`) instead, use those names in the steps. The content is the same.

### Step 2: Upload the Files to OneDrive

1. In your browser, go to `https://www.office365.us` (the Microsoft 365 GCC portal) and sign in with your DWR credentials.
2. Select **Apps** in the navigation pane, then select **OneDrive**.
3. Select **+ Add new** > **Folder** and create a folder named **DWR-Copilot**.
4. Open the folder, select **+ Add new** > **Files upload**, and upload all of the resource files.
5. Confirm every file appears in the **DWR-Copilot** folder.

> [!IMPORTANT]
> Microsoft 365 Copilot can only ground on files it can reach in OneDrive or SharePoint. Files left on your local PC are not visible to Copilot.

### Step 3: Prime Your Most Recently Used List

Some Copilot experiences only suggest files from your **Most Recently Used (MRU)** list. Open each file once so it is easy to reference:

1. In **OneDrive**, open `Duty_Statement_reference.md` and `Duty_Statement_DRAFT_rough.md`. Once each loads, close the tab.
2. Open `Alternatives_Analysis_source.md`, `Permit_Conditions.csv`, and `Weekly_Project_Notes.md` the same way.

### Step 4: Confirm You Can Reach Copilot

1. Go to the **Microsoft 365 Copilot** app for your GCC tenant (your instructor will share the link).
2. Confirm the Copilot chat prompt box opens and that you can reference a file (type `/` and pick a file from your **DWR-Copilot** folder).
3. If you cannot reach it, tell your instructor before the first exercise.

### Step 5: Email Yourself the Practice Inbox Pack (for Exercise 2b)

The optional Exercise 2b works a real email thread, so you need real messages in your own mailbox. Because Copilot in Outlook reasons over the mail you can open, do this **before** the session:

1. Open `Practice_Inbox_Pack.md` from the resource pack. For each thread, create a new message **to yourself**, set the **subject line exactly** as written, paste **Message 1**, and send it.
2. **Reply** to yourself with each following message so the thread builds up the way a real conversation would.
3. Confirm all four subject lines appear in your Outlook inbox.

Everything in the pack is fictional; do not add real DWR data. If you would rather use your own real, non-sensitive threads in Exercise 2b, you can skip this step.

### Workshop Structure

Four short exercises, one per module, each about 12 minutes, each on a real DWR task — plus an optional deeper-dive (Exercise 2b) on working an email thread.

| Exercise | Module | What you do |
|---|---|---|
| **Ex 1** | 1 | Write a GCSE prompt, then ground it on your own file |
| **Ex 2** | 2 | Catch up on an email thread and a Teams meeting, then draft a reply |
| **Ex 2b** *(optional)* | 2 | Work an email thread: catch up, extract actions, turn it into a manager update, and draft a reply |
| **Ex 3** | 3 | Draft a duty statement and build an alternatives-analysis deck |
| **Ex 4** | 4 | Summarize a permit-conditions workbook and draft a weekly summary |

### The GCSE Prompting Framework

Every strong prompt names four elements. Keep **GCSE** in front of you all morning:

- **Goal**. What you want Copilot to do. *Example: "Draft a duty statement for a new Water Resources Program Analyst position."*
- **Context**. Who you are and why. *Example: "I am an HR analyst at DWR filling a vacancy in the Division of Integrated Regional Water Management."*
- **Source**. Which of your files to use. *Example: "Follow the structure in Duty_Statement_reference and use the notes in Duty_Statement_DRAFT_rough."*
- **Expectations**. Format, tone, length. *Example: "State classification format, percentages of time that total 100, neutral professional tone."*

A clear Goal is the foundation. Context, Source, and Expectations are what make the response accurate and safe to use with government data.
