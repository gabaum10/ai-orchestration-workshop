# Validation Brief: AI Orchestration Workshop

**For:** AI-fluent reviewer (comfortable with Claude, understands Projects)
**Purpose:** Strategic validation of curriculum approach before broader deployment
**Repo:** https://github.com/gabaum10/ai-orchestration-workshop

## What We're Building

A Level Two prompt engineering workshop for business professionals. The audience has completed basic prompt engineering training - they can write decent prompts, understand temperature/tokens at a conceptual level, and use Claude effectively for single-shot tasks. They've never built custom Claude Projects, designed persona systems, or thought about chaining AI interactions into workflows.

The core concept: Teach people to create specialized AI personas using Claude Projects and orchestrate them into a processing pipeline. Instead of "ask Claude to do everything," we're teaching "design specialized experts and chain them."

## The Workshop Structure

**Show, then build.** Participants first see pre-built personas working together on a realistic business document (a project proposal with hidden gaps). Then we teach the underlying framework (Role/Lens/Behavior/Constraints), then they build their own personas and run their own documents through the pipeline.

Three 90-minute sessions:
1. Introduction + demo of the two-persona pipeline
2. Framework deep-dive + building the Challenger
3. Building the Executor + running the full pipeline

## The Two-Persona Pipeline

**The Challenger** - A Claude Project configured as a strategic advisor. Stress-tests documents by finding blind spots, unstated assumptions, missing stakeholder considerations, feasibility concerns. Produces a structured analysis with findings categorized by impact and confidence level.

**The Executor** - A separate Claude Project configured as an implementation specialist. Takes the Challenger's analysis + the original document and produces an improved version. Maintains the original author's voice and intent while addressing the identified gaps.

**The handoff:** Manual copy-paste. User submits document to the Challenger, receives analysis, copies that analysis + original document into the Executor's conversation with a handoff prompt. The Executor produces the improved version.

Both personas are defined through Claude Project custom instructions (~500 words each). We're keeping Projects focused - one persona per Project, not trying to make a single Project handle both modes.

## What We Need You to Validate

These are open questions. We want your experience and judgment, not just "yes it works."

### 1. Does the Project-per-persona model hold up?

We're instructing participants to create a separate Claude Project for each persona. This felt cleaner than switching modes within a single Project ("now be the Challenger, now be the Executor"). But is this actually the best approach for non-technical users?

**Alternative we considered:** Single Project with explicit mode-switching prompts. We rejected it because we thought context bleed between personas would confuse the model and the user. But maybe we're overengineering?

**What we'd like to know:** In your experience, is the separate-Projects model the right call? Or is there a simpler pattern we're missing? How do you handle persona separation when you need distinct behaviors from Claude?

### 2. How smooth is the handoff in practice?

The pipeline depends on copying output from one Project conversation and pasting it into another. On paper this seems simple. In practice, what's the actual experience like?

**What we'd like to know:** Are there friction points we should warn participants about? Does Claude handle "here's an analysis from another conversation" prompts reliably? Is there a better way to move output between Projects that we're not leveraging?

### 3. Do personas stay consistent?

When you write detailed custom instructions for a Claude Project (~500 words defining role, lens, behavior, constraints), does Claude actually maintain that persona consistently across a conversation? Or does it drift back to default assistant mode after a few exchanges?

**What we'd like to know:** From your experience with custom Projects, are there instruction-writing patterns that improve consistency? Things to avoid? Is there a length/complexity threshold where instructions stop being effective?

### 4. Artifact behavior

We're considering instructing personas to produce their output as Artifacts (the Challenger's analysis as an Artifact, the Executor's revised document as an Artifact). The goal is cleaner handoffs - copy the Artifact content rather than extracting it from conversational output.

**What we'd like to know:** Is this reliable? Does Claude consistently create Artifacts when instructed to in Project custom instructions, or is it hit-or-miss? Does it depend on output type/length? Is the added instruction complexity worth it for this audience, or should we just teach them to copy text from responses?

### 5. What tier do participants actually need?

We're planning to recommend Claude Pro ($20/mo). Is that sufficient for everything we're teaching? Specifically:

- Creating multiple Projects (Challenger + Executor minimum, possibly more for experimentation)
- Extended conversations within Projects (iterating on persona definitions, refining outputs)
- Processing multi-page documents through the pipeline

Are there features we're using that require a higher tier? Could parts of this work on the free tier if budget is a constraint for some organizations?

### 6. What would you do differently?

Open-ended. Given the goal - teach non-technical business professionals to think in specialized AI personas and chain them into workflows - is there anything about our approach you'd change?

- Claude features we're not leveraging that we should be?
- Gotchas from your experience that we haven't accounted for?
- Simpler patterns that achieve the same outcome?
- Concepts that are harder to teach than we think?

We're particularly interested in gaps between "how we think this will work" and "how it actually works when you hand it to someone." We've built and tested this internally, but we're too close to it.

## What Success Looks Like

A participant leaves the workshop able to:
1. Articulate when to use specialized personas vs. general prompting
2. Design a persona using the Role/Lens/Behavior/Constraints framework
3. Implement that persona as a Claude Project with custom instructions
4. Chain multiple personas into a processing pipeline
5. Apply this pattern to their own business documents and workflows

The workshop isn't about teaching Claude's features comprehensively. It's about teaching a specific pattern - persona specialization and orchestration - that unlocks more sophisticated use cases than they could achieve with single-shot prompting.

## Testing the Validation

If you have 30-60 minutes and want to actually try the approach:

1. Look at `materials/sample-docs/proposal.md` (the realistic but flawed proposal we demo with)
2. Try the Challenger persona on it (custom instructions in `materials/personas/challenger.md`)
3. Try the Executor handoff (custom instructions in `materials/personas/executor.md`)

Not required - we'll value your strategic input regardless. But if you want to see the actual experience, that's the path.

## Timeline

We're aiming to pilot this workshop in March. Validation feedback by end of February would be ideal, but we'll take insights whenever you have them. Even a quick "here's what jumped out at me" response is valuable.

Thanks for lending your expertise. We want to get this right before we teach it to people.
