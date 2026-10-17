# AI School Skills

Run your own school with Claude or Codex. You pick the classes, and each class gets its own teacher. The teacher researches the subject, plans your lessons around your strengths and weak spots, and tutors you. That means guiding you to the answer instead of handing it over, and when you're wrong, figuring out why and fixing the thinking behind it.

The goal is to actually understand what you learn, well enough to use it on your own and explain it out loud in a job interview.

> **Built for Claude Projects.** This is built and optimized for the Projects feature in Claude (in beta right now, and for Projects once it is fully released). In a Project, the project chat acts as your principal, every class gets its own thread with its own teacher, and lessons can arrive on a schedule. It also works in Claude Code, the Claude app and Codex, with one conversation per class.

## What's inside

Two skills that work together:

- **`ai-school-setup`, the admissions counselor.** Interviews you before school starts: first a set of standard questions, then personal follow-ups built from your answers until it really knows where you stand. Then it writes your student profile, sets up your classes and opens one teacher per class.
- **`school-teacher`, the teacher.** Teaches one class:
  - **Plans four weeks at a time,** with a goal for each week and a small project you can show off at the end.
  - **Teaches one small lesson a day:** a warm-up quiz on earlier lessons, the big idea in plain English with an analogy from your world, a hands-on task you do yourself, a "teach it back" step, and one line you could say in an interview.
  - **Guides instead of telling.** When you're stuck it asks a question, then gives a hint, then shows a similar example, and only shows the answer as a last resort.
  - **Holds you to the problem as given.** Requirements are stated up front. A better idea gets praise, but you still solve what was asked, because real work comes with set requirements.
  - **Fixes the thinking behind mistakes,** not just the wrong line, and keeps bringing weak spots back until you get them right twice in a row.
  - **Keeps a record** of your strengths, weak spots and misconceptions.
  - **Follows a weekly rhythm:** lessons on weekdays, a free day, and a planning day where it reviews your week and writes a short report for the principal.

## Install

Pick the one that matches what you use. Each block can be copied and pasted as is.

### Claude Projects, Claude.ai or the Claude app (as skills)

1. Download this repository (green **Code** button, then **Download ZIP**) and unzip it.
2. Make two zips: one of the `skills/ai-school-setup` folder and one of the `skills/school-teacher` folder.
3. In Claude, go to **Settings > Capabilities**, find **Skills**, click **Upload skill** and upload each zip. (Code execution needs to be turned on.)

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

Start setup with `/ai-school:ai-school-setup`.

### OpenAI Codex

Codex reads skills from a `.agents/skills` folder. Paste this in a terminal (Mac, Linux, or Git Bash on Windows) to install both skills for every project:

```
git clone https://github.com/Jaesonmoment/AI-School-Skills.git
mkdir -p ~/.agents/skills
cp -r AI-School-Skills/skills/* ~/.agents/skills/
```

To use them in one project only, copy the folders into that project's `.agents/skills/` folder instead. You can also ask Codex's built-in `$skill-installer` to install them from this repository's link.

## Getting started in a Claude Project

1. **Create a project** for your school.
2. **Turn on memory for the project** if it's offered. The principal and teachers then remember your decisions between sessions instead of asking again.
3. **Paste in a goal and instructions** (see "Copy and paste setup" below). You can also let the admissions counselor write these for you in step 4.
4. **In the project chat, say:** `Run ai-school-setup and enroll me.` The counselor interviews you, reads back what it heard, then sets up your school and opens a thread for each class.
5. **Answer each teacher's starting questions** in its thread. Lessons start after that.

From then on, the project chat is your principal: go there to add, drop or pause a class, or to ask how things are going.

## Getting started anywhere else

1. Start a conversation and say `Run ai-school-setup and enroll me.` (In Claude Code: `/ai-school:ai-school-setup`.)
2. When it's done, open a new conversation for each class and say `You're my teacher for [class]. Follow the school-teacher skill.`

Prefer to skip the interview? Copy `skills/school-teacher/student-template.md` into a `school/` folder as `student.md`, fill it in, and start your class conversations.

## Copy and paste setup

Claude can't change your settings for you, so setup comes down to a few blocks you paste in yourself. The admissions counselor writes personalized versions for you at the end of its interview, or you can start from the ones below.

**Before you paste anything, read it through.** Fix anything that's wrong, missing or not how you'd say it. Whatever you paste is what your teachers will follow.

Change anything in brackets.

**Project goal:**

```
My goal is to actually understand what I learn, well enough to use it on my own and [explain it in a job interview / pass my exam / build my project].

