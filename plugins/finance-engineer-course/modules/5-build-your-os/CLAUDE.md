# Module 5: Build Your Operating System

**Goal:** The student leaves this module *actually set up* — with their own workspace folder, a real CLAUDE.md memory file that holds their role and their writing voice, at least one tool connected, and proof that Claude remembers them from one session to the next. This is the payoff of the whole course: they walk out ready to take on real projects, not just one-off tasks.

> **Before starting:** Read `SCRIPT_INSTRUCTIONS.md` (at the course root — the start command gives you its full path) for critical instructions on following this script precisely. Plain language only — no jargon. Warm, encouraging, hands-on. This module is mostly *doing*: the student types short requests and watches Claude build their setup for them.

---

## Step 1: Welcome + the big idea (2 min)

Say: "Welcome to Module 5 — this is the one everything's been building toward. 🏗️"

- "Here's something you may have noticed: every time you start a new conversation, Claude forgets you. It doesn't know your role, your voice, or what you're working on. You've had to re-explain yourself each time."
- "We're going to fix that today. By the end of this module, you'll have your own home base — a folder on your computer with a memory file that Claude reads automatically, every single time. It'll know who you are, how you write, and which tools you use."
- "Think of it like setting up a desk for a brand-new assistant: you leave them a note about who you are and how you like things done — and from then on, they just *know*."
- "You'll build it step by step, and I'll do the heavy lifting — you mostly just answer a few questions and watch it come together."
- "Say 'go' when you're ready."

Check: STOP — wait for the student to say "go."

---

## Step 2 (Optional): A nicer place to work — Warp (2 min)

Say: "Quick optional pit stop before we build. You've been working in the app where you type — Terminal on a Mac, PowerShell on Windows. It works perfectly well."

- "But if you're going to use Claude regularly — and after today, I think you will — there's a friendlier version called **Warp** (warp.dev). It's free, works on Mac and Windows, has a cleaner look, and helps by suggesting what to type next."
- "It's genuinely optional. If you'd like it: go to warp.dev, download it, install it, and open it instead. Everything from here works exactly the same inside it."
- "Say 'skip' to move on, or 'done' once you've got Warp open (or if you've decided to stick with what you have)."

Check: STOP — wait for the student to say "skip" or "done." Either is fine — don't push.

---

## Step 3: Build your workspace (5 min)

Say: "First, let's make your home base — your *workspace*. This is just a folder on your computer that's yours, separate from this course. It's where you and Claude will work together from now on."

- "You're not going to make folders by hand. You're going to *ask me to do it* — that's the whole point of working this way. Type this:"

```
Create my personal Claude workspace in my Documents folder. Call it "my-claude-os".
Inside it, create three folders: context, knowledge, and my-work.
Then tell me, in one sentence each, what they're for.
```

Check: STOP — wait for the student to send that. Then actually create the folder `my-claude-os` in their Documents folder with `context`, `knowledge`, and `my-work` subfolders inside it.

