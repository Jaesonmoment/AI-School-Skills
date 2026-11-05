---
name: class-planning
description: Plan a class the way strong teachers do. Research the subject first, find the student's real level with a placement check built from that research, then plan backward from what they must be able to do. Use when starting a new class, writing or revising a course plan, planning next week, or preparing a lesson.
---

# Class planning

Real teachers at every level plan the same way: first decide what the learner must be able to do, then decide what will prove it, and only then plan the lessons. And they plan from two kinds of evidence: how the subject is actually built, and what this learner can actually do. This skill walks you through that for a whole class, a week and a single lesson.

It works inside an AI school (with the `school-teacher` skill, whose ground rules always apply) or on its own for anyone planning how to learn something. Outside a school, keep the plan in the conversation or a file the student picks.

## Starting a new class
Don't plan from a handful of questions, and don't judge their level before you know the subject. Work in this order:

1. **Aim first.** One short message with only what you need to aim your research: what they want out of this class (as concrete as possible), the role they want for it (study helper, full teacher or work checker; see `school-teacher`), any outside target (a job posting, a certification, an exam, a project), and what they've already done with the subject. Read `student.md` and `progress.md` first and only ask what's missing. This message aims the research. It doesn't measure their level.
2. **Research the subject before judging their level,** using `subject-research`. Find out how real teachers and respected courses already teach it (their syllabi and lesson plans), plus official docs and current versions, standards or certification outlines if they exist, job postings that match their goal, and the misconceptions beginners usually have. Read and fact-check what you find before relying on it. From that, build a **skill map**: the skills in the subject, in the order they build on each other, from the basics up to their goal. Save it in `research.md` with sources.
3. **Run a placement check built from the skill map.** Measure their real level against the map with real tasks, never with self-ratings:
   - Start at the basics of the map and work up: predict what this does, explain why, spot the mistake, write a few lines. Keep every task answerable right in the chat, with nothing to open, install or build (the first ground rule in `school-teacher`).
   - Go in rounds, one round per message. Where they succeed, jump ahead. Where they miss twice on a skill, stop that branch, because that's where teaching starts.
   - Keep going until you know where they stand on every part of the map that matters for their goal. A complex subject takes more rounds, and that's fine.
   - Tell them it isn't graded. Its only job is to find where to start, so "I don't know" is a useful answer.
   - Record the result for each skill in `progress.md` under "Starting point."
4. **Check for a big category** (see "Big categories" below). If the skill map turns out to be several distinct skills, suggest a split before planning.
5. **Write the plan** for the role (see "By role" below) into `plan.md`.
6. **Write the first lesson plan** into `lessons/` (see "Preparing a lesson"), then check that `plan.md` and the first lesson file both exist. Only then give the student their first real task or step. This is the first ground rule in `school-teacher`, and it holds even if the student says "let's start."
7. **Read it back.** Send a short summary of where they stand, what the plan is and why, and let them correct it before the first lesson.
8. **Write `README.md`**: how this class works and its role, in the same style as the other classes.

**By role:**
- **Full teacher:** every step above, then the full course map below.
- **Study helper:** research and place them on the topic they want to solidify, not the whole subject. Instead of a course map, keep a **focus list** in `plan.md`: the topics to solidify, weakest first, each with what "solid" will look like (for example "explains it without notes and solves a fresh problem").
- **Work checker:** no course map or placement rounds. Research the kind of work they'll bring (its language or tools, usual requirements and common mistakes) with `subject-research`, so your checks are accurate. Judge their level from the first pieces of work and record it in `progress.md`.

**Light mode** (see `school-teacher`): research with two strong sources, run one combined placement round, and keep the plan short.

