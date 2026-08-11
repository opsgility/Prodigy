---
lab:
  title: 'Exercise 2b: Work a Thread in GCC — Beyond the Summary'
  description: 'Interrogate an Outlook thread with Microsoft 365 Copilot in GCC — catch up, extract decisions and action items, turn it into a manager update, ask it targeted questions, and draft a reply in your voice — verifying every fact against the thread.'
  duration: 18 minutes
  level: 200
  islab: true
  primarytopics:
    - Microsoft 365 Copilot
    - Outlook
    - Prompting
---

# Exercise 2b: Work a Thread in GCC — Beyond the Summary (18 min)
---

A one-line summary tells you a thread happened. Real work needs more: what was decided, what you now owe people, what is at risk, and a reply that sounds like you. In this exercise you go past "summarize this" and *interrogate* a thread with Microsoft 365 Copilot — pulling structured decisions and action items, turning the thread into a manager update, asking it pointed questions, and drafting the reply and the leadership note you would otherwise write from scratch. You work entirely in your DWR GCC tenant, so Copilot reasons over the mail you can open, not the open web, and it **sends nothing** — every draft waits for you.

> [!TIP]
> Keep **GCSE** in front of you even for a "quick" question: a specific ask ("list the open action items with owners and due dates") beats "tell me more" every time. Two GCC realities shape this exercise: **Copilot in Outlook works over the mail you can open** (with web off by default, it reasons over the thread and your Microsoft 365 content, not the public web), and **Copilot never hits send** — you review and send. To point Copilot at a specific thread, open the **Copilot chat pane** (in Outlook or the Microsoft 365 Copilot app), type `/`, start typing the **subject line**, and select the thread from the list.

### Before you start

* [ ] You emailed yourself the four threads from the [Practice Inbox Pack](resources/Practice_Inbox_Pack.md) (or you have your own real, non-sensitive threads to use instead).
* [ ] You can open **Outlook** on the web in your GCC tenant and see the threads by subject.

---

## Part A — Catch up and extract

### Task 1 — Catch up across the inbox (3 min)

Start wide: let Copilot triage everything at once instead of opening each thread.

1. Open the **Copilot chat pane** and run:

   ```text
   Catch me up on my email from the last few days. Group by topic. For each topic give a one-line status, any deadline, and who owns the next step. Flag anything that needs a decision from me.
   ```

2. Read the result. It should be grouped by topic with owners and deadlines, not one long paragraph.

**Validate:** You can see, at a glance, which threads need something from *you* versus which are just informational.

### Task 2 — Turn a thread into a 2-on-2 update (4 min)

Now go deep on one thread and shape it into the update you would bring to your manager check-in.

1. In the **Copilot chat pane**, type `/`, start typing **North Delta Levee — Reach 3 Design Review Status**, and select it. Then run:

   ```text
   Summarize this thread into five bullets for my 2-on-2 with Priya, my program manager: key decisions, open action items with owners, current status, any risks or blockers, and next steps. Use a professional status-update tone. End with one line labeled "Decision needed from you."
   ```

2. Check every bullet against the thread. Select a **citation** and confirm it points to the message it came from.

> [!NOTE]
> This is where naming the thread as your Source earns its keep. With web off in GCC, Copilot has only the messages you point it at, so the update reflects the actual thread, not a generic template. If a name, date, or dollar figure appears that you cannot trace to a message, treat it as unverified until you confirm it.

**Validate:** Your five bullets name the real decision (escalate to Cordova, no slip past Friday without sign-off), at least one open action with an owner, the Cordova boring-logs risk, and a clear "Decision needed from you" line.

### Task 3 — Pull the action items as a checklist (3 min)

Different thread, tighter ask: just the open commitments.

1. Type `/`, select **Contract Amendment #7 — Geotech Extension**, then run:

   ```text
   From this thread, list only the open action items as a checklist. For each: the owner, exactly what they committed to, and the due date or deadline. Leave out anything already resolved.
   ```

2. Confirm the owners and dates against the messages before you rely on them.

