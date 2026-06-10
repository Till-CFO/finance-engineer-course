# Module 3: Meeting Machine

**Goal:** Walk into every meeting prepared. Walk out with a clean action list. Leave with template prompts for recurring meeting types.

---

## Step 1: Welcome to Module 3 (1 min)

Say: "Welcome to Module 3 — the Meeting Machine! 📅"

- "If you spend a lot of time in meetings, this module will save you hours every week."
- "Three things: pre-meeting prep, post-meeting cleanup, and turning notes into SOPs."
- "Say 'let's go' when you're ready."

Check: STOP — wait for student to say they're ready (any variation of "ready", "let's go", "go", etc.)

---

## Step 2: Pre-meeting briefs (2 min)

Say: "A pre-meeting brief is a one-page cheat sheet: who you're meeting, what the context is, what you want to get out of it, and what questions to ask."

- "Claude can build one from almost nothing — even just a calendar invite."
- "Here's the basic prompt pattern:"

```
Help me prepare for a meeting. Here's the context:
- Meeting name: [X]
- Attendees: [list]
- Goal of this meeting: [what you're trying to accomplish]
- Any background: [paste any relevant context]

Give me:
1. A one-paragraph context summary
2. My top 3 goals for this meeting
3. 3 questions I should be ready to answer or ask
4. Any risks or things to watch for
```

Check: STOP — wait for student to say they understand or are ready to try it

---

## Step 3: Exercise 1 — Build a pre-meeting brief (5 min)

Action: The calendar invite is in `modules/3-meeting-machine/attachments/calendar-invite.md`

Say: "There's a calendar invite for a Quarterly Business Review with Brightline Ventures — it doesn't have much in it, which is exactly the point. Easiest way to do this: type in the message box:"

```
Read the file modules/3-meeting-machine/attachments/calendar-invite.md
and build a pre-meeting brief for this meeting using the pattern above.
```

Check: STOP — wait for student to share their brief

---

## Step 4: Debrief Exercise 1 (1 min)

When student shares their brief, say:

**Action:** Write the pre-meeting brief to `my-work/meeting-brief.md`.

**Say:**

"Saved to `my-work/meeting-brief.md`. This is the kind of thing you can generate before any meeting in seconds — and now you're not walking in blind."

Say: "But here's the most important habit, especially for anything client-facing: notice that Claude *filled in gaps the invite didn't actually contain*. It made reasonable assumptions — but assumptions aren't facts. Read the brief and ask yourself: which parts did Claude actually know from the invite, and which did it guess?"

- "Where it guessed something you know is wrong, correct it: *'Actually, this isn't a renewal — it's our first QBR with them. Redo the brief with that in mind.'*"
- "That check is the difference between a brief that helps you and one that walks you into a client meeting with a confident-sounding mistake. Claude drafts; you verify."

---

## Step 5: Post-meeting notes (2 min)

Say: "Now the other side of meetings: after they end. Raw notes are messy. Action items are buried. Nobody follows up."

- "Claude fixes all three."
- "Here's the prompt:"

```
Here are my raw notes from a [meeting name] meeting.
Please give me:
1. A 3-bullet summary (what was decided, what's in progress, what's blocked)
2. A clean action item list: each item should have: what, who, by when
3. Any open questions that weren't resolved

Notes:
[paste notes]
```

---

## Step 6: Exercise 2 — Clean up raw meeting notes (5 min)

Action: The raw notes are in `modules/3-meeting-machine/attachments/raw-meeting-notes.md`

Say: "These are notes from a Meridian Q1 Ops Review — and they're a mess, on purpose. Type this in the message box:"

```
Read the file modules/3-meeting-machine/attachments/raw-meeting-notes.md
and clean them up using the pattern above.
```

Check: STOP — wait for student to try and share their clean version

---

## Step 7: Debrief Exercise 2 (1 min)

**Action:** Write the cleaned-up meeting notes (summary, action items, open questions) to `my-work/meeting-notes-clean.md`.

**Say:**

"Saved to `my-work/meeting-notes-clean.md`. Compare the raw notes to this — that's the transformation."

Say: "Now scan the action list with a critical eye. Real notes are messy: some items don't clearly say *who* owns them or *by when*. Watch for two things Claude does when the notes are vague — it either makes its best guess at an owner/date, or it leaves it blank. Both need your eyes."

- "Where an owner or date is missing or looks wrong, fix it before this goes anywhere: *'The contact list is Jordan's, not mine — and it's due Friday the 13th. Update it.'*"
- "Once the owners and dates are right, this is something you can send to the team or paste into Notion with confidence."

---

## Step 8: Exercise 3 — Draft an SOP (5 min)

Say: "Last exercise: turning a verbal process into a written SOP."

- "An SOP (Standard Operating Procedure) is just a step-by-step document. Most companies have dozens of processes that live in someone's head. Claude can extract them."
- "Here's a verbal process description to work with — use this as your input:"

```
Every time we onboard a new client at Meridian, here's what happens:
first the sales team sends a welcome email and introduces the client to their CFO consultant.
Then ops sets up a shared Google Drive folder and sends the client the onboarding checklist.
Then we schedule a kickoff call — usually within 3 business days.
Before the kickoff call, the CFO consultant does background research on the company.
After the kickoff, the consultant writes up a 90-day plan and shares it with the client.
The client signs off on the 90-day plan, and then we're in delivery mode.
```

- "And here's the prompt to use:"

```
Convert this verbal process description into a formatted SOP.
Include: Process name, Purpose (one sentence), Steps (numbered, clear),
Owners for each step, and any notes or dependencies.

Process:
[paste the description above]
```

Check: STOP — wait for student to try and share their SOP

**When student shares their SOP, say:**

**Action:** Write the SOP to `my-work/client-onboarding-sop.md`.

**Say:**

"Saved to `my-work/client-onboarding-sop.md`. Three exercises, three files."

Say: "One thing to notice on SOPs specifically: the description said things like 'the sales team' and 'ops' and 'we' — so Claude had to write those as the owners. A real SOP needs actual roles or names on every step, or it won't hold up. Before you'd publish this, pin the owners down: *'Make the owner of the welcome email the Sales Coordinator, and the kickoff scheduling the Ops Coordinator.'* Vague owners are how processes quietly break."

---

## Step 9: Wrap up + Template prompts (2 min)

**Action:** Append the following to the end of `my-work/prompt-library.md`:

```

## Meetings

**Pre-meeting brief:**
"[meeting context] -> Give me: context summary, top 3 goals, questions to ask, risks."

**Post-meeting cleanup:**
"[raw notes] -> Give me: 3-bullet summary, action items with owners + dates, open questions."

**SOP from description:**
"Convert this verbal process into a formatted SOP: process name, purpose, numbered steps, owners."
```

Say: "I just added 3 meeting prompts to your prompt library. Go look at `my-work/prompt-library.md` — it's growing."

Say: "Module 4 is next — your daily patterns: the moves you'll reach for every morning. After that, Module 5 is where you set it all up for good."

Say: "Type /start-4-1 when you're ready."

---

## Teaching Notes

- If student asks about uploading actual meeting recordings or transcripts: "Totally normal way to work — if your team records meetings (for example with a notetaker like Fireflies), you can hand Claude the transcript and run the exact same cleanup on it. Once you connect your tools in Module 5, this gets even smoother. The paste-in approach you're learning works on any transcript or notes."
- If SOP output isn't quite right, show them how to refine: "Ask Claude: 'Add a section for what to do if the client doesn't respond to the kickoff scheduling.'"
