# Introduction to Claude - Facilitator Guide (Level 1)

**Duration:** 90 minutes
**Target Audience:** Wide audience - business professionals, technical staff, anyone who wants to understand Claude as a tool
**Prerequisites:** None. This session assumes participants may have never used Claude.
**Platform:** Claude web interface (claude.ai)

**What participants will learn:** How to use Claude effectively for analysis, writing, reasoning, and code. How to structure prompts, use Projects for persistent context, work with Artifacts, and understand when Claude adds value to their work.

## Before the Workshop

**Send participants this email 2-3 days in advance:**

Subject: Workshop Access - Introduction to Claude

Hi [name],

Looking forward to the Introduction to Claude session on [date]. Please confirm before the workshop:

- You can access claude.ai from the workshop location
- You have a Claude account (free tier is fine - you can create one at claude.ai)

If you encounter any access issues, let me know before the session.

See you soon,
[Your name]

**Pre-session checklist:**
- [ ] Test your Claude account and Projects feature access
- [ ] Prepare 3-4 example documents participants might recognize (proposal draft, meeting notes, technical spec, email chain)
- [ ] Have a Project pre-built with custom instructions and uploaded documents ready to demo
- [ ] Prepare an Artifact example that will resonate with the audience (formatted report, checklist, or simple visualization)
- [ ] Test all demos in advance - know what responses to expect
- [ ] Have backup examples in case live demos produce unexpected responses

## Materials Checklist

For facilitator:
- Pre-built Project with context loaded
- Sample documents relevant to audience's work
- Example Artifact ready to iterate on
- Backup screenshots of demos in case of connectivity issues

For participants:
- Access to claude.ai
- Link to Anthropic docs (optional post-workshop resource)

## Part 1: Meet Claude (15 min)

### Introduction (3 min)

**Facilitator Script:**
"We're here to learn about Claude - what it is, what it's good at, and how to use it effectively in your work. This isn't a lecture. I'm going to show you Claude working, then you're going to use it."

**What Claude is - keep it plain:**
"Claude is an AI assistant built by Anthropic. It's a large language model trained on text from the internet and other sources. When you type something to Claude, it generates a response based on patterns it learned during training."

"Think of it as a very well-read colleague who can analyze, write, reason through problems, and write code - but doesn't have access to the internet, can't remember conversations unless you're in a Project, and isn't perfect. It's a tool. A powerful one. Let's see what it can do."

**Set expectations clearly:**
"Three things to know up front:"

1. **Not a search engine:** "Claude doesn't browse the web. It works from what it learned during training, which has a cutoff date. For current events or real-time data, use search. For analysis, reasoning, and synthesis, use Claude."

2. **Not infallible:** "Claude can get things wrong. It can sound confident about incorrect information. Always verify important outputs, especially facts, numbers, and technical details."

3. **Not a replacement for human judgment:** "Claude is a thinking partner, not a decision-maker. It can help you analyze options, draft documents, and work through complexity - but you're still the one making decisions."

**Time warning at 2.5 minutes:**
Transition to demo.

**What success looks like:**
Participants understand Claude is a reasoning tool, not a search engine or oracle. Expectations are grounded in reality.

### Live Demo: A Basic Conversation (12 min)

**Facilitator Script:**
"Let me show you what a conversation with Claude looks like. I'm not going to use a toy example. This is something real."

**Choose a demo that matches your audience's work:**
- For business professionals: "Review this project proposal and identify potential risks I should address before presenting it to leadership."
- For technical staff: "Explain the tradeoffs between synchronous and asynchronous API design. What factors should I consider?"
- For general audience: "I need to write a follow-up email after a difficult client meeting where we didn't reach agreement on timeline. Help me draft something that's professional but firm about our constraints."

**Share your screen. Open Claude.**

**Type the prompt. Hit send.**

"Watch what happens. Claude reads the request, generates a response, and formats it in a readable way."

**Let the response generate. Read highlights aloud, don't read every word.**

