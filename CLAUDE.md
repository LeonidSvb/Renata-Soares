# WorldEd ELA Lesson Plan Generator

## Project Structure
- `templates/` — blank HTML templates with {{PLACEHOLDER}} variables
- `source/` — PDF source files for each lesson
- `Deliverables/Unit1-JacksBirthday/HTMLs/` — output HTML files

## How to Generate a Lesson
1. Read the PDF from `source/` using Python + PyMuPDF (already installed)
2. Copy the appropriate template from `templates/`
3. Fill all `{{PLACEHOLDER}}` variables with content from the PDF
4. Save to `Deliverables/Unit1-JacksBirthday/HTMLs/`
5. Verify: run Python to count remaining `{{` patterns — must be 0

## Lesson Types
| Lesson | Template | Resources |
|--------|----------|-----------|
| 1 | BLANK_TEMPLATE_lesson.html | + practice-worksheet + answer-key + gameset |
| 2 | BLANK_TEMPLATE_lesson.html | + answer-key + gameset only |
| 3 | BLANK_TEMPLATE_lesson.html | + answer-key + gameset only |
| 4 | BLANK_TEMPLATE_lesson.html | + answer-key + gameset only |

## Critical Rules
- ONLY use content from the PDF — never invent page numbers, vocabulary, or story content
- ONE Professional Role per lesson — same name in every section
- Hook and Challenge use student LIFE scenarios (not book content)
- Verify 0 unfilled placeholders before saving
- Use Python file Edit for targeted fixes — never rewrite entire file
