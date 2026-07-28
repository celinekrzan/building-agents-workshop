---
name: crucible
description: Pressure-test a market-facing artifact before it ships by generating meaningfully different variants, judging them from the named recipient's perspective in isolated context, killing weak options, polishing survivors, and preserving new objections in a reusable rubric. Use for cold emails, headlines, pitches, value propositions, posts, and one-pagers whose real fitness is a human reaction. Do not use for code, open-ended ideation, or work with a computable metric.
---

# Crucible

Generate many → judge hard → keep few → compound.

Use this when the outcome depends on a human reaction that cannot be scored by a
shell command. If the outcome has a numeric, automatable metric, use
`autoresearch` instead.

## Workflow

```text
LOAD RUBRIC
    ↓
GENERATE DISTINCT ANGLES
    ↓
JUDGE IN ISOLATED RECIPIENT CONTEXT
    ↓
KILL WEAK VARIANTS
    ↓
POLISH SURVIVORS
    ↓
APPEND NEW OBJECTIONS TO THE RUBRIC
```

### 1. Load the rubric

Read the artifact-specific rubric. It should contain:

- the real recipient and their situation;
- the pass/fail bar;
- objections learned from earlier attempts;
- evidence or constraints the artifact must respect.

If no rubric exists, create a short one from the user's brief and identify it as
a first-pass rubric.

### 2. Generate distinct angles

Create several variants that differ in strategic angle—not merely wording.
Possible angles include proof, risk, cost, urgency, peer behavior, curiosity, or
the recipient's current problem.

### 3. Judge without author context

Run the judge in isolated context. Give it only:

- the recipient persona and situation;
- the rubric;
- the candidate artifacts.

Do not provide the author's intent or preferred option. For each variant, the
judge must:

1. score it against the rubric;
2. pass or kill it;
3. name the single strongest reason the recipient would ignore or reject it.

### 4. Keep few and polish

Keep only candidates that clear the bar. Give each survivor one revision focused
on its strongest objection. If none survive, report the shared failure and
generate new angles.

### 5. Compound the rubric

Append each distinct new objection to the rubric so the next run begins with what
this run learned. Do not discard negative evidence.

## Output

```text
CRUCIBLE — <artifact type>
Recipient: <who judged>
Survivors: <k>/<n>

Killed
- <variant>: <strongest objection>

Survivors
- <variant>: <polished artifact>

Rubric update
- <new objections preserved>
```

## Boundaries

- Recipient simulation improves scrutiny; it does not predict a real response.
- The judge must not see the author's intent.
- Variants must test different angles.
- One decisive objection is more useful than a cloud of minor edits.
- The real result must be fed back into the rubric after the artifact ships.
