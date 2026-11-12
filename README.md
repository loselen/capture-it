# capture

A tiny agent skill for catching ideas while you're busy, and deciding what to explore next once you're free.

## How it works

1. **Capture** — whenever something interesting pops into your head, throw it in. It's appended to `~/Documents/ideas.md`, in your own words.
2. **Repeat** — keep capturing as long as your current project runs.
3. **Eliminate** — when the project is done, go through every idea one by one and mark it:
   - **Interesting**
   - **Not interesting**
   - or leave a **comment**
4. **Synthesize** — the AI combines your interesting ideas and comments into **one** next thing to explore.
5. **Reset** — the idea file is cleared, ready for the next cycle.

## Install

```bash
npx skills add loselen/capture
```

## Usage

Capture an idea:

```
/capture a tool that turns voice memos into todo lists
```

Run elimination when you're done with your current project:

```
/capture elimination
```

## Where are my ideas stored?

`~/Documents/ideas.md` — a plain markdown list. You can open and edit it by hand anytime.
