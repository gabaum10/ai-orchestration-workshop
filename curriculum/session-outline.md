# AI Orchestration Workshop - Facilitator Guide

**Duration:** 2.5-3 hours
**Target Audience:** Business professionals who completed Level One prompt engineering
**Prerequisites:** Claude Pro account ($20/mo minimum), basic prompting skills
**Platform:** Claude web platform (claude.ai) only

**What participants will build:** Two specialized AI personas that work in a pipeline to transform their own business documents

## Before the Workshop

**Send participants this email 3-5 days in advance:**

Subject: Workshop Prep - Bring Your Own Work

Hi [name],

Looking forward to the AI Orchestration workshop on [date]. To make this immediately valuable, please bring a document you're currently working on - something you'd genuinely like to improve:

- A proposal or pitch deck
- A strategy document or plan
- An important email or communication
- A project brief or requirements doc

The document should be something you care about getting right, ideally 2-5 pages. If you don't have something handy, no problem - we'll provide a sample business proposal.

Also, please confirm before the workshop:
- You have Claude Pro access (required for Projects feature)
- You can log into claude.ai from the workshop location

See you soon,
[Your name]

**Pre-session checklist:**
- [ ] Framework template handout (Role/Lens/Behavior/Constraints)
- [ ] Handoff template handout
- [ ] Sample business proposal (backup for those without their own document)
- [ ] Persona library starter document (reference personas for after-workshop use)
- [ ] Pre-built Challenger and Executor personas loaded and ready to demo
- [ ] Test the demo pipeline on sample document (verify output quality)

## Materials Checklist

For each participant:
- Framework template (printed or digital)
- Handoff template (printed or digital)
- Persona library starter document
- Sample business proposal (as backup)

For facilitator:
- Pre-built Challenger persona (from `/personas/challenger.md`)
- Pre-built Executor persona (from `/personas/executor.md`)
- Claude Pro account with demo document ready

## Block 1: The Hook (30 min)

### Warmup Exercise: Two Attempts (10 min)

**Facilitator Script:**
"We're starting with what you already know. Open Claude - standard chat, not a Project yet. You're going to review the document you brought. If you didn't bring one, use the sample I've provided."

**First attempt (3 minutes):**
"Write a prompt asking Claude to review your document. Keep it straightforward. You have 3 minutes to write and run it."

**What to say while they work:**
"Use your Level One skills - be clear about what you want, give Claude context. This is your baseline."

**At 3 minutes:**
"Save that output somewhere. Now do it again."

**Second attempt (4 minutes):**
"Same document, but this time use what you know about good prompting. Be more specific. Add constraints. Define your audience. Make it better. You have 4 minutes."

**At 7 minutes:**
"Time's up. Compare your two outputs. Pick the better one and save it. That's your benchmark for today."

**Debrief (2 minutes):**
"Quick show of hands - who got noticeably better output on the second try?"

Most hands will go up.

"Good. Level One skills matter. Now let me show you why even your best single prompt isn't enough for high-stakes work."

**What success looks like:**
Participants have a "best single-prompt output" saved. They've experienced that prompting skill makes a difference, but they're primed to see its limits.

**Common pitfall:**
People spending too long crafting the perfect prompt. At 3 and 7 minutes, call time firmly. "Good enough - we're moving on."

### The Problem: Why One Conversation Isn't Enough (10 min)

**Facilitator Script:**
"Here's what you just experienced: you asked Claude to review your document. What did you get back? Probably balanced feedback - some concerns, some suggestions, some encouragement. Nothing wrong with that. But there's a problem."

**Live Demo Setup:**
Share your screen. Pull up two Claude chat windows side by side.

**Window 1:**
"Review this business proposal. Be thorough and critical. Find weak points, unstated assumptions, and risks."

**Window 2:**
"Review this business proposal. Focus on helping me strengthen and polish it. Build on what's working."

Use the same sample document for both. Let them run.

**While results load:**
"Watch what happens. Same document. Same AI. Different cognitive modes."

**When results appear:**
"Look at the difference. Window 1 found problems. Window 2 built solutions. These are contradictory mental states. Can one conversation do both of these things simultaneously?"

Pause.

