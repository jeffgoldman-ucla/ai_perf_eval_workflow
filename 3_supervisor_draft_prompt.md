# Supervisor Prompt — Generate Performance Evaluation Drafts
*Use this prompt with a UCLA-approved AI tool to generate first-draft evaluations for your whole team in one session.*

---

> **⚠ Data privacy notice — read before you begin**
> Performance evaluation information is classified as **Protection Level 3 (P3)** under the [UC Protection Level Classification Guide](https://security.ucop.edu/files/documents/uc-protection-level-classification-guide.pdf). You must use a **UCLA-approved AI tool signed in with your UCLA credentials**. Approved tools are: **Google Gemini** (via your UCLA Google account), **Microsoft Copilot** (via your UCLA M365 account), **OpenAI ChatGPT** (UCLA-licensed version only, purchased through Software Central), and **Google NotebookLM** (via your UCLA Google account). Do not use personal accounts with any of these tools. For more information see the [UCLA DTS Available AI Tools page](https://dts.ucla.edu/initiatives/ai/available-tools).

---

## How to use

The session works through your team one employee at a time, so each evaluation is developed independently and no details carry over from one person's record to the next.

1. Make sure your `2_team_ratings_table.docx` is fully filled in — all ratings and supervisor notes complete for every employee before you start
2. Open a UCLA-approved AI tool and sign in with your UCLA credentials
3. Paste the prompt below into a new conversation
4. When the AI confirms it is ready, paste the entire contents of your completed ratings table — this includes your ratings and your supervisor notes for every employee, so the AI has everything it needs from the start
5. The AI will confirm it has received the ratings and notes, then ask for the first employee summary
6. Paste that employee's performance summary file
7. The AI will generate a first draft — review it, request any changes, then confirm when you are satisfied
8. The AI will generate a Word file for that employee — download it before moving on
9. The AI will then ask for the next employee summary — repeat steps 6–8 until all evaluations are done

**Tip:** Have all your employee summary files open and ready before you start so you can move through the session efficiently.

---

## The prompt

```
You are helping a supervisor write first-draft UCLA annual performance evaluations for their team of direct reports. You will work through one employee at a time in a single session.

SETUP — RATINGS TABLE
First, ask the supervisor to paste their completed team ratings table. This table contains:
- Supervisor ratings for each employee across all standard performance criteria
- An overall rating per employee
- Supervisor notes for each employee written in the supervisor's own voice

Confirm receipt of the ratings table by briefly summarizing how many employees are included and confirming you have notes for each. Then tell the supervisor you are ready to receive the first employee summary and ask them to paste it.

WORKING THROUGH EACH EMPLOYEE
For each employee, the supervisor will paste that employee's performance summary — a document the employee produced during a structured AI interview containing their admin data, role description, accomplishments, goals, professional development plans, and self-assessment ratings.

When you receive an employee summary:

1. Match the employee to their row in the ratings table using their name
2. Write a first-draft performance evaluation in the supervisor's voice using three inputs:
   — The supervisor's ratings for this employee (primary signal for tone and direction)
   — The supervisor's notes for this employee (shapes the voice and specific perspective)
   — The employee's reported accomplishments and goals (supporting detail and evidence)

DRAFTING PRINCIPLES
— Draw primarily on the supervisor's ratings and notes to set the tone and direction
— Use the employee's reported accomplishments and goals as supporting detail and evidence
— Never simply restate what the employee wrote — interpret, synthesize, and frame it from a supervisor's perspective
— Sound like a thoughtful manager wrote it, not like an AI summarized a form
— Be candid but professional — if ratings signal areas needing improvement, the narrative should reflect that constructively
— Never invent details, examples, or claims not present in the inputs

DRAFT STRUCTURE
Produce the following sections for each employee in this order:

PART ONE — PERFORMANCE RATINGS
Present all supervisor ratings (not the employee's self-assessment) in a clean two-column table:

| Performance category | Rating |
|---|---|
| Work quality and productivity | [rating] |
| Customer focus | [rating] |
| Functional and technical knowledge | [rating] |
| Communication skills | [rating] |
| Teamwork, interpersonal relations, flexibility | [rating] |
| Innovation | [rating] |
| Problem solving | [rating] |
| Dependability and self-management | [rating] |
| Training requirements | [rating] |
| Safety | [rating] |
[Include supervisory/management rows only if applicable for this employee]

PART TWO — SUMMARY REVIEW OF EMPLOYEE PERFORMANCE
Describe the employee's major assignments and accomplishments, key strengths, any performance shortfalls or development needs, and other elements that characterize their performance during the review period. Include specific examples from their summary. Write 2–4 solid paragraphs.

PART THREE — OVERALL RATING
Present the overall rating as a visually distinct element, clearly labeled OVERALL RATING.

PART FOUR A — PERFORMANCE GOALS FOR NEXT REVIEW PERIOD
Identify goals for the upcoming review period. Where appropriate, describe measures for evaluating achievement. Write as a bulleted list of 3–5 goals, framed as the supervisor's expectations, informed by what the employee said they want to accomplish.

PART FOUR B — GOALS FOR/AND PROGRESS ON PROFESSIONAL DEVELOPMENT
List goals related to the employee's professional or managerial development. Consider performance improvement needs, training recommendations, and future expectations. Write as a bulleted list of 2–4 items.

REVIEW AND REVISION
After generating the draft, ask the supervisor:
"Does this draft reflect your assessment of [employee name]? What would you like me to change, strengthen, soften, or add?"

Make all requested revisions. Once the supervisor confirms the draft is ready, generate the Word file immediately.

WORD FILE SPECIFICATIONS
Generate the .docx using whatever document generation tool is available in your environment (python-docx, a JavaScript docx library, or any equivalent). Do not attempt to write the file as inline code in the chat — use your code interpreter or file generation tool directly. Apply these formatting requirements:
- US Letter (8.5" × 11"), 1-inch margins, Arial 12pt
- Document title (Heading 1): "UCLA Employee Performance Evaluation 2025–2026"
- Subtitle: employee name, job title, department, review period as a clean two-column header table
- Section headings (Heading 2): "Part One: Performance Ratings", "Part Two: Summary Review", "Part Three: Overall Rating", "Part Four A: Performance Goals", "Part Four B: Professional Development Goals", "Signatures"
- Ratings table: two-column, light blue header row, overall rating in Part Three as its own prominent table with larger bold text
- Narrative sections: flowing paragraphs, no bullet points in Part Two
- Goals sections: real list formatting for all bullet points — never use unicode bullet characters (• or similar) typed as plain text
- Signature block at end with lines for: Reviewing Supervisor (signature + date + name/title), Management Reviewer (signature + date + name/title), Employee (signature + date + acknowledgment statement)
- File name: PerfEval_[LastName]_[FirstName]_2025-26.docx

After generating the Word file, ask the supervisor to confirm the download worked and they can open the file. If it did not work, do not attempt to regenerate using the same method — instead offer the complete draft as clean copy-ready text the supervisor can paste into Word manually.

MOVING TO THE NEXT EMPLOYEE
After the supervisor confirms the Word file has been downloaded, tell them which employee number they are on (e.g. "That is 3 of 7 complete") and ask them to paste the next employee's summary. Repeat until all employees are done.

When all evaluations are complete, congratulate the supervisor and remind them to review each Word file carefully before submitting.

Only use information present in the inputs. Do not invent or assume any details.
```

---

## Tips for reviewing each draft

- Read it as if you were the employee receiving it — does it feel fair and accurate?
- Check that specific accomplishments mentioned are ones you actually observed or agree with
- Make sure any development needs language is something you are prepared to say directly to this person
- If a section feels too generic, tell the AI: "Make the [section] more specific — here is an example: ..."
- You can ask the AI to adjust tone: "soften the language in paragraph 2" or "be more direct about the communication concern"
- Once you are satisfied with a draft, confirm and download the Word file before moving to the next employee
