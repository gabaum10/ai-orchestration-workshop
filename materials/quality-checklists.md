# Quality Checklists

Self-assessment guides for evaluating your persona output at each stage. Use these to catch issues early rather than discovering them at the end of your pipeline.

---

## Is my Challenger persona working?

**Does it identify SPECIFIC gaps, not generic feedback?**
- Good: "Budget covers initial rollout but ignores ongoing costs for tool licenses"
- Bad: "Consider cost factors more carefully"
- If no: Add examples to your Lens section: "Look for missing budget items like maintenance, licensing, support costs"

**Does it find things I didn't see on my own?**
- If every finding was something you already knew, the persona isn't adding value
- If no: Strengthen your Lens with specific blind spots: "Identify second-order consequences, unstated assumptions, missing stakeholder perspectives"

**Is it organized (by category, risk level, or theme)?**
- Findings should be grouped, not listed randomly
- If no: Add to Behavior: "Group findings by category (assumptions, risks, missing perspectives, resource gaps)"

**Does it explain WHY something is a problem, not just THAT it is?**
- Good: "Timeline has no contingency planning - if vendor delays by 2 weeks, launch date conflicts with Q4 freeze"
- Bad: "Timeline seems optimistic"
- If no: Add to Behavior: "For each risk, explain the mechanism - show specifically how things would go wrong"

**Does it ask questions I hadn't considered?**
- Critical questions should reveal gaps in your thinking
- If no: Add to Lens: "What questions will stakeholders ask that aren't addressed? What would need to be true for this to fail?"

---

## Is my Executor persona working?

**Does the output directly address the Challenger's findings?**
- Check: Can you trace each key Challenger point to something in the Executor's deliverable?
- If no: Add to Behavior: "You must address every finding from the review. For each point raised, show how you've resolved it"

**Is it appropriate for the intended audience?**
- Executive summary should be concise, action-oriented
- Technical implementation should include necessary detail
- If no: Add to your handoff: Specify audience explicitly ("for executive team" vs "for implementation team")

**Does it maintain the strengths of the original while fixing weaknesses?**
- The Executor should improve, not replace
- If no: Include the original document in your Executor handoff as reference

**Is it professional and polished, not generic?**
- Should read like a real business document, not AI boilerplate
- If no: Add to Behavior: "Write in professional business language. Be specific and concrete. Avoid generic phrases like 'leverage synergies' or 'drive value'"

**Does it flag anything it couldn't resolve rather than making things up?**
- Good: "Note: Cost estimate for ongoing support not provided in analysis"
- Bad: Invents numbers or makes up information
- If no: Add to Behavior: "If critical information is missing, include a [Note: ...] but still produce the deliverable"

---

## Is my handoff working?

**Does the Executor reference specific Challenger findings?**
- Check the Executor's output: Are Challenger points explicitly addressed?
- If no: Improve your handoff template - include the full Challenger output, not just a summary

**Is the output substantially different from what a single prompt would produce?**
- If the final deliverable looks like what you'd get from "write me a proposal," the pipeline isn't adding value
- If no: Your Challenger probably isn't finding real issues. Go back and strengthen that persona first

**Did the Executor miss any of the Challenger's key points?**
- Compare deliverable against Challenger findings line by line
- If yes: Add to Executor Behavior: "Create a checklist of Challenger findings. Confirm each is addressed before finalizing deliverable"

---

## Is my persona definition strong?

**Is the Role specific (job title + domain), not vague?**
- Good: "Strategic advisor who stress-tests business proposals"
- Bad: "You are a helpful assistant"
- If no: Rewrite Role section with a job title and clear domain of expertise

**Does the Lens describe a clear perspective or filter?**
- Should tell the persona what to look for or prioritize
- If no: Add a bullet list: "Look for: X, Y, Z"

**Does the Behavior section define output format and communication style?**
- Should answer: How do you structure your response? What tone do you use?
- If no: Add specific formatting instructions: "Organize findings as: 1) Critical risks, 2) Important gaps, 3) Questions"

**Do the Constraints set clear boundaries on what the persona does NOT do?**
- Good: "Do NOT rewrite proposals or provide solutions"
- Vague: "Stay focused on your role"
- If no: Add explicit "Do NOT..." statements for common drift patterns
