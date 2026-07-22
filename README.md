# Momentum — a calmer to-do

A single-file, private, ADHD-aware daily planner. Open `index.html` in any
browser. Everything saves locally in that browser (nothing leaves your device,
no account, no internet needed). Built to sit alongside the Optimum Safety tools
— same near-black + red look — but this one is personal.

---

## Why this exists (the short version)

Most to-do apps are built for a brain that can hold a 30-item list without
panicking, estimate time accurately, and start a boring task on command. That's
not how ADHD works, and it's not how a mind fighting anxiety/perfectionism works
either. A standard list quietly becomes a **wall of guilt**: everything is
visible, everything feels urgent, nothing signals where to start, and the
undone items pile up as evidence that you're failing.

Momentum is designed the opposite way. The whole thing is organized around four
moves your brain actually needs: **get it out**, **pick a few**, **do one**,
**stop on purpose.**

---

## The system (and the research behind each piece)

### 1. Brain Dump first — capture ≠ commitment
ADHD working memory is the bottleneck. Unfinished tasks don't sit quietly; they
loop (the *Zeigarnik effect* — open loops keep pinging for attention), which
burns focus and spikes anxiety. The fix is **externalizing** everything into one
trusted place so your head can let go of it. The Brain Dump tab takes anything,
in any order, with zero required fields. Writing it down is *not* a promise to do
it today — that separation is the point, and it's what lets the loop close.

> Grounded in: GTD's "capture everything" + "mind like water," and the Zeigarnik
> effect on intrusive task rumination.

### 2. A Big 3 — beat choice paralysis
A long list triggers overwhelm and freeze; more visible options = harder to
start (choice overload). So each day you promote **at most three** tasks to your
Big 3: *if you only do these, today is a win.* Three is deliberate — small enough
to actually finish, which protects the daily sense of "I did what I set out to
do" instead of the usual "I cleared 6 of 22 and still feel behind." Everything
else lives under "Also today" as a genuine bonus, not a debt.

> Grounded in: the "1–3 MITs / Most Important Tasks" method and Ivy Lee's
> six-task rule, trimmed to three for ADHD load.

### 3. Tag by energy and size, not just priority
For ADHD + depression, the real constraint usually isn't time or importance —
it's **available energy and executive bandwidth right now.** So each task can be
tagged **Quick / Focus / Deep** (size) and **Low / Med / High** (energy). On a
flat day you filter your own list by eye: *what can I do with the fuel I actually
have?* Matching the task to your current state is what turns "I should" into "I
can," and it kills the trap of saving a huge task for a moment of perfect energy
that never arrives.

> Grounded in: energy-management / "spoon theory" approaches and executive-function
> coaching, which consistently outperform pure priority sorting for ADHD.

### 4. Break it down to the next tiny step
Task initiation is the classic ADHD wall — you avoid the task because the *first
physical action* is fuzzy. Any task expands into micro-steps, and the prompt is
always the same: **"what's the very next physical action?"** "File the WPAFB
report" is paralyzing; "open the report template" is doable. You only ever have
to see the next step.

> Grounded in: GTD's "next action" principle and cognitive-behavioral task
> chunking.

### 5. Focus mode — one task, one timer
Time blindness (poor felt sense of duration) makes both starting and stopping
hard. Focus mode shows exactly **one** task, hides everything else, and runs a
visible countdown (10 / 15 / 25 / 45 min). Short, bounded sprints lower the
activation cost of starting ("it's only 25 minutes") and make time concrete. The
single-task view removes the overwhelm of the full list while you work.

> Grounded in: the Pomodoro technique and time-boxing; single-tasking under
> visible time cues.

### 6. Shutdown — the part other apps skip
This is the piece built specifically for *"I can't relax or finish tasks fully."*
A day with no defined end never really ends — the list keeps pulling at you, so
rest never feels allowed. The Shutdown tab gives the day a **deliberate close:**

- **What you moved forward** — your wins, framed as *done = you moved it, not you
  perfected it.* (Direct counter to perfectionism, which redefines "done" as
  "flawless" and so nothing ever qualifies.) Finishing and *seeing* the finish
  gives the dopamine hit ADHD brains are short on.
- **Rolling over to tomorrow** — undone items, explicitly framed as *next, not
  failed.* They quietly return to the Brain Dump. Nothing ever turns red or
  screams "OVERDUE." Shame is not a productivity strategy; it just adds
  avoidance.
- **Permission to rest** — a plain statement that you're allowed to stop. Rest
  isn't a reward you earn by clearing the list; it's a need. "Close the day"
  parks everything and clears the board so tomorrow starts calm.

> Grounded in: Cal Newport's "shutdown ritual" for closing open loops, plus
> self-compassion research (Kristin Neff) showing self-kindness beats
> self-criticism for follow-through — especially with ADHD and anxiety.

---

## Your daily loop (the 4-minute version)

1. **Morning (2 min):** open **Brain Dump**, empty your head. Then move to
   **Today** and star your **Big 3.** Stop at three.
2. **During the day:** when it's time to work, go to **Focus**, pick one thing,
   start the timer. Feeling flat? Tag/scan by **energy** and grab a Low-energy
   Quick win to build momentum.
3. **Evening (2 min):** open **Shutdown.** Look at your wins. Let the rest roll
   over. Hit **Close the day** and actually stop.

Do that and skip everything else and it still works. The system is designed so
the *minimum* version is the whole thing.

---

## A few deliberate design choices

- **A short list is a kind list.** Empty states congratulate you instead of
  nagging. Blank is a valid, good state.
- **No streaks-you-can-break, no red overdue badges.** Pressure mechanics
  backfire for anxiety. Momentum nudges; it never scolds.
- **One place, low friction.** Four tabs, quick-add always visible, works
  offline. The fastest system is the one you'll actually open.
- **Private by default.** All data lives in your browser's `localStorage`. No
  server, no sign-in, no sync (yet — see below).

---

## Running / hosting it

No build step. Options:

- **Simplest:** download `index.html` and open it. Bookmark it. Done.
- **On your phone:** host it (Netlify drag-and-drop, or add it to the Optimum
  tools portal) and "Add to Home Screen" so it opens like an app.
- **Alongside the portal:** drop this folder in as `tools/momentum/` and add one
  card to the `TOOLS` array in the portal's `dashboard.html`. It already uses the
  same brand tokens, so it'll match.

> Note: because storage is per-browser, your tasks won't sync between your phone
> and laptop yet. If you want that, the natural next step is a small sync layer
> (or wiring the day's time-blocks straight into your Google Calendar — ask and
> that can be built).

---

## Possible next iterations

- **Google Calendar sync** — push your Big 3 / time-blocks into your calendar as
  real blocks (you already have Calendar connected).
- **Cross-device sync** so phone and laptop share one list.
- **A weekly review view** — a gentle Sunday look-back, wins tallied.
- **Recurring tasks** and a light morning reminder.

None of these are needed for the system to work. They're comfort, not
foundation. Start with the four moves.
