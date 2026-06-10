# Module 4: Your Daily Patterns

**Goal:** Use Claude as a daily co-pilot for planning, project updates, and admin tasks. Leave with a set of daily habits you can use starting tomorrow — and the prompts saved, ready to fold into your own setup in the next module.

---

## Step 1: Welcome to Module 4 (1 min)

Say: "Welcome to Module 4! 🏁"
- "This one is about the daily moves — turning Claude from a one-off tool into a habit you reach for every morning."
- "You'll do 3 quick exercises. Then in the very next module, we'll take everything you've built and make it permanent — your own setup that Claude remembers."
- "Say 'go' when ready."

Check: STOP — wait for student to say "go"

---

## Step 2: Morning priority triage (2 min)

Say: "The first habit: start every morning with a 2-minute priority triage."
- "You have a task list. It's probably overwhelming. Claude can help you cut through it and tell you: what to do first, what to defer, and what to delegate."
- "The prompt:"

```
Here's my task list for today. Help me prioritize:
1. What should I definitely do today? (time-sensitive, high-impact)
2. What can wait until tomorrow or later this week?
3. What could I delegate to someone else?
4. Is there anything I should just drop entirely?

Task list:
[paste your tasks]
```

---

## Step 3: Exercise 1 — Morning priority brief (5 min)

Action: Tell the student to open `modules/4-daily-os/attachments/task-list.md`

Say: "This is a sample weekday-morning task list. Use the prompt above to triage it."
- "Or paste your own actual tasks for today — even better."

Check: STOP — wait for student to share their prioritized list

---

## Step 4: Debrief Exercise 1 (1 min)

When student shares their list:

**Action:** Write the prioritized task list to `my-work/morning-priorities.md`.

**Say:**

"Saved to `my-work/morning-priorities.md`. This is a 2-minute habit you can do every morning."

Say: "Notice how Claude distinguishes between urgent and important? That's the pattern: it doesn't just tell you what's on your list — it helps you think about it."

Say: "Now the most important part — does the order actually match your gut? You know things Claude doesn't. If something's in the wrong bucket, tell Claude why and have it re-sort. For example:"
- "*'Actually, the board deck is urgent — it's due before tomorrow's 9am meeting. Re-sort with that in mind.'*"
- "That back-and-forth is the real skill. Claude gives you a strong first pass; you bring the context only you have. You can do this every morning in under 2 minutes."

Check: STOP — if the student wants to refine, let them go a round with Claude before moving on.

---

## Step 5: Project status updates (2 min)

Say: "Next: project status updates. These take forever to write. Claude can cut it to 5 minutes."
- "The pattern is: dump in the messy state, ask for a clean update."

```
Here's the current state of [project name]:
[bullet points of what's happened, what's in progress, what's blocked]

Please write a project status update for [audience — e.g. leadership, client].
Keep it to 3 short paragraphs:
1. What we accomplished this week
2. What's in progress and any blockers
3. What's happening next week
Tone: [professional / casual / executive-brief]
```

---

## Step 6: Exercise 2 — Draft a project status update (5 min)

Say: "Here's your scenario. Paste this into Claude:"

```
Project: Brightline Ventures Onboarding
Here's the current state:
- Kickoff call happened on March 10 — went well
- The lead consultant (Casey) is working on the 90-day plan
- Waiting on Brightline to share their financial statements (requested March 8, still pending)
- Target delivery for 90-day plan: March 21
- Minor risk: if financials don't arrive by March 14, we may need to push delivery

Write a status update for leadership (Drew and Riley).
Professional but concise. 3 short paragraphs.
```

Check: STOP — wait for student to share the update

**When student shares the update, say:**

**Action:** Write the status update to `my-work/status-update.md`.

**Say:**

"Saved to `my-work/status-update.md`."

Say: "Before you'd ever send something like this, read it once as if you were the person receiving it — here, that's Drew or Riley. Does anything sound overclaimed, or is anything important missing? If so, tell Claude exactly what's off and have it tighten — for example: *'Don't say the plan is on track; the financials are still pending. Make the risk clearer.'* You're the editor; Claude is the drafter."

---

## Step 7: Debrief + delegation (2 min)

Say: "One more skill before we wrap up: delegation."
- "When you delegate work, the quality of your handoff determines the quality of what comes back. Claude can help you write airtight task briefs."

```
Help me write a clear task brief for a team member.

Task: [describe the task]
Person: [their role or name]
Context: [why this matters / what they need to know]
Deadline: [date]
Success looks like: [what done looks like]

Please format this as a short, clear task brief I can send directly.
```

- "Try this with anything you're about to delegate this week."

---

## Step 8: Wrap up (3 min)

**Action:** Append the following to the end of `my-work/prompt-library.md`:

```

## Daily Ops

**Morning triage:**
"Prioritize this task list: today / defer / delegate / drop."

**Status update:**
"[state] -> 3-paragraph update for [audience]."

**Task delegation brief:**
"Help me write a clear task brief: task, person, context, deadline, success criteria."
```

Say: "I just added your daily ops prompts to the library. Let's take a look at everything you've built."

**Action:** Read `my-work/prompt-library.md` and display its full contents to the student.

Say: "That's your prompt library — built up across 3 modules, and it's saved in `my-work/prompt-library.md`. It's yours to keep, customize, and add to."

Say: "Let's recap what you've built so far:"

```
✅ Module 1: Slack thread cleanup + polished email
✅ Module 2: Inbox triage + your first prompt library
✅ Module 3: Meeting brief + clean notes + an SOP
✅ Module 4: Morning priorities + a status update
```

Say: "Everything is in your `my-work` folder — real files you can use, reuse, and build on."

Say: "Here's the thing, though: right now all of this only lives in this one folder, and Claude starts fresh every time you open a new conversation. You still have to re-explain who you are, how you write, what you're working on."

Say: "That's exactly what the next module fixes. Module 5 — **Build Your Operating System** — is the payoff. In about 40 minutes you'll set up your own workspace and a memory file so Claude remembers your role, your voice, and your tools every single time. By the end, you're not just *using* Claude — you're set up to take on real projects with it."

Say: "When you're ready, type: `/start-5-1`"

Say: "Take a break first if you need one. Your progress is always here when you come back."

---

## Teaching Notes

- **Students may share real tasks** in Exercise 1 instead of the sample file — that's great, encourage it.
- **If a student asks about the difference between urgent and important**, briefly explain: urgent = needs to happen today, important = has high impact but may not be time-sensitive. Both matter; the triage helps separate them.
- **If student asks about giving Claude permanent memory of their role and style:** Say "That's exactly what the next module — Module 5, Build Your Operating System — is all about. You'll set that up right here on your computer, so hold that thought and we'll get there."
