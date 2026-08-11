---
lab:
  title: 'Exercise 4: Summarize a Permit Workbook and Draft a Weekly Summary'
  description: 'Use Microsoft 365 Copilot to summarize and question a DWR permit-conditions workbook the GCC-safe way, understand why in-grid Excel analysis is not used here, and draft a weekly project summary from OneNote-style notes.'
  duration: 12 minutes
  level: 200
  islab: true
  primarytopics:
    - Microsoft 365 Copilot
    - Excel
    - OneNote
---

# Exercise 4: Summarize a Permit Workbook and Draft a Weekly Summary (12 min)

In this final exercise you do two everyday jobs at the California Department of Water Resources (DWR): make sense of a spreadsheet of environmental permit conditions, and turn a week of rough project notes into a clean weekly summary. You work entirely in your GCC tenant, so you use the approaches that actually run there today, not the ones from the public demos.

Both tasks use the same core move you learned in Module 4: instead of asking Copilot to work inside the grid of a spreadsheet, you reference the file in the **Microsoft 365 Copilot chat pane** and ask a grounded question about it.

> [!TIP]
> In GCC, analyze a spreadsheet by referencing the file in the **Microsoft 365 Copilot chat pane**, not by working inside the grid. Attach the workbook with the **+** button, or type **/** and pick it from the **ContextIQ** menu, then ask for a written answer about its contents. Copilot can reason over a file you give it and describe what is in it in plain language.

### Scenario

You are a project analyst at DWR supporting the **North Delta Levee Rehabilitation** capital water project. It is the week of April 6, 2026. You have two things to produce before Friday: a quick read of where the project's environmental permit conditions stand for a compliance check-in with the program manager, and the weekly project report that goes up to leadership. Both start from files, and both are faster if Copilot reads them for you.

Before you start, confirm the resource files from Lab Setup are in your **DWR-Copilot** folder in OneDrive: `Permit_Conditions.csv` (or the `Permit_Conditions.xlsx` version if your instructor provided one) and `Weekly_Project_Notes.md`.

## Task 1: Summarize the permit workbook in the Copilot chat pane (5 min)

You want a written picture of the permit conditions before the check-in: how many there are, how many are done versus still open, and who carries the most. In GCC you get this from Copilot reading the workbook, not from Copilot rearranging the sheet.

1. Open **Microsoft 365 Copilot** for your GCC tenant (the same place you used in the earlier exercises).
2. In the prompt box, attach the permit workbook: select the **+** button and pick `Permit_Conditions` from your **DWR-Copilot** folder, or type **/** and choose it from the **ContextIQ** menu. Confirm the file appears as an attachment chip.
3. Ask for a written summary with a GCSE-framed prompt:

   ```text
   Goal: summarize the permit conditions in this workbook for a compliance check-in. Context: I am a project analyst at the California Department of Water Resources reviewing the North Delta Levee Rehabilitation project. Source: the attached Permit_Conditions workbook. Expectations: tell me the total number of conditions, then a count of how many are Complete, In Progress, Not Started, and At Risk, and a count grouped by responsible agency. Keep it to a short paragraph plus a bulleted list.
   ```

4. Read the response. It should be a paragraph of prose plus grouped counts, not a reformatted grid.

**Validate against the file.** Spot-check the numbers before you would ever put them in a briefing. Copilot summarizes what it reads, so verifying is part of the job.

- **Total conditions:** 14.
- **By status:** Complete 4, In Progress 4, Not Started 4, At Risk 2.
- **By responsible agency:** State Water Board 3, USACE 3, CDFW 3, DWR 3, Central Valley FPB 2.

> [!NOTE]
> Why this is the Copilot chat pane and not in-grid Excel analysis: in GCC, GCC High, and DoD, Copilot's ability to analyze structured Excel data is impacted until "Edit with Copilot in Excel" is released in those clouds, and Edit with Copilot in Word, Excel, PowerPoint, and OneNote is not currently available there. In plain terms, do not expect Copilot to sort, filter, highlight, suggest formulas, generate insights, or build a PivotTable inside the sheet in your tenant today. What does work now is exactly what you just did: reference the workbook in the Copilot chat pane and get a document-level summary. Feature availability is dated and changes over time, so recheck the Microsoft 365 Copilot service description rather than assuming today's limit is permanent.

