---
name: progress-reports
description: Keep an honest record of what a learner can really do, and write session reports, weekly reports and handoff notes built on evidence, not impressions. Use after every session, on planning day, when a concern needs raising, or when a learner moves to another teacher or class.
---

# Progress reports

A good record answers one question: what can the student do now, without help, and how do we know? Schools that track this well use evidence (real work the student produced), note how much help was given, and turn the record into decisions. Teachers hate reports that only repeat data someone can already read, so every report here adds judgment and a next step.

It works inside an AI school (with the `school-teacher` skill, whose ground rules always apply) or on its own for anyone tracking their own learning. If a skill named here isn't installed, do that part yourself as well as this file allows, and tell the student once which skill to add.

## The student's record (progress.md)
Keep these sections:
- **Starting point:** the placement check result for each skill on the skill map (see `class-planning`), or for a work checker, their level from the first pieces of work.
- **Skills:** one line per skill with its step on the ladder of independence (introduced, done with help, done alone on a fresh task, still done alone later, used in a new situation; see `practice-and-review`), the most recent evidence and its date. Update it with the newest evidence instead of averaging.
- **Finished lessons:** date, topic, turned in or not, exit check result, notes.
- **Strengths:** specific ("traces loops correctly on paper"), not vague ("good at loops").
- **Weaknesses and open misconceptions:** synthesize, don't just list. Name the pattern and its likely cause (for example "mixes up = and === because they read both as 'equals'").
- **Fixed misconceptions:** with the date fixed and the evidence that showed it.
- **What helps:** supports and approaches that worked for this student, and ones that didn't (see `learner-support`).
- **Recurring mistakes** (work checker): mistakes that keep showing up across pieces of work, with dates and examples.

A full teacher keeps every section. A study helper keeps them for the topics on its focus list. A work checker keeps the starting point, recurring mistakes, strengths and fixed misconceptions.

**Light mode** (see `school-teacher`): keep `progress.md` current, keep session reports to four lines (what happened, the evidence, help given, next time), and keep the weekly report to a few lines.

## Session reports
A class session is one sitting where the student works with you: a lesson, an assignment, a quiz or a long back-and-forth. When a session ends (they finish the work, sign off or stop replying for the day), write a private report to `sessions/<YYYY-MM-DD>_<n>.md` so nothing is lost when the conversation gets long or older messages get summarized.

Include:
- **What happened:** the topic, what they turned in and the result (grade, check, star, quiz score).
- **Evidence:** the specific answers, mistakes and questions that show what they understand, quoted or described exactly.
- **Help given:** which hints, examples or answers you supplied, and whether the exit check was done alone. This keeps a polished answer made with lots of help from being mistaken for learning.
- **Analysis:** what clicked, what didn't and why (the misconception behind each miss), how engaged they were and anything that helped or got in the way.
- **Their view:** anything they said was useful, confusing or frustrating.
- **What changed:** progress since the last session, and any misconception that is now fixed.
- **Next time:** what to review, reteach or push on.
- **Recap for next time:** the few lines you will open the next session with (where you stopped, the rule of the day, what to check first).

Don't send the report to the student or mention it unless they ask to see it. Before each session, read your latest session reports and open with the recap from them (see "Opening a session" in `lesson-teaching`). Use them to keep `progress.md` current and to write the weekly report.

## Weekly report
Every role writes one. A study helper or work checker keeps it short: what the student brought, what got solid or fixed, what keeps coming back, and what's next.

On planning day, write `school/reports/<YYYY-MM-DD>_<class>.md` from the week's session reports. Organize it around four questions:
1. **What was the student supposed to learn this week?** The goals from `plan.md`.
2. **What's the evidence they learned it?** For each goal: the task or explanation they produced, how much help it took, and what that evidence actually supports (done with help, done alone, held up later).
3. **Where they didn't, what are we doing about it?** The recurring difficulty described specifically, its likely cause, and the next teaching decision.
4. **Where they already had it, how are we stretching them?**

Then add:
- Each session in a line.
- Test scores with your breakdown (or "held for the weekly progress report" if the student chose to wait).
- One specific strength and one specific next step.
- The student's own feedback on the week.
- Anything that affects another class (for example "this class needs a topic next week that another class doesn't cover until week 3").

Report what they can do against the goals, not just scores or how many lessons got done. Add interpretation and decisions; don't restate logs the principal can already read.

If the school has a principal, send it the report in a few lines with the file path.

## Raising a concern
Use a ladder so concerns get handled early and in proportion:
1. **Normal.** Progress shows up in the weekly report as usual.
2. **Watch.** When the student misses a goal two weeks running, or skips several sessions: write a measurable goal with a starting point and a target (for example "from 2 of 5 to 4 of 5 correct on fresh loop problems"), check it every few sessions, and try a different approach (see `learner-support` and "Learning from what didn't work" in `class-planning`).
3. **Team up.** If there's still no improvement after a few weeks of trying: flag it to the principal with the evidence, what you've tried and what you think is going on, so you can agree on who does what, by when, and how you'll know it's working. If there's no principal, raise it with the student directly.

## Handoff notes
When the student moves to another teacher or class (a split category, a paused class picked back up, a new teacher), write a handoff note in the class folder:
- current level and growth, with evidence
- approaches that worked and didn't
- their preferences and routines
- open concerns and goals
Keep what you observed separate from your impressions. The next teacher reads it before their first lesson.

## For the record (optional): the research behind this skill
- The four questions come from professional learning communities (DuFour and Eaker): [summary](https://academyofsingaporeteachers.moe.edu.sg/professional-excellence/our-plc-journey/ideas-questions-dimensions-for-effective-plcs/).
- Teachers object to compiling data reports leaders can already read: [EdWeek 2024](https://www.edweek.org/the-state-of-teaching/2024/teaching-learning/dear-administrators-teachers-want-you-to-get-these-8-tasks-off-their-plates/).
- The concern ladder is modeled on MTSS (tiers of support with measurable goals and scheduled progress checks): [Alabama MTSS manual 2025](https://www.alabamaachieves.org/wp-content/uploads/2025/10/MTSS_20251021_PST-Manual_V1.0.pdf).
- IEP goals use a baseline, a measurable target and a set way of checking progress: [Parent Center Hub](https://www.parentcenterhub.org/iep-progress/).
- Year-end "articulation" handoffs between teachers: [Otus (vendor source)](https://otus.com/blog/transferring-knowledge-at-the-end-of-the-school-year-how-to-facilitate-impactful-articulation-meetings).
- Most parents think their child is on track when about half aren't, so report mastery, not just grades: [Learning Heroes 2023](https://bealearninghero.org/wp-content/uploads/2023/04/Parents-2023-Go-Beyond-Grades.pdf).
- Polished work done with AI help hid weak independent skill: [Bastani et al. 2025](https://pubmed.ncbi.nlm.nih.gov/40560616/).
