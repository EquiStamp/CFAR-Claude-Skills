---
name: murphyjitsu
description: >
  CFAR rationality technique for bulletproofing plans by systematically imagining failure modes
  and creating defenses. Combines Murphy's Law with pre-mortem analysis. Use when the user:
  (1) has a plan they want to stress-test, (2) wants to identify what could go wrong before
  it does, (3) needs to build a more robust plan, (4) wants to practice pre-mortem thinking,
  or (5) is about to start a project and wants to anticipate obstacles.
  Triggers: "murphyjitsu", "what could go wrong", "pre-mortem", "stress test my plan",
  "inner simulator", "surprise-o-meter", "failure modes", "plan review", "CFAR".
---

# Murphyjitsu (Inner Simulator)

A CFAR technique for bulletproofing plans by deliberately imagining failure, identifying the most likely failure modes, and creating defenses. Named after Murphy's Law + martial arts ("jitsu").

## Three Modes

1. **Design Mode** — Help create a robust plan with failure modes already addressed
2. **Practice Mode** — Walk through the technique on a practice plan to build skill
3. **Execute Mode** — Stress-test a real plan the user is about to implement

## Core Algorithm

```
1. State a concrete plan
2. Imagine: "It's the day after. The plan failed. What happened?"
3. Check the surprise-o-meter
4. If genuinely shocked → done
5. Otherwise → identify the most likely failure mode
6. Create a defense against it
7. Go to step 2
```

## The Surprise-o-Meter

After imagining failure, assess how surprised you'd be:
- **"Yeah, sounds right"** → Keep iterating. You have known failure modes.
- **"Somewhat surprised"** → Getting close. Address remaining risks.
- **"Genuinely shocked"** → Your inner simulator endorses the plan. Stop here.

The technique continues until you'd be genuinely shocked to see the plan fail.

## Step-by-Step Facilitation

### 1. Articulate the Plan
"What's your concrete plan? What specific actions, in what order, by when?"
Ensure the plan is concrete enough to simulate. Vague goals can't be Murphyjitsued.

### 2. Initial Simulation
"Imagine you've executed this plan and suddenly realize it failed. Oh no — why? What happened?"
Don't answer from analysis. Let intuition respond. The first answer is often most accurate.

### 3. Identify the Failure Mode
"What's the most likely way this goes wrong?"
"If you had to bet money on what would derail this, what would you say?"

### 4. Create the Defense
"What action or preparation would prevent this failure mode?"
Defenses should be: specific, actionable, low-cost, and preventive.

### 5. Re-simulate
"Now imagine the plan WITH this defense. It still failed. What happened this time?"
Repeat until the surprise-o-meter reads "shocked."

## Key Insight: Outside View Correction

Your inner simulator is better at predicting OTHER people's failures than your own. Correction: "Take your plan and imagine another person made it. How would it likely fail for them?"

## Facilitation Prompts

**Opening**: "Tell me your plan. Be specific — what exactly will you do and when?"

**Simulation**: "Close your eyes. It's [deadline day]. The plan didn't work. What went wrong?"

**Probing**: "What's the single most likely failure point?" / "What have you seen go wrong in similar situations?"

**Defense**: "What's the simplest thing you could do to prevent that?" / "What would someone who's done this before do differently?"

**Calibration**: "If I told you the plan failed, how surprised would you be — genuinely shocked, or just disappointed?"

## Common Failure Modes of the Technique

- **Self-bias**: Your inner sim is optimistic about your own plans. Use outside view.
- **Unpredictable domains**: Works best for tactical, near-term plans. Less useful for existential life questions.
- **Unrealistic expectations**: No plan is foolproof. Goal is "shocked if it fails," not "impossible to fail."
- **Emotional failure modes**: Murphyjitsu handles logistical failures well but may miss motivation loss. Combine with IDC.

## Practice Exercise

1. Pick an upcoming plan (meeting, project, event)
2. Run 3-5 failure simulation cycles
3. Write down each failure mode and its defense
4. After 5 minutes: "Would you be genuinely shocked if this failed now?"
5. If not, continue. If yes, commit to the plan with defenses.

## Integration

- **Goal Factoring**: Factor goals first, then Murphyjitsu the plan
- **TAPs**: Create TAPs for implementing the defenses
- **Resolve Cycles**: If Murphyjitsu reveals the plan is fundamentally broken, do a 5-minute Resolve Cycle to find a better approach
