---
name: practice-and-review
description: Make learning stick with the practice methods that have the strongest research behind them, recall from memory, spaced review and mixed practice, plus quizzes, tests, mastery checks, notes and refreshers. Use for warm-ups, homework, drills, review days, quizzes and tests, or when the student asks to be quizzed or refreshed.
---

# Practice and review

Most of what the student learns will fade unless they keep pulling it back out of memory, spread out over days and weeks. The methods with the strongest evidence in all of learning science are about exactly that, and they work the same for a child or an adult, in a classroom or one-on-one. This skill is how to use them.

It works inside an AI school (with the `school-teacher` skill, whose ground rules always apply) or on its own for anyone who wants to practice or be quizzed. It is the main skill for the study helper role, working through the focus list in `plan.md`, and full teachers use it every lesson.

**Light mode** (see `school-teacher`): keep the warm-ups and spaced review, which cost little and matter most. Use shorter quizzes and skip the block test's extras.

## Repetition that actually works
"Learning by repetition" works when the repetition means **pulling the idea back out of memory, again and again, with gaps in between**. Rereading notes or hearing the same explanation again feels like learning but does little. So:
- **Recall before you remind.** Ask first, closed-book, then check. Never show the answer before they try.
- **Space it out.** Bring each idea back a few days later, about a week later and a few weeks later. A gap that's too long costs little; one that's too short costs a lot. Adjust: shorten the gap after a miss, lengthen it after a confident success.
- **Vary the form each time.** Recall it, use it in a familiar task, fix a broken example, apply it in a new situation, explain why it works. Change the surface details too (different data, names, wording) so the skill isn't tied to one example.
- **Mix it up once they can start each type alone.** When they've learned two or three related kinds of problem, mix them in one practice set so they have to choose the method, not just repeat it. Mixing helps most when the types are easy to confuse.
- **Keep practice at about 80% success.** Much lower and they're guessing, so drop back to a worked example. Much higher and they're coasting, so raise the difficulty or lengthen the gaps. Struggle only helps when they can win it.

## Warm-ups
Every session opens with a short recap and 2 or 3 recall questions (multiple choice, short answer, predict the output, find the bug), in every role and without the student asking (see "Opening a session" in `lesson-teaching`). Pick the questions from:
- `notes.md` and your latest session reports
- several earlier lessons, not only the last one
- open misconceptions in `progress.md`
- whatever is due on the spacing schedule
Don't show the answers. When they reply, grade them and explain the reasoning behind each correct answer. Bring old weak spots back in warm-ups until they get them right twice in a row.

## Hands-on practice for step-by-step skills
For skills built from steps (code, math, procedures, tools), climb this ladder over several lessons:
1. Study a worked example, with the reasoning said out loud.
2. Put scrambled steps or lines in the right order (a "Parsons problem").
3. Find and fix the bug in broken work.
4. Build it from scratch.
5. Build it from scratch again, days later, without looking.
6. Explain it out loud (see `explain-it-out-loud`).

Practice in both directions: read work and predict what it does, and write work that makes something happen. When their work can be checked automatically (tests, a checker, a known output), give that instant feedback, and have them write their own tests or checks first.

For foundations that need to become automatic, a short timed recall drill with a personal "meet or beat your last score" chart works well. Teach the strategy first, then time it.

## Is it learned yet?
- **Mastery loop:** teach, check, correct with a different explanation, then recheck with a fresh but similar problem (not the same one), then move on or stretch.
- **Track each skill on a ladder of independence:**
  1. Introduced
  2. Done with help
  3. Done alone on a fresh task
  4. Still done alone later, after other learning
  5. Used in a new situation
  Only steps 4 and 5 count as learned. Tools the student genuinely needs for access can stay during independent checks; independence means doing the thinking, not giving up a support.
- **Keep the most recent evidence** for each skill, not an average. Old misses shouldn't hide new mastery, and old wins shouldn't hide new gaps.
- **Ask for a confidence rating** (1 to 5) before a check, then compare it with the result. It teaches them to judge their own learning, which most people overestimate.

## Quizzes and tests
- **Weekly quiz:** on the last lesson day of the week, replace the warm-up with a short quiz (5 to 8 questions) on that week's topics plus one or two old weak spots. Mix formats: multiple choice, predict the output, find the bug, explain it in one sentence.
- **Block test:** at the end of each block of weeks in the plan, give a longer test on the whole block, with at least one hands-on task done from scratch and one "explain it out loud" question.
- **On request:** give a quiz or test on any topic whenever they ask.
- **Test results:** follow the student's choice in `student.md`. If they want results right away, give them when you grade. If they'd rather wait, save the score and your breakdown in `quizzes/` and in the weekly report, and let the principal announce it in the weekly progress report. If they ask for a result early, tell them.
- Save each quiz and test in `quizzes/` with the results. Don't show answers until they reply. Grade with the reasoning behind each answer, handle misses with `tutoring-and-feedback`, and log scores and misses in `progress.md`.
- Keep quizzes low-stakes. Their job is practice and information, not judgment.

## Notes and refreshers
Keep `notes.md` in the class folder: the student's study notes, written so they can review without rereading every lesson.
- After each lesson, add a short entry: the big idea in a sentence or two, new terms with plain-English meanings, one small example, mistakes to avoid, and the interview line.
- Also add things they learn outside lessons that belong to this class (for example something that came up in another conversation, passed along by the student or the principal). Note where it came from.
- When they ask for notes on a topic, give them the matching part of `notes.md`, cleaned up.
- The refresher at the start of every session is built from here: a recap from `notes.md` and the latest session report, then the warm-up. The student never has to ask for it.
- When they ask for a refresher at any other time, ask 2 or 3 recall questions first, then give a short recap from `notes.md` aimed at what they missed. Recall first, recap second.

## For the record (optional): the research behind this skill
- Practice testing and spaced practice were the only "high utility" techniques in a major review; rereading and highlighting rated low: [Dunlosky et al. 2013](https://journals.sagepub.com/doi/10.1177/1529100612453266).
- Quizzing with feedback rated Strong, spacing Moderate, in the federal practice guide: [IES, Organizing Instruction and Study](https://ies.ed.gov/ncee/WWC/Docs/PracticeGuide/20072004.pdf).
- Mixed practice scored 72% vs 38% two weeks later in a classroom trial: [WWC review of Rohrer et al.](https://ies.ed.gov/ncee/WWC/Study/80702); when mixing helps and when it doesn't: [Brunmair and Richter 2019](https://pubmed.ncbi.nlm.nih.gov/31556629/).
- "Desirable difficulties": practice that feels harder often lasts longer, if the learner can succeed: [Bjork and Bjork 2011](https://bjorklab.psych.ucla.edu/wp-content/uploads/sites/13/2016/04/EBjork_RBjork_2011.pdf).
- Parsons problems gave the same learning as writing code, in less time: [Ericson, Georgia Tech](https://hg.gatech.edu/node/603172).
- Mastery learning (check, correct, recheck): [Kulik et al. 1990](https://www.academia.edu/81783373/Effectiveness_of_Mastery_Learning_Programs_A_Meta_Analysis); with caveats: [EEF Toolkit](https://educationendowmentfoundation.org.uk/education-evidence/teaching-learning-toolkit/mastery-learning).
- The 80% success target: [Rosenshine, Principles of Instruction](https://www.aft.org/sites/default/files/periodicals/Rosenshine.pdf).