This is my own school. I pick the classes I want, and each class gets its own teacher. The teacher researches the subject, plans my lessons around my strengths and weaknesses, and tutors me. That means guiding me to the answer instead of handing it over, and when I'm wrong, figuring out why and fixing the thinking behind it.

How the week works: lessons [Monday to Friday], [Saturday] is my free day, and [Sunday] is when teachers review my progress and plan the next week. Lessons should be fun and tied to things I already know and the projects I'm working on.
```

**Project instructions:**

```
Teachers follow the school-teacher skill. New students start with the ai-school-setup skill.

Keep goals, project descriptions, skills and templates general. Only get specific when I ask for one specific thing.

Teacher attitude: [compassionate, eager to teach, helpful, pushy about drilling topics until they stick].
```

**Personal preferences** (in Claude's settings, under your personal preferences; these apply to every chat, so only include what you want everywhere):

```
About me: [who you are, what you do, what you're learning and why].

How I like to be taught: [for example plain English, short lessons, real examples, challenge me].

Rules: [anything Claude should always or never do, for example how it writes or tools to avoid].
```

### Example: the school this was built for

This came out of my own AI school, which runs in a Claude Project with one thread per class and the project chat as principal. My project goal, word for word:

> My goal is to actually understand what I learn, well enough to use it on my own and explain it out loud in a job interview.
> This is my own school. I pick the classes I want, and each class gets its own teacher. The teacher researches the subject, plans my lessons around my strengths and weaknesses, and tutors me. That means guiding me to the answer instead of handing it over, and when I'm wrong, figuring out why and fixing the thinking behind it.
> How the week works: lessons Monday to Friday, Saturday is my free day, and Sunday is when teachers review my progress and plan the next week. Lessons should be fun and tied to things I already know and the projects I'm working on.

And my project instructions:

> Match how specific my request is. Goals, project descriptions, skills and templates stay general (no specific class names, tools or current details). Only get specific when I ask for one specific thing.
>
> Disregard the "Decision System" format of writing. I need teachers not minions.
>
> #Teacher Attitudes
> Compassionate, Eager to teach, Helpful, Pushy when it comes to drilling topics into student's head.

(The "Decision System" line switches off a reply format from my personal Claude settings. You won't need it unless you use something similar.)

Each class thread also has a daily scheduled task that loads the teacher skill, so lessons show up on their own every lesson day, and the teachers send the principal a short report every planning day.

## Make it your own

Everything is written in plain English in [`skills/school-teacher/SKILL.md`](skills/school-teacher/SKILL.md) and [`skills/ai-school-setup/SKILL.md`](skills/ai-school-setup/SKILL.md). Change the interview questions, the lesson format, the weekly schedule or the teaching style to fit how you learn. Pull requests with improvements are welcome.

## What's in this repo

- `skills/ai-school-setup/SKILL.md`: the admissions counselor.
- `skills/school-teacher/SKILL.md`: the teacher.
- `skills/school-teacher/student-template.md`: the "about me" file, if you'd rather fill it in yourself.
- `.claude-plugin/`: the files that let Claude Code install this as a plugin.

Sources: [Claude Code plugins](https://code.claude.com/docs/en/plugins/install), [Skills in Claude](https://support.claude.com/en/articles/12512180-using-skills-in-claude), [Codex skills](https://developers.openai.com/codex/skills). The admissions interview draws on [Learning Styles: Concepts and Evidence](https://digitalcommons.usf.edu/psy_facpub/1765/) (why it doesn't sort you into a "learning style"), [the OARS method from motivational interviewing](https://health.uconn.edu/sbirtacademy/wp-content/uploads/sites/101/2018/03/MI-OARS-Handout.pdf) (open questions, reflecting back, summaries) and [diagnostic assessment](https://www.learningguild.com/articles/designing-it-right-making-an-impact-with-diagnostic-assessments) (checking real level, not just self-ratings).

## License

MIT. Use it, change it, share it.
