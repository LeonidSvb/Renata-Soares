# WorldEd Lesson Plan Generator
### Soar in Reading — ELA Course | Powered by Claude Code

---

## What Is This Folder?

This folder contains everything you need to automatically generate lesson plans for the **Soar in Reading** course using Claude Code (AI assistant).

**What was already generated (Unit 1 — Jack's Birthday):**
- 4 complete lesson plan HTML files → ready to paste into Canvas
- 12 supporting files: worksheets, answer keys, and bingo game-sets

**What this tool can generate for you (Units 2–20):**
- Same set of files for every unit in the book
- You provide the lesson PDFs → Claude Code does the rest

---

## Folder Structure

```
WorldEd-LessonGenerator/
│
├── README.md                      ← You are reading this
├── CLAUDE.md                      ← Rules for Claude Code (do not edit)
│
├── templates/                     ← HTML templates (do not edit)
│   ├── BLANK_TEMPLATE_lesson.html
│   ├── BLANK_TEMPLATE_practice-worksheet.html
│   ├── BLANK_TEMPLATE_answer-key.html
│   └── BLANK_TEMPLATE_gameset-bingo.html
│
├── source/                        ← Put your lesson PDFs here
│   ├── Lesson_1_JacksBirthday_...pdf   (example — Unit 1)
│   ├── Lesson_2_JacksBirthday_...pdf
│   ├── Lesson_3_JacksBirthday_...pdf
│   └── Lesson_4_JacksBirthday_...pdf
│
└── Deliverables/
    └── Unit1-JacksBirthday/       ← Already generated, ready to use
        ├── HTMLs/                 (4 lesson plans)
        └── Worksheets/            (12 files)
```

---

## PART 1 — Using the Unit 1 Files (Already Done)

The files in `Deliverables/Unit1-JacksBirthday/` are ready to use right now.

### How to upload a lesson to Canvas

1. Open Canvas → go to the course page
2. Find the page for the lesson (or create a new page)
3. Click **Edit** on the page
4. Click the **HTML editor** button (looks like `</>` or `[ ]`)
5. **Select all** the existing content and **delete it**
6. Open the HTML file from `HTMLs/` folder in a text editor (Notepad, VS Code, etc.)
7. **Select all** (Ctrl+A) → **Copy** (Ctrl+C)
8. **Paste** into Canvas HTML editor (Ctrl+V)
9. Click **Save**

**Files to upload:**
| Canvas Page | File to use |
|-------------|-------------|
| Lesson 1 page | `HTMLs/lesson1_jacks_birthday.html` |
| Lesson 2 page | `HTMLs/lesson2_jacks_birthday.html` |
| Lesson 3 page | `HTMLs/lesson3_jacks_birthday.html` |
| Lesson 4 page | `HTMLs/lesson4_jacks_birthday.html` |

Worksheets and bingo games are print-ready — open in browser, print to PDF.

---

## PART 2 — Generating New Units (Units 2–20)

### What you need

**Claude Code desktop app** — installed on your computer.
Download at: https://claude.ai/download

**4 lesson PDF files per unit** — downloaded from Canvas LMS.
These are the lesson plan pages (like the Jack's Birthday PDFs in the `source/` folder).

---

### Step-by-step: Generating a new unit

**Step 1 — Download the 4 lesson PDFs from Canvas**

For each unit, Canvas has 4 lesson plan pages. Export or print each one as PDF:
- Lesson 1 PDF → save as `Lesson_1_[UnitName]_BP-English1A-2026.pdf`
- Lesson 2 PDF → save as `Lesson_2_[UnitName]_BP-English1A-2026.pdf`
- Lesson 3 PDF → save as `Lesson_3_[UnitName]_BP-English1A-2026.pdf`
- Lesson 4 PDF → save as `Lesson_4_[UnitName]_BP-English1A-2026.pdf`

Example for Unit 2 (Coach):
```
Lesson_1_Coach_BP-English1A-2026.pdf
Lesson_2_Coach_BP-English1A-2026.pdf
Lesson_3_Coach_BP-English1A-2026.pdf
Lesson_4_Coach_BP-English1A-2026.pdf
```

**Step 2 — Put the PDFs in the source/ folder**

Copy your 4 PDFs into the `source/` folder in this project.

**Step 3 — Open this folder in Claude Code**

1. Open the **Claude Code** desktop app
2. Open this project folder (`WorldEd-LessonGenerator/`)
3. Claude Code will automatically read the `CLAUDE.md` rules file

**Step 4 — Send this message to Claude Code**

Copy the message below. Replace the words in [brackets] with your unit information:

```
Generate all 4 lesson HTMLs and all worksheets for Unit [NUMBER] — [UNIT NAME].

The 4 lesson PDFs are in the source/ folder:
- Lesson_1_[UnitName]_BP-English1A-2026.pdf
- Lesson_2_[UnitName]_BP-English1A-2026.pdf
- Lesson_3_[UnitName]_BP-English1A-2026.pdf
- Lesson_4_[UnitName]_BP-English1A-2026.pdf

Save all outputs to:
- Deliverables/Unit[NUMBER]-[UnitName]/HTMLs/
- Deliverables/Unit[NUMBER]-[UnitName]/Worksheets/

Use the HTML templates from the templates/ folder.
Verify that 0 placeholders are left unfilled before finishing.
```

**Example for Unit 2 (Coach):**
```
Generate all 4 lesson HTMLs and all worksheets for Unit 2 — Coach.

The 4 lesson PDFs are in the source/ folder:
- Lesson_1_Coach_BP-English1A-2026.pdf
- Lesson_2_Coach_BP-English1A-2026.pdf
- Lesson_3_Coach_BP-English1A-2026.pdf
- Lesson_4_Coach_BP-English1A-2026.pdf

Save all outputs to:
- Deliverables/Unit2-Coach/HTMLs/
- Deliverables/Unit2-Coach/Worksheets/

Use the HTML templates from the templates/ folder.
Verify that 0 placeholders are left unfilled before finishing.
```

**Step 5 — Wait for Claude Code**

Claude Code will read the PDFs, generate all files, and report:
> "All 16 files generated — 0 unfilled placeholders. DONE."

This takes about 2–5 minutes.

**Step 6 — Upload to Canvas**

Your new files are in `Deliverables/Unit2-Coach/`. Follow the same Canvas upload steps from Part 1.

---

## Lesson Types Reference

| Lesson | Focus | Worksheets included |
|--------|-------|---------------------|
| Lesson 1 | Reading Comprehension | practice-worksheet + answer-key + bingo |
| Lesson 2 | Word Work | rfs-worksheet + answer-key + bingo |
| Lesson 3 | Writing / Personal Connection | rfs-worksheet + answer-key + bingo |
| Lesson 4 | Review + Quick Check | rfs-worksheet + answer-key + bingo |

---

## Troubleshooting

**"Claude Code says there are unfilled placeholders"**
> Tell Claude: *"Please fill all remaining placeholders using content from the lesson PDFs."*

**"The wrong content appeared in a lesson"**
> Tell Claude: *"Lesson 2 has incorrect content. Please regenerate it using only Lesson_2_[UnitName].pdf."*

**"I don't know how to get the PDFs from Canvas"**
> In Canvas, open the lesson plan page → click Print → Save as PDF. Or right-click → Print → Save as PDF.

**"The files are very large — can I send them by email?"**
> Use a file transfer service like WeTransfer (wetransfer.com) — free, no account needed, up to 2GB.

---

## Important Rules (Do Not Change These)

- **Never edit the files in `templates/`** — these are the master templates
- **Never edit `CLAUDE.md`** — this file controls how Claude Code behaves
- **Always put new PDFs in `source/`** before asking Claude Code to generate
- **Content must come from the PDFs only** — Claude Code will not invent information

---

## Unit Map — Soar in Reading 1

| Unit | Title | Status |
|------|-------|--------|
| Unit 1 | Jack's Birthday | ✅ Complete |
| Unit 2 | Coach | ⬜ Not generated |
| Unit 3 | Determining Theme | ⬜ Not generated |
| Unit 4 | Determining Main Idea | ⬜ Not generated |
| Unit 5 | Comparing and Contrasting Events | ⬜ Not generated |
| Unit 6 | Using Meaning Clues: Literature | ⬜ Not generated |
| Unit 7 | Using Meaning Clues: Informational | ⬜ Not generated |
| Unit 8 | Understanding Story Structure | ⬜ Not generated |
| Unit 9 | Comparing and Contrasting Text | ⬜ Not generated |
| Unit 10 | Analyzing Point of View | ⬜ Not generated |
| Unit 11 | Comparing and Contrasting Characters | ⬜ Not generated |
| Unit 12 | Using Visuals: Literature | ⬜ Not generated |
| Unit 13 | Using Visuals: Informational | ⬜ Not generated |
| Unit 14 | Identifying Supporting Reasons | ⬜ Not generated |
| Unit 15 | Making Inferences: Literature | ⬜ Not generated |
| Unit 16 | Combining Information | ⬜ Not generated |
| Unit 17 | Summarizing: Informational | ⬜ Not generated |
| Unit 18 | Using Mental Images: Literature | ⬜ Not generated |
| Unit 19 | Relating Events | ⬜ Not generated |
| Unit 20 | Relating Ideas | ⬜ Not generated |

---

*Generated with Claude Code — WorldEd School ELA Lesson Generator*
*Contact: leo@systemhustle.com*
