# Momentum — a calmer to-do

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/irvinkali/To-Do)

**One-click deploy:** click the button above, authorize Netlify with GitHub if
asked, and it'll host Momentum at its own URL. No build settings to change —
the `netlify.toml` handles everything. Then open the URL, tap **Connect**, and
paste your Supabase URL + publishable key (same project as your command app).


A single-file, ADHD-aware **daily lens** over your existing synced task list.
Open `index.html` in any browser. It reads and writes the **same tasks as your
command app** (via that app's Supabase), so everything syncs across your devices
automatically. Built to sit alongside the Optimum Safety tools — same near-black
+ red look — but this one is personal.

It is deliberately *not* another separate silo. Your command app stays your
capture point and warehouse; Momentum sits on top and answers only "what am I
doing today, and did today count?"

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

### 2. Anchors — beat choice paralysis
A long list triggers overwhelm and freeze; more visible options = harder to
start (choice overload). So each day you promote a tiny set of **anchors** —
*if you only do these, today is a win.* Everything else lives under "Small &
quick" or "Also today" as a genuine bonus, not a debt.

> Grounded in: the "1–3 MITs / Most Important Tasks" method and Ivy Lee's
> six-task rule, trimmed hard for ADHD load.

**Work Big 3 + one Home/Life anchor.** A single shared Big 3 is cleanest in
theory, but real life isn't balanced: work is deadline-dense and eats most of
the day, while home is more "when there's time." So the anchors split into
**up to 3 for work** and **exactly 1 for home** — four total, still small enough
to protect the "I did what mattered" feeling, but weighted the way your actual
day is. The single home anchor guarantees life never silently drops off the list,
without pretending you'll do three home projects on a Tuesday. Star (★) a task to
anchor it; the app routes it to Work or Home by its category and enforces each
cap (3 and 1). The **View** filter (All / Work / Home / Life) lets you see just
one side when you're in that headspace.

**Small work tasks live in their own lane — and never count against you.** Work
throws off a pile of little things that just have to happen, usually more than
three. Those are *maintenance*, not the day's *meaning*, so mixing them into the
Big 3 is exactly what makes the list feel crushing. Tag a task **quick** and it
drops into the **Small & quick** batch — uncapped, meant to be swept in one
low-energy pass. Checking them off gives you the dopamine wins; *not* finishing
them is never failure, because they were never your win-condition. This is the
core mechanic that lets a low-output day still feel worthy: the thing that
measures your day (the Big 3) stays small and reachable, while the busywork
stays visibly *bonus.*

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

### 4. Break it down to the next tiny step — and surface *that* step
Task initiation is the classic ADHD wall — you avoid the task because the *first
physical action* is fuzzy. Any task expands into micro-steps, and the prompt is
always the same: **"what's the very next physical action?"** "File the WPAFB
report" is paralyzing; "open the report template" is doable. You only ever have
to see the next step.

**Steps can be surfaced onto today as their own quick task.** This is the fix
for long, multi-day projects — the kind home life is full of ("repaint the
fence," "sort the garage"). You'd never finish the whole project in a day, and
being forced to check off the *overarching* task means it sits there, permanently
un-done, quietly reading as failure. Instead the project lives in your backlog,
and each day you **surface one step** (`→ today`) so *that step* becomes the thing
on your plan. Checking it off is a real, complete win, and the project advances —
without the project itself needing to be "done." A surfaced step can even be your
Home/Life anchor for the day. Progress on a step *is* progress; the system treats
it that way.

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
- **One place, low friction.** Four tabs, quick-add always visible. The fastest
  system is the one you'll actually open.
- **It never scolds and never destroys.** No streaks to break, no red "OVERDUE."
  And Momentum only ever *adds* to a task or marks it done — see below.

---

## How it connects to your command app

Momentum and the command app share one Supabase `tasks` table. Each task is
stored as a flexible JSON blob, so Momentum layers its own fields onto the *same*
task without changing anything the command app relies on:

| Command-app field | How Momentum uses it |
|---|---|
| `category` (rolled up to work / personal) | the **area filter** and the coloured area chip |
| `done` / `status` | the **checkbox** (checking sets `status: "Done"`) |
| `steps` (`{id, text, done}`) | **subtasks** — written back in the exact same shape |
| `title`, `note`, `dueDate` | shown as-is (due date is a gentle chip, never red) |
| *new, additive:* `mBig3`, `mSize`, `mEnergy`, `mDay`, `mDoneDay` | the Big 3, energy/size tags, and "on today's plan" |

**Safety guarantees (built into the code):**
- Every write is an **upsert** (`resolution=merge-duplicates`). Momentum never
  issues a DELETE.
- The **✕** on a task means *"take it off today's plan"* (`mDay = null`) — the
  task stays in your warehouse and in the command app, untouched.
- Momentum-only fields are prefixed `m…` and ignored by the command app, so the
  two apps can't step on each other.
- If the cloud is unreachable, it falls back to the same `localStorage` backup
  key the command app uses and shows an **offline** dot; writes resume on
  reconnect.

It refreshes from the cloud on window-focus and every 60 s, so a task you add by
voice in the command app shows up in Momentum shortly after.

---

## Running / hosting it

No build step. Options:

- **Simplest:** open `index.html`. Bookmark it.
- **On your phone:** host it (Netlify drag-and-drop, or add it to the Optimum
  tools portal) and "Add to Home Screen" so it opens like an app. Because it's
  cloud-synced, your phone and laptop show the same list automatically.
- **Alongside the portal:** drop this folder in as `tools/momentum/` and add one
  card to the `TOOLS` array in the portal's `dashboard.html`. It already uses the
  same brand tokens, so it'll match.

---

## Possible next iterations

- **Google Calendar sync** — push your Big 3 / time-blocks into your calendar as
  real blocks (you already have Calendar connected).
- **Read the command app's `inbox` table** — surface raw voice captures as
  unsorted items to convert into tasks.
- **A weekly review view** — a gentle Sunday look-back, wins tallied.
- **Recurring tasks** and a light morning reminder.

None of these are needed for the system to work. They're comfort, not
foundation. Start with the four moves.
