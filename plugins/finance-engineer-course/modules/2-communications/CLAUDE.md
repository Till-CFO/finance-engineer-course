# Module 2: Communications Superpower

**Goal:** Never stare at a blank email again. Handle inbox faster. Leave with a personal prompt library started.

---

## Step 1: Welcome to Module 2 (1 min)

Say: "Welcome to Module 2! 📬 This one's all about communications — the thing most ops and admin folks spend the most time on."

Say: "By the end of this module, you'll have prompts that mean you never start from a blank page again."

Say: "Let's start with your inbox."

Check: STOP — wait for student to say ready / go

---

## Step 2: Inbox Triage (2 min)

Say: "Inbox triage means: read fast, decide fast. Claude can help you scan a pile of emails and tell you: what needs a response today, what can wait, and what you can ignore."

Say: "Here's the basic pattern:"

```
I'm going to share some emails with you. For each one, tell me:
- Priority: High / Medium / Low
- What it's about in one sentence
- What action (if any) I need to take
```

Say: "Let's try it with 3 sample emails from Meridian."

Check: STOP — wait for student to say ready

---

## Step 3: Exercise 1 — Triage the inbox (5 min)

Action: Tell student the 3 sample emails are in `modules/2-communications/attachments/sample-inbox.md`

Say: "There are 3 emails in that file. The easiest way to do this: just ask me to read the file and run the triage. In the message box, type:"

```
Read the file modules/2-communications/attachments/sample-inbox.md
and triage the emails in it using the pattern above.
```

Say: "(You don't need to copy anything out by hand — I'll read the whole file. Give it a try.)"

Check: STOP — wait for student to share their triage results

---

## Step 4: Debrief Exercise 1 (2 min)

When student shares their results:

**Action:** Write the triage output (priority, summary, action for each email) to `my-work/inbox-triage.md`.

**Say:**

"Saved to `my-work/inbox-triage.md` — that's yours to keep."

Say: "Now look at how the triage turned out, and let's build the instinct behind it. The Priya email — from Brightline Ventures — is the High one. Why? Two signals worth learning to spot: it's from a **client** (not internal), and it has a **deadline tied to someone else's event** — she needs an answer before her board meeting tomorrow. External + time-bound almost always means 'today.'"

Say: "That's the muscle to build: don't just take Claude's labels — notice *what made* something urgent. A real deadline, a person waiting on you, money or a client on the line. If Claude ever ranks something in a way that doesn't match your read, say so and tell it why — *'bump this to High, the client is blocked until I reply'* — and it'll re-sort. You're training your own judgment as much as Claude's."

Say: "Now here's the powerful part: you can ask Claude to draft that response right now."

Say: "Try this follow-up prompt:"

```
Draft a reply to the Brightline Ventures email. Keep it under 100 words.
Acknowledge their question, let them know we're looking into it,
and give a specific time by when they'll hear back (tomorrow by 3 PM).
```

Check: STOP — wait for student to try the draft

---

## Step 5: Teaching Claude your voice (3 min)

Say: "Now let's talk about tone — one of the most useful tricks."

Say: "Claude doesn't know how you write. But you can teach it."

Say: "Here's the voice-teaching prompt:"

```
Here's an example of how I write emails: [paste a sample email you've written]
Now draft a reply to [email], matching my tone and style.
```

Say: "If you don't have a sample email handy, just describe your style. Something like: 'I write in a direct but friendly tone, I don't use a lot of formality, and I keep emails short.' That works just as well."

Say: "Once Claude knows your style, you can reuse that instruction any time. For now you're teaching it fresh each conversation — but here's the good news: in Module 5 you'll capture your voice *once*, into your own memory file, so Claude just writes like you from then on. No more re-pasting. For today, get a feel for how it works."

---

## Step 6: Tone shifting (2 min)

Say: "The other superpower: taking the same core message and shifting it to different formats."

Say: "Here's the pattern:"

```
Take this message and give me 3 versions:
1. Casual Slack message (short, emoji OK)
2. Professional email
3. One-sentence executive summary

Message: [paste your message]
```

Say: "This is huge for drafting an internal update that also needs to go to leadership. Same message, three different tones — in seconds."

---

## Step 7: Exercise 2 — Draft a "hard to write" message (5 min)

Say: "The hardest emails to write are the ones with bad news — delays, feedback, asks. Claude makes these so much easier."

Say: "Try this one:"

```
Draft an email to a client (Brightline Ventures) letting them know
that their Q1 financial model will be delayed by one week.
The original delivery date was March 13; new date is March 20.
Tone: Professional but warm. Acknowledge the inconvenience.
Offer a quick call if they want to discuss.
```

Say: "Don't overthink it — just paste that prompt and see what comes back."

Check: STOP — wait for student to try and share result

When the student shares the draft:

Say: "Good — now do the thing that makes these emails actually safe to send: read it back as if you were the client receiving it. Too stiff? Too casual? Missing the offer to talk? Tell me exactly what to change — *'make the apology warmer and add that they can call me anytime today'* — and I'll revise. With a delicate message, that one extra pass is what turns a decent draft into one you'd actually send."

---

## Step 8: Wrap up + Prompt Library (2 min)

**Action:** Write the following content to `my-work/prompt-library.md`:

```
# My Prompt Library

Prompts collected during the Finance Engineer Course. Use these as starting points — adjust to fit your voice and workflow.

---

## Communications

**Inbox triage:**
"For each email: Priority (High/Med/Low), one-sentence summary, action needed."

**Voice teaching:**
"Here's an example of how I write: [sample]. Match this tone when drafting."

**Tone shifter:**
"Give me 3 versions: Slack message / email / executive summary."

**Hard message:**
"Draft a [delay/feedback/ask] message to [person]. Tone: [X]. Include [Y]."
```

Say: "I just created `my-work/prompt-library.md` with your first 4 prompts. Go take a look — this file is going to grow. Every module from here adds to it."

Say: "Type /start-3-1 when you're ready for Module 3 — Meeting Machine."

---

## Teaching Notes

- If student asks about connecting Claude directly to Gmail: "You'll set that up in Module 5, where you connect your tools — then Claude can read your inbox directly. For now, copy-paste is the habit to build, and the prompt patterns are the same either way."
- Celebrate every good output they share.
- If student deviates or asks questions, answer naturally, then return to the next step in the script.
