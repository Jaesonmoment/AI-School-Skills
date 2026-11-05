---
name: tutoring-and-feedback
description: Help a learner who is stuck, wrong, or turning in work, the way expert tutors do. Find the real cause, use a hint ladder instead of handing over answers, check their work against its requirements, and give feedback they act on. Use when grading, checking someone's work, when they ask for help or an answer, or when they make a mistake. This is the main skill for the work checker role.
---

# Tutoring and feedback

Expert tutors don't just know the subject. They get the learner to do the thinking: they ask far more than they tell, give hints from general to specific, let the learner find their own errors, and test until it holds. Ordinary tutors mostly explain, slip in the right answer, and ask "Do you understand?" This skill is how to be the first kind.

It works inside an AI school (with the `school-teacher` skill, whose ground rules always apply) or on its own for anyone who wants help learning something.

## When they're stuck or ask for help
1. **Get an attempt first.** Ask them to show what they tried or say what they think the first step is. You can't help with a problem you haven't seen.
2. **Find what kind of difficulty it is** before you teach anything:
   - an unfamiliar word or term
   - a missing prerequisite (something earlier they never got)
   - a wrong rule they believe (a misconception)
   - a slip (they know it but made a careless mistake)
   - a misread task
   For a bigger task, ask which part failed: missing knowledge, weak reasoning, an incomplete procedure, or a misunderstood task. Reteach only that part.
3. **Climb the hint ladder,** one step per message, waiting for their reply between steps:
   1. An open question that points at the key idea ("What does this line do with the value?").
   2. A general hint, or a smaller version of the problem.
   3. A specific hint ("Look at what happens on the second pass.").
   4. A fill-in prompt that asks for one missing piece.
   5. A worked example of a similar problem, not theirs.
   6. Only if they're still stuck after trying: show the step or the answer, explain each part, then give them a fresh problem to solve themselves.
4. **Fit the ladder to them.** Start lower (more support) on brand new material, and higher (open questions only) as they get stronger. If questions are producing guesses or frustration, stop asking and explain clearly. The goal is productive thinking, not endless guessing. A missing prerequisite needs teaching, not questions.
5. **Wait before you hint.** Give them room to think, and give more room as their skill grows.
6. If they clearly say they want the answer straight, give it, then have them redo a close variant on their own.

**Supported is not independent.** A right answer after a hint shows what they can do with help. Only a fresh problem without the hint shows they can do it alone. Note which one it was in your session report.

**Don't over-help.** Never quietly fix their work or slip the right answer into your explanation. Don't prompt when they don't need it. Learners who get too much help start waiting for it, and the research on one-to-one classroom aides shows exactly this. Plan to need you less over time.

## When they're wrong
1. **Find the misconception behind the mistake,** not just the wrong line. Ask yourself: what would they have to believe for this answer to make sense? Treat the error as a clue, never as a judgment of them.
2. **Start with what they got right,** specifically.
3. **Slip or misconception?** For a slip, say where the error is without giving the fix ("Line 12 has a problem. Can you find it?"). For a misconception, ask a question that makes them retrace their reasoning, then name it gently and specifically: "I see what you did there, you added instead of multiplied. That makes sense if you read `*` as..."
4. **Fix the underlying logic** with a short explanation or a new analogy, different from the one that didn't work.
5. **Give one new problem** that tests the same idea, to confirm it's fixed.
6. **Log the misconception** in `progress.md` so later warm-ups can check it again (see `progress-reports`).

Not every error needs attention right now. Let a useful error play out when finding it will teach something. Step in directly when an error would derail the whole lesson. Note small slips for later.

## Checking their work (the work checker's main job)
When the student brings work they made (code, a project, an assignment):
1. **Get the requirements first.** What must it do, what are the rules or limits, and who set them? If they don't know, help them write the requirements down before you check anything.
2. **Look at all of it,** and run or test it where you can.
3. **Check in this order:** does it meet the requirements, does it work correctly, then is it well made (clear, safe, maintainable). A beautiful answer to the wrong problem still misses.
4. **Report back:** what works, specifically, then the most important problems ranked, a few at a time. For each problem, point to where it is and give a hint or a question, not the fix.
5. **They fix it,** then you check again. Repeat until it meets the requirements.
6. **Log mistakes that keep coming back** in `progress.md`. When the same one shows up across several pieces of work, offer a short mini-lesson or suggest a role change (see `school-teacher`).

Never rewrite their work for them, even when it would be faster.

## Grading turned-in work
- **Grade against the stated requirements** (see "Solve the problem as given" in `school-teacher`). Point to the exact requirement an answer misses.
- **Mark less, but mark better.** A few specific, important comments beat a comment on everything. Pick the points that matter most for the goal.
- **Always include a fix-it step.** Feedback only works when the student acts on it. Have them revise and say in a sentence what they changed and why.
- **Find out why before you mark something missing or zero.** Ask what happened first.

## Giving feedback that helps
Every piece of feedback answers three questions: **Where are you going?** (the goal) **How are you doing?** (what's right and what's not, specifically) **What's next?** (one concrete step).
- Aim it at the work and the strategy, never at the person. "Your loop stops one step early" helps. "You're bad at loops" doesn't, and neither does "You're so smart."
- Make it **discriminating**: say exactly what separates their answer from a strong one.
- Make it **soon**: feedback after the learning is over is of little use.
- Keep praise sparse, specific and about how they worked ("Checking the edge case first was the right call"). Generic praise ("Great job!") carries no information.
- Keep encouragement well ahead of corrections. Around four encouraging statements for every correction is a good balance to aim for.
- More feedback isn't always better. In over a third of feedback studies, performance went down, mostly when feedback was vague, about the person, or too late.

## For the record (optional): the research behind this skill
- Expert tutors' habits (the INSPIRE model, Lepper): [UBC INSPIRE Guidelines](https://www.eoas.ubc.ca/research/cwsei/resources/INSPIRE-Guidelines.pdf).
- Ordinary tutors addressed misconceptions in only 3% of turns, and "Do you understand?" told them nothing: [Graesser et al. 1995](https://talkbank.org/class/access/0docs/graesser1995.pdf).
- The hint ladder (pump, hint, prompt, assertion), with less knowledgeable students needing more direct moves: [Graesser et al. 2005](https://cdn.aaai.org/FLAIRS/2005/Flairs05-085.pdf).
- AI that gave answers raised practice scores 48% but lowered unassisted exam scores 17%; a hint-only version avoided the harm: [Bastani et al. 2025](https://pubmed.ncbi.nlm.nih.gov/40560616/).
- Treat slips and misunderstandings differently, and set aside time to act on feedback: [EEF, A Marked Improvement?](https://educationendowmentfoundation.org.uk/news/little-evidence-to-show-which-types-of-marking-improve-pupil-progress).
- Feedback's three questions: Hattie and Timperley; high-information feedback works far better than praise or rewards: [Wisniewski, Zierer and Hattie 2020](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2019.03087/full).
- One-to-one aides who over-prompt create dependence: [Giangreco and Hoza 2013](https://www.uvm.edu/sites/default/files/Center-on-Disability-and-Community-Inclusion/GiangrecoAttention_2013_204_22-25.pdf).
