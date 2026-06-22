---
name: weekly-dashboard
description: Turn a messy brain-dump or a screenshot of your calendar, planner, whiteboard, or sticky notes into a clean, prioritized weekly dashboard. Use whenever someone wants to plan their week, get organized, make sense of a pile of tasks, see what's due, or "spin up a dashboard" from notes or an image of their schedule. Trigger on phrases like "plan my week," "here's everything I need to do," "make me a dashboard," "organize this," "what should I focus on," or when someone pastes a list of tasks or uploads a photo of a calendar or to-do list.
---

# Weekly Dashboard

Take whatever the person gives you about their week and turn it into one clean, prioritized dashboard they can actually use. The input is almost always messy. A photo of a wall calendar. A screenshot of their Google Calendar week. A wall of typed tasks with no structure. A few sticky notes. Your job is to read it, find the signal, and hand back order.

The whole point is that they should not have to organize their own thoughts before they get value. They dump, you structure.

## When to use

- Someone uploads an image of a calendar, planner, whiteboard, or sticky notes and wants it made sense of.
- Someone pastes or types a brain-dump of tasks, events, and deadlines.
- Someone says "plan my week," "what should I focus on," "make me a dashboard," or similar.
- Start of the week, or any time the week has gotten away from them and they need a reset.

## Inputs

Accept any of these, in any combination:

- An image (screenshot or photo) of a schedule, calendar, planner, to-do list, or notes.
- Typed or pasted text: tasks, events, deadlines, half-formed intentions.
- Nothing structured at all. If they just say "help me plan my week," ask them to brain-dump everything on their mind or drop a screenshot.

## Steps

1. **Read everything they gave you.** If it's an image, extract every task, event, time, and date you can see. Read handwriting carefully. If part of the image is unreadable, note it rather than guessing.

2. **Figure out the week.** Use today's date to anchor the current week (Monday to Sunday). If the input clearly refers to a different week, use that one. Don't ask if it's obvious.

3. **Separate events from tasks.** Events are time-bound and happen whether or not the person acts (meetings, appointments, calls). Tasks are things they have to do (write the proposal, book the dentist, reply to Sam). Treat them differently in the output.

4. **Infer priority.** You usually won't be told. Use signal: hard deadlines, words like "urgent," "ASAP," "EOD," dependencies ("can't start X until Y"), and anything that looks like it has consequences if it slips. When genuinely unsure, make a call and mark it so they can correct you.

5. **Ask only what you must.** If something critical is ambiguous (a date with no clear deadline, a task that might be huge or tiny), ask one or two tight questions. Otherwise build the dashboard first and invite corrections after. Don't interrogate them before delivering value.

6. **Build the dashboard** using the structure below.

7. **Write it to a file** so they can keep it: `weekly-dashboard.md`. Also show it in the reply.

8. **Close with a short, honest read.** One or two sentences: the day that looks overloaded, the deadline most at risk, or the one thing that matters most this week. Then offer to adjust.

## Dashboard structure

Use this exact shape. Keep it tight. This is a working document, not a report.

```
# Week of [Mon date] – [Sun date]
[One sentence on what this week is really about, based on what's in it.]

## Focus this week
[The 3 to 6 things that actually matter. Ordered. Not everything — the things that, if they slip, the week slips.]
- [ ] [Task] — [why it matters or when it's due]

## Schedule
**Mon [date]**
- [time] [event]
**Tue [date]**
- [time] [event]
[...through Sun. Skip empty days or mark them "Open."]

## Tasks
[Everything that needs doing but isn't time-locked. Group by priority, or by area/role if the person works across clearly different domains.]

**High**
- [ ] [task] — [due / context]

**When you can**
- [ ] [task]

## Watch out for
[Honest flags. An overloaded day. A deadline with no time blocked for it. Two things that conflict. A task that depends on something not scheduled yet. If nothing's at risk, say so plainly.]

## Notes
[Leave this open for them to jot completions and changes as the week goes.]
```

### Rules for the Focus section

Cap it at six. The discipline is the value. If you list fifteen "priorities," you've given them their brain-dump back with checkboxes. Pick the few that carry the week and put the rest under Tasks.

Order Focus by what's most consequential, not alphabetically and not by date alone. A small task with a hard external deadline can outrank a big one with no deadline.

### Handling images

When the input is a screenshot or photo:

- Pull out every dated or timed item you can read.
- Map times to the right day. Calendar screenshots put days in columns. Read carefully so a Wednesday event doesn't land on Thursday.
- If text is cut off or unreadable, list what you got and flag the gap. Never invent an event to fill a hole.

## Personalization (optional)

If the person tells you their roles or focus areas (founder, parent, the side project, study), group the Tasks section by those instead of by priority. It helps people who switch between very different modes see each world clearly. Don't force this if they haven't given you the context.

## Tone and writing

This is for one person to read fast on a Monday. Write like a sharp assistant who respects their time.

- No filler, no hedging, no corporate language.
- No em-dashes. Use a comma, a period, or restructure.
- Bold only for the few things that matter.
- Short lines. A dashboard is scanned, not read.
- Take a stance on priority. "This is the one that matters" beats "you may want to consider."

## Output

A file named `weekly-dashboard.md`, plus the dashboard rendered in the reply.

## Safety

This skill only organizes and plans. It never sends messages, books anything, or takes external action on the person's behalf. If a task involves sending or scheduling something, it stays a checkbox for the person to do.