"The answer is no. Not effectively. When you ask for 'balanced' feedback, you get mushy middle ground. When you specialize, you get sharp, focused output. An AI can't be adversarial AND constructive at the same time any more than you can."

**What to emphasize:**
"This is why we orchestrate. We don't ask one AI to do everything. We create specialists. We run them in sequence. Each one does its job, then hands off to the next. Today you're going to build that pipeline."

**Time warning at 8 minutes:**
Wrap the comparison, transition.

**What success looks like:**
Participants see the visible difference between specialized and generalist prompting. They understand why one conversation hits a ceiling.

**Common question:**
"Why not just make a really long, detailed single prompt that covers everything?"

**Answer:** "Try it. You'll get shallow coverage across everything instead of depth in anything. The cognitive load is too high for one conversation to maintain. We're about to prove that."

### The Solution Preview: See the Pipeline Work (10 min)

**Facilitator Script:**
"Before I teach you how to build this, let me show you what you're building toward. Watch this."

**Demo the pre-built pipeline:**

1. **Open your pre-built Challenger Project**
   - "This is a persona I built called The Challenger. It stress-tests ideas. Watch what it does."
   - Paste the sample business proposal into the chat
   - Let it run, show the output briefly (don't read line by line)
   - "Look at those questions. Look at those risk assessments. Specific, focused, adversarial."

2. **Open your pre-built Executor Project**
   - "This is The Executor. It takes critical feedback and produces improved output."
   - Use the handoff template to brief The Executor
   - Context: "This is a business proposal that was reviewed by a critical analyst."
   - Previous step output: [paste Challenger's output]
   - Task: "Revise the original proposal to address these concerns. Produce a strengthened version."
   - Let it run, show the output

3. **Compare side-by-side**
   - Pull up the original proposal, the Challenger output, and the Executor output
   - "Original proposal. Critical analysis. Revised proposal. That's the pipeline."

**What to emphasize:**
"You just saw two specialists do their jobs. The Challenger found problems. The Executor fixed them. Neither one tried to do both. That's orchestration."

**Pause for effect.**

"Now here's the question: how much better is the final output than the original?"

Let them answer. The improvement should be visible.

"By the end of today, you'll have built this pipeline yourself. And you'll have run YOUR document through it. Not mine. Yours."

**Time warning at 9 minutes:**
Transition to Block 2.

**What success looks like:**
Participants have seen a working pipeline produce tangibly better output. They understand the destination before they start navigating.

**Common reaction:**
"That's not that complicated."

**Response:** "It's not. That's the point. Two specialized prompts beat one generalist prompt every time. The trick is knowing HOW to specialize. That's what we're learning next."

## Block 2: Understanding Personas (25 min)

### Framework Introduction (10 min)

**Facilitator Script:**
"You just saw The Challenger and The Executor work. Now let's look under the hood. What makes a persona different from a regular prompt?"

**Distribute the framework template handout.**

"There are four components. Just four. Let's break them down."

**Walk through each element:**

1. **Role:** "Who is this AI? What's their identity? 'You are a critical analyst' produces different output than 'You are a supportive editor.' Role primes the cognitive mode."

2. **Lens:** "What perspective do they bring? What do they look for? The Challenger looks for risks and gaps. The Executor looks for clarity and completeness. Lens determines what the persona notices."

3. **Behavior:** "How do they work? Do they ask questions first? Do they use a framework? Do they prioritize findings? This defines the workflow."

4. **Constraints:** "What are the rules? What should they NOT do? The Challenger doesn't suggest solutions. The Executor doesn't second-guess the strategy. Constraints prevent scope creep."

**What to emphasize:**
"You've been doing some of this in your Level One prompts - defining what you want, setting constraints. We're making it explicit and repeatable. When you put these four components into a Claude Project's custom instructions, you get a specialist."

**Visual aid (if using slides):**
Show the framework as a 2x2 grid:
```
ROLE          LENS
Who are they? What do they see?

BEHAVIOR      CONSTRAINTS
How do they work? What don't they do?
```

**Time warning at 8 minutes:**
Transition to deconstruction.

**What success looks like:**
Participants understand the four-part structure and have the template in hand.

**Common confusion:**
Role vs. Lens. Clarify: "Role is identity. Lens is perspective. 'Critical analyst' is a role. 'Looking for unstated assumptions' is a lens."

### Deconstruct the Demo (15 min)

**Facilitator Script:**
"You saw The Challenger work. Now let's see WHY it worked. I'm going to show you the custom instructions that define that persona."

**Pull up your pre-built Challenger Project, show the custom instructions on screen.**

**Walk through section by section:**

**Role section:**
"'You are a strategic advisor who stress-tests ideas.' That's the identity. Not 'helpful assistant.' Not 'reviewer.' Strategic advisor. Adversarial role."

**Lens section:**
"Look at what it's told to look for: unstated assumptions, missing stakeholders, second-order consequences, blind spots. That's the filter. When you give the persona a specific lens, it notices things a generalist wouldn't."

**Behavior section:**
"'Start by asking probing questions.' 'Rate risks as high, medium, low.' 'End with the strongest version of this idea would...' Those are workflow rules. They structure the output."

**Constraints section:**
"'Do NOT rewrite proposals.' 'Do NOT provide implementation details.' This keeps the persona in its lane. Without constraints, it would drift into solving problems instead of identifying them."

**Ask:**
"Why does this matter? Why not just tell Claude 'be critical'?"

Let them answer. Guide toward: specificity produces depth, constraints prevent drift, structure produces consistency.

**Now do the same with The Executor:**

**Pull up the pre-built Executor Project, show custom instructions.**

**Role:** "Implementation specialist. Not analyst. Not critic. Builder."

**Lens:** "Clarity, completeness, audience fit, actionability. Different filter than The Challenger."

**Behavior:** "Follow the structure provided. Produce complete deliverables. Use clear formatting."

**Constraints:** "Do NOT second-guess the strategy. Do NOT introduce new analysis. Work within the framework given."

**What to emphasize:**
"Same four components. Different specialization. The Executor doesn't question the plan - it executes. The Challenger doesn't build solutions - it finds problems. Two specialists, two jobs."

**Ask:**
"What would happen if you collapsed these into one persona? Told it to 'find problems AND fix them' in one conversation?"

Let them answer. Guide toward: cognitive overload, shallow coverage, mushy output.

**Time warning at 13 minutes:**
Wrap up, announce break.

**Transition to break:**
"After break, you're building your own Challenger. Then your own Executor. Then you're running YOUR document through the pipeline. Questions before we break?"

**What success looks like:**
Participants understand the anatomy of a persona. They've seen the custom instructions that produced the demo output. The framework makes intuitive sense now.

**Common question:**
"How long should custom instructions be?"

**Answer:** "As long as they need to be. The demo personas are about 200 words each. You can go longer if you need to. Shorter is better if it's clear."

## BREAK (10 min)

**During break:**
- Check in with anyone who looks confused or lost
- Be available for account issues (people who can't access Projects)
- Review your demo personas - you may need to reference them again

## Block 3: Build Your Own (50 min)

### Setup and Context (5 min)

**Facilitator Script:**
"Welcome back. Here's what we're doing in this block: you're building two personas - your own Challenger and your own Executor. Then you're running your document through them."

"Open Claude and create a new Project. Name it something like 'My Challenger' or 'Critical Analyst' - whatever makes sense to you. Pull up your document and the framework template."

**While they set up:**
"If you brought your own document, great - that's what you'll use. If you're using the sample, that's fine too. Either way, you need a document ready to test."

**Time warning at 3 minutes:**
"One more minute, then we start building."

**What success looks like:**
Everyone has a Project open, a document ready, and the framework template visible.

### Build Your Challenger (25 min)

**Facilitator Script:**
"Start with The Challenger - the persona that stress-tests your document. Open your Project's custom instructions and write them using the framework template as your guide."

"Define all four components: Role, Lens, Behavior, Constraints. Remember: this persona finds problems. It doesn't solve them."

**Circulate actively. This is where people need help.**

**Common issues you'll see:**

**Issue 1: Too vague**
Example: "You are helpful and give feedback."
Fix: "That's too generic. What KIND of feedback? From what perspective? Use the Lens section to get specific."

**Issue 2: Scope too broad**
Example: "You review everything - logic, grammar, tone, structure, risks, and financials."
Fix: "Pick one domain. That's why you're building two personas. Let this one own critical analysis. The Executor will handle the rest."

**Issue 3: Missing behavior rules**
Example: "You are a critical analyst."
Fix: "How do you analyze? Do you ask questions? Make statements? Organize by severity? Define the workflow."

**Issue 4: No constraints**
Example: "You help improve proposals."
Fix: "What should you NOT do? Constraints keep the persona from drifting. Try: 'You do not suggest solutions. You only identify what needs to change.'"

**Issue 5: Copying the demo verbatim**
Example: Someone has copied the exact Challenger instructions from your demo.
Response: "That's a starting point, but customize it for YOUR document type. Are you reviewing a strategy doc? A product pitch? An email? Adjust the lens for what matters in your context."

**What to say at 10 minutes:**
"If you haven't tested yet, do that now. Run your document through your Challenger and see what comes back. You'll learn more from testing than from staring at instructions."

**What to say at 15 minutes:**
"Everyone should have output from their Challenger by now. Read it. What worked? What didn't? Refine your instructions and run it again."

**What to say at 20 minutes:**
"Last few minutes. Make sure you have Challenger output saved. You'll need it for the next step."

**Time warning at 23 minutes:**
"Two more minutes, then we're building The Executor."

**What success looks like:**
Participants have custom instructions written, have run their document through their Challenger at least once, and have output saved.

**Common pitfall:**
Perfectionism. People want perfect instructions before testing. Redirect: "Test first, refine based on results. Good enough to test beats perfect on paper."

**Quality check while circulating:**
Scan custom instructions. Look for:
- All four framework components present?
- Role is specific (not "helpful assistant")?
- Lens defines WHAT to look for?
- Behavior defines HOW to work?
- Constraints define what NOT to do?

If you see weak instructions, give immediate feedback: "Your Lens is vague. What specifically should this persona look for?"

### Build Your Executor (25 min)

**Facilitator Script:**
"Create a second Project. This is The Executor - the persona that takes your Challenger's feedback and produces improved output."

"Use the framework template again. But this time, the specialization is different. This persona isn't adversarial - it's constructive. It builds, it polishes, it delivers."

**Distribute the handoff template.**

"When you're ready to test, use this handoff template. You're briefing The Executor with three things:"

1. Context: What is this document? What happened in the previous step?
2. Previous Step Output: The actual findings from your Challenger (copy-paste).
3. Task for This Persona: What do you want The Executor to produce?

**Example handoff:**
"Context: This is a business proposal that was reviewed by a critical analyst who identified gaps in the market analysis and budget assumptions.

Previous Step Output: [paste your Challenger's findings]

Task: Revise the original proposal to address these concerns. Strengthen the market analysis section and add detail to the budget justification. Produce a revised draft ready to present."

**Circulate actively. Common issues:**

**Issue 1: Executor straying into analysis**
Example: "It started finding new problems instead of fixing the ones I gave it."
Fix: "Tighten your Constraints. Add: 'You do not perform new analysis. You work within the findings provided.' Also check your handoff - did you clearly say what to produce?"

**Issue 2: Output too generic**
Example: "It gave me generic advice, not specific revisions."
Fix: "Adjust your Behavior section. Add: 'You reference specific elements from the original document and the findings. You do not give generic advice.' Also strengthen your handoff - be explicit about what you want."

**Issue 3: Ignoring Challenger findings**
Example: "The revised output doesn't actually address what the Challenger found."
Fix: "Check your handoff. Did you paste the full Challenger output? Did you say 'address these concerns' or just 'improve the document'? The Executor needs clear instructions."

**Issue 4: Not producing a deliverable**
Example: "It gave me suggestions instead of a revised draft."
Fix: "Your Behavior section should say 'Produce complete deliverables' and your handoff should say exactly WHAT to produce: 'Write a revised proposal' not 'give me ideas for improving the proposal.'"

**What to say at 10 minutes:**
"If you haven't run your handoff yet, do that now. Take your Challenger output, use the handoff template, and run it through your Executor."

**What to say at 15 minutes:**
"You should have output from your Executor by now. Does it address what the Challenger found? Is it actually a deliverable, or just more feedback? Refine and rerun if needed."

**What to say at 20 minutes:**
"Last few minutes. Make sure you have the full pipeline run: your document → Challenger → Executor. Save all three pieces."

**Time warning at 23 minutes:**
"Two more minutes, then we compare results."

**What success looks like:**
Participants have built both personas, run the full pipeline, and have three artifacts: original document, Challenger output, Executor output.

**Pre-flight check while circulating:**
Identify any pipelines that aren't producing good results. Help troubleshoot now - don't wait for Block 4. Look for:
- Executor output that doesn't reference Challenger findings → weak handoff
- Generic advice instead of specific revisions → vague task definition
- New analysis appearing → missing constraints

**If someone's pipeline clearly isn't working:**
Offer to look at their setup. Check custom instructions and handoff. Give direct feedback: "Your Executor doesn't have tight enough constraints. It's analyzing instead of executing. Add this line: 'You do not introduce new analysis.' Then rerun."

## Block 4: The Payoff (20 min)

### Side-by-Side Comparison (10 min)

**Facilitator Script:**
"Pull up two things: the output from your warmup exercise in Block 1, and the final output from your Executor. Put them side by side."

"Give yourself 3 minutes to read them both. What do you notice?"

**Let them compare silently for 3 minutes.**

**At 3 minutes:**
"Who wants to share what they're seeing?"

**Facilitate discussion. Listen for these insights:**

- "The pipeline output is way more specific to my document."
- "It caught things the single prompt completely missed."
- "The single prompt was balanced but shallow. The pipeline went deep."
- "I have a clear path forward now. The warmup output was just feedback."
- "The Executor actually revised my document. The warmup just told me what to fix."

**After 2-3 shares, ask:**
"What's the cost? You ran two specialized prompts instead of one general prompt. Was it worth it?"

Let them answer. Most will say yes.

**If anyone's pipeline didn't outperform their warmup:**
Acknowledge it. "Not every pipeline works perfectly on the first try. The framework is sound, but execution matters. The good news: now you have reusable personas you can refine. This is where the real value starts - you don't rebuild from scratch every time."

**Ask the business question:**
"If you were presenting to a client, your boss, or your board, which output would you rather hand over - the warmup result or the pipeline result?"

Pause. Let the answer speak for itself.

**Time warning at 8 minutes:**
Wrap up individual comparison, move to group discussion.

**What success looks like:**
Participants see visible, tangible difference in output quality. They understand the value proposition of orchestration.

### Group Discussion (10 min)

**Facilitator Script:**
"Let's go broader. What did the pipeline catch that the single prompt missed?"

**Facilitate open discussion. Listen for patterns:**

- Depth vs. breadth tradeoffs
- The value of adversarial thinking separated from constructive thinking
- How constraints kept each persona in its lane
- The handoff as a forcing function for clarity

**Key questions to surface:**

"Why did specialization work better than asking one AI to 'do everything'?"

Guide toward: cognitive load, contradictory modes, depth vs. breadth.

"Could you have written one really good prompt that got the same results?"

Let them debate. The answer: theoretically maybe, practically no. The cognitive load is too high for one conversation to maintain.

"What surprised you about the output?"

Common surprises: how specific it got, how well the Executor incorporated Challenger findings, how much clarity the handoff template added.

**Address the elephant in the room:**
"This took longer than one prompt. When is the pipeline worth the extra time?"

**Guide discussion toward honest boundaries:**

- High-stakes work: presentations to leadership, client proposals, strategy decisions
- Complex documents where quality matters more than speed
- Work you'll iterate on (because the personas are reusable)

**When a single prompt is fine:**
- Routine communications
- First-draft brainstorming
- Low-stakes, low-complexity work

**Emphasize:**
"You don't orchestrate everything. You orchestrate what matters. This is for work where quality trumps speed."

**Time warning at 8 minutes:**
Wrap discussion, transition to Block 5.

**What success looks like:**
Participants articulate why the pipeline worked, understand when to use it, and accept the time/quality tradeoff for high-stakes work.

**Common question:**
"Can I automate this so I don't have to copy-paste between Projects?"

**Answer:** "Yes, with the API. But that's beyond today's scope. Master the manual pipeline first. Prove the personas work. Then automate."

## Block 5: Real Talk and What's Next (25 min)

### When to Orchestrate vs When to Keep It Simple (5 min)

**Facilitator Script:**
"Real talk: you don't need a pipeline for every prompt. Let's be honest about boundaries."

**When to orchestrate:**
- High-stakes work: Board presentations, client proposals, strategic decisions
- Complex documents: Multi-layered plans, proposals with technical and business components
- Iterative work: Anything you'll refine over time (personas are reusable)
- When quality matters more than speed

**When a single prompt is fine:**
- Routine communications: Standard emails, updates, summaries
- First-draft brainstorming: Getting ideas on the page
- Low-stakes, low-complexity work: Internal memos, quick reviews
- When speed matters more than depth

**What to emphasize:**
"The pipeline you built today isn't for everyday use. It's for work that matters. Use your Level One skills for routine tasks. Use orchestration when you need depth."

**Ask:**
"How will you decide when to use the pipeline?"

Let a few people answer. The goal: they develop their own decision heuristic.

**Time warning at 4 minutes:**
Transition to extending the pattern.

**What success looks like:**
Participants have realistic expectations about when orchestration adds value vs. when it's overkill.

### Extending the Pattern (5 min)

**Facilitator Script:**
"Today you built two personas: Challenger and Executor. Divergent thinking, then convergent thinking. Problem-finding, then solution-building. That's the core pattern."

"But sometimes you need a middle step."

**Introduce The Structurer briefly:**
"When your Challenger finds a LOT of issues - 20, 30 findings - they can be hard to act on. That's when you add a middle persona: The Structurer. Its job is to organize findings into themes, prioritize them, create a framework for action."

"So the pipeline becomes: Challenger → Structurer → Executor. Find problems, organize them, solve them."

"You can extend this further. Three, four, five personas. You can run personas in parallel - three different Challengers with different lenses, all feeding into one Structurer."

**Mention other persona types:**
- Researcher: Finds sources, evidence, data to support claims
- Editor: Polishes language and tone
- Customer Advocate: Reviews from end-user perspective
- Risk Analyst: Identifies legal, compliance, or operational risks

**Mention Project Knowledge:**
"You can upload reference documents to a Project. Give your personas frameworks, style guides, domain knowledge to work with. That makes them even more specialized."

**Mention Styles:**
"Claude Projects have a separate Styles feature for controlling voice and tone. You can layer that on top of your persona's behavior."

**What to emphasize:**
"The framework you learned today - Role, Lens, Behavior, Constraints - works for any persona you want to build. You're not limited to what I showed you. You have the pattern."

**Distribute the persona library starter document:**
"This has more pre-built persona templates. Use them as starting points, not rules."

**Time warning at 4 minutes:**
Transition to takeaways.

**What success looks like:**
Participants understand the core pattern (divergent → convergent) and see pathways for extending it.

**Common question:**
"How many personas is too many?"

**Answer:** "When the handoff overhead outweighs the value. Three to five is common. If you're building ten personas for one document, you're over-engineering."

### Your Toolkit (5 min)

**Facilitator Script:**
"Let's recap what you're walking away with."

**List on screen or whiteboard:**

1. Two working personas: Challenger and Executor
2. The framework: Role/Lens/Behavior/Constraints
3. The handoff template: How to brief the next persona
4. The persona library: Pre-built templates for other specialists
5. A new mental model: Specialization beats generalization in AI workflows

**What to emphasize:**
"The real skill you learned today isn't 'how to build a Challenger.' It's how to think about breaking work into specialized cognitive modes. That's orchestration."

**Time warning at 4 minutes:**
Transition to post-workshop path.

**What success looks like:**
Participants have clarity on what they built and why it matters.

### Post-Workshop Path (5 min)

**Facilitator Script:**
"Your homework is simple: use your Challenger on ONE real document this week. Just the Challenger."

"Not the full pipeline. Just run one document through your critical analyst and see what it finds. Build the habit with one persona before you chain them."

**Why this matters:**
"The barrier to using orchestration isn't understanding it - you get it now. The barrier is remembering to actually use it when you're in the flow of work. Practice with one persona first."

**Mention office hours (if available):**
"I hold twice-weekly office hours for troubleshooting and refinement questions. Bring your personas, bring your output, we'll tune them."

**Encourage refinement:**
"Your personas will get better as you use them. Every time you run a document through, you'll see something to improve in the instructions. That's normal. Iteration is the point."

**Final advice:**
"Start small. Master two personas. Then expand. Don't try to build a five-persona pipeline tomorrow. Prove the pattern works for you first."

**Time warning at 4 minutes:**
Open for Q&A.

**What success looks like:**
Participants have a clear, actionable next step: use the Challenger once this week.

### Q&A Buffer (5 min)

**Facilitator Script:**
"Open questions. What are you still wondering about?"

**Common questions and answers:**

**Q: Can I share my personas with my team?**
A: Yes. You can't directly export custom instructions, but you can copy-paste them. Share the instructions and the framework template with your team.

**Q: What if I want different personas for different document types?**
A: Build them. You can have multiple Challengers - one for proposals, one for technical plans, one for strategy docs. Specialize by domain.

**Q: Can I use this with other AI tools, not just Claude?**
A: The framework works anywhere. ChatGPT custom instructions, API calls, any platform that lets you define behavior. The principles are universal.

**Q: How do I know if my personas are good?**
A: Compare the output. Does the pipeline produce noticeably better results than a single prompt? If yes, they're good enough. Refine from there.

**Q: What if my Executor ignores my Challenger's findings?**
A: Check your handoff. Are you explicitly telling it to address those findings? Are you pasting the full Challenger output? Strengthen the task section of the handoff template.

**Be ready to troubleshoot individual issues:**
If someone's pipeline didn't work, offer to look at their setup after the session or in office hours.

**Wrap at 5 minutes:**
"Thank you for being here. Go use what you built."

**What success looks like:**
Participants leave with remaining questions answered and confidence that they can refine on their own.

## Facilitator Mindset

**Your job is to:**
- Keep momentum. Don't let perfectionism stall progress.
- Normalize iteration. "Good enough to test" beats "perfect on paper."
- Show, then teach. Block 1 demo is critical - they need to SEE it work before they understand why.
- Troubleshoot actively. Circulate during build blocks. Catch weak personas early.
- Celebrate discoveries. When someone has an "aha" moment, pause and let the group hear it.

**Time management:**
- You will run behind. Plan for it. The most flexible blocks are discussions - compress those if needed.
- You cannot compress build blocks. People need time to write, test, and iterate.
- Block 3 (building personas) is where time slips. Be disciplined about time warnings.

**Energy management:**
- Block 1 is high energy - they're seeing the magic for the first time. Ride that.
- Block 3 is where people hit resistance. Circulate, encourage, troubleshoot actively.
- Block 4 is the victory lap. Energy should be high. If it's not, someone's pipeline didn't work - help them.

**Common participant types:**

- **The Perfectionist:** Wants perfect instructions before testing. Redirect: "Test first, refine based on results."
- **The Skeptic:** "Why can't I just write one really good prompt?" Show them the Block 4 comparison. Let the output speak.
- **The Overbuilder:** Wants to add five personas and automate everything today. Redirect: "Master two first. Then expand."
- **The Lost:** Can't get their personas to work. Troubleshoot: weak instructions? Poor handoff? Wrong document type? Fix systematically.

**Quality checkpoints while circulating:**

During Block 3, scan for:
- Vague role definitions: "You are helpful" → NO. "You are a critical analyst" → YES.
- Missing constraints: Will lead to scope drift. Insist on constraints.
- Weak handoffs: Just pasting Challenger output with no context → weak Executor output.

**Your goal:**
Every participant walks away with two working personas and the confidence to build more. If they leave thinking "I can do this," you've succeeded.

**If something goes wrong:**
- Participant's Claude account doesn't support Projects → have them pair with someone, observe today, set up later
- Pipeline produces worse output than single prompt → troubleshoot: usually weak constraints or vague handoff
- Running way behind schedule → compress discussions, protect build time

**Post-workshop:**
- Follow up with anyone whose pipeline didn't work
- Share any additional resources or examples requested
- Remind about office hours or support channels
