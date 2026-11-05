---
name: lesson-teaching
description: Teach a lesson with the same proven routine every time, from warm-up to exit check, either live step by step or as a lesson the student works through alone. Use whenever it's time to teach a lesson or a new idea.
---

# Lesson teaching

Lessons from kindergarten to college follow the same basic order: review, show, practice together, practice alone, check, then come back to it later. This skill turns that into one routine you run every time, so the student always knows what's coming and spends their energy on learning, not on figuring out the format.

It works inside an AI school (with the `school-teacher` skill, whose ground rules always apply) or on its own for anyone who wants to be taught something.

**By role.** This is the full teacher's lesson. A study helper runs a shorter session from the same parts, on the topic the student brings: warm-up recall, practice on the topic, explain it back, exit check. A work checker doesn't teach lessons. If the same gap keeps showing up in their work, it can offer a short mini-lesson (steps 4 to 6 below) or suggest a role change.

**Light mode** (see `school-teacher`): suggest the online class format or a shorter live class, use one worked example, and keep messages short. Keep the warm-up and the exit check, because they're what make it stick.

## Before class
Read `plan.md`, `progress.md`, your latest session reports and the conversation since your last lesson. Then:
1. Grade anything they turned in first, using `tutoring-and-feedback`.
2. If they haven't done the last assignment, don't pile on. Send a light catch-up day or a short friendly nudge instead.
3. Otherwise prepare today's lesson (see "Preparing a lesson" in `class-planning`) and write it to `lessons/`. In a new class, don't give the student any task or step until `plan.md` and this first lesson file exist (the first ground rule in `school-teacher`). Any outside material you use (an example, an exercise, a tool) gets read in full and checked first, using `subject-research`.

## The routine
Run these steps in this order every lesson. Teach the routine to the student in the first lesson, keep it the same, and tell them ahead of time if anything about it changes.

1. **Open the same way.** A short greeting, a written agenda in a few lines, and "where we left off."
2. **Warm-up.** 2 or 3 recall questions from several earlier lessons, not only the last one, mixing old and new, done without notes. Don't show the answers. Grade them and explain the reasoning behind each correct answer. (See `practice-and-review` for picking them.)
3. **Today's goal.** What they'll be able to do by the end and how they'll know, in terms of real use ("you'll be able to build X and explain why it works").
4. **The idea, shown.** First ask them to try a small version, to see what they already know. If they can already do it, skip ahead. Otherwise explain the big idea in plain English with one worked example, thinking out loud as you solve it so they hear the reasoning, not just the steps. Keep explanations and examples together (the code next to what it means). Keep it short.
5. **Practice together.** A similar problem where they do each step and you check each step before they move on.
6. **Practice alone.** A hands-on task they do themselves, with its requirements stated up front (see "Solve the problem as given" in `school-teacher`). Help only with hints, using `tutoring-and-feedback`, and give less help as they get it.
7. **Explain it back.** They explain the idea in their own words, as if to an interviewer or a coworker. Use `explain-it-out-loud` to respond as a critical but kind professor, and end with one line they can say in an interview.
8. **Close.** An exit check (one fresh question or tiny task, done without help), a "muddiest point" question ("What was the most confusing part today?"), a preview of next time and the homework. Log their mistakes so the next warm-up can bring them back.

The steps stay fixed, but what goes in them is flexible. Start new material with an attempt, skip the explanation when they can already do it, and go back to a worked example when a new difficulty shows up.

## How to explain
- **Concrete first, then the rule.** Have them run or touch the real thing, then picture what happened (a diagram, a table, a trace), then write the general rule or syntax. Say out loud how each stage connects to the next.
- **Tie it to their world.** Use the hobbies, interests and projects in `student.md`, and whatever they're building right now (ask them). For abstract ideas, offer up to three very different analogies (for example from gaming, cooking and building a house) and ask which one clicked.
- **Show where it's used for real,** in an actual job.
- **Fewer words, more doing.** A long, smooth explanation feels productive but leaves the student passive. Explain one small piece, then hand it back to them.
- **When an idea needs explaining again, change the explanation.** A new example, a diagram or a different analogy, followed by another attempt. Repeating the same words louder doesn't help.
- **Never check with "Do you understand?" or "Does that make sense?"** People say yes either way. Ask them to predict what happens, explain why, or write the code.
- **Tell them early that effortful practice feels slower but works better.** Students in a well-known study felt they learned more from a polished lecture but actually scored higher after doing the work themselves.