"Notice a few things:"

1. **It structures the response:** "Headings, bullets, clear sections. Claude formats output to be readable."

2. **It reasons through the problem:** "It's not just retrieving information. It's thinking through what you asked, considering context, organizing its response."

3. **You can iterate:** "If this response isn't quite what I need, I can ask for changes. Watch."

**Follow-up prompt:**
"Focus more on timeline risks and budget assumptions. Be more specific about what could go wrong."

**Let the response generate.**

"Same conversation, refined output. That's the interaction model. You ask, Claude responds, you iterate."

**Ask the group:**
"What questions do you have so far? Anything about how this works or what you're seeing?"

**Take 1-2 quick questions. Don't let this expand into full Q&A.**

**Time warning at 10 minutes:**
"We're going to talk about how to ask Claude for what you actually want. That's prompting. Let's dig in."

**What success looks like:**
Participants have seen Claude work on a realistic task. They understand the basic interaction model: you ask, it responds, you iterate.

**Common question:**
"Is Claude reading my data? Where does it go?"

**Answer:** "Claude processes your inputs to generate responses. Anthropic has data retention policies - free tier conversations can be used for training, paid tiers have different policies. Check Anthropic's privacy docs for specifics. For sensitive work, understand what tier you're using."

## Part 2: How to Talk to It (20 min)

### Prompting Fundamentals (8 min)

**Facilitator Script:**
"Prompting is a skill. The difference between a vague ask and a clear ask is the difference between mediocre output and output you can actually use. Let me show you."

**Live Demo: Same Task, Different Prompts**

**Share screen. Open two Claude chat windows side by side.**

**Window 1 - Vague Prompt:**
"Write something about our new product feature."

**Window 2 - Clear Prompt:**
"Write a 3-paragraph announcement for our team Slack channel explaining the new batch export feature. Audience is non-technical sales reps. Focus on what problem it solves (no more manual CSV downloads) and how to access it (new button in the Reports tab). Keep the tone friendly and practical."

**Let both generate. Show the outputs side by side.**

**Point out the difference:**
"Window 1 gave me generic marketing copy. Window 2 gave me something I can actually post. What changed?"

**Guide discussion toward these points:**

1. **Specificity:** "I told it the format (3 paragraphs), the audience (sales reps), the channel (Slack), the tone (friendly and practical). Specific input produces specific output."

2. **Context:** "I explained what the feature does and what problem it solves. Claude can't read your mind. Give it context."

3. **Constraints:** "I said 'focus on' and 'keep the tone' - those are constraints. They prevent Claude from wandering into territory you don't need."

**What to emphasize:**
"You don't need to write perfect prompts on the first try. But the more specific, contextual, and constrained you are, the better the output."

**Time warning at 7 minutes:**
Transition to techniques.

**What success looks like:**
Participants see the visible difference between vague and clear prompting. They understand that specificity, context, and constraints drive quality.

### Key Prompting Techniques (12 min)

**Facilitator Script:**
"Here are the techniques that make the biggest difference. You don't need to memorize these - you'll internalize them as you use Claude. But knowing they exist helps."

**Walk through each technique with a brief example:**

**1. Role-setting**
"Tell Claude who it should be. 'You are a technical editor reviewing documentation for clarity.' 'You are a financial analyst assessing budget assumptions.' Role primes how Claude thinks about the task."

**Live example:**
Type: "You are a customer support specialist. Review this email draft and flag anything that sounds defensive or might escalate the situation."

Let it run briefly, show output.

"Notice how the role shaped the feedback. It's looking for tone issues, not grammar."

**2. Providing examples**
"Show Claude what good looks like. If you want a specific format or style, give an example."

