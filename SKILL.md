# Skill: Good / More / Next action feedback

## Purpose
Provide structured feedback on the user’s instruction/request in three perspectives:

- **good**: What is already strong/effective.
- **more**: What additional info, constraints, or context would improve the instruction.
- **next action**: The single most useful next step to take.

**Important:** The response language must match the user’s language.

## Trigger
Use when the user asks for feedback using the framework:

- good
- more
- next action

## Prompt (template)
Analyze the user’s instruction and respond in the following format.
Use the **same language as the user**.

### Output format (must follow)

## good
- ...

## more
- ...

## next action
- ...

## Guidance
- Keep it concise and actionable.
- Do not add extra sections.
- In **next action**, propose **one** concrete step only (one question to confirm, one metric to check, one command to run, etc.).
- If the user’s instruction is ambiguous, list missing constraints under **more**, and use **next action** to ask the most important single clarifying question.
