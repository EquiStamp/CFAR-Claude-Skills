# CFAR Rationality Skills for Claude

A collection of 12 Claude skills based on techniques taught at [CFAR](https://rationality.org/) (Center for Applied Rationality) workshops. Each skill turns Claude into a rationality coach that can help you **design**, **practice**, and **execute** evidence-based thinking techniques.

## What Are These?

"Skills" are add-ons that teach Claude new capabilities. Once you install one of these skills, Claude will know how to guide you through the corresponding CFAR rationality technique — like having a personal rationality coach available any time you need one.

Each skill supports three modes:

- **Design Mode** — Customize the technique for your specific situation
- **Practice Mode** — Build the skill on low-stakes examples before you need it for real
- **Execute Mode** — Apply the technique to a real problem you're currently facing

Just tell Claude which mode you want, or it will figure it out from context.

## The 12 Skills

| Skill | What It Does |
|-------|-------------|
| **Goal Factoring** | Decompose actions into underlying goals to find better strategies. Based on the "Parable of the Orange." |
| **Trigger-Action Planning** | Install reliable automatic behaviors by pairing sensory triggers with physical actions. Based on implementation intentions research (0.65 SD effect size). |
| **Double Crux** | Resolve disagreements by finding the key belief (crux) where changing it would change your conclusion. |
| **Internal Double Crux** | Resolve internal conflicts using parts-work. When part of you wants X and part wants Y, facilitate a conversation between them. |
| **Murphyjitsu** | Stress-test plans by simulating failures. Uses a "surprise-o-meter" loop to iterate until your plan survives scrutiny. |
| **Hamming Questions** | Ask "What's the most important problem in your field, and why aren't you working on it?" Systematically identify and unblock your highest-value work. |
| **Aversion Factoring** | Decompose aversions into component parts (like LEGO bricks) to find which specific sub-aversion is actually blocking you. |
| **Bucket Errors** | Detect when your brain is treating two separate questions as one, causing you to flinch away from evidence that only threatens one bucket. |
| **Focusing** | Access your body's "felt sense" about a situation using Gendlin's 6-step process, adapted for text-based facilitation. |
| **Resolve Cycles** | Break decision paralysis with 5-minute time-boxed problem-solving sprints. Two cycles: "Solve It" then "Plan It." |
| **Freedom of Action** | Expand your perceived action space by testing whether constraints are real or assumed. |
| **Pride / Self-Recognition** | Convert frustrations into recognized values. Discover what you care about by examining what bothers you. |

---

## How to Get the Files

First, you need to download this repository to your computer.

**Option 1: Download as a ZIP (easiest — no coding required)**

1. On the GitHub page for this repository, look for the green **"Code"** button near the top right
2. Click it, then click **"Download ZIP"**
3. Find the downloaded file (usually in your Downloads folder) and unzip it
4. You now have a folder called `CFAR-Claude-Skills` (or `CFAR-Claude-Skills-main`) with everything inside

**Option 2: Using the terminal** (if you're comfortable with that)

Open a terminal and run:

```
git clone https://github.com/YOUR_USERNAME/CFAR-Claude-Skills.git
```

---

## Installation

Pick the section below that matches how you use Claude.

### Claude.ai (Web) or Claude Desktop App

These two work the same way. You upload `.skill` files through Claude's settings.

**Step 1:** Open the `dist` folder inside the repository you downloaded. You'll see 12 `.skill` files — one for each technique.

**Step 2:** Open Claude:
- If you use **Claude in your browser**, go to [claude.ai](https://claude.ai)
- If you use the **Claude Desktop app**, open it

**Step 3:** Click your **profile icon** (bottom-left corner), then click **Settings**.

**Step 4:** Go to **Capabilities**, then find the **Skills** section.

**Step 5:** Click **"Upload skill"** and select the `.skill` file you want to install. For example, `trigger-action-planning.skill`.

**Step 6:** Repeat for each skill you want. You can install all 12 or just the ones you're interested in.

That's it! The skills are now active. They sync automatically between the web and desktop versions of Claude, so you only need to upload each skill once.

> **Tip:** Not sure which to start with? **Trigger-Action Planning** and **Murphyjitsu** are two of the most immediately practical techniques. **Goal Factoring** is great if you feel stuck on a decision.

---

### Claude Code (Terminal / CLI)

If you use Claude Code (the command-line version), skills are installed by placing folders in a specific location on your computer. No uploading needed.

**Step 1:** Open your terminal.

**Step 2:** Make sure the skills directory exists:

```
mkdir -p ~/.claude/skills
```

(This creates a hidden folder called `.claude` in your home directory, with a `skills` folder inside it. If it already exists, this command does nothing — safe to run either way.)

**Step 3:** Copy the skill folders into it. From inside the downloaded repository folder:

```
cp -r goal-factoring ~/.claude/skills/
cp -r trigger-action-planning ~/.claude/skills/
cp -r double-crux ~/.claude/skills/
cp -r internal-double-crux ~/.claude/skills/
cp -r murphyjitsu ~/.claude/skills/
cp -r hamming-questions ~/.claude/skills/
cp -r aversion-factoring ~/.claude/skills/
cp -r bucket-errors ~/.claude/skills/
cp -r focusing ~/.claude/skills/
cp -r resolve-cycles ~/.claude/skills/
cp -r freedom-of-action ~/.claude/skills/
cp -r pride-self-recognition ~/.claude/skills/
```

Or copy all 12 at once with this shortcut:

```
for skill in goal-factoring trigger-action-planning double-crux internal-double-crux murphyjitsu hamming-questions aversion-factoring bucket-errors focusing resolve-cycles freedom-of-action pride-self-recognition; do
  cp -r "$skill" ~/.claude/skills/
done
```

**Step 4:** Verify it worked by opening Claude Code and asking: *"What skills do you have available?"*

> **Note for advanced users:** You can also install skills for a single project by placing them in `your-project/.claude/skills/` instead of the global `~/.claude/skills/` directory. And if you'd like automatic updates when this repo changes, you can symlink the skill folders instead of copying them.

---

### Cowork Mode (Claude Desktop)

If you use Cowork mode in the Claude Desktop app:

1. Click **"Select folder"** and choose the downloaded `CFAR-Claude-Skills` folder
2. The skills are automatically available for that session

To make them available permanently (not just in Cowork mode), follow the Claude Desktop/Web instructions above and upload the `.skill` files from the `dist` folder.

---

## Using the Skills

Once installed, just talk to Claude naturally. The skills will activate based on what you're talking about:

- **"I keep procrastinating on writing my thesis"** — Claude may suggest Goal Factoring or Aversion Factoring
- **"I want to build a habit of reviewing my task list every morning"** — Trigger-Action Planning
- **"My cofounder and I disagree about whether to pivot"** — Double Crux
- **"Part of me wants to quit my job but part of me is scared"** — Internal Double Crux
- **"I'm launching a product next month — what could go wrong?"** — Murphyjitsu
- **"I feel stuck but I don't know why"** — Focusing or Hamming Questions
- **"I should go to the gym but I just... don't"** — Aversion Factoring
- **"Help me practice the resolve cycles technique"** — Practice Mode

You can also ask for a technique directly:

- *"Let's do a murphyjitsu on my travel plans"*
- *"Help me design a trigger-action plan for drinking more water"*
- *"I want to practice double crux — give me a scenario"*
- *"Can we do an internal double crux? I'm conflicted about taking this job offer."*

## What's in This Repository

```
CFAR-Claude-Skills/
├── README.md                        ← You are here
├── goal-factoring/
│   └── SKILL.md
├── trigger-action-planning/
│   └── SKILL.md
├── double-crux/
│   └── SKILL.md
├── internal-double-crux/
│   └── SKILL.md
├── murphyjitsu/
│   └── SKILL.md
├── hamming-questions/
│   └── SKILL.md
├── aversion-factoring/
│   └── SKILL.md
├── bucket-errors/
│   └── SKILL.md
├── focusing/
│   └── SKILL.md
├── resolve-cycles/
│   └── SKILL.md
├── freedom-of-action/
│   └── SKILL.md
├── pride-self-recognition/
│   └── SKILL.md
└── dist/                            ← Pre-packaged .skill files for easy upload
    ├── goal-factoring.skill
    ├── trigger-action-planning.skill
    ├── double-crux.skill
    ├── internal-double-crux.skill
    ├── murphyjitsu.skill
    ├── hamming-questions.skill
    ├── aversion-factoring.skill
    ├── bucket-errors.skill
    ├── focusing.skill
    ├── resolve-cycles.skill
    ├── freedom-of-action.skill
    └── pride-self-recognition.skill
```

Each skill folder contains a `SKILL.md` file — that's the instruction file that teaches Claude the technique. The `dist` folder contains pre-packaged versions of each skill for easy upload to the web or desktop app.

## Background

These skills are based on techniques from [CFAR](https://rationality.org/) (Center for Applied Rationality), an organization that runs workshops on applied rationality — practical tools for making better decisions, overcoming cognitive biases, and aligning your actions with your actual goals.

The techniques draw from cognitive behavioral therapy, implementation intentions research, Gendlin's Focusing, parts-work / Internal Family Systems, and the broader rationality community (LessWrong, Effective Altruism, etc.).

Each skill is designed to be maximally useful for people who care about becoming more rational — not just knowing about rationality techniques, but actually using them in daily life.

## License

These skills are open source. The underlying CFAR techniques are publicly documented across LessWrong, the CFAR website, and rationality community resources.