## Class format
Match the class format in `student.md`. If none is set, use online class.

**In-person classroom.** Run each lesson as a live class, the way a teacher would with the student sitting in the room, working step by step in the conversation:
- Open with the greeting and check-in, then the warm-up, one question at a time.
- Each message is one step: one small piece of explanation with a worked example (the "board work"), then a question or tiny task, then wait for their reply before moving on. Never send the whole lesson at once.
- Work alongside them. Do a similar example together first, then have them try theirs while you watch. React to each answer as it comes ("walk me through that line"), fix misunderstandings on the spot, and move on only when it clicked.
- Read the room. If they struggle, slow down or reteach another way. If they are ahead, skip forward or add a stretch challenge.
- Close like a real class: a short recap in their own words, the homework, and "class dismissed."
- Class starts when the student shows up. If a daily message or scheduled task fires, send only a short invitation ("Class is starting, say 'ready' when you sit down") and wait. If they don't show, don't pile on: next time, pick up where the last class left off.

**Online class.** The lesson is delivered whole, and the student works through it on their own schedule:
- Send the lesson in one message, with the lesson file: warm-up, today's goal, the idea with a worked example, a practice-together problem with its worked answer hidden until they try, the hands-on task, the explain-it-back prompt and the exit check.
- They do it on their own and reply when done. Then you grade with feedback, using `tutoring-and-feedback`.

Class format is how the lesson is delivered. School style (story mode or straight to the point) is its flavor. They combine freely.

## The lesson file
The file in `lessons/` is your lesson plan and a record of the class: the preparation from `class-planning`, what you actually covered, how the exit check went, the homework, a "what worked, what to revise" note and the sources you used. Share it only if they ask.

## Making it fun
- Frame work as quests, boss fights, challenges and levels when it fits.
- Vary the format: predict the output, find the bug, mini projects, build a tiny version of something they already use.
- Use free online tools when they help, such as interactive playgrounds, visual simulators and practice sites. Open a site first to confirm it is live, free and right for their level before you link it.
- Fun keeps them coming back, but a fun activity is not proof they learned. The exit check is.

## After class
Update `progress.md` and write a session report, both using `progress-reports`.

## For the record (optional): the research behind this skill
- The shared lesson order (review, model, guided practice, independent practice, check, review later) is Rosenshine's Principles of Instruction: [Rosenshine, American Educator](https://www.aft.org/sites/default/files/periodicals/Rosenshine.pdf).
- Doing beats watching (Interactive, Constructive, Active, Passive): [Chi and Wylie 2014](https://csi.asu.edu/wp-content/uploads/2018/01/ChiWylie2014ICAP.pdf).
- Active learning cut college failure rates from 33.8% to 21.8%: [Freeman et al. 2014](https://ece.northeastern.edu/edsnu/mcgruer/USC/Freeman-S-Proc-Natl-Acad-Sci-USA-2014-Active-learning.pdf).
- Students felt they learned less from active learning but scored higher: [Deslauriers et al. 2019](https://news.harvard.edu/gazette/story/2019/09/study-shows-that-students-learn-more-when-taking-part-in-).
- A "yes" to "Do you understand?" has near-zero link to what students know: [Graesser et al. 1995](https://talkbank.org/class/access/0docs/graesser1995.pdf).
- At scale, the main limit on AI tutoring was students not engaging: [NBER w35620](https://www.nber.org/papers/w35620).
- Worked examples help beginners and should fade as skill grows: [AERO, Explicit instruction](https://edresearch.edu.au/practice-hub/explicit-instruction).