**Validate:** Your checklist captures the items assigned to you (file the no-cost bridge extension today; confirm the field crew's site-access badging before obligating) and does not list the already-approved decision as an open item.

### Task 4 — Interrogate the thread (4 min)

This is the step that separates working a thread from skimming it. Ask Copilot the questions you would have to answer in a meeting — and **name the people in the thread**, because Copilot can attribute who said and decided what. Stay on the **Contract Amendment #7** thread and ask one at a time:

```text
What two options did Daniel analyze, what does each cost, and which one stays within the task-order ceiling?
```

```text
What did Tanya approve, what conditions did she attach, and what has to happen before September 30?
```

```text
What is still unanswered in this thread, and who owes the next step?
```

Read each answer against the messages. The goal is not a summary — it is getting the thread to hand you the specific facts, trade-offs, and attributed decisions you would otherwise dig out by re-reading every reply.

> [!NOTE]
> Naming a person in the prompt ("what did Tanya approve," "what is Priya waiting on") is one of the most useful thread moves in GCC. Copilot is reasoning over the one thread you named, so it can tell you who committed to what and who still owes a reply — as long as you point it at the thread and check the citation before you repeat it.

**Validate:** Copilot correctly returns the $163K (60-day) versus $185K (90-day) trade-off and the ~88% ceiling point, the Sept 30 lapse risk with its owner, and at least one genuinely open item (for example, the field-crew badging still to be confirmed).

---

## Part B — Draft as a professional

### Task 5 — Draft a reply in your voice (2 min)

1. Type `/`, select **Permit Condition PC-006 — Nesting Bird Window**, then run:

   ```text
   Draft a reply from me to Priya and the group confirming I will set up the 10:00 call for tomorrow with the contractor, Environmental, and Scheduling; bring the current clearing plan with the May 1 nesting-bird constraint marked for a live redline; and target the revised clearing sequence back to Hector by Friday. Professional, three short paragraphs. Do not send — I will review.
   ```

2. Read it aloud. If it does not sound like you, tell Copilot what to change — "shorter," "warmer," "more direct" — or use **Adjust with Copilot** and **Coaching by Copilot** to tune tone and length. Do not accept a draft that is not your voice.

**Validate:** The draft confirms the 10:00 call, the plan with the May 1 constraint, and the Friday target back to Hector; every date and commitment matches the thread; and it reads the way you would actually write it. Do not select send.

### Task 6 — Draft the leadership one-pager (2 min)

1. Type `/`, select **Weekly Leadership One-Pager — North Delta**, then run:

   ```text
   Draft the half-page one-pager Priya asked for. Cover where Reach 3 and Amendment #7 stand: status, cost, approvals outstanding, and the top risks. Add one line on the PC-006 nesting-bird risk. Where a figure is not stated in my mail, leave a [confirm] placeholder rather than guessing. Do not send.
   ```

2. Fill or confirm each `[confirm]` placeholder against the source before this goes anywhere near leadership.

> [!NOTE]
> The `[confirm]` instruction is doing safety work. Copilot drafts from what it can read; asking it to mark unknowns instead of inventing them keeps a made-up number out of a leadership document. In a government tenant, that verify-before-you-rely habit is the point.

**Validate:** The one-pager pulls Reach 3 status, the Amendment #7 60-day/$163K decision and outstanding approvals, the top risks, and the PC-006 line — with placeholders wherever the mail does not actually state a figure.

---

## Hands-On Practice: Your Turn

Pick a real, non-sensitive thread from your own inbox and run the same flow end to end:

1. **Catch up**, then **turn it into a 2-on-2 update** with decisions, actions, owners, risks, and a "Decision needed from you" line.
2. **Interrogate it**: ask the two or three questions you would have to answer about it in a meeting, and click a citation to confirm one answer.
3. **Draft a reply** in your voice and adjust it once, and **draft the note or update** you owe someone, using `[confirm]` for anything the thread does not actually state.

Confirm every date, name, figure, and commitment against the source before you would send. Notice how much of the thread you can now act on in a few minutes, without re-reading a single message.

## Key takeaways

* Working a thread is more than summarizing it: extract decisions and owners, interrogate the trade-offs, and shape the output into the update you actually owe.
* Naming the thread as your Source is what grounds the answer in GCC, where web is off by default.
* Copilot drafts; you verify. Confirm every fact against the messages, use `[confirm]` for unknowns, and keep the send button yours.
