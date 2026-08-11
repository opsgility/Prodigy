---
lab:
  title: 'Exercise 2: Catch Up and Draft in Outlook and Teams'
  description: 'Use Microsoft 365 Copilot (GCC) to catch up on a long email thread and a missed Teams meeting at the California Department of Water Resources, then draft and refine a reply.'
  duration: 12 minutes
  level: 200
  islab: true
  primarytopics:
    - Microsoft 365 Copilot
    - Outlook
    - Teams
---

# Exercise 2: Catch Up and Draft in Outlook and Teams (12 min)

You have been out of the office and come back to a full inbox and a project meeting you missed. In this exercise you use Microsoft 365 Copilot to get through the backlog fast: summarize a long email thread, catch up on the meeting through its recap, then draft a reply and refine its tone and length before you send it. You work entirely in your DWR GCC tenant, so Copilot reasons over your own email, chats, and meeting content, not the open web.

> [!TIP]
> Keep the **GCSE** framework from the Lab Setup in front of you. Even a quick "catch me up" answer is better when you name the **Goal**, add a little **Context**, point Copilot at the right **Source** (this thread, this meeting), and state your **Expectations** for format and length. A specific ask like "list the decisions and the open action items with owners" beats "summarize this."

### Scenario

You are back at DWR after two days out, facing a full inbox and a project meeting you could not attend. One email thread on a permit renewal has grown to a dozen replies, and a planning meeting happened while you were away. Rather than read every message and watch the whole recording, you will let Copilot bring you current, then help you reply. You will use your own real thread and meeting throughout.

> [!NOTE]
> This exercise uses **your own** recent work so every attendee has real material. If you do not have a long thread or a recent meeting with a recap, pair with a colleague in class and use a thread that includes both of you, or the class kickoff meeting if it was recorded and transcribed. Copilot can only summarize a meeting that has a **transcript or recording**, and intelligent recap requires a Teams Premium or Microsoft 365 Copilot license.

### Task 1: Summarize a long email thread in Outlook (4 min)

Catch up on a busy thread without reading every message.

1. Go to `https://www.office365.us`, sign in with your DWR credentials, and open **Outlook**.
2. In your inbox, open a **long email thread** (aim for six or more messages). If you do not have one, use a thread you share with a classmate.
3. At the top of the email thread, select **Summarize by Copilot** (on some clients the control reads **Summarize**). Copilot returns a short summary with numbered citations.
4. Select a numbered **citation** to jump to the exact message a point came from. Get in the habit of confirming anything you will act on.
5. Ask Copilot to pull out what you owe people. In the same summary experience, enter a follow-up:

   ```text
   List the decisions this thread reached and the open action items, with who owns each and any dates mentioned.
   ```

**Validate:** Your result names the decisions the thread reached and the open action items. If the summary only recaps discussion, make the prompt more specific (name "decisions" and "action items" explicitly) and try again.

### Task 2: Catch up on the meeting you missed in Teams (4 min)

Use intelligent recap to catch up on the meeting without watching the recording.

1. Open **Teams** and go to your **Calendar** (or the meeting's **chat**). Open a recent meeting you attended or missed that has a recording or transcript.
2. Select the **Recap** tab. Review the **AI meeting notes** and the **AI recommended tasks**. Use the **speaker** and **topic** markers to jump to a moment or a chapter that matters to you.
3. Ask Copilot a targeted follow-up about your own commitments:

   ```text
   Based on this meeting, what was I asked to do, by when, and what decisions were made that affect my work?
   ```

**Validate:** You can name the meeting's key decisions and at least one task assigned to you, without watching the recording. Because AI notes and tasks are generated and can misattribute an item, confirm ownership before you treat a task as yours.

> [!NOTE]
> If you have no meeting with a recap, use a busy **Teams chat or channel** instead. Open the **Copilot** side panel and use a prewritten prompt such as "Catch up," then ask **"What decisions were made and what am I expected to do?"** In GCC, Copilot summarizes up to 30 days of that single chat thread and cannot reach into other chats, transcripts, emails, or files.

### Task 3: Draft and refine a reply in Outlook (4 min)

Turn what you learned into a reply, then adjust its tone and length before sending.

1. Return to the email thread from Task 1 and select **Reply**.
2. Select the **Copilot** icon on the toolbar, then select **Draft with Copilot**. Type a short prompt that acknowledges the thread and confirms one action you own:

   ```text
   Reply to the thread confirming that I will complete my action item by the agreed date, thank the group for catching me up while I was out, and ask one clarifying question about the next step.
   ```

3. Review the draft. Copilot drafts, it does not verify, so confirm every date, name, and figure against the thread before you rely on it.
4. Refine the draft. Use the draft's **Adjust with Copilot** control (or type an instruction) to shorten it and make the tone right for the audience:

   ```text
   Make this more concise and use a professional, courteous tone suitable for an interagency reply.
   ```

5. Iterate once with **Coaching by Copilot**. Select the **Copilot** icon in the message, then select **Coaching by Copilot**. Copilot reviews your draft and gives an assessment of tone, clarity, and reader sentiment with suggestions to improve. Apply one suggestion you agree with, and ignore any you do not.

**Validate:** Your final reply is shorter than the first draft, reads in a professional tone, and every fact in it (dates, names, commitments) matches the source thread. Do not select send; this is a drafting exercise.

> [!NOTE]
> Two GCC realities apply here. Copilot reasons over your Microsoft 365 content and the conversation at hand, not the public web. And **"Schedule with Copilot"** (turning the email into a meeting invite) and **"Themes by Copilot"** are not yet available in GCC, so do not build this reply into a meeting request. If the "Adjust with Copilot" control looks slightly different on your client (web, new Outlook for Windows, Mac, or mobile), the concept is the same: adjust length and tone, and rewrite a selection.

### Hands-On Practice: Your Turn

Pick a real thread or meeting from your own week and run the same flow end to end:

1. **Catch up.** Summarize a long thread in Outlook, or open the Recap tab for a recent meeting (or catch up on a busy chat). Click a citation to confirm one point.
2. **Ask for your part.** Follow up with:

   ```text
   What am I expected to do next, by when, and what decisions affect my work?
   ```

3. **Draft and refine.** Draft a reply with Copilot, adjust its length and tone, and run Coaching by Copilot once. Confirm every fact against the source before you would send.

Notice how much of your morning triage this replaces: instead of an hour of reading, you spend a few minutes catching up and a few more producing a reply you would be comfortable sending.
