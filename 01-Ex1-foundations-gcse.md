---
lab:
  title: 'Exercise 1: Write and Refine a GCSE Prompt in Microsoft 365 Copilot'
  description: 'Build the GCSE prompting habit in three steps — write a structured prompt, ground it on your own file, then do it on real work — in a GCC tenant where web grounding is off.'
  duration: 12 minutes
  level: 200
  islab: true
  primarytopics:
    - Microsoft 365 Copilot
    - Prompting
---

# Exercise 1: Write and Refine a GCSE Prompt in Microsoft 365 Copilot (12 min)
---

In Module 1 you learned that a strong prompt names four elements (Goal, Context, Source, Expectations), and that in a government tenant Microsoft 365 Copilot grounds on your own work content, not the open web. This exercise builds that habit in three steps: write a structured prompt (crawl), add a file and ground it (walk), then do it on real work of your own (run).

> [!TIP]
> Keep **GCSE** in front of you: **G**oal (what to produce), **C**ontext (why and who), **S**ource (which of your files), **E**xpectations (tone, length, format). In your DWR GCC tenant, public-web grounding is off by default, so on real DWR work the **Source** element matters most: if you do not name the file, Copilot cannot reach out to the web to fill the gap. You'll add Source in Task 2 — start without it.

### Task 1 — Crawl: Write your first structured prompt (3 min)

Start with the shape of a good prompt, before touching any files. Here you use three of the four GCSE elements — **Goal, Context, Expectations** — on a general-knowledge task, and add the fourth (Source) in Task 2.

1. Open **Microsoft 365 Copilot** in your GCC tenant.
2. Run this deliberately vague prompt and read what comes back:

   ```text
   tell me about atmospheric rivers
   ```

3. Now give it Goal, Context, and Expectations. Paste and run:

   ```text
   Goal: Write a plain-language, two-sentence definition of an atmospheric river. Context: it is for a public fact sheet aimed at California residents with no technical background. Expectations: neutral, non-alarming tone, under 40 words, no jargon.
   ```

4. Compare the two. Same topic, but the structured ask comes back tighter, shorter, and ready to paste.

> [!NOTE]
> You did not name a **Source** here because an atmospheric river is general knowledge — with web grounding off, Copilot still answers general questions from its underlying model. But most of your real DWR work is not general knowledge; it lives in your files. Pointing Copilot at those files is the Source element, and that is what Task 2 adds.

**Validate:** Your structured answer is noticeably shorter and more usable than the "tell me about atmospheric rivers" reply.

### Task 2 — Walk: Add the Source and ground on your file (5 min)

Now add the fourth element. In your GCC tenant, **Source** does the heavy lifting: with web off, naming a file is what gives Copilot something DWR-specific to work from.

1. Staying in **Microsoft 365 Copilot**, attach a file so Copilot grounds on it. Type `/` and select **Weekly_Project_Notes** from the ContextIQ menu, or select the **+** button and choose the file. Naming the file this way is what points Copilot at your content instead of leaving it to guess.
2. Paste and run this full GCSE prompt (all four elements, each labeled so you can see them):

   ```text
   Goal: Draft a one-page weekly status update for my supervisor. Context: I am an analyst in the Division of Flood Management at DWR, summarizing my week for our Monday check-in. Source: Use only the notes in Weekly_Project_Notes. Expectations: Plain, professional language, grouped under Accomplishments, In Progress, and Blockers, no more than six bullets total, and flag anything that needs my supervisor's decision.
   ```

3. Evaluate the response against your Source. Every point should trace back to something in `Weekly_Project_Notes`. Select a citation and confirm it points to your file, not the web.

> [!NOTE]
> Notice how much the Source line is doing. With web grounding off in GCC, if you had left out "Use only the notes in Weekly_Project_Notes," Copilot would have nothing DWR-specific to draw on and the draft would be generic. Naming the file is not optional in a government tenant, it is what makes the answer real.

**Validate:** Your response is organized into Accomplishments, In Progress, and Blockers, stays within six bullets, and every bullet traces to content in `Weekly_Project_Notes` (confirmed by clicking a citation).

### Task 3 — Run: Your turn on real work (4 min)

Pick one real task you own this week at DWR and write one full GCSE prompt for it, naming a specific file in your **DWR-Copilot** folder as the Source. Run it, read the response against your Source, and refine once. Be ready to read your prompt aloud and point to where each of the four GCSE elements appears.

> [!TIP]
> A quick self-check before you run any prompt in the DWR tenant: can you point to your Goal, your Context, your Source file, and your Expectations? If the Source is missing, stop and add it, because with web off there is nothing else for Copilot to stand on.
