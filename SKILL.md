---
name: prompt-feedback-skill
description: >
  Provide structured feedback on the user's instruction or request
  using the "good / more / next action" framework. Use when the user
  asks for feedback with those keywords. Saves feedback to a local file.
allowed-tools: Bash(mkdir:*) Bash(cat:*)
---

# Instructions

Analyze the user's instruction and provide feedback in three perspectives.
Always respond in the **same language as the user**.

## Steps

1. Read the user's instruction carefully.
2. Identify strengths (**good**), missing information (**more**), and the single most useful next step (**next action**).
3. Respond using the output format below.
4. Save the feedback to a file (see [Saving feedback](#saving-feedback)).

## Output format (must follow)

```
## good
- ...

## more
- ...

## next action
- ...
```

## Guidance

- Keep it concise and actionable.
- Do not add extra sections.
- In **next action**, propose **one** concrete step only (one question to confirm, one metric to check, one command to run, etc.).
- If the user's instruction is ambiguous, list missing constraints under **more**, and use **next action** to ask the most important single clarifying question.

## Saving feedback

After generating the feedback, save it to a Markdown file:

- **Directory:** `~/.local/share/prompt-feedback-skill/`
  - Create the directory if it does not exist: `mkdir -p ~/.local/share/prompt-feedback-skill`
- **Filename:** `YYYYMMDD-HHMMSS.md` (local timezone)
- **File content:**

```
# <one-line summary of the conversation>

## good
- ...

## more
- ...

## next action
- ...
```
