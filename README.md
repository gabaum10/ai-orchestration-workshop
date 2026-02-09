# AI Orchestration Workshop

A practical, hands-on workshop teaching multi-persona AI orchestration for complex business deliverables. Learn to coordinate specialized AI agents to produce executive-ready work faster and with higher quality.

## Overview

This ~2.5-3 hour workshop teaches you how to break down complex work into specialized roles, coordinate handoffs between AI agents, and maintain quality across a multi-agent pipeline. You'll learn by seeing the approach demonstrated first, then building your own orchestrated workflow.

**Core Approach:** Show then build. We demonstrate a complete two-persona pipeline on a real document, then guide you in building your own with your actual work materials.

## What You'll Learn

- **Pipeline thinking:** How to decompose complex deliverables into specialized roles
- **Persona design:** Creating focused AI agents with clear responsibilities and constraints
- **Handoff protocols:** Structured coordination between agents to prevent quality drift
- **Quality gates:** Checkpoints that ensure rigor at each stage
- **Iteration patterns:** When to refine within a stage vs. when to escalate back

## Workshop Structure

### Part 1: Demonstration (45-60 min)
**The Challenger-Executor Pipeline**

We demonstrate a complete two-persona workflow:

1. **Challenger Persona** - Stress-tests the brief
   - Pokes holes in assumptions
   - Surfaces hidden constraints
   - Forces clarity on success criteria

2. **Executor Persona** - Delivers the artifact
   - Receives refined brief from Challenger
   - Produces publication-ready deliverable
   - Adheres to quality standards

**Live demo:** Watch a real business proposal go through the pipeline, see handoffs in action, observe quality gates working.

### Part 2: Guided Build (60-75 min)
**Build Your Own Pipeline**

You construct a two-persona workflow for your actual work:

1. **Choose your deliverable** (bring your own document/brief, or use provided scenario)
2. **Design your Challenger** (what assumptions need stress-testing?)
3. **Design your Executor** (what does publication-ready mean for your context?)
4. **Define handoff protocol** (what must Challenger deliver to Executor?)
5. **Set quality gates** (what checks prevent garbage output?)
6. **Run the pipeline** (execute on your real work)
7. **Iterate and refine** (debug handoffs, tune constraints)

### Part 3: Debrief & Next Steps (15-30 min)

- Review what worked and what didn't
- Discuss extension patterns (adding a third persona, parallel branches)
- Explore post-workshop support options

## Directory Structure

```
ai-orchestration-workshop/
├── README.md                           # This file
├── curriculum/
│   └── session-outline.md             # Detailed session plan with timing
├── exercises/
│   └── business-proposal-scenario.md  # Optional scenario if participants don't bring work
├── templates/
│   ├── handoff-templates.md           # Minimal viable handoff structure
│   └── persona-framework.md           # Template for designing personas
├── materials/
│   ├── quality-checklists.md          # Verification checklists for common deliverables
│   └── troubleshooting-guide.md       # Common failure modes and fixes
└── personas/
    ├── challenger-persona.md          # Reference Challenger implementation
    ├── executor-persona.md            # Reference Executor implementation
    └── qa-persona.md                  # Optional third persona for quality assurance
```

## Prerequisites

**Required:**
- Access to Claude (API or web interface)
- A document or brief you want to improve (business proposal, technical spec, research report, etc.)
- Willingness to iterate and debug

**Helpful but not required:**
- Experience with prompt engineering
- Familiarity with your domain's quality standards

## Bringing Your Own Work

**Strongly encouraged.** The workshop is designed for you to apply the framework to real work. Bring:

- A draft document that needs refinement
- A brief for something you need to create
- A complex deliverable you're currently working on

**If you don't have something ready:** Use the provided business proposal scenario in `exercises/business-proposal-scenario.md`.

## Post-Workshop Support

- **Office hours:** Monthly drop-in sessions for troubleshooting and iteration
- **Community forum:** Share persona designs, discuss failure modes, get feedback
- **Extended patterns:** Documentation for three-persona pipelines, parallel branches, conditional routing

## Getting Started

1. **Review the session outline:** `curriculum/session-outline.md` - understand the flow
2. **Explore the reference personas:** `personas/` directory - see working examples
3. **Read the handoff template:** `templates/handoff-templates.md` - understand coordination structure
4. **Prepare your document:** Bring something real, or use `exercises/business-proposal-scenario.md`

## Facilitator Notes

If you're running this workshop:

- **Emphasize show-then-build:** The demo in Part 1 is critical. Participants need to see the full workflow before building their own.
- **Encourage real work:** Generic scenarios teach less than actual documents participants care about.
- **Expect iteration:** First pipelines rarely work perfectly. Budget time for debugging handoffs and refining personas.
- **Quality gates matter:** The checkpoints are what prevent AI slop. Don't skip them.

## Key Insights

**From the curriculum:**

- **Two personas can be enough.** Start simple. Add complexity only when needed.
- **Handoffs are where quality breaks.** Explicit structure prevents drift.
- **Constraints are features.** Tight persona boundaries prevent scope creep and maintain focus.
- **Show the mess.** Real workflows have dead ends and revisions. Demonstrate iteration, not just success.

## Credits

Developed by Geoff Baum (gabaum10) based on practical experience orchestrating AI agents for complex business deliverables.

## License

MIT License - use freely, adapt for your context, share improvements.

---

**Questions or feedback?** Open an issue or reach out via GitHub.
