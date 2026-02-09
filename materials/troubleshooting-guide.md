# Troubleshooting Guide

When your pipeline isn't producing useful output, use this guide to diagnose and fix the problem. Work backward from symptoms to root causes.

---

## Symptom: "My Challenger just says everything looks good"

**Diagnosis:** Role/Lens too vague, or Constraints too permissive

**Fix:**
1. Strengthen the Lens with specific things to look for:
   - "Identify unstated assumptions, missing stakeholder perspectives, second-order consequences"
   - Add domain-specific categories: "For business proposals, examine budget assumptions, timeline feasibility, market risks"

2. Add to Behavior:
   - "You should always find at least 3 areas for improvement - even strong proposals have blind spots"
   - "Rate every finding by severity (high/medium/low) and explain why it matters"

3. Check your input: If you're giving the Challenger a 2-sentence sketch, there's nothing to analyze. Feed it complete drafts.

---

## Symptom: "My Challenger is too harsh / tears everything apart"

**Diagnosis:** Lens too aggressive, missing the "constructive" aspect

**Fix:**
1. Add to Behavior:
   - "Rate issues by severity. Not everything is a critical risk."
   - "Acknowledge what's working before identifying gaps"
   - "End with 'The strongest version of this idea would...' - show the path forward"

2. Adjust Lens language:
   - Replace: "Find everything wrong with this"
   - With: "Identify gaps, risks, and unstated assumptions that would strengthen this proposal"

---

## Symptom: "My Executor just rewrites the original without using the Challenger's input"

**Diagnosis:** Handoff is weak - Executor didn't receive or prioritize the Challenger's findings

**Fix:**
1. Improve your handoff:
   - Include the full Challenger output, not just "here's what the reviewer said"
   - Be explicit: "Your job is to address these findings while maintaining the proposal's strengths"

2. Add to Executor Behavior:
   - "You must address every finding from the review. Create a mental checklist and confirm each point is resolved."

3. Check if you included the original document: The Executor needs both the Challenger's findings AND the original to produce a revision.

---

## Symptom: "The pipeline output isn't better than my single prompt"

**Diagnosis:** Work backward through the chain

**Step 1:** Check the Executor's deliverable
- Does it address specific issues?
- If not → Check what the Challenger provided

**Step 2:** Check the Challenger's findings
- Are they specific ("Budget omits ongoing license costs") or generic ("Consider costs more carefully")?
- If generic → Your Challenger persona is too weak

**Step 3:** Fix from the top
- Strengthen the Challenger's Lens and Behavior first
- Re-run the pipeline with improved Challenger output
- If Challenger findings are strong but Executor ignores them → Strengthen the handoff

**Common root cause:** The Challenger wasn't specific enough. A vague challenge produces a vague revision.

---

## Symptom: "My persona keeps breaking character / going off-script"

**Diagnosis:** Constraints section is too loose

**Fix:**
1. Add explicit "Do NOT..." statements:
   - For Challenger: "Do NOT rewrite proposals or provide solutions"
   - For Executor: "Do NOT second-guess the strategy or introduce new analysis"

2. Be specific about boundaries:
   - Instead of: "Stay in your lane"
   - Write: "Your role ends at identifying gaps. Do not move into execution planning or implementation details."

3. Check your handoff prompt:
   - If you're asking the persona to do multiple jobs ("review this AND rewrite it"), you're creating role confusion
   - Break into separate handoffs: Challenger reviews, Executor rewrites

---

## Symptom: "The handoff is awkward / I don't know what to paste"

**Diagnosis:** Unclear on what the next persona needs

**Fix:**
1. Use the minimal viable handoff template:
   ```
   Here's my original [document]: [paste]
   Here's what my reviewer found: [paste Challenger output]
   Please produce a revised version that addresses these findings.
   ```

2. For each persona transition, ask: "What does this persona need to do their job?"
   - Challenger needs: The original document
   - Executor needs: The original document + Challenger's findings

3. Start simple, add detail if needed:
   - First try: Minimal handoff (3 sentences)
   - If output is weak: Add constraints (audience, length, format)
   - If still weak: Add specific instructions (must include X, Y, Z)

---

## Symptom: "My personas produce long, rambling output"

**Diagnosis:** Behavior section doesn't constrain output format

**Fix:**
1. Add structure requirements to Behavior:
   - "Organize findings into 3 categories: Critical risks, Important gaps, Questions"
   - "Limit your analysis to 10 key findings maximum"

2. Add format constraints:
   - "Use bullet points, not paragraphs"
   - "Each finding: one sentence description + one sentence explanation"

---

## Symptom: "I don't know if my output is good enough"

**Diagnosis:** Missing success criteria

**Fix:**
1. Before running the pipeline, define done:
   - What does "good Challenger output" look like for this task?
   - What does the final deliverable need to include?

2. Use the quality checklists (see quality-checklists.md)

3. Test with a simple case first:
   - Don't start with your most complex proposal
   - Build the pipeline with a straightforward example
   - Once the personas work reliably, tackle the hard stuff

---

## General Debugging Strategy

**When something isn't working:**

1. Isolate the problem:
   - Is it the Challenger? (Findings are weak/generic)
   - Is it the Executor? (Deliverable ignores findings)
   - Is it the handoff? (Information lost between steps)

2. Fix from the top down:
   - If Challenger is weak, fix that before blaming the Executor
   - If handoff is unclear, improve that before tweaking personas

3. Test incrementally:
   - Don't change 5 things at once
   - Adjust one section (Lens or Behavior), re-run, evaluate
   - Iterate until the output improves

4. Use examples:
   - Your personas learn from examples better than from abstract instructions
   - Add a good example to your Behavior section: "Example of a strong finding: ..."
