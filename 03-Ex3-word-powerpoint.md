---
lab:
  title: 'Exercise 3: Draft a Duty Statement and Build an Alternatives-Analysis Deck'
  description: 'Use Microsoft 365 Copilot to draft a duty statement in Word, turn an accomplishments list into a narrative, and build an alternatives-analysis deck in PowerPoint — then verify every figure, in a GCC tenant where web grounding is off.'
  duration: 12 minutes
  level: 200
  islab: true
  primarytopics:
    - Microsoft 365 Copilot
    - Word
    - PowerPoint
---

# Exercise 3: Draft a Duty Statement and Build an Alternatives-Analysis Deck (12 min)

Government artifacts are held to a higher bar than everyday writing: a duty statement is posted for a civil-service recruitment, an accomplishments narrative goes into the record, and an alternatives-analysis deck supports a funding decision. In this exercise you use Microsoft 365 Copilot to draft each one fast, then you do the part Copilot cannot do for you: verify every figure, confirm nothing was invented, and keep internal notes out of published text. You work entirely in your DWR GCC tenant, so Copilot grounds on the resource files in your **DWR-Copilot** OneDrive folder, not the open web.

> [!TIP]
> Keep the **GCSE** framework from the Lab Setup in front of you: name the **Goal**, add the **Context** (who you are, what the artifact is for), point Copilot at the right **Source** file, and state your **Expectations** for structure, tone, and length. For government work, add one discipline on top of GCSE: **Copilot drafts, a person verifies.** Every percentage must total 100, every figure must trace back to the source, and nothing internal-only may appear in a public document. Read before you rely on it.

### Scenario

You are an analyst in the Division of Integrated Regional Water Management at the California Department of Water Resources (DWR), filling a vacancy and prepping a leadership readout in the same week. First you need a clean duty statement for a new Water Resources Program Analyst position, built from a hiring manager's rough notes and following an approved reference. Then you need a project team's bulleted accomplishments turned into a short narrative for the record. Finally, you need a leadership deck that summarizes an alternatives-analysis memo for an upcoming funding decision. The resource files stand in for real DWR work.

> [!NOTE]
> DWR runs in a **GCC** tenant, so the newer in-canvas **Edit with Copilot** agent is not available in Word or PowerPoint, and the PowerPoint **Idea Coach** agent and **Allow editing** agent mode may not appear. Everything in this exercise uses features that work in GCC today: **Draft with Copilot** and **Rewrite with Copilot** in Word, document summarization, **create a presentation from a file** in PowerPoint, and the **Copilot chat pane** inside each app. Wherever an in-app control is missing in your build, the fallback is the same: open the **Copilot chat pane** in that app, reference the file with `/`, and ask for the same outcome.

### Task 1: Draft the duty statement in Word (5 min)

Turn the hiring manager's rough notes into a properly structured, verifiable duty statement that follows the approved reference.

1. Go to `https://www.office365.us`, sign in with your DWR credentials, select **Apps** > **Word**, and open a **blank document**.
2. Select the **Copilot** icon in the left margin of the page to open **Draft with Copilot**.
3. In the prompt box, type `/` to open the file reference menu and select **`Duty_Statement_reference.md`** from your **DWR-Copilot** folder. Type `/` a second time and also reference **`Duty_Statement_DRAFT_rough.md`**. (Copilot in Word lets you reference several files in one prompt.)
4. Enter a full GCSE prompt. Note that it tells Copilot to follow the reference for structure and use the rough notes for content, and it names the one thing to leave out:

   ```text
   Goal: draft an official California civil-service duty statement for a new vacancy. Context: I am an HR analyst at DWR filling a Water Resources Program Analyst position in the Division of Integrated Regional Water Management. Source: follow the exact structure, headings, and neutral tone of Duty_Statement_reference, and use only the duties described in Duty_Statement_DRAFT_rough for content. Expectations: include the Department, Division, Classification, Working Title, and Supervision Received header lines; an Essential Functions section where each function has a percent of time and the percentages total exactly 100; a Knowledge, Skills, and Abilities section; and a Work Environment section. Do not invent any duty that is not in the notes, and do not include any internal hiring preference or any note the manager marked as not for the posting.
   ```

5. Select **Generate**. Review the draft, then **Keep it** to insert it (or select **Regenerate** to try again).

> [!NOTE]
> If your build does not show the **Draft with Copilot** box on a blank document, open the **Copilot chat pane** in Word instead, reference both files with `/`, and paste the same prompt. Ask Copilot to "write the duty statement into the document." The Copilot chat pane is available in GCC.

**Validate:** Before you would use this, confirm four things. (1) The sections and headings match `Duty_Statement_reference` (Department/Division/Classification/Working Title/Supervision Received, Essential Functions, Knowledge/Skills/Abilities, Work Environment). (2) The Essential Functions percentages **total exactly 100** (the rough notes deliberately do not add up, so this is where a person must fix the math). (3) Every duty traces to a line in `Duty_Statement_DRAFT_rough`; nothing is invented. (4) The internal note about preferring someone who has used the state's grant management system does **not** appear anywhere in the draft. If any of these fail, correct it yourself; do not publish it as-is.

