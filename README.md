# AI School Skills

Run your own school with Claude or Codex. You pick the classes, and each class gets its own teacher. The teacher researches the subject, plans your lessons around your strengths and weak spots, and tutors you. That means guiding you to the answer instead of handing it over, and when you're wrong, figuring out why and fixing the thinking behind it.

The goal is to actually understand what you learn, well enough to use it on your own and explain it out loud in a job interview.

## What a teacher does

- **Starts by getting to know you.** Before the first lesson it asks five questions to find your real level.
- **Plans four weeks at a time,** with a goal for each week and a small project you can show off at the end.
- **Teaches one small lesson a day:** a warm-up quiz on earlier lessons, the big idea in plain English with an analogy from your world, a hands-on task you do yourself, a "teach it back" step, and one line you could say in an interview.
- **Guides instead of telling.** When you're stuck it asks a question, then gives a hint, then shows a similar example, and only shows the answer as a last resort.
- **Fixes the thinking behind mistakes,** not just the wrong line, and keeps bringing weak spots back until you get them right twice in a row.
- **Keeps a record** of your strengths, weak spots and misconceptions.
- **Follows a weekly rhythm:** lessons on weekdays, a free day, and a planning day where it reviews your week and writes a short report.

## Install

Pick the one that matches what you use. Each block can be copied and pasted as is.

### Claude Code (as a plugin)

Type this at the Claude Code prompt:

```
/plugin install ai-school --marketplace Jaesonmoment/AI-School-Skills
```

Answer `y` to add the marketplace, then pick where to install it. On older versions of Claude Code, use these two lines instead:

```
/plugin marketplace add Jaesonmoment/AI-School-Skills
/plugin install ai-school@ai-school-skill
```

### Claude.ai or the Claude app (as a skill)

1. Download this repository (green **Code** button, then **Download ZIP**) and unzip it.
2. Zip up just the `skills/school-teacher` folder.
3. In Claude, go to **Settings > Capabilities**, find **Skills**, click **Upload skill** and choose that zip. (Code execution needs to be turned on.)

### OpenAI Codex

Codex reads skills from a `.agents/skills` folder. Paste this in a terminal (Mac, Linux, or Git Bash on Windows) to install it for every project:

```
git clone https://github.com/Jaesonmoment/AI-School-Skills.git
mkdir -p ~/.agents/skills
cp -r AI-School-Skills/skills/school-teacher ~/.agents/skills/
```

To use it in one project only, copy the folder into that project's `.agents/skills/` folder instead. You can also ask Codex's built-in `$skill-installer` to install it from this repository's link.

## Getting started

1. Make a folder for your school (for example `school/`).
2. Copy `skills/school-teacher/student-template.md` into it as `student.md` and fill it in: your background, goals, interests, how you like to learn, and your schedule. Teachers read it before every lesson.
3. Start a new conversation for each class and say something like "You're my teacher for [subject]. Let's begin."

The teacher sets up the class folder, asks its five starting questions and takes it from there.

## Make it your own

Everything the teacher does is written in plain English in [`skills/school-teacher/SKILL.md`](skills/school-teacher/SKILL.md). Change the lesson format, the weekly schedule or the teaching style to fit how you learn. Pull requests with improvements are welcome.

## What's in this repo

- `skills/school-teacher/SKILL.md`: the teacher skill itself.
- `skills/school-teacher/student-template.md`: the "about me" file you fill in.
- `.claude-plugin/`: the files that let Claude Code install this as a plugin.

Sources for the install steps: [Claude Code plugins](https://code.claude.com/docs/en/plugins/install), [Skills in Claude](https://support.claude.com/en/articles/12512180-using-skills-in-claude), [Codex skills](https://developers.openai.com/codex/skills).

## License

MIT. Use it, change it, share it.
