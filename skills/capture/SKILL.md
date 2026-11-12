---
name: capture
description: Capture passing ideas into ~/Documents/ideas.md, and later run elimination mode to judge each idea and synthesize one next thing to explore. Use when the user wants to jot down an idea/thought, or says they finished a project and want to review/eliminate ideas.
---

# Ideas: capture & elimination

Idea file: `~/Documents/ideas.md`

Decide the mode from the user's message:
- They give an idea or thought → **Capture mode**
- They say elimination / review ideas / project done → **Elimination mode**
- Unclear → ask which one.

## Capture mode

1. If `~/Documents/ideas.md` doesn't exist, create it.
2. Append the idea as one bullet, in the user's own words (do not rewrite or expand it):
   ```
   - <idea>
   ```
3. Confirm in one short line. Nothing else.

## Elimination mode

1. Read `~/Documents/ideas.md`. If it's empty or missing, say so and stop.
2. Go through the ideas **one at a time**. For each, use AskUserQuestion showing the idea text, with options:
   - **Interesting**
   - **Not interesting**
   - (the built-in "Other" field is the **Comment** option — the user types their comment there)
   Record each answer.
3. After all ideas are judged, synthesize **one** next thing to explore:
   - Build only from ideas marked Interesting and from comments.
   - Ignore Not interesting ideas.
   - Output: the one next thing, plus a short reason showing which ideas/comments it came from.
4. Clear `~/Documents/ideas.md` (leave it as an empty file).
