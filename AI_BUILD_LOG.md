# AI build log: RAY Growth Experiments

I used AI throughout this build: to gather secondary research, understand Razorpay's existing products, synthesize what I learned, and challenge my thinking as a devil's advocate. Once I had chosen the problem and product direction, I used it to articulate the concept, draft the one-page product note and visual PDF, build the clickable prototype, and publish it. I supplied the ideas, field conversations, decisions, and feedback. AI helped me sharpen and execute them.

RAY Growth Experiments is a proposed product for Razorpay's AI PM Build Challenge. The prototype is a simulation, not a connection to a live Razorpay merchant account.

## Tools and models

| Tool or model | How I used it |
| --- | --- |
| OpenAI Codex, using a GPT-6 family model | Helped research and synthesize the problem, critique my hypothesis, articulate the product concept, draft the note and PDF layout, and write and revise the prototype's HTML, CSS, and JavaScript.  |
| Reddit Pain Research and YouTube Researcher, open-source research skills | Collected and organized recent public merchant discussions. These were research tools, not AI models or a representative sample of Razorpay merchants. |
| Browser and web research tools | Checked Razorpay's public product material and reviewed the prototype as it evolved. |
| GitHub and GitHub Pages | With Codex's help, published the static prototype and made its source available. |

Razorpay's Vulcan is part of the **proposed product architecture**. I did not access Vulcan, train a model on Razorpay data, or connect the prototype to RAY, Agent Studio, or Magic Checkout APIs.

## Key prompts and workflow

I worked with Codex in short cycles instead of asking it to generate a complete submission in one step. These are shortened versions of the instructions that shaped the work:

1. **Understand the space:** Explain how Razorpay's products fit together, research recent merchant friction, and identify what RAY, the Agentic Dashboard, Agent Studio, Magic Checkout, and Vulcan already do.
2. **Challenge the problem:** Suggest possible merchant problems from the secondary research, then act as a devil's advocate when I propose a different problem. Check whether the evidence supports it and where the assumptions are weak.
3. **Make the product specific:** Show the merchant's signal, relevant peer evidence, a proposed experiment, what the merchant can edit or stop, and the measured result. Make clear what Razorpay can reuse and what must be built.
4. **Turn the thinking into a submission:** Help me express the problem, product decisions, and measures in a clear one-page note, then draft a visual PDF. I reviewed and corrected the writing and layout.
5. **Make the prototype legible:** Start with RAY in a WhatsApp-style interface. Move to the Agentic Dashboard for evidence, AI-assisted setup, and merchant approval. Show Magic Checkout as the place where the approved checkout change appears, then return to the dashboard for results.

## An AI output I rejected and improved

AI's early problem suggestions focused on individual failures, including captured payments without an order and failed checkout payments. These were plausible problems, but the public evidence could not tell me how common they were across merchants. More importantly, the suggestions did not yet capture the decision that came into focus: merchants can see performance numbers but struggle to know which change is worth trying and whether it actually helped. I did not use the AI's first recommendation as my problem statement.

I spent about two weeks defining the problem before building the prototype. AI helped me gather and organize secondary material, but I treated public comments as leads rather than evidence of how widespread a problem was. I explored Razorpay's products, formed a hypothesis, and spoke with merchants, Razorpay PMs, and others who work closely with payment gateways and aggregators. Those conversations helped me frame a sharper problem: merchants lack a reliable way to learn what comparable businesses tried, choose a change for their own context, and measure whether it improved delivered, profitable orders. I then asked AI to act as a devil's advocate. It challenged the strength of the peer evidence, the risk of mistaking correlation for causation, Razorpay's existing capabilities, and what data would be needed to claim a profit improvement. I kept the problem and refined the solution to show uncertainty, require merchant approval, and measure the change against an unchanged group.

## What AI did and what I decided

**My decisions:** I explored Razorpay's merchant-facing products, synthesized the research, spoke with merchants, Razorpay PMs, and people close to payments, and defined the problem. I brought the comparable-learning and experimentation idea to AI, chose the initial Magic Checkout example, set the MVP boundaries, and decided the merchant controls and success measures. I reviewed the note, PDF, and prototype and told AI what to keep, change, or reject.

**AI's contribution:** Codex gathered and organized secondary material, helped articulate my ideas, critiqued assumptions, suggested edge cases, drafted the note and PDF layout, generated and revised the prototype code, and helped publish it on GitHub Pages. It made each iteration faster, but I supplied the direction and judged the outputs. The research tools did not establish how common a problem is across Razorpay's merchant base.

## Limitations, risks, and checks

- The merchant, peer group, figures, experiment results, and AI setup sequence in the prototype are illustrative. No live AI agent prepares an experiment, no shoppers are assigned to test groups, and no checkout configuration is changed.
- Similar merchants having better outcomes with a setting does not prove that the setting caused the difference. A real product would need eligible peer groups, clear uncertainty, controlled tests, and checks for data quality.
- Razorpay may not hold delivery, return, shipping, and product-cost data for every merchant. Without those inputs, the product should report verified checkout or payment outcomes rather than claim a profit increase.
- Any real use of merchant data would need to follow applicable agreements, access controls, privacy requirements, and approval rules. The concept shows aggregated peer learning, not another merchant's identity or individual results.
- I checked the concept against Razorpay's public product descriptions, reviewed the prototype screens through successive iterations, and confirmed that the published GitHub Pages site loads. This is a concept demonstration, not a production integration or a validated estimate of business impact.
