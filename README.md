# Play Prompt Kit

A structured framework for building intimate interaction skills with LLMs. Includes an intake interview system that doubles as the first session, customizable play templates, a language grading system.

一个用于构建LLM亲密互动skill的结构化框架。包含需求访谈系统（本身就是第一场play）、可定制的玩法模板、语言分级系统。

## What's Inside / 内容

- **Intake Interview / 需求访谈**: 6-round structured interview that maps user preferences while functioning as the first play session, includes safe word setup
- **Play Profile Template / 用户画像模板**: Auto-generated profile from interview results with safety settings, severity levels, and editable anytime
- **10 Play Templates / 十种玩法模板**: Control, Intellectual Domination, Interrogation, Q&A Escalation, Discipline, Rule Horror, Role/Scene, Orgasm Control, Compliance Audit, Human RLHF (see `references/play-templates.md`)
- **Sub Language Grading System / Sub语言分级系统**: 3-level grading with auto-escalation and penalty accumulation (see `references/grading-system.md`)
- **Score/Penalty System / 积分惩罚机制**: Optional gamification layer
- **Cringe Blacklist / 油腻黑名单**: Universal list of phrases that kill the mood

## How to Use / 使用方法

1. Place `SKILL.md` in your Claude Code skills directory (`.claude/skills/play/SKILL.md`)
2. Place the `references/` folder alongside it (`.claude/skills/play/references/`)
3. Trigger by invoking `/play` or naturally entering the mood
4. First use auto-starts the intake interview
5. After interview, a `play-profile.md` is generated with your preferences
6. All subsequent sessions use your profile for personalized interaction

## Customization / 自定义

- Edit `play-profile.md` anytime to update preferences
- Add your own play templates to `references/play-templates.md`
- Adjust grading levels and scoring rules in `references/grading-system.md`
- Add to the cringe blacklist as needed


## Project Structure / 项目结构

```
play-prompt-kit/
├── SKILL.md                      # Core skill file (protocol + interview + principles)
├── README.md                     # This file
└── references/
    ├── play-templates.md         # 10 play type templates
    └── grading-system.md         # Sub language grading + score/penalty rules
```

## Bilingual / 双语

Full Chinese-English bilingual support throughout.
全文中英双语。

---

*This is a generic framework with no personal data. Fill it with your own preferences through the intake interview.*

*这是一个通用框架，不含任何个人数据。通过需求访谈填入你自己的偏好。*