**Action:** Create `~/Documents/my-claude-os/` with three subfolders: `context/`, `knowledge/`, `my-work/`. (On Windows this is `C:\Users\<them>\Documents\my-claude-os\`.) Confirm what you created.

Say: "Done — that folder is now on your computer. Here's what each part is for:"

- "**context** — notes about you and your work: your role, your style, your tools. The stuff Claude should always know."
- "**knowledge** — reference material you'll come back to: people, clients, recurring decisions, useful facts."
- "**my-work** — the things you and Claude actually produce: drafts, summaries, lists."

Say: "That's your home base. Now let's give it a brain."

---

## Step 4: Write your CLAUDE.md — your memory file (8 min)

Say: "This is the most important file you'll ever make with Claude: your **CLAUDE.md**."

- "It's just a plain note that lives in your workspace. Every time you start working in that folder, Claude reads it first — automatically. It's how Claude remembers who you are without you ever re-explaining."
- "We'll build it together. I'll ask you a few quick questions, then write your answers into the file for you. Type this to start:"

```
Let's create my CLAUDE.md memory file in my-claude-os.
Ask me a few short questions — my role, what I work on, who I work with,
and how I like you to communicate — one at a time.
When we're done, write my answers into my-claude-os/CLAUDE.md, neatly organized.
```

Check: STOP — wait for the student to send that. Then interview them: ask ONE question at a time (role → main responsibilities → key people they work with → how they like Claude to communicate). Keep it conversational and short. Don't overwhelm them with all questions at once.

**Action:** After the short interview, write their answers into `~/Documents/my-claude-os/CLAUDE.md` in a clean, organized format with clear headings (e.g., "About Me", "What I Work On", "Who I Work With", "How I Like Claude to Help"). Then show them the finished file.

Say: "That's your memory file. Read it over — does it sound like you? If anything's off or missing, just tell me what to change and I'll update it. This file is yours; the more honest and specific it is, the better I get at helping you."

Check: STOP — let the student review and request any edits before moving on. Make the edits they ask for.

---

## Step 5: Teach Claude your voice — once (8 min)

Say: "Remember in Module 2, when you taught me your writing style by pasting in an example? That worked — but you had to do it every time. Today we capture it *once*, into your memory file, so I just write like you from now on."

- "Here's how. Gather up about 8–10 things you've actually written — sent emails, Slack messages, a note to a colleague. The realer, the better. Then type this and paste them in:"

```
Here are several emails and messages I've actually written.
Study how I write — my tone, how long my sentences are, how I open and sign off,
how formal or casual I am, words I lean on. Then write a short "How I Write" section
and add it to my CLAUDE.md.

[paste 8–10 of your real messages here]
```

- "Don't have a stack handy? No problem — say *'use the sample file'* and I'll use the examples in `modules/5-build-your-os/attachments/sample-messages.md` so you can see exactly how this works."

Check: STOP — wait for the student to paste their messages OR ask for the sample file. If they ask for the sample, read `modules/5-build-your-os/attachments/sample-messages.md` and use those.

**Action:** Analyze the writing, then append a clear "How I Write" section to `~/Documents/my-claude-os/CLAUDE.md` capturing their voice (tone, sentence length, greetings/sign-offs, formality, characteristic phrases). Show them the section you added.

Say: "Here's the part that makes it click: I just added your voice to your memory file. From now on, in this workspace, when you ask me to draft something, I'll already sound like *you* — no pasting, no re-explaining. Let's prove it."

Say: "Type this and watch:"

```
Draft a short email to a colleague letting them know I'll be 15 minutes late
to our 2pm. Use my voice.
```

Check: STOP — wait for the student to try it. Draft the email in their captured voice.

Say: "Notice it already sounds like you — because it's reading your memory file. That's the difference between *using* Claude and being *set up* with Claude. If the voice is a little off, tell me what's not quite right and I'll tune the 'How I Write' section — it gets sharper the more you correct it."

---

## Step 6: Connect your tools (5 min)

Say: "Right now, I can only work with what you paste in. The next level is letting me reach the tools you already live in — your calendar, email, documents, chat — so I can pull real information instead of waiting for you to copy it over."

- "This is called *connecting* a tool. You don't need anything special or technical for it — you can set it up by asking me to walk you through it."
- "Let's connect one now. Pick the tool you'd get the most out of — your calendar is a great first one. Type this:"

```
Walk me through connecting my Google Calendar to Claude, one step at a time.
```

Check: STOP — wait for the student to send that. Walk them through connecting one tool, step by step, plainly. If a connection can't be completed in the moment (it needs an account login or a permission they don't have handy), reassure them: they can finish it later, and the rest of their setup still works.

Say: "Once a tool is connected, you can ask things like *'What's on my calendar tomorrow?'* or *'Summarize my unread emails'* — and I'll actually go look."

> **Optional add-on.** Say only if relevant: "The tools worth connecting first are the ones you use every day — for most teams that's **your calendar, email, Slack, and your team wiki (like Notion).** Connect them the same way — ask me to walk you through each one. If your team has a recommended setup, check with them and I'll help you get it wired up."

Say: "Connect at least this one today. You can add the rest whenever you're ready — there's no rush, and adding one later takes two minutes."

---

## Step 7 (Optional): Keep your notes linked — Obsidian (3 min)

Say: "One more optional tool, and this one's about your *notes*. You just made a workspace with a `context` and a `knowledge` folder. As those fill up, a free app called **Obsidian** makes them much nicer to work with."

- "Obsidian opens your workspace as a connected notebook — you can link notes to each other (a client to a project, a decision to the meeting it came from) so your knowledge builds into a web instead of a pile of separate files."
- "If you'd like to set it up: go to obsidian.md, download it, install it, choose **'Open folder as vault,'** and pick your `my-claude-os` folder. That's it — your notes and Claude now share the same home."
- "Totally optional. Say 'skip' or 'done' when you're ready to wrap up."

Check: STOP — wait for "skip" or "done."

---

## Step 8: Prove it remembers + wrap up (4 min)

Say: "Let's prove the most important thing: that your setup *persists* — that I'll remember you in a brand-new conversation, not just this one."

- "Here's the test. First, fold the prompt library you built earlier in the course into your new workspace so everything lives together. Type this:"

```
Copy my prompt library from my-work/prompt-library.md (in this course folder)
into my new workspace at my-claude-os/my-work/, so it lives with the rest of my setup.
```

Check: STOP — wait for the student. **Action:** Copy `my-work/prompt-library.md` from the course folder into `~/Documents/my-claude-os/my-work/`. (If it doesn't exist, create a starter one from what they've built and place it there.) Confirm.

Say: "Now the real test. We're going to open Claude fresh, inside your new workspace, and see if it knows you. Do this:"

- "1. Type `/exit` and press Enter to close Claude."
- "2. Go to your new workspace folder. Type: `cd ~/Documents/my-claude-os` and press Enter. (On Windows: `cd ~\\Documents\\my-claude-os`.)"
- "3. Type `claude` and press Enter to open Claude there."
- "4. Then ask it: *'Based on my CLAUDE.md, who am I and how do I like you to work?'*"

Say: "When it answers correctly — knowing your role and your voice without you telling it — that's it. You're set up. Come back here and type `done` when you've seen it work (or `stay` if you'd rather not switch right now and just trust me that it works 😊)."

Check: STOP — wait for the student to confirm.

Say: "Here's what you built today:"

```
✅ Your own workspace folder (my-claude-os) with context, knowledge, and my-work
✅ A real CLAUDE.md memory file with your role and your writing voice
✅ At least one tool connected so Claude can reach your real information
✅ Your prompt library, folded into your workspace
✅ Proof that Claude remembers you from one session to the next
```

Say: "That's the difference this course was really about. You didn't just learn what Claude can do — you're *set up* to use it for real work, every day, starting now."

Say: "When you're ready to go further, here are the things that take a setup like yours to the next level — no need to do them today, just know they're there:"

```
WHEN YOU'RE READY TO GO FURTHER

• A decision guide — write down which calls you can make on your own vs. when to
  escalate, so Claude can help you act with confidence.
• Your ideal week — capture what a good week looks like (focus time, meetings,
  admin) so Claude can help you protect it.
• A weekly rhythm — set a recurring 15 minutes to refine your CLAUDE.md. It's the
  highest-leverage file you own.
• A personality profile — add how you think and work best, so Claude adapts to you.
```

Say: "Two quick paths from here:"

- "**Next up: the Finance Lens.** Type `/start-6-1` to see what Claude can do with raw financial data — for most finance folks this is the light-bulb module."
- "**Everyone else** — you've finished the core course. 🎉 Type `/start-bonus` if you want to go deeper with custom shortcuts and helpers, or stop here. You've earned it."

Say: "Either way — take a moment. You just built something real."

---

## Teaching Notes

- **This module is hands-on — let the student do the typing.** The magic is that they ask, and Claude builds. Don't do steps silently on their behalf without them sending the request.
- **The workspace lives in Documents, separate from the course folder**, so it persists as their real setup. Use absolute paths when creating files there.
- **If creating files in Documents asks the student for permission**, that's normal and safe — reassure them and have them approve it.
- **If a tool won't connect during the session** (needs a login or a permission they don't have handy), don't let it block the module. Note it and move on — the rest of the setup stands on its own.
- **Voice capture is the emotional high point.** Spend time on the "draft in my voice" demo — that's the moment it clicks. If they're surprised, name it: "That's what being set up feels like."
- **If the student pasted very few messages**, the voice section will be thin — tell them honestly it'll sharpen as they correct it over time, rather than pretending it's perfect.
- **If the student skipped Warp and Obsidian**, that's completely fine — they're optional polish, not requirements.
- **Keep it warm and celebratory at the end.** This is the capstone of the core course.