**Quick example:**
"Write three bullet points summarizing this meeting. Format like this:
- Decision: [what was decided]
- Owner: [who's responsible]
- Deadline: [when it's due]"

"Claude will match the pattern you show it."

**3. 'Think step by step' or 'explain your reasoning'**
"When you need Claude to work through something complex, ask it to show its thinking. This often improves accuracy."

**Live example:**
Type: "I have a budget of $50k for this project. The vendor quoted $35k for development and $18k for design. Think step by step - does this fit my budget, and what are my options?"

Let it run briefly.

"See how it broke down the math and reasoning? That's more reliable than just asking 'does it fit?'"

**4. Asking for revisions**
"Don't restart if the output is close but not quite right. Ask Claude to revise. 'Make this more concise.' 'Add more detail to section 2.' 'Change the tone to be more formal.' Iteration is faster than starting over."

**5. Being explicit about format**
"If you want a table, say 'format this as a table.' If you want markdown, say 'use markdown formatting.' If you want bullet points, say 'give me bullet points.' Claude doesn't guess."

**Quick live example:**
"Give me a comparison of async vs sync API design. Format as a table with columns for Approach, Pros, Cons, and Best Used When."

Let it generate quickly, show the table.

"That's explicit formatting. You asked, it delivered."

**Pause and check for understanding:**
"Questions on any of these techniques?"

**Take 1-2 questions. Keep it brief.**

**Time warning at 11 minutes:**
"Next we're talking about Projects - how to give Claude persistent context so it remembers your work. That's where this gets powerful."

**What success looks like:**
Participants have seen 5 core techniques demonstrated live. They don't need to master them yet - just know they exist and have seen them work.

**Common question:**
"How long should my prompts be?"

**Answer:** "As long as they need to be. Short prompts are fine for simple tasks. Complex tasks need detail. There's no magic number. Clarity matters more than length."

## Part 3: Projects - Persistent Context (20 min)

### What Projects Are (5 min)

**Facilitator Script:**
"Everything we've done so far has been in basic chat. That's fine for one-off tasks. But what if you're working on something over time? What if you want Claude to know your context, your style, your constraints without re-explaining every conversation?"

"That's what Projects do. They're workspaces where Claude remembers."

**Three key features:**

**1. Custom Instructions:**
"You can teach Claude about your work, your domain, your preferences. Once. Then every conversation in that Project starts with that context."

**2. Document Uploads:**
"You can give Claude reference material - style guides, domain docs, examples of past work. It can reference those documents in every conversation."

**3. Persistent Context:**
"Projects remember conversation history within that workspace. Claude can reference earlier discussions, build on previous work, maintain continuity."

**What to emphasize:**
"This is the shift from 'disposable chat' to 'workspace that knows my world.' For recurring work, Projects are where you should be."

**Time warning at 4 minutes:**
Transition to live demo.

**What success looks like:**
Participants understand Projects as persistent context workspaces, distinct from basic chat.

### Live Demo: Create and Use a Project (15 min)

**Facilitator Script:**
"I'm going to create a Project live, add custom instructions, upload a document, and show you how responses change. Watch."

**Step 1: Create the Project (2 min)**

**Share screen. Navigate to Projects in Claude.**

"Click 'Create Project.' Give it a name - something that describes the work. I'll call this 'Product Documentation.'"

**Create the Project. Open it.**

"Now we're in the Project workspace. Notice the sidebar - that's where custom instructions and knowledge go."

**Step 2: Add Custom Instructions (5 min)**

**Open custom instructions panel.**

**Facilitator Script:**
"Custom instructions tell Claude how to behave in this Project. I'm going to write instructions for documentation work."

**Type custom instructions live (adapt to your audience's domain):**

```
You are a technical writer helping me create user-facing documentation.

Context:
- Our audience is non-technical business users
- Our product is a workflow automation platform
- Clarity and simplicity are more important than comprehensiveness

When I ask you to write or review documentation:
- Use plain language, avoid jargon
- Lead with what the user can accomplish, not how the system works
- Include concrete examples
- Keep paragraphs short (3-4 sentences max)
- Use active voice

Do NOT:
- Assume technical knowledge
- Use placeholder text like "[insert example]" - always provide real examples
- Write in passive voice
```

**Save the instructions.**

"Those instructions now apply to every conversation in this Project. Let me show you the difference."

**Step 3: Compare Responses (5 min)**

**Facilitator Script:**
"I'll ask the same question in two places - basic chat and this Project."

**Open basic chat in another window. Type:**
"Explain how to set up a webhook in our automation platform."

**Let it generate.**

**Switch to the Project. Type the same prompt:**
"Explain how to set up a webhook in our automation platform."

**Let it generate.**

**Show both side by side.**

"Look at the difference. Basic chat gave me technical documentation. The Project gave me user-facing instructions with examples. Same question. Different context. The custom instructions shaped the response."

**Step 4: Upload a Document (3 min)**

**Facilitator Script:**
"Now I'll upload a document - a sample of past documentation or a style guide - and show Claude using it."

**Upload a sample document (prepare this in advance - a 1-2 page doc with examples of good documentation).**

**Type in the Project chat:**
"Review this draft documentation for the new export feature. Compare it to the style in the uploaded examples. Flag anything that doesn't match."

**Let it generate briefly.**

"See how it's referencing the uploaded document? That's persistent knowledge. Any conversation in this Project can pull from that reference material."

**Wrap up:**
"Projects: custom instructions + uploaded documents + conversation history. That's your workspace. For recurring work - documentation, specific types of analysis, domain-specific tasks - build a Project. You'll save time and get more consistent output."

**Time warning at 14 minutes:**
"Questions on Projects before we move to Artifacts?"

**Take 1-2 quick questions.**

**What success looks like:**
Participants have seen a Project created from scratch, watched custom instructions shape output, and seen uploaded documents referenced. The "aha" moment: Claude can remember my context.

**Common question:**
"Can I have multiple Projects?"

**Answer:** "Yes. As many as you want. Create Projects for different types of work - one for technical writing, one for data analysis, one for customer communications. Each maintains its own context."

**Common question:**
"What if I want to use the same custom instructions across multiple Projects?"

**Answer:** "Copy-paste. There's no template feature yet. Write good instructions once, then reuse them."

## Part 4: Artifacts - Interactive Outputs (15 min)

### What Artifacts Are (5 min)

**Facilitator Script:**
"So far, everything Claude has produced has been text in the chat. That's fine for many tasks. But sometimes you need more than text. You need a deliverable you can use directly."

"That's what Artifacts are. They're not just responses - they're usable outputs."

**Types of Artifacts:**

**1. Documents**
"Formatted documents - reports, memos, briefs. You can edit them directly in Claude, then copy them out."

**2. Code**
"Claude can write code and display it as an Artifact. You can copy it, test it, iterate on it."

**3. Visualizations**
"Diagrams, charts, simple visualizations. Not publication-quality graphics, but useful working drafts."

**4. Interactive Components**
"Forms, calculators, interactive tools. Claude can build simple web components you can use immediately."

**What to emphasize:**
"Artifacts are deliverables, not conversations. You get something you can take and use. And you can iterate on them - ask Claude to edit specific parts, refine the output, change the format."

**Time warning at 4 minutes:**
Transition to demo.

**What success looks like:**
Participants understand Artifacts as distinct from chat text - they're interactive, editable, usable outputs.

### Live Demo: Generate and Iterate on an Artifact (10 min)

**Facilitator Script:**
"I'm going to generate an Artifact, edit it live, and show you the iteration loop. This is practical - not a toy example."

**Choose a demo relevant to your audience:**
- For business: "Create a decision matrix comparing three vendor options"
- For technical: "Write a Python function that parses CSV files and flags rows with missing data"
- For general: "Create a formatted project status report template"

**Example demo (using the decision matrix):**

**Type in Claude:**
"Create a decision matrix as an Artifact. I'm comparing three vendors for project management software. Criteria: Cost, Ease of Use, Integration Options, Support Quality. Vendors: Vendor A, Vendor B, Vendor C. Format as a table. Leave space for me to fill in scores later."

**Let Claude generate the Artifact.**

**Point out what happened:**
"See how it appeared in a separate panel? That's an Artifact. It's a table I can use directly."

**Now iterate on it:**
"Add a column for Notes. Change 'Support Quality' to 'Customer Support.' Make the vendor names bold."

**Watch the Artifact update.**

"That's iteration. I don't start over. I tell Claude what to change. It updates the Artifact."

**Keep iterating:**
"Actually, add example scoring criteria for each row. Under Cost, note '1 = >$50/user, 5 = <$10/user.' Do similar for the others."

**Watch it update again.**

"Now this is a usable decision matrix. I can copy this into a doc, send it to my team, use it in a meeting. That's the point - it's not just chat. It's a deliverable."

**Show how to copy the Artifact:**
"Click here to copy the code or content. Now I can paste it into whatever tool I'm using."

**Ask the group:**
"What kind of Artifacts would be useful in your work?"

**Let them answer briefly. Common responses: formatted reports, checklists, templates, code snippets, comparison tables.**

**Acknowledge their answers:**
"All of those are possible. Ask Claude to format it as an Artifact, specify what you need, iterate until it's right."

**Time warning at 9 minutes:**
Wrap up, transition to Part 5.

**What success looks like:**
Participants have seen an Artifact generated from scratch, edited through iteration, and understood as a reusable deliverable.

**Common question:**
"Can I save Artifacts for later?"

**Answer:** "Not directly in Claude. Copy the content out and save it wherever you keep your work files. Artifacts exist within the conversation - if you need them later, copy them out."

## Part 5: Putting It Together (15 min)

### End-to-End Workflow Demo (12 min)

**Facilitator Script:**
"You've seen conversation, Projects, Artifacts. Now let's see how they work together. I'm going to show you a real workflow from start to finish."

**Pick a scenario that ties everything together (adapt to your audience):**
"I need to write a proposal for a new internal process. I'll use a Project with context about our team's work style, have a conversation that builds understanding, and produce a formatted proposal as an Artifact."

**Step 1: Start in the Project**

**Open a pre-built Project (prepare this beforehand with relevant custom instructions and an uploaded document - e.g., examples of past proposals or a team style guide).**

**Facilitator Script:**
"I'm in my 'Internal Proposals' Project. It already has custom instructions about my team's preferences and examples of past successful proposals. That context is loaded."

**Step 2: Have a conversation to build understanding**

**Type:**
"I need to propose a new code review process for our team. Current state: reviews are ad-hoc, no consistent checklist, feedback quality varies. Proposed state: standardized checklist, required reviews before merge, documentation of review comments. What questions should I answer in the proposal to make it convincing?"

**Let Claude respond.**

"See how it's asking about objections, resource requirements, success metrics? That's Claude helping me think through what the proposal needs to address. This isn't the proposal yet - this is the planning conversation."

**Step 3: Refine based on the questions**

**Type:**
"Good points. Here's more context: main objection will be 'this slows us down.' Counterpoint: current process causes bugs that cost more time to fix than reviews would take. Resources: no new tools needed, just process change. Success metric: reduce post-merge bugs by 30% in first quarter."

**Let Claude respond.**

"Now it's building on my answers. We're developing the argument together. Still in conversation mode - not writing the proposal yet."

**Step 4: Produce the Artifact**

**Type:**
"Write the proposal as an Artifact. Format: 1-page max, sections for Problem Statement, Proposed Solution, Anticipated Concerns, Success Metrics. Tone: collaborative, not top-down. Use the style from the uploaded examples."

**Let Claude generate the proposal Artifact.**

**Point out what happened:**
"Now we have a deliverable. The conversation built understanding. The Project provided context. The Artifact is the usable output. That's the workflow."

**Step 5: Iterate if needed**

**Type:**
"Make the 'Anticipated Concerns' section more specific. Address the 'this will slow us down' objection directly with the bug-fixing time data."

**Watch the Artifact update.**

"Refinement. I didn't start over. I told it what to adjust. The Artifact updated."

**Show the final output:**
"This is a proposal I can take to my team meeting. It's formatted, clear, addresses objections, includes metrics. I didn't write it from scratch - Claude and I built it together. The Project had the context. The conversation developed the thinking. The Artifact is the deliverable."

**What to emphasize:**
"This isn't magic. It's a workflow. The features compound. Projects remember your context. Conversations build understanding. Artifacts produce deliverables. That's how you use Claude for real work."

**Time warning at 11 minutes:**
Open for reactions.

**Ask:**
"What are you thinking about this workflow? Where could you use this in your work?"

**Let 1-2 people answer. Keep it brief.**

**What success looks like:**
Participants see the features working together, not in isolation. The workflow feels natural, not forced. They're thinking about how to apply it to their own work.

**Common reaction:**
"This seems like it takes longer than just writing the proposal myself."

**Response:** "For simple work, maybe. But for complex deliverables - proposals that need to be airtight, reports that need to be thorough, communications that need to be carefully worded - the thinking time with Claude often saves you revision time later. Use it where quality matters more than speed."

## Part 6: Where to Go From Here (5 min)

### The Broader Ecosystem (2 min)

**Facilitator Script:**
"What you've learned today is Claude through the web interface - claude.ai. That's the most accessible way to use it. But there's more to the ecosystem. You don't need to learn this today. Just be aware it exists."

**Briefly mention:**

**1. Claude Code**
"A CLI tool for developers. Lets Claude edit files, run commands, work directly in your development environment. If you're a developer, it's worth exploring. If you're not, the web interface is what you need."

**2. Claude API**
"How engineers build custom tools that use Claude. If your organization wants to integrate Claude into internal applications, that's done through the API. Not something most users need to touch directly - but it's how custom tooling gets built."

**3. MCP (Model Context Protocol)**
"A way for Claude to connect to external tools and data sources. Lets Claude pull information from databases, APIs, other systems. Again, not something you configure yourself - but if your org sets up MCP integrations, you'll be able to use them through Projects."

**What to emphasize:**
"You don't need any of that today. I'm just planting seeds. The web interface is powerful on its own. If you get curious about deeper integrations, those options exist."

**Time warning at 1.5 minutes:**
Transition to L2 mention.

**What success looks like:**
Participants know these capabilities exist but don't feel overwhelmed. Awareness, not mastery.

### The Advanced Workshop (1 min)

**Facilitator Script:**
"For those of you who want to go deeper - to learn how to build specialized AI personas and orchestrate them into workflows for complex deliverables - we have an advanced workshop."

"It's called the AI Orchestration Workshop. You learn to design multiple specialized AI agents, coordinate handoffs between them, and produce executive-ready work faster and with higher quality."

"Today you learned to use Claude. That workshop teaches you to orchestrate Claude. If that sounds useful, here's how to sign up: [provide details or link]."

**Keep this brief. No hard sell.**

**Time warning at 1 minute:**
Move to resources.

### Resources and Wrap-Up (2 min)

**Facilitator Script:**
"Three resources for you:"

**1. claude.ai**
"Where you'll use Claude. Free tier gets you started. Paid tiers (Pro, Team, Enterprise) unlock higher usage limits and additional features."

**2. Anthropic Documentation**
"docs.anthropic.com - official guides, best practices, detailed feature explanations. If you want to go deeper, start there."

**3. Internal Channels (if applicable)**
"[Your organization's Slack channel / Teams channel / support contact] - if you have questions, run into issues, or want to share what you've built, that's where to go."

**Final advice:**
"Start simple. Pick one task this week - something real from your work - and try Claude on it. A draft email. A document review. A summary of meeting notes. Don't try to master everything at once. Use it, see what works, iterate."

"Questions?"

**Take final questions. Keep this to 2 minutes max.**

**Wrap:**
"Thank you for being here. Go use what you learned."

**What success looks like:**
Participants leave with clear next steps: try Claude on one real task this week. They know where to find resources. They feel capable of starting.

## Facilitator Mindset

**Your job is to:**
- Show, don't lecture. Every feature should be demonstrated live before explained.
- Use real examples. Nothing generic. Use documents, tasks, and scenarios your audience recognizes from their work.
- Be honest about limitations. When Claude gets something wrong in a demo, acknowledge it. "See? Not perfect. This is why you verify important outputs."
- Keep energy high. Live demos are more engaging than slides. Your enthusiasm for the tool should be visible but not hype.
- Answer questions briefly. Don't let Q&A derail the flow. Park complex questions for after the session.

**Time management:**
- You will run long if you're not disciplined. Watch the clock.
- Part 3 (Projects) and Part 5 (workflow demo) are the most likely to slip. Keep demos tight.
- If you're running behind, compress Part 6 (Where to Go From Here). The core content is Parts 1-5.
- Do NOT skip live demos to save time. The demos are the teaching. Cut discussion instead.

**Energy management:**
- Start high energy in Part 1 - this is their first impression of Claude.
- Part 2 (prompting) can feel dry. Keep it practical with live examples.
- Part 3 (Projects) is usually the "aha" moment. Lean into it.
- Part 5 (workflow) is the payoff. Make it feel like a natural culmination, not a forced demo.

**Common participant types:**

- **The Skeptic:** "I can just do this myself." Response: "Absolutely. Claude's a tool. Use it where it adds value, skip it where it doesn't. Let me show you where it tends to shine."

- **The Overwhelmed:** Looks lost, not engaging. Check in during demos: "Make sense so far?" Offer to help them catch up.

- **The Power User:** Already uses ChatGPT or other tools, wants to know what's different about Claude. Answer: "Longer context windows, better at nuanced reasoning, strong performance on analysis and synthesis. Try both, see which fits your work better."

- **The Evangelist:** Wants to talk about AI changing everything. Redirect: "Lots of big picture stuff to discuss. Today we're focused on practical use. Let's make sure you can use the tool first."

**Quality checkpoints during demos:**

- Does the live demo produce output you can use as a real example? If not, have a backup ready.
- Are participants following along? Check faces. If you see confusion, pause and clarify.
- Are questions piling up? If you're getting a lot of "wait, how did you do that?" you're moving too fast.

**Your goal:**
Every participant leaves able to log into Claude, ask it to do something useful, and get a decent result. That's success. They don't need to be experts. They need to be capable of starting.

**If something goes wrong:**

- **Demo produces bad output:** Acknowledge it. "That wasn't what I expected. Let me refine the prompt." Show the iteration. It's more honest than pretending everything works perfectly.

- **Claude is slow or down:** Have backup screenshots of expected outputs. Walk through what you would have shown. Not ideal, but better than stalling.

- **Participant can't access Claude:** Have them pair with someone who can. They can observe today, set up access later.

- **Running way behind schedule:** Compress Part 6. Keep Parts 1-5 intact - that's the core content.

**Post-session:**
- Share links to Anthropic docs, internal channels, and L2 workshop signup (if applicable).
- Be available for 5-10 minutes after for individual questions.
- If anyone struggled during the session, offer to follow up with them directly.

**Facilitator preparation:**
- Run through all demos at least once before the session. Know what responses Claude typically produces.
- Have backup examples ready in case live demos go sideways.
- Test your Project setup. Make sure custom instructions and uploaded documents are working as expected.
- If your audience is domain-specific (engineering, finance, legal, etc.), tailor examples to that domain. Generic examples teach less.

**What makes this session work:**
- **Live demos, not slides.** Participants see Claude working in real-time.
- **Real examples, not toy tasks.** Use work they recognize.
- **Honesty about limitations.** Don't oversell. Build trust by being realistic.
- **Practical focus.** No theory. No hype. Just "here's how to use this tool effectively."

**If participants leave saying:**
"I understand what Claude is, I know how to ask it for what I need, and I'm going to try it on something real this week" - you've succeeded.