## The course map (plan.md, full teacher)
Plan backward from the skill map and the placement results, in this order:
1. **Outcomes.** Write 3 to 6 "By the end, you will be able to..." statements with verbs you can observe (build, explain, fix, compare, choose), never "understand" or "know about."
2. **Proof.** For each outcome, decide what would show it, before planning any lessons. Make the proof look like real use: a realistic task built from a blank start without notes, a bug found and fixed, a choice explained the way they'd explain it to an interviewer or a coworker. Recall quizzes check the pieces; real tasks check the outcome.
3. **Prerequisites.** List what has to come first, from the skill map, and use the placement results to see which ones the student already has.
4. **Units.** Group the lessons into units, each with one open "big question" that ties it together and comes back each week.
5. **Return points.** Mark where earlier ideas come back later, so review is planned, not left to chance.
6. **Weeks.** Lay out the current 4 weeks: a goal for each week and a milestone at the end of each week the student can show off, tied to their own projects where possible.

Rules for the map:
- **Pace by mastery, not the calendar.** Label lessons "Unit 2, day 3," not by date, because some ideas take more tries than planned. Leave room in every week for reteaching. When the evidence says they need another example or a missing prerequisite, the evidence wins over the map.
- **Separate the tool from the skill.** If the goal is explaining a concept, don't let an unfamiliar tool or confusing directions get in the way. If using the tool is the goal, teach the tool directly.
- **Map to outside targets.** If the student has one (a certification, a job posting's skill list, an exam), map each unit to it.
- **Mix lesson types.** Tag each planned lesson as learning something new, making sense of it, or using it in a new situation. Make sure "new situation" lessons show up regularly, not only at the end.

## Planning day: the next week
A full teacher does all of this. A study helper does steps 1, 2 and 4 against its focus list. A work checker skips planning and only writes its weekly report.

On the weekly planning day (and whenever a block of weeks ends):
1. Look back first using `progress-reports`. Answer four questions: What was the student supposed to learn? What is the evidence they learned it? What do we do where they didn't? What do we do where they already had it?
2. Research next week's topic.
3. Pick next week's focus: one central topic from the map, adjusted to their weak spots.
4. **Plan the review, not just the new material.** Every week brings back last week's material. Every month brings back last month's. Old weak spots come back until they're right twice in a row (see `practice-and-review`).
5. Open each unit with a short pre-check (what do they already know?) and close it with a post-check against the unit's proof.
6. Rewrite next week in `plan.md`. When the 4 weeks are nearly done, write the next 4.
7. Send the student one short message: what went well, what next week is about, and why.

## Preparing a lesson
Before teaching any lesson, prepare it the way Japanese teachers prepare a research lesson. Write it at the top of the lesson file:
- **Goal and success criteria:** what they'll be able to do by the end, and what that looks like.
- **The key example:** the one worked example that carries the idea.
- **A verified answer:** check your own solution to every exercise before class (run it, test it, or look it up). Teaching a wrong answer does real damage.
- **Likely mistakes:** the misconceptions this topic usually causes, and a planned response to each (a question, a hint, a different example).
- **The acceptance question:** "After this lesson, can they do something useful with this idea and explain the important choices, with less help than before?" If you can't say how you'll know, fix the plan.

Keep the plan short. It's a set of slots to fill, not a script. The lesson itself runs on `lesson-teaching`.

## Research
Research comes before planning, before placement and before teaching any topic you haven't covered yet. `subject-research` has the full method (finding real courses and lesson plans, reading them fully, fact-checking and judging them). At minimum, cover:
- Official docs and current versions, so lessons aren't outdated.
- Common beginner mistakes and misconceptions for the topic.
- Good exercises and free interactive tools.
- How the topic comes up in junior-level interviews and job postings.
- How it fits in the skill map: what it builds on and what builds on it.

Save short notes and links in `research.md` and list sources at the bottom of each lesson.

## Learning from what didn't work
- **Keep a "what worked, what to revise" note** after each lesson, in the lesson file. Read it before you reuse or redo a lesson.
- **Change one thing at a time** in the student's routine, so you can tell what helped.
- **When an approach keeps failing,** study one real exchange: what was the student meant to learn, what did they actually do, where did the explanation or task misfire, what will you try next, and how did the new result compare? Write it in `research.md`.

## Big categories
Some subjects are really a big category with several separate skills inside. Those work better split into their own classes (each with its own teacher and thread) than run as one class, because one teacher can't go deep on every skill and the lessons start to blur together.

**Spotting one.** A subject is a big category when getting good at it means building several distinct skills, each big enough to fill a class, usually with different tools or ways of thinking.

**Example splits** (examples, not templates):
- Making a game on a game platform: one class on designing and planning the game itself, one teaching the programming language, one on building it in the platform's editor, and more departments added as they come up (for example animation).
- Building a web app: design, front end, back end and deployment.
Other categories will split differently, so work out the split from the subject and the student's project, not from these examples.

**Suggesting a split.** When a student picks a subject that looks big enough, or you notice a class has quietly become several, suggest how it could break apart. Offer a couple of different splits, say in a sentence why each department is its own class, and let the student pick one, change it or keep it as one class. Teachers suggest and the student decides. Never open a new class or thread for it until the student says yes. If you are a teacher, take the suggestion to the principal, who puts it to the student.

**One shared project.** The departments of a category share one real project (the game, the app) that every lesson ties back to. Keep one shared file for it, `school/<category>/project.md`, that every department reads before each lesson and updates when it makes a decision or the project changes: what is being built, where it stands, decisions made, what each department is working on next. Use the student's actual project for examples and practice tasks.

**classes.md and the class limit.** In `classes.md`, list a split category as a group, with the category name and one row per department (class, where its conversation lives, folder, status). Each department counts as one class toward the school's active class limit, because each has its own teacher and its own lessons. Departments the student hasn't started yet are listed as Planned and don't count until the student starts them.

**No teaching the same topic twice.** When a category is split, write an "owns / doesn't teach" list for each department in `project.md`. Before teaching a topic that might overlap, check that list and the other departments' `plan.md` files. If another department owns the topic, don't teach it: tell the student which department covers it. If you need a bit of it to move on, explain only that bit inside the lesson. Tell the principal about overlaps, gaps and dependencies (for example "this department needs something the other one doesn't reach until week 3"), and the principal settles who owns it and updates the list. When a new department is added later, with the student's yes, the principal adds it to `classes.md` and to the ownership lists.

## For the record (optional): the research behind this skill
- Backward design (Understanding by Design, Wiggins and McTighe) is the main planning model in US schools and colleges: [Vanderbilt summary](https://cdn.vanderbilt.edu/vu-cft/resources/teaching_resources/theory/design.htm).
- Outcomes with observable verbs and matching assessments ("alignment"): [Carnegie Mellon Eberly Center](https://www.cmu.edu/teaching/assessment/basics/alignment.html).
- "Forward-looking" assessment that copies real use: [Fink, Guide to Designing Courses](https://medicine.wright.edu/sites/medicine.wright.edu/files/page/attachments/Self_Directed_Guide_to_Course_Design.pdf).
- The four questions come from professional learning communities (DuFour and Eaker): [summary](https://academyofsingaporeteachers.moe.edu.sg/professional-excellence/our-plc-journey/ideas-questions-dimensions-for-effective-plcs/).
- Diagnose prior knowledge before teaching, because it can help or get in the way, and don't trust self-reports: [How Learning Works summary](https://fctl.ucf.edu/wp-content/uploads/sites/15/2020/06/Teaching-and-Learning-Principles.pdf).
- Rigid pacing guides crowd out reteaching: [ASCD, What Research Says About Pacing Guides](https://ascd.org/el/articles/pacing-guides).
- Japanese lesson study plans the expected answers and mistakes in advance: [NCTM, Lewis and Perry 2017](https://nctm.org/Publications/Journal-for-Research-in-Mathematics-Education/2017/Vol48/Issue3/Lesson-Study-to-Scale-Up-Research-Based-Knowledge_-A-Randomized,--Controlled-Trial-of-Fractions-Learning).
- A structured AI tutor that worked used pre-written, verified solutions: [Kestin et al. 2025](https://pmc.ncbi.nlm.nih.gov/articles/PMC12179260/).
