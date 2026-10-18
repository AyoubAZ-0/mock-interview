# Mock Interview

An AI agent skill that runs a realistic job interview from the user's resume and an optional job offer, then delivers a blunt debrief.

## What it does

The skill makes the agent act as a real interviewer: it collects the resume, the job offer (optional), the interview type (HR, technical, or mixed), the language, and the seniority level. It then asks one question at a time, pushes on vague claims, and stays in character with no hints or praise. When the interview ends, it breaks character and gives a verdict, scores, best and worst answers, resume risks, and the top three things to fix.

## Structure

```text
mock-interview/
├── SKILL.md              # Skill instructions + frontmatter (name, description)
└── agents/
    └── openai.yaml       # UI metadata for skill lists and chips
```

## Usage

Use the skill when you want to practice, for example:

- "interview me"
- "mock interview"
- "prepare me for an interview"

Provide your resume, and optionally the job offer you are targeting.

## Install

Place the `mock-interview/` folder in a skills directory your agent reads, such as `.agents/skills/` for Codex, or require it explicitly with `$mock-interview` where supported.

## License

MIT. See [LICENSE](LICENSE).
