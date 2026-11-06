---
name: subject-research
description: Research a subject the way a careful teacher does. Find how real teachers and courses already teach it, pull their lesson plans and materials, read them in full, fact-check every claim and example, and keep only what holds up. Use before planning or placing a student, before teaching a new topic, and before using any outside material, in any subject (math, science, code, life skills and more).
---

# Subject research

Good teachers don't invent a subject from memory, and they don't paste in the first lesson plan they find. They look at how experienced teachers and respected courses already teach it, read those materials closely, check that they're right, and build from what holds up. This skill is how to do that, and how to prove the material is sound before the student ever sees it.

It works inside an AI school (with the `school-teacher` skill, whose ground rules always apply) or on its own for anyone researching how to learn or teach something. If a skill named here isn't installed, do that part yourself as well as this file allows, and tell the student once which skill to add.

## When to use it
- **Starting a class:** to build the skill map before the placement check (see `class-planning`).
- **Before teaching a topic you haven't covered yet.**
- **Before using any outside material:** a lesson plan, worksheet, tutorial, video, example or exercise.
- **When the student asks something factual you're not sure of.**
- **Before checking work in an unfamiliar area** (for a work checker).

## 1. Find how it's already taught
Look for several independent sources, not one:
- **Respected courses:** syllabi and lesson plans from universities (many publish open course materials), established online courses, and experienced teachers who share their plans.
- **Official outlines:** standards, curricula, certification or exam outlines for the subject, if they exist.
- **Official references:** the official docs and current versions for tools and languages; established textbooks and their tables of contents.
- **Real use:** job postings or real tasks that match the student's goal, to see what actually matters.
- **Known trouble spots:** the misconceptions and mistakes beginners usually have with each topic.

Compare them. Where respected courses agree on what to teach and in what order, that's a strong signal. Where they differ, note why.

## 2. Read it fully and check it
Never use material after a skim. For every piece you plan to use:
- **Read the whole thing,** start to finish, not just the headings or the summary.
- **Do every example and exercise yourself.** Run the code. Redo the math. Follow each step of reasoning and make sure each step actually follows from the last.
- **Check every factual claim** against an authoritative source (see the table below). One authoritative source is the minimum; two independent ones for anything important or surprising.
- **Check the date and version.** Old material can be wrong now even if it was right once (changed APIs, updated guidelines, new research).
- **Check who made it and why.** What are their credentials or track record? Are they selling something? Do they cite sources?

| Subject | How to check it |
|---|---|
| Code | Run it on a current version. Check it against the official docs. Test edge cases, not just the happy path. Watch for outdated or insecure patterns. |
| Math | Re-derive or re-solve it yourself. Check the result another way (plug the answer back in, estimate, try a special case). Check definitions against a standard textbook. |
| Science | Check against established textbooks, review articles or major scientific bodies. Separate settled science from open questions, and say which is which. |
| History, language, other facts | Check against primary sources or established references. Watch for myths that get repeated everywhere. |
| Life skills (money, health, careers, relationships) | Check against government agencies, professional bodies or peer-reviewed research. Separate evidence from opinion. Flag anything that depends on location, law or personal circumstances, and point to a qualified professional where real advice is needed. |
| Teaching methods | Check against research reviews (see the other skills' "For the record" sections). Popular isn't the same as proven. |

## 3. Judge the material
Score each piece before using it:
- **Accurate:** every claim and example checked and correct?
- **Current:** right version and up to date?
- **Fits the goal:** matches the skill map and the student's level?
- **Teaches well:** clear explanation, worked examples, practice, a way to check understanding?
- **Trustworthy source:** credible author, cites sources, no hidden agenda?

Use it as is, use it with fixes (note what you fixed and why), or reject it (note why). Never pass along material you haven't checked.

## 4. Build from what holds up
- **Synthesize, don't copy.** Combine the best parts of several sources into your own skill map, lesson plans and exercises, in your own words, fitted to this student.
- **Respect the original.** Link to and credit the sources you drew from. Don't copy whole lesson plans word for word unless the license allows it (openly licensed material can usually be adapted with credit).
- **Write down disagreements.** Where good sources disagree, say how you decided.

## 5. Keep a record
In `research.md` for the class:
- the skill map, with sources
- each source with its verdict: used, used with fixes (what and why), or rejected (why)
- facts you checked and where you checked them
- open questions you couldn't settle
List the sources at the bottom of each lesson.

## Honesty rules
- **If you couldn't verify it, say so.** Never present an unchecked claim as fact. Mark it as uncertain, or leave it out.
- **"Checked" means you verified it against authoritative sources.** Only call something "certified" if an actual certifying body certified it.
- **When you find an error in material you already taught,** tell the student, correct it, and fix the notes.

## For the record (optional): the research behind this skill
- A structured AI tutor that worked used pre-written, expert-checked solutions, because language models make errors otherwise: [Kestin et al. 2025](https://pmc.ncbi.nlm.nih.gov/articles/PMC12179260/); language models can lose track of math content: [Education Next, von Hippel 2024](https://www.educationnext.org/two-sigma-tutoring-separating-science-fiction-from-science-fact/).
- Teachers increasingly study and adapt existing, high-quality lessons rather than writing everything from scratch: [RAND, American Instructional Resources Survey](https://www.rand.org/content/dam/rand/pubs/research_reports/RRA100/RRA134-30/RAND_RRA134-30.pdf).
- Japanese lesson study plans from existing research materials and anticipates student answers and mistakes: [NCTM, Lewis and Perry 2017](https://nctm.org/Publications/Journal-for-Research-in-Mathematics-Education/2017/Vol48/Issue3/Lesson-Study-to-Scale-Up-Research-Based-Knowledge_-A-Randomized,--Controlled-Trial-of-Fractions-Learning).
- Plenty of widely repeated teaching ideas (learning styles, the "learning pyramid") have no solid research behind them, which is why popular isn't proof: [Pashler et al. 2008](https://pubmed.ncbi.nlm.nih.gov/26162104/).