### Task 2: Turn the accomplishments list into a narrative (3 min)

Convert a bulleted list into two short paragraphs for the project record, then rewrite for length and tone.

1. Open a new **blank document** in Word. Open **Draft with Copilot**, type `/`, and reference **`Project_Accomplishments_List.md`** from your **DWR-Copilot** folder.
2. Enter a GCSE prompt for a narrative:

   ```text
   Goal: write a two-paragraph narrative summary of a capital project's accomplishments for the project record. Context: this is a year-end writeup for the North Delta Levee Rehabilitation project at DWR. Source: use only the accomplishments in Project_Accomplishments_List. Expectations: two paragraphs, third person, plain professional government tone, and do not add any accomplishment, dollar figure, or statistic that is not in the list.
   ```

3. Select **Generate**, then **Keep it** to insert the narrative.
4. Refine the tone and length. Select the narrative text, then choose **Rewrite with Copilot** from the Copilot options next to the selection. Give it a specific instruction and iterate once:

   ```text
   Rewrite this to be more concise and neutral in tone, suitable for an official project record. Keep every figure exactly as written and do not add anything new.
   ```

5. Compare the suggestion, then select **Replace** to accept it (or keep your original).

> [!NOTE]
> If the in-selection **Rewrite with Copilot** control does not appear in your build, open the **Copilot chat pane** in Word, reference the document, and ask it to "rewrite the selected passage to be more concise and neutral, keeping every figure." Rewrite and the chat pane are both available in GCC; the **Edit with Copilot** canvas is not.

**Validate:** Read the final narrative against `Project_Accomplishments_List`. Every fact must trace to a bullet: the 60% design figure, the 140 workshop attendees, the $4.2 million grant, 11 of 14 permit conditions closed, and the schedule slip cut from 5 months to 2. If Copilot rounded, merged, or added a number, fix it. A narrative for the record inherits the accuracy of the list, nothing more.

### Task 3: Build the alternatives-analysis deck in PowerPoint (4 min)

Create a short, conclusion-first leadership deck from the source memo, with speaker notes.

1. Select **Apps** > **PowerPoint** and open a **new presentation** (start from your branded DWR template if your instructor provided one, so the deck respects DWR design).
2. Select the **Copilot** icon in the bottom-right corner of the slide to open the Copilot pane, then choose **Create presentation from file**.
3. In the prompt field, type `/` (or select the **paperclip** icon) and reference **`Alternatives_Analysis_source.md`** from your **DWR-Copilot** folder. Add your shaping instructions in the same prompt:

   ```text
   Create a concise executive presentation from Alternatives_Analysis_source for a DWR leadership funding decision. Keep it to about seven slides. Lead with the recommendation, then one slide per alternative, then the evaluation criteria. Write slide titles as conclusion-first statements, not topics. Use a professional, data-driven tone for executives with limited time. Add brief speaker notes to each slide. Use only the costs, service-life figures, schedules, and risks in the file; do not add any figure that is not in the source.
   ```

4. Review the outline Copilot proposes, refine it in the pane if needed (for example, **"combine the two low-environmental-impact points"** or **"add a closing slide that restates the recommended alternative"**), then confirm to generate the deck.

> [!NOTE]
> In GCC the **Idea Coach** agent and the **Allow editing** agent mode described in some Microsoft docs may not be available. If the **Create presentation from file** option is missing, open the **Copilot chat pane** in PowerPoint (or the Microsoft 365 Copilot app), reference `Alternatives_Analysis_source` with `/`, paste the same prompt, and ask Copilot to build the outline; then use PowerPoint's light commanding to add the slides. Create-a-presentation and summarization are available in GCC.

**Validate:** This deck supports a funding decision, so accuracy is not optional. Confirm that (1) the recommended alternative is **Alternative 1, Rehabilitate in place**, matching the memo's Recommendation; and (2) every figure on every slide matches the source exactly, for example Alternative 1 at $18.5 million / 25-year service life / 14 months, Alternative 2 at $41.0 million / 50 years / 30 months, and Alternative 3 at $22.0 million near-term. If a slide shows a number that is not in `Alternatives_Analysis_source`, delete or correct it before you present.

### Hands-On Practice: Your Turn

Pick one of these three flows and run it on a real document or deck from your own DWR work:

1. **Draft grounded on a reference.** Open a real approved document you can use as a structure reference, and a set of rough notes for something new. Use **Draft with Copilot** in Word, referencing both files, and write a GCSE prompt that says "follow the reference for structure, use the notes for content, invent nothing." Then verify: structure matches, figures are right, nothing internal leaked in.
2. **List to narrative.** Take a real bulleted list of yours (status updates, accomplishments, meeting outcomes) and draft it into a short narrative, then **Rewrite with Copilot** for tone and length. Confirm every fact traces back to your list.
3. **Source doc to deck.** Take a real memo or report and use **Create presentation from file** in PowerPoint for a conclusion-first summary deck with speaker notes. Verify the recommendation and every figure against the source.

Whichever you choose, keep the government discipline in front of you: Copilot produces the draft in seconds, and the few minutes you spend verifying it are what make the artifact safe to post, file, or present.
