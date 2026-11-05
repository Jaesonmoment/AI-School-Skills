---
name: class-planning
description: Plan a class the way strong teachers do, working backward from what the student must be able to do. Use when starting a new class, writing or revising a course plan, planning next week, or preparing a lesson before teaching it.
---

# Class planning

Real teachers at every level plan the same way: first decide what the learner must be able to do, then decide what will prove it, and only then plan the lessons. This skill walks you through that for a whole class, a week and a single lesson.

It works inside an AI school (with the `school-teacher` skill, whose ground rules always apply) or on its own for anyone planning how to learn something. Outside a school, keep the plan in the conversation or a file the student picks.

## Starting a new class
1. **Get to know where they start.** Before teaching anything, send 5 targeted questions in one message: what they already know, what they have built with it, their goal for this subject, how they like to learn, and one small "show me" question they can answer in a few lines, with nothing to open or build, that reveals their real level. If `progress.md` already has a starting point from the admissions interview, read it first and only ask what is still missing. Don't trust self-ratings alone; the "show me" answer is the real evidence.
2. **Check if it's a big category** (see "Big categories" below). If it is, suggest a split before planning.
3. **Research the subject** (see "Research").
4. **Write the course map** in `plan.md` (see below).
5. **Write `README.md`**: how this class works, in the same style as the other classes.
6. **Write the first lesson plan** into `lessons/` (see "Preparing a lesson"), then check that `plan.md` and the first lesson file both exist. Only then give the student their first task or step. This is the first ground rule in `school-teacher`, and it holds even if the student says "let's start."

## The course map (plan.md)
Plan backward, in this order:
1. **Outcomes.** Write 3 to 6 "By the end, you will be able to..." statements with verbs you can observe (build, explain, fix, compare, choose), never "understand" or "know about."
2. **Proof.** For each outcome, decide what would show it, before planning any lessons. Make the proof look like real use: a realistic task built from a blank start without notes, a bug found and fixed, a choice explained the way they'd explain it to an interviewer or a coworker. Recall quizzes check the pieces; real tasks check the outcome.
3. **Prerequisites.** List what has to come first, and check the student has it.
4. **Units.** Group the lessons into units, each with one open "big question" that ties it together and comes back each week.
5. **Return points.** Mark where earlier ideas come back later, so review is planned, not left to chance.
6. **Weeks.** Lay out the current 4 weeks: a goal for each week and a milestone at the end of each week the student can show off, tied to their own projects where possible.

Rules for the map:
- **Pace by mastery, not the calendar.** Label lessons "Unit 2, day 3," not by date, because some ideas take more tries than planned. Leave room in every week for reteaching. When the evidence says they need another example or a missing prerequisite, the evidence wins over the map.
- **Separate the tool from the skill.** If the goal is explaining a concept, don't let an unfamiliar tool or confusing directions get in the way. If using the tool is the goal, teach the tool directly.
- **Map to outside targets.** If the student has one (a certification, a job posting's skill list, an exam), map each unit to it.
- **Mix lesson types.** Tag each planned lesson as learning something new, making sense of it, or using it in a new situation. Make sure "new situation" lessons show up regularly, not only at the end.

## Planning day: the next week
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
Before planning a week, and before teaching any topic you haven't covered yet, research it:
- Official docs and current versions, so lessons aren't outdated.
- Common beginner mistakes and misconceptions for the topic.
- Good exercises and free interactive tools.
- How the topic comes up in junior-level interviews and job postings.

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
- Rigid pacing guides crowd out reteaching: [ASCD, What Research Says About Pacing Guides](https://ascd.org/el/articles/pacing-guides).
- Japanese lesson study plans the expected answers and mistakes in advance: [NCTM, Lewis and Perry 2017](https://nctm.org/Publications/Journal-for-Research-in-Mathematics-Education/2017/Vol48/Issue3/Lesson-Study-to-Scale-Up-Research-Based-Knowledge_-A-Randomized,--Controlled-Trial-of-Fractions-Learning).
- A structured AI tutor that worked used pre-written, verified solutions: [Kestin et al. 2025](https://pmc.ncbi.nlm.nih.gov/articles/PMC12179260/).
