# AI-Assisted Performance Evaluation System
**UCLA Samueli School of Engineering | 2025–2026 Review Cycle**

*Developed by Jeff Goldman, Assistant Dean, UCLA Samueli School of Engineering, with help from an AI assistant*

---

## What this system is

This is a set of files and prompts that use an AI assistant to streamline the annual performance evaluation process. Instead of filling out the UCLA form from scratch for each person, the system lets employees document their own performance through a guided AI interview, lets you rate the whole team at once, and then has the AI write a first draft of each evaluation in your voice — which you review and edit before it becomes final.

The prompts in this package are designed to work with UCLA-approved AI tools. See the **Data Privacy and Approved Tools** section below before you begin.

---

## The files in this package

| File | What it is |
|---|---|
| `0_README.md` | This file |
| `1_employee_interview_prompt.md` | The prompt you send to each team member |
| `2_team_ratings_table.docx` | Your ratings and notes for the whole team |
| `3_supervisor_draft_prompt.md` | The prompt you use to generate each eval draft |
| `PerfEval_SAMPLE_Chen_Maya_2025-26.docx` | Example of the final Word output |

---

## How the workflow works

### Step 1 — You send the interview prompt to your team
Send each team member the file `1_employee_interview_prompt.md`. Tell them to:

1. Open one of the UCLA-approved AI tools in a browser (see the Data Privacy and Approved Tools section), and sign in with their UCLA credentials
2. Copy the entire contents of the file and paste it into a new conversation
3. Follow the AI's interview — it will ask about their role, accomplishments, goals, and self-assessment
4. At the end, the AI will attempt to generate a Word file to download — what happens next depends on which tool they are using:

| Tool | What to expect |
|---|---|
| **ChatGPT** (UCLA licensed) | A direct .docx download link should appear |
| **Gemini** (UCLA Google account) | The AI may offer to export to Google Docs — accept this, then download as Word from Google Docs using File > Download > Microsoft Word |
| **Copilot** (UCLA M365) | The AI may save to Word Online / OneDrive — download from there |
| **Any tool** | If none of the above produce a file, the AI will display copy-ready text — copy and paste it into a new Word document and save as `PerfSummary_[LastName]_[FirstName]_2025-26.docx` |

5. Email the Word file (or saved document) to you

The interview covers:
- Administrative data (name, ID, title, department, supervisor, review period)
- Role description
- Major accomplishments from the past year
- Performance goals for next year
- Professional development goals
- Self-assessment on all standard UCLA performance criteria

Employees can go back and change anything at any point during the interview before they send it to you.

---

### Step 2 — You collect the summaries
When you receive each employee's file, save them all to a single folder. Depending on which AI tool they used, files may arrive as a .docx attachment or as a Google Doc link — either is fine. If an employee sends a Google Doc, you can open it and download it as Word using File > Download > Microsoft Word. Files are named `PerfSummary_[LastName]_[FirstName]_2025-26.docx`.

---

### Step 3 — You fill in the team ratings table
Open `2_team_ratings_table.docx` in Word. The document has three parts:

**Part 1 — Standard criteria ratings grid** — one row per employee, one rating per major performance category. Use the codes from the rating scale at the bottom of the document (E, EE, FM, PM, DN). Type the full label in the OVERALL column (e.g. Exceeds Expectations). Do this for your whole team in one sitting so you can think across people comparatively.

**Part 2 — Supervisory criteria grid** — complete only for employees with management responsibilities, using the same rating codes.

**Part 3 — Supervisor notes** — write your own assessment of each employee in your own voice. Your perspective on what you observed, what stood out, and what needs to improve is central to an effective evaluation — the AI draws on your notes to write the draft, so thorough feedback here will produce a much stronger result than relying on the employee's summary alone. These notes are your working document and are not shared with employees.

---

### Step 4 — You generate first drafts for your whole team in one session
Open `3_supervisor_draft_prompt.md`. Then:

1. Open a UCLA-approved AI tool and sign in with your UCLA credentials
2. Copy the full prompt from the file and paste it into a new conversation
3. When the AI confirms it is ready, paste the entire contents of your completed ratings table — the AI reads all your ratings and notes for every employee at once
4. The AI will confirm receipt and ask for the first employee summary — paste it
5. The AI writes a complete first draft for that employee — review it and ask for any changes
6. When you are satisfied, confirm and the AI generates a Word file — download it before continuing
7. The AI then asks for the next employee summary — repeat until all evaluations are done

The AI keeps track of progress and tells you how many employees are complete after each one. Have all your employee summary files open before you start so you can move through the session without interruption.

---

## What the final Word doc contains

The output matches the structure of the UCLA performance evaluation form:

- Employee administrative information
- Performance ratings table (your ratings, not the employee's self-assessment) with the overall rating called out separately
- Part Two: Summary review narrative
- Part Four A: Performance goals for next review period
- Part Four B: Professional development goals
- Signature lines for supervisor, management reviewer, and employee

See `PerfEval_SAMPLE_Chen_Maya_2025-26.docx` for an example.

---

## Tips

- **Fill in the ratings table before you start generating drafts.** Having all your ratings and notes done first means you can move through the drafts quickly without stopping to think.
- **The more specific your supervisor notes, the better the draft.** A sentence like "Jane stepped up to manage the vendor transition when it went sideways in October and handled it well" gives the AI something real to work with. "Strong performer" does not.
- **You can ask the AI to revise any part of the draft** — adjust the tone, add an example, soften or sharpen language, rewrite a section entirely. Keep iterating until it sounds like you.
- **Employees can update anything during their interview.** If a team member realizes mid-interview they forgot an accomplishment or want to rephrase something, they just tell the AI and it picks up where it left off.

---

## Data privacy and approved tools

### How this data is classified

Performance evaluation data — including employee names, IDs, job titles, and written assessments of job performance — is classified as **Protection Level 3 (P3)** under the [UC Protection Level Classification Guide](https://security.ucop.edu/files/documents/uc-protection-level-classification-guide.pdf). P3 covers UC personnel records, which require meaningful data protections but are not subject to the most restrictive P4 controls (which apply to medical records, SSNs, and similar highly sensitive data).

### Which AI tools are approved

UCLA Digital & Technology Solutions has approved the following tools for use with P1–P3 data. **You must sign in with your UCLA credentials** — personal accounts with the same tools do not carry the same data protections.

| Tool | How to access |
|---|---|
| **Google Gemini** | [gemini.google.com](https://gemini.google.com) — sign in with your UCLA Google account |
| **Microsoft Copilot** | [copilot.microsoft.com](https://copilot.microsoft.com) — sign in with your UCLA M365 account |
| **OpenAI ChatGPT** | Requires a UCLA-purchased license via Software Central — personal ChatGPT accounts are not approved for P3 data |
| **Google NotebookLM** | [notebooklm.google.com](https://notebooklm.google.com) — sign in with your UCLA Google account |

For the full list of UCLA-approved AI tools and current guidance, visit the [UCLA DTS Available AI Tools page](https://dts.ucla.edu/initiatives/ai/available-tools).

### A note for colleagues at other institutions

If you are adapting this system for use outside UCLA, consult your institution's IT and HR policies to determine which AI tools are approved for personnel data before distributing these materials to your team.

---

## Questions

If something in this process isn't working the way you expect, the most useful thing to do is tell your AI assistant exactly what you were trying to do and what happened. It can help you troubleshoot, adjust the output, or try a different approach.

For questions or feedback about the system itself, contact Jeff Goldman, Assistant Dean, UCLA Samueli School of Engineering.
