# Handoff Templates

Copy these templates to move work between personas in your pipeline. Start with the minimal version and add detail only if needed.

---

## Core Pipeline: Challenger → Executor

### Minimal Viable Handoff

Use this for most cases. It works.

```
Here's my original [document type]: [paste original]

Here's what my strategic reviewer found: [paste Challenger output]

Please produce a revised version that addresses these findings while maintaining the document's strengths.
```

That's it. Three sentences, three paste operations, done.

### Full Version (with context and constraints)

When you need more control over the output, use this version with explicit instructions.

```
I need you to act as an Executor. I've reviewed a business proposal using a strategic advisor lens, and now I need a revised version that addresses the identified gaps.

ORIGINAL DOCUMENT:
[Paste your original proposal/plan/document here]

CHALLENGER FINDINGS:
[Paste the complete Challenger output here - all gaps, risks, assumptions, and questions]

DELIVERABLE REQUESTED:
[Be specific: revised proposal, risk mitigation plan, executive summary, etc.]

CONSTRAINTS:
- Audience: [Who will read this?]
- Length: [How long should it be?]
- Required elements: [What must be included?]
- Format: [Any specific format requirements?]

Focus on addressing the identified issues while preserving what's working in the original.
```

### Filled Example: AI Training Program Proposal

**Context:** You've drafted a proposal for an enterprise AI training program. The Challenger found gaps in data security, change management, and success metrics. You need a revised proposal.

**Minimal version:**

```
Here's my original proposal: [paste AI training program proposal]

Here's what my strategic reviewer found:

The proposal assumes universal employee interest without addressing resistance or skepticism. Success metrics are vague with no baseline measurements. Data security and privacy concerns are completely unaddressed. Timeline has no contingency planning. Budget covers initial rollout but ignores ongoing costs. No change management strategy for cultural resistance. Missing stakeholder analysis. No plan for measuring actual productivity impact. Treats AI literacy as uniform when different roles need different skills.

Please produce a revised version that addresses these findings while maintaining the document's strengths.
```

**Full version with constraints:**

```
I need you to act as an Executor. I've reviewed my AI training program proposal using a strategic advisor lens, and now I need a revised version that addresses the identified gaps.

ORIGINAL DOCUMENT:
[Paste your 6-month rollout, $185K budget proposal here]

CHALLENGER FINDINGS:
The proposal assumes universal employee interest without addressing resistance or skepticism. Success metrics are vague ("increase productivity") with no baseline or target numbers. Data security and privacy concerns are completely unaddressed - this is critical when employees are using AI tools with company data. Timeline is optimistic with no contingency planning for delays. Budget covers initial rollout but ignores ongoing costs for tool licenses, content updates, and support. No mention of change management strategy or how to handle cultural resistance. Missing stakeholder analysis - who champions this internally? Who might resist or undermine it? No plan for measuring actual productivity impact beyond self-reported time savings. The proposal treats "AI literacy" as uniform across roles when different departments need very different skills. No discussion of what happens to employees who don't adopt AI tools.

DELIVERABLE REQUESTED:
A revised business proposal that addresses these gaps and is ready to present to executive leadership.

CONSTRAINTS:
- Audience: Executive team (CEO, CFO, CHRO)
- Length: 3-4 pages maximum
- Required elements: Executive summary, revised success metrics with baselines, data governance section, change management plan, stakeholder analysis, budget breakdown including ongoing costs
- Format: Professional business proposal format

Focus on addressing the identified issues while preserving what's working in the original.
```

---

## Tips for Effective Handoffs

**Start minimal, add detail if needed**
Try the 3-sentence version first. If the output isn't what you want, add constraints and try again.

**Be specific about deliverables**
- Vague: "Make this better"
- Specific: "Create a 2-page risk mitigation addendum addressing data security and change management"

**Include all the context**
Don't summarize the Challenger's output. Paste it completely. The Executor needs the full picture.

**Iterate when needed**
If the first output isn't quite right, give specific feedback: "This addresses the data security gap well, but the change management section is too generic. Add specific tactics for handling resistance."

**Preserve the chain**
Save each persona's output. You may need to reference the Challenger's findings when evaluating the Executor's deliverable.

---

## Advanced: Three-Persona Pipeline (Optional)

When your pipeline needs a middle step to organize findings before execution, add the Structurer persona between Challenger and Executor.

**Use case:** Complex projects where the Challenger identifies 15+ findings across multiple categories and you need them organized before producing a deliverable.

### Template: Challenger → Structurer Handoff

```
I need you to act as a Structurer. I've completed a Challenger analysis and need the findings organized into a coherent framework.

ORIGINAL DOCUMENT:
[Brief description - 1-2 sentences]

CHALLENGER FINDINGS:
[Paste all Challenger output]

YOUR TASK:
Organize these findings into:
- Critical risks (must address before moving forward)
- Important gaps (need clarity or resolution)
- Questions for stakeholders
- Assumptions that need validation

Make this actionable for someone who needs to revise the proposal or create an implementation plan.
```

### Template: Structurer → Executor Handoff

```
I need you to act as an Executor. I have structured findings from a proposal analysis, and I need you to produce a specific deliverable.

CONTEXT:
[1-2 sentence description of original proposal]

STRUCTURED ANALYSIS:
[Paste the Structurer's organized framework - all categories and findings]

DELIVERABLE REQUESTED:
[Specify exactly what you want: revised proposal, risk mitigation plan, implementation roadmap, etc.]

CONSTRAINTS:
- Length: [specify]
- Audience: [specify]
- Required elements: [specify]

Focus on producing a concrete, actionable document ready to use immediately.
```

### When to Use Three Personas vs. Two

**Use two (Challenger → Executor) when:**
- The Challenger finds 10 or fewer key issues
- Findings naturally fall into clear categories
- You want fast turnaround
- The proposal isn't highly complex

**Use three (Challenger → Structurer → Executor) when:**
- The Challenger identifies 15+ findings
- Findings span multiple domains (technical, financial, organizational, market)
- You need prioritization before execution
- Multiple stakeholders need different views of the same analysis

Start with two. Add the Structurer only when you need it.
