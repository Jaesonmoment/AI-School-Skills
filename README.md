# AI School Skills

Run your own school with Claude or Codex. You pick the classes, and each class gets its own teacher. The teacher researches the subject, plans your lessons around your strengths and weak spots, and tutors you. That means guiding you to the answer instead of handing it over, and when you're wrong, figuring out why and fixing the thinking behind it.

The goal is to actually understand what you learn, well enough to use it on your own and explain it out loud in a job interview.

> **Built for Claude Projects.** This is built and optimized for the Projects feature in Claude (in beta right now, and for Projects once it is fully released). In a Project, the project chat acts as your principal, every class gets its own thread with its own teacher, and lessons can arrive on a schedule. It also works in Claude Code, the Claude app and Codex, with one conversation per class.

## Quick start (Claude Projects)

Follow these steps in order. Every gray box can be copied and pasted as is.

1. **Install the skills.** Follow "Claude Projects, Claude.ai or the Claude app" under [Install](#install) below.
2. **Create a new project** in Claude for your school.
3. **Turn on memory for the project** if it's offered, so your principal and teachers remember your decisions between sessions.
4. **Start the admissions interview.** Paste this into the project chat:
   ```
   Run ai-school-setup and enroll me.
   ```
5. **Answer the counselor's questions.** First a standard set, then personal follow-ups built from your answers. When it reads back its summary, correct anything it got wrong.
6. **Paste in your setup blocks.** The counselor hands you a project goal, project instructions and personal preferences, each in its own copy box with where it goes. **Read each one before you paste it** and fix anything that's wrong or missing. (Prefer to write your own? Start from the templates in [Copy and paste setup](#copy-and-paste-setup).)
7. **Meet your teachers.** The counselor opens one thread per class. Answer each teacher's starting questions there, and lessons begin.

From then on, the project chat is your principal: go there to add, drop or pause a class, or to ask how things are going.

## What's inside

Eleven skills that work together. The teacher skill is home base and points to the others, so a teacher always knows which skill fits the job in front of it. Each skill also works on its own, outside a school: use `tutoring-and-feedback` while you learn something, or `explain-it-out-loud` to get ready for an interview, without setting anything up first.

| Skill | What it does |
|---|---|
| `ai-school-setup` | The admissions counselor. Interviews you before school starts, writes your student profile, sets up your classes and opens one teacher per class. |
| `school-teacher` | Home base for every teacher: who the teacher is, the ground rules, the school folder, the weekly rhythm, and which skill to use for each job. |
| `subject-research` | Researches a subject the way a careful teacher does. Finds how real teachers and courses already teach it, pulls their lesson plans, reads them in full and fact-checks every claim and example before anything reaches you. |
| `class-planning` | Starts a class with research first and a real placement check, then plans backward: what you must be able to do, what would prove it, then the lessons. Plans each week and each lesson, and suggests splitting a big subject into separate classes. |
| `lesson-teaching` | Teaches every lesson with the same routine, either live step by step (in-person classroom) or as a whole lesson you work through on your own (online class). |
| `tutoring-and-feedback` | Helps when you're stuck, wrong or turning in work, and checks work you made against its requirements. Finds the real cause, uses a hint ladder instead of handing over answers, and gives feedback you act on. |
| `practice-and-review` | Warm-ups, spaced review, quizzes, tests, notes and refreshers, built on the practice methods with the strongest research behind them. |
| `explain-it-out-loud` | Has you explain ideas in your own words and pushes the answer until it would hold up in a job interview. |
| `progress-reports` | Keeps an honest record of what you can do without help, and writes session reports, weekly reports and handoff notes. |
| `school-principal` | Runs the school from the project chat. Keeps the workload fair, reads the teachers' reports critically and sends you a weekly progress report. |
| `learner-support` | Adapts to how you focus and feel, using what works for neurodivergent learners as defaults that help everyone. |

What that adds up to:

- **Three roles per class, your pick.** A **study helper** helps you solidify something you're learning elsewhere, or go deep on one topic. A **full teacher** gives you the full classroom experience from the ground up. A **work checker** checks work you made and guides you to fix it without rewriting it for you. Every skill adapts to the role.
- **Researches first, then runs a real placement check.** A new class doesn't start from five questions. The teacher studies how real courses teach the subject, fact-checks what it finds, builds a skill map, and then tests you in rounds from the basics up, as long as the subject needs. It writes the class plan and the first lesson plan before it gives you a single task or step, even if you say "let's start."
- **Plans backward, four weeks at a time,** from what you must be able to do, with a goal for each week and a small project you can show off at the end.
- **Teaches one small lesson a day with the same routine:** a warm-up on earlier lessons, today's goal, the big idea with a worked example and an analogy from your world, practice together, a hands-on task you do yourself, a "teach it back" step with one line you could say in an interview, and a short exit check.
- **Guides instead of telling.** When you're stuck it asks a question, then gives a hint, then shows a similar example, and only shows the answer as a last resort.
- **Holds you to the problem as given.** Requirements are stated up front. A better idea gets praise, but you still solve what was asked, because real work comes with set requirements.
- **Fixes the thinking behind mistakes,** not just the wrong line, and keeps bringing weak spots back until you get them right twice in a row.
- **Counts help honestly.** Something you got right with hints shows what you can do with help. A skill counts as learned when you do a fresh one without help, ideally days later.
- **Keeps study notes for you.** After every lesson it adds the key idea, new terms, an example and mistakes to avoid to your class notes. Ask for "my notes on X" or "a refresher on X" any time.
- **Quizzes and tests you.** A short quiz at the end of each week, a bigger test at the end of each four-week block, and a quiz on any topic whenever you ask. Old topics come back a few days, a week and a few weeks later so they stick.
- **Keeps a record** of your strengths, weak spots, misconceptions and quiz results, and **writes a private report after every class session** so nothing gets lost when a long conversation gets summarized.
- **Follows a weekly rhythm:** lessons on weekdays, a free day, and a planning day where it reviews your week and writes a report for the principal.
- **The principal** (your project chat) oversees the school. Every week it reads all the teachers' reports and sends you a progress report: how you're doing in each class, where you grew, your test scores and its honest take on what to focus on next.
- **Class format, your call.** Pick **in-person classroom** (a live class where your teacher works with you step by step in the conversation, one small piece at a time, waiting for you at each step) or **online class** (each lesson arrives whole and you work through it on your own schedule, the default).
- **Your style, your call.** Pick story mode (it feels like a real school, with teachers in character, quests and a report-card ceremony) or straight to the point (no roleplay, the default). Get test scores right away, or have them announced in your weekly progress report.
- **Light mode** for anyone low on Claude usage. It skips extras and keeps messages short, but always keeps the fact-checking.
- **Made for how you focus.** The counselor asks what helps you focus, and teachers use written steps, short blocks and breaks on request as defaults, and fade the support as you get stronger.
- **Portal (optional).** A visual home page for your school, built as an interactive Claude artifact, with your classes, progress, notes and results in one place. The counselor offers it during setup with a heads-up that it uses noticeably more of your Claude usage, so it's only built if you say yes.

## Install

Pick the one that matches what you use. Each block can be copied and pasted as is.

### Claude Projects, Claude.ai or the Claude app (as skills)

1. Download this repository (green **Code** button, then **Download ZIP**) and unzip it.
2. Make one zip for each of the eleven folders inside `skills/`, so you end up with eleven zips. On Windows, right-click a folder and choose **Send to > Compressed (zipped) folder**. On Mac or Linux, you can paste this in a terminal instead:
   ```
   cd AI-School-Skills-main/skills
   for d in */; do zip -r "${d%/}.zip" "$d"; done
   ```
   (If your unzipped folder has a different name, use that name in the first line.)
3. In Claude, go to **Settings > Capabilities**, find **Skills**, click **Upload skill** and upload each zip. Upload all eleven, because the teacher skill points to the others. (Code execution needs to be turned on.)

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

Codex reads skills from a `.agents/skills` folder. Paste this in a terminal (Mac, Linux, or Git Bash on Windows) to install all eleven skills for every project:

```
git clone https://github.com/Jaesonmoment/AI-School-Skills.git
mkdir -p ~/.agents/skills
cp -r AI-School-Skills/skills/* ~/.agents/skills/
```

To use them in one project only, copy the folders into that project's `.agents/skills/` folder instead. You can also ask Codex's built-in `$skill-installer` to install them from this repository's link.

## Quick start without Projects (Claude Code, Claude app, Codex)

1. Start a conversation and say `Run ai-school-setup and enroll me.` (In Claude Code: `/ai-school:ai-school-setup`.)
2. When it's done, open a new conversation for each class and say `You're my teacher for [class]. Follow the school-teacher skill.` (It points the teacher to the other skills it needs.)

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
This project chat is the school's [principal]. Introduce yourself as the [principal] when I talk to you here.

Teachers follow the school-teacher skill, which points to the other skills. New students start with the ai-school-setup skill.

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

Everything is written in plain English in the `SKILL.md` file inside each folder under [`skills/`](skills/). Change the interview questions, the lesson routine, the weekly schedule or the teaching style to fit how you learn. Each skill ends with a short "For the record" list of the research behind it. Pull requests with improvements are welcome.

## What's in this repo

- `skills/<skill-name>/SKILL.md`: the eleven skills listed in the table above, one folder each.
- `skills/school-teacher/student-template.md`: the "about me" file, if you'd rather fill it in yourself.
- `.claude-plugin/`: the files that let Claude Code install this as a plugin.

Sources: [Claude Code plugins](https://code.claude.com/docs/en/plugins/install), [Skills in Claude](https://support.claude.com/en/articles/12512180-using-skills-in-claude), [Codex skills](https://developers.openai.com/codex/skills). The admissions interview draws on [Learning Styles: Concepts and Evidence](https://digitalcommons.usf.edu/psy_facpub/1765/) (why it doesn't sort you into a "learning style"), [the OARS method from motivational interviewing](https://health.uconn.edu/sbirtacademy/wp-content/uploads/sites/101/2018/03/MI-OARS-Handout.pdf) (open questions, reflecting back, summaries) and [diagnostic assessment](https://www.learningguild.com/articles/designing-it-right-making-an-impact-with-diagnostic-assessments) (checking real level, not just self-ratings).

## License

MIT. Use it, change it, share it.