## Task 2: Ask targeted follow-up questions (3 min)

Now narrow in on the two things the program manager will ask about: what is slipping, and what is coming due. Stay in the same chat so Copilot keeps the workbook in context.

1. In the same conversation, ask a focused follow-up:

   ```text
   Using the same workbook, which conditions are marked At Risk, and which conditions are due within 60 days of April 6, 2026? For each one, list the condition ID, description, due date, status, and owner.
   ```

2. Read the answer and check it against the file.

**Validate against the file.**

- **At Risk (2):** PC-006, avoid nesting bird season for tree removal, due 2026-05-01, owner M. Okafor; and PC-013, quarterly mitigation site monitoring, due 2026-07-01, owner R. Chen.
- **Due within 60 days of April 6, 2026 (through June 5, 2026):** PC-005 (2026-04-10, M. Okafor), PC-006 (2026-05-01, M. Okafor), PC-002 (2026-06-01, J. Alvarez), and PC-010 (2026-06-01, J. Alvarez).

Notice that PC-013 is At Risk but is not due in the next 60 days, and that the nesting-bird condition PC-006 is both At Risk and due soon. That is the kind of nuance the plain-language answer surfaces quickly, and the kind of thing worth confirming against the sheet before you repeat it.

## Task 3: Draft the weekly project summary from your notes (4 min)

Now turn the week's rough notes into the weekly report. The notes live in `Weekly_Project_Notes.md`, the kind of loose page you might keep in OneNote through the week.

1. Choose your path based on where your notes are:
   - **If your notes are on a OneNote page:** open that page, open the **Copilot chat pane in OneNote**, which is available in GCC, and ask it to summarize the page. Note that "Edit with Copilot" (writing directly onto the page) is not available in GCC, so you draft in the chat pane and place the text yourself.
   - **Otherwise (recommended for this exercise):** open **Microsoft 365 Copilot** and reference `Weekly_Project_Notes` with the **+** button or by typing **/**, the same way you attached the workbook in Task 1.
2. Ask for a structured draft with a GCSE-framed prompt:

   ```text
   Goal: draft a weekly project summary from these notes. Context: I am the project analyst for the North Delta Levee Rehabilitation project at DWR, and this update goes to my program manager. Source: the attached Weekly_Project_Notes for the week of April 6, 2026. Expectations: organize it under three headings, Accomplishments, Risks, and Next Week. Use only what is in the notes. Keep it under 200 words in a neutral, professional tone.
   ```

3. Read the draft, then tighten it with a follow-up:

   ```text
   Tighten this into a five-bullet executive summary a program manager can read in 30 seconds. Keep the May 1 nesting-bird deadline and the open borrow-material cost risk.
   ```

**Validate against the notes.** Every item in the draft must trace back to something written in `Weekly_Project_Notes.md`. If Copilot added a status that is not in the notes, cut it. Confirm both of these appear, because they are the two risks that matter:

- The **May 1 bird window**: tree removal must finish before May 1 (PC-006) or it slips a season.
- The **borrow-material cost risk**: still open, and the PM wants a number by next Wednesday.

Other items that should trace cleanly to the notes include the 60% design review acceptance for Reach 3 with two comments, grant reimbursement #3 submitted, the right-of-way parcel status, and the aligned milestone tracker. Because Copilot drafts only from what it reads, anything not in the notes should not appear, and a decision that was never written down will not either. Review and correct the draft before it becomes the official update.

### Hands-On Practice: Your Turn

Apply the same Chat-referencing approach to your own work.

1. Pick one of your own files: a spreadsheet you keep an eye on, or a page of running notes.
2. Attach it in **Microsoft 365 Copilot** with the **+** button or by typing **/**.
3. For a spreadsheet, ask for a written summary and one targeted follow-up (for example, what is overdue, or which category has the most open items), then spot-check the numbers against the file. For notes, ask for a structured summary under your own headings, then verify every point traces back to what you wrote.

Remember the two habits from this morning: route the task to the capability that exists in GCC (the Copilot chat pane referencing the file), and verify the output against the source before you use it.
