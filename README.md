# prompt-feedback-skill

Provide structured feedback on the user's messages in the conversation using the **good / more / next action** framework.

## Features

- **Structured feedback** in three perspectives: good, more, next action
- **Auto-save** — feedback is saved to `~/.local/share/prompt-feedback-skill/YYYYMMDD-HHMMSS.md` (local timezone)
- **Multilingual** — responds in the same language as the user

## Usage

```bash
/prompt-feedback-skill

✦ I will activate the prompt-feedback-skill to provide structured feedback on your messages.

✦ I will provide feedback on your messages based on the prompt-feedback-skill instructions and save it to a file.

✦ good
   - スキルの目的を理解した上で、「3つの選択肢を提示する」という具体的で実装可能な改善案を提示できている点。
   - フィードバックスキルを明示的に呼び出し、プロンプトの質を向上させようとする姿勢。

  more
   - 選択肢の提示形式（番号入力、キーワード選択など）や、候補の具体性（どのような差分ならどう出すか）についての詳細な好
     みがあれば、より意図に沿った修正が可能です。

  next action
   - 修正した SKILL.md の指示通りに動作するか、実際に何らかのファイルをステージングしてコミットを試行してみることをお勧めします。
```
