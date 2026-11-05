# AI and Manufacturing Training: Montcalm Community College

Materials for the **AI & Manufacturing Workshop**, a hands-on training that helps manufacturing professionals understand and apply artificial intelligence in real production environments.

The workshop focuses on **practical, applied AI** that reduces downtime, improves quality, and supports the people on the floor.

## Training Format
- 3 days
- 3 hours per day, 9:00 AM to 12:00 PM
- 9 hours total

No prior AI or coding experience is required.

---

# Before Day 1

Please have these ready before the first session:

- **Your work Microsoft account**, signed in to Copilot at [m365.cloud.microsoft](https://m365.cloud.microsoft).
- **A laptop with a webcam** and Chrome or Edge.
- **Nothing to install.** Everything runs in your browser.

Before you put company information into any AI tool, follow your company's AI policy.

---

# Workshop Sessions

## Day 1: Computer Vision and Your AI HQ
**Theme:** See how AI learns from data, then build an AI HQ in Copilot that remembers how you work

| Time | Block |
|---|---|
| 9:00 to 9:10 | Welcome, introductions, and agenda |
| 9:10 to 9:20 | The state of manufacturing: what keeps you up at night, the workforce outlook, and the adoption gap |
| 9:20 to 10:15 | Computer vision: train a model to spot defective cast parts |
| 10:15 to 10:25 | Break |
| 10:25 to 10:45 | Context beats prompts, and how I run my work with AI |
| 10:45 to 11:45 | Build your AI HQ in Copilot |
| 11:45 to 12:00 | Your turn and what's next |

Topics covered:

- The state of manufacturing: the workforce shortage and the technology adoption gap
- Computer vision in manufacturing: inspection, sorting, and robot guidance
- Hands-on: training a defect detection model with **Teachable Machine**
- Training data, overfitting, and bias, seen in your own model
- Context beats prompts: instructions, knowledge, and memory
- Hands-on: building an AI HQ in Microsoft Copilot with instructions, files, and a memory file
- Keeping AI honest: a guardrail that stops it from making up prices

**Slides**

[Day 1 Slides (PDF)](slides/Day1-Montcalm.pdf)

### Computer Vision Hands-On

1. Download the dataset: [casting_data.zip](data/casting_data.zip) (OK and defective cast parts)
2. Train your model at [Teachable Machine](https://teachablemachine.withgoogle.com/)
3. Test it in the Preview panel with pictures from the test folders
4. Instructor demo: Export Model > Upload my model, then test it with a webcam in the demo below

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/grcc-resendiz/teachable-machine-demo)

The demo needs a free GitHub account. You don't need one today; it's here so you can run it back at work.

### AI HQ Workshop

**Theme:** Save your context once, so Copilot works the way you do every time

**1. Your Copilot instructions**

Paste the interview prompt into a new Copilot chat. Copilot asks you five questions, then writes your instructions. Save them under **Settings > Personalization > Customize Copilot**.

<details>
<summary><b>Interview prompt</b> (click to open, then copy)</summary>

```
Help me write my personal instructions for Copilot (Settings > Personalization > Customize Copilot).

Interview me first. Ask these questions one at a time, and wait for my answer before asking the next:

1. What's your role, what does your company make, and who are your customers?

2. What do you use Copilot for most, and who reads the result?

3. When you give Copilot a bigger task, how should it work with you? Ask questions first, show a plan first, or just do it? Give one recommendation or a few options?

4. How should my answers look? Pick one from each line, or describe your own:
   Tone: formal / friendly professional / casual
   Length: a few lines / a short paragraph / as detailed as needed
   Format: bullet points / paragraphs / bullets for lists, paragraphs for explanations
   Anything you never want to see? (for example: long intros, buzzwords, emojis)

5. What names, terms, or acronyms should Copilot always get right?

Keep each question short. If an answer is vague, ask one short follow up, then move on.

When the interview is done, write my instructions in plain text, under 1,500 characters, using this format:

About me:
(from answers 1 and 2)

How to work with me:
(from answer 3)

How to respond:
(from answer 4)

Our terms:
(from answer 5, one line each)

Rules:
When I say "remember this," save it to your memory and confirm.
Never invent numbers, prices, dates, or part specs. If you don't have them, ask me.
If you're not sure about something, say so. Don't guess.
Lead with the answer, then a short explanation.

Copy the four rules above exactly as written. Then tell me to paste the result into Settings > Personalization > Customize Copilot and click Save.
```

</details>

**2. Test your memory**

```
Remember this: I don't take meetings before my second cup of coffee.
```

Look for **Memory saved**, then open a new chat and ask:

```
When's a good time to schedule a meeting with me?
```

**3. Demo HQ: Example Equipment Co.**

Example Equipment Co. is a fictional conveyor shop. Its customers, prices, and quotes are made up for this demo.

1. In Copilot, open **Notebooks** (on some screens, **Workspaces**) and create **Example Equipment Co. HQ**
2. Click **...** > **Instructions** and paste the HQ instructions below
3. Download the three files and upload them to the notebook

| File | Part of context |
|---|---|
| [Example Equipment Co. Price List.docx](files/Example%20Equipment%20Co.%20Price%20List.docx) | Knowledge |
| [Example Equipment Co. Past Quote.docx](files/Example%20Equipment%20Co.%20Past%20Quote.docx) | Knowledge |
| [Example Equipment Co. MEMORY.docx](files/Example%20Equipment%20Co.%20MEMORY.docx) | Memory |

<details>
<summary><b>HQ instructions</b> (click to open, then copy)</summary>

```
Identity: You are the quoting assistant for Example Equipment Co., a 60 person shop in West Michigan that designs and builds custom conveyors and material handling equipment for food processing and industrial plants. Use this notebook for customer requests, quotes, and follow up emails.

Context: Before answering, read the files in this notebook:
"Example Equipment Co. Price List" for prices.
"Example Equipment Co. Past Quote" for the quote format.
"Example Equipment Co. MEMORY" for customers, open requests, and decisions.
Use them without announcing that you read them.

Pricing rule: Never give a price that isn't in the price list. If an item is missing, say "Not on the price list, needs an estimate from engineering" and leave it out of the total.

Quote rules:
Always follow the past quote's format.
Always state the lead time and any assumptions.
Always apply each customer's requirements from the memory file.
Quotes are valid for 30 days.
Standard lead time is 8 to 10 weeks from approved drawings.
Freight and installation are always quoted separately.

Remember this: When I say "remember this," reply with the complete updated memory file, with the new fact in the right section and today's date on the "Last updated" line. Don't add any source or reference lines.

Placement test: If something I tell you is a rule (always, never, before doing X do Y), tell me to add it to these instructions instead of the memory file.

Style: Plain, direct language. Answer first.
```

</details>

**4. Demo prompts**

<details>
<summary><b>All demo prompts, in order</b> (click to open)</summary>

Prompt 1, draft a quote (expect about $35,070):

```
Draft a quote for this request in the same format as our past quote:

From: Purchasing Manager, Customer A
Subject: Quote request, incline conveyor
Hi,
We need a quote for a 40 foot incline belt conveyor to move bagged snacks from our packing line up to the palletizer, about 600 bags per hour. Please include a control panel and guarding. We'd like the quote by Friday.
Thanks
```

Prompt 2, what's open:

```
What quotes are open and what's due first?
```

Prompt 3, the guardrail (expect "Not on the price list"):

```
Customer A also wants a metal detector on this conveyor. Add it to the quote.
```

Remember this:

```
Remember this: Customer A requires stainless steel frames and guarding on every conveyor in their plant because of daily washdown.
```

Save it: copy Copilot's reply, paste it into the MEMORY Word file, save, remove the old file from the notebook, and upload the new one.

Ask again in a new chat inside the notebook (expect about $64,785):

```
Redo the Customer A quote.
```

</details>

**5. Make It Yours**

Start with the HQ closest to your job. Each starter has notebook instructions and a starter memory file.

| Starter HQ | Good for |
|---|---|
| [Requests and Quotes](starters/requests-and-quotes.md) | Customer requests, estimates, quotes, and follow ups |
| [Production Data](starters/production-data.md) | Line data, shift numbers, graphs, and analysis |
| [Reports and Communication](starters/reports-and-communication.md) | Weekly reports, emails, and updates to leadership |
| [Team](starters/team.md) | Coaching notes, training plans, and team updates |

**6. What Carries Over from Claude to Copilot**

<details>
<summary><b>Comparison table</b> (click to open)</summary>

✅ = yes, 🟡 = partly (you do that part by hand), ❌ = no. Premium means Microsoft 365 Copilot with Copilot Cowork turned on, based on Microsoft's documentation.

| Feature | Claude | Copilot Basic | Copilot Premium |
|---|---|---|---|
| Root instructions | ✅ | ✅ | ✅ |
| "Remember this" | ✅ | ✅ | ✅ |
| Workstations | ✅ | ✅ Notebook | ✅ Project |
| Knowledge files | ✅ | ✅ | ✅ |
| Workstation memory file | ✅ | ✅ | ✅ |
| Saves the memory update | ✅ | 🟡 You paste it and upload again | ✅ With your approval |
| Sorts facts into the right section | ✅ | 🟡 Check it | 🟡 Check it |
| Routing between workstations | ✅ | 🟡 You open the Notebook | 🟡 You open the Project |
| Folders inside folders | ✅ | ❌ | ❌ |
| Skills | ✅ | ❌ | ✅ |
| Scheduled tasks | ✅ | ❌ | ✅ |
| Files on your own computer | ✅ | ❌ Uploads only | ❌ OneDrive only |

</details>

**8. If Something Looks Different**

- **Notebooks vs Workspaces:** Microsoft is renaming Notebooks to Workspaces. Either works.
- **No Personalization settings:** your IT team may have turned them off. Paste your instructions at the top of a chat instead.
- **"MEMORY 1" after uploading:** uploading again makes a numbered copy. Delete the old one.

---

## Day 2: AI Agents
**Theme:** Turn what you built on Day 1 into an AI agent your whole team can use

| Time | Block |
|---|---|
| 9:00 to 9:10 | Welcome back and Day 1 recap |
| 9:10 to 9:35 | What makes an AI agent, and where agents fit on the floor |
| 9:35 to 10:20 | Build an agent together: the Example Equipment Co. Quote Desk |
| 10:20 to 10:30 | Break |
| 10:30 to 11:05 | Build your own agent, then try to break it |
| 11:05 to 11:25 | Skills: teach your agent a repeatable method |
| 11:25 to 11:50 | Premium: agents that research, analyze, and run on a schedule |
| 11:50 to 12:00 | Where agents help most and what's next |

Topics covered:

- From chat to HQ to agent: what changes when AI does a job instead of answering a question
- The anatomy of an agent: a job, instructions, knowledge, and tools
- Three kinds of agents: ones that answer, ones that do tasks, and ones that run on their own
- Hands-on: building an agent in Copilot with **Agent Builder**, on the free version
- Guardrails: asking for missing details, staying in its lane, and handing off to a person
- Hands-on: designing your own agent, then having a neighbor try to break it
- Skills: adding a packaged method (a SKILL.md file) to an agent, on the free version
- Premium: Researcher, Analyst, agents grounded in SharePoint and Teams, scheduled prompts, Workflows, and Copilot Studio
- Deciding which jobs are a good fit for an agent

**Slides**

[Day 2 Slides (PDF)](slides/Day2-Montcalm.pdf)

### Before You Start

Sign in at [copilot.cloud.microsoft](https://copilot.cloud.microsoft) (the old address, m365.cloud.microsoft, takes you there too). Look under your name:

- **Copilot Chat (Basic):** the free version. Everything in sections 1 to 6 works for you.
- **Anything with Premium, or Microsoft 365 Copilot:** the paid version. Do sections 1 to 6, then section 7.

On the free version, an agent can use its instructions and public websites at no cost. Agents that read your company's SharePoint or files may need the paid version or a pay as you go setting from your IT team. That's why today's agents carry everything they need inside their instructions.

Before you put company information into any AI tool, follow your company's AI policy.

### AI Agent Workshop

**Warm up: Agent or Not?**

Number a sheet 1 to 8. Mark each task **Chat** (ask once, done), **Agent** (a job you repeat the same way), or **Keep a human** (judgment, money, or safety calls). You have 4 minutes. Then add your numbers to the columns on the whiteboard, and be ready to defend one choice.

1. **Quality:** Summarize a new customer's 60 page supplier quality manual before Friday's kickoff.
2. **Sales:** Turn every RFQ email into a draft quote from the price list, for the estimator to review.
3. **Operations:** Answer second shift's questions from our 140 SOPs when no lead is on the floor.
4. **Shipping:** Decide whether to ship 2,000 scratched brackets so the customer's line doesn't go down.
5. **Maintenance:** Every morning at 6, flag any machine with more than 60 minutes of downtime yesterday.
6. **Quality:** Find the root cause of the cracked housings the customer sent back.
7. **Safety:** Walk a trainee through the C-12 conveyor lockout, one step at a time.
8. **Training:** Translate this week's toolbox talk into Spanish for second shift.

<details>
<summary><b>How we'd sort them</b> (open after the debrief)</summary>

- **Chat:** 1 and 8. One time jobs. Just ask Copilot.
- **Agent:** 2, 3, 5, and 7. The same job, done the same way, from written rules.
- **Keep a human:** 4 and 6. Judgment calls with a customer, money, or a root cause on the line.

The tricky ones:

- **8:** translate one talk once, and it's a chat. Every week, with your glossary written in, it's an agent.
- **7:** the agent coaches the written lockout steps. The trainee does every step and owns it.
- **5:** runs on its own every morning. That's the paid version.
- **4 and 6:** an agent can draft the deviation request or the 8D. A person makes the call.

Most real jobs split: the agent drafts, a person decides.

</details>

**1. Open Agent Builder**

If you've built a custom GPT in ChatGPT, this is the same idea in Copilot: a name, instructions, knowledge, and suggested prompts, shared with a link.

1. In Copilot, select **Agents** in the left pane, then **New agent**.
2. Select **Skip** (top right) to go straight to the form.
3. If a "No access" or "What's new" message pops up, select **Close** or **Got it**. The builder still works.
4. Fill in the name (click **New Agent** at the top and replace it), the description under it, and the instructions from step 2.

Don't see **New agent** under **Agents**? Your IT team may have turned agent building off. Use a Notebook instead: create one, paste the same instructions under **...** > **Instructions**, and follow along. Everything works the same except sharing.

**2. Demo agent: Example Equipment Co. Quote Desk**

Example Equipment Co. is the same fictional conveyor shop from Day 1. Its customers, prices, and quotes are made up.

| Field | Paste this |
|---|---|
| Name | Example Equipment Quote Desk |
| Description | Turns customer requests into draft quotes and reply emails for Example Equipment Co. |
| Instructions | Copy the block below |

<details>
<summary><b>Quote Desk starter instructions</b> (click to open, then copy)</summary>

One customer rule is missing on purpose. You'll find it in step 3.

```
Job: You are the Quote Desk for Example Equipment Co., a 60 person shop in West Michigan that builds custom conveyors for food processing and industrial plants. Estimators and sales staff use you to turn customer requests into draft quotes and reply emails. You draft. A person reviews and sends.

Steps for every request:
1. Check the request for what you need: conveyor length, conveyor type, the product it moves, and what to include. If anything is missing, list what's missing and ask. Don't draft a quote until you have it.
2. Find the customer below and apply every one of their requirements.
3. Draft the quote in the quote format below, using only the price list below.
4. If I ask for an email, draft a short reply to the customer. Never say it was sent.

Rules:
Never give a price that isn't on the price list. If an item is missing, write "Not on the price list, needs an estimate from engineering" and leave it out of the total.
Never offer or approve a discount, a rush date, or a change to terms. Say "That needs approval from the sales manager."
Every conveyor quote includes one motor and gearbox and 8 hours of engineering and drawings, even if the request doesn't mention them.
Always show the subtotal, the surcharge, and the total.
Always state the lead time and your assumptions.
If you're not sure about something, say so. Don't guess.

Price list (fictional, effective October 1, 2026):
Flat belt conveyor, painted carbon steel frame: $450 per foot
Flat belt conveyor, stainless steel frame: $1,000 per foot
Incline section, any frame (add on): $4,000 each
Motor and gearbox, 1 HP: $2,200 each
Motor and gearbox, 1 HP, washdown rated: $3,500 each
Safety guarding, painted: $125 per foot
Safety guarding, stainless: $250 per foot
Basic control panel (start, stop, e-stop, speed): $3,000 each
Engineering and drawings: $150 per hour
Recommended spare parts kit (belt, bearings, sprockets): $1,500 each

Customers:
Customer A, snack food plant.
Customer B, pet food plant: include a recommended spare parts kit in every quote.
Customer C, automotive parts plant: expects quotes within 3 business days. Terms are Net 45.

Pricing decision: through December 31, 2026, add a 5 percent material surcharge to every quote because steel prices went up.

Quote format:
Example Equipment Co., Quote (number to be assigned)
Date, Customer, Valid for: 30 days
Scope: one or two sentences
Table: Item, Qty, Unit price, Total
Subtotal, Material surcharge (5 percent), Total
Lead time: 8 to 10 weeks from approved drawings.
Assumptions: customer provides power to the control panel location. Freight and installation quoted separately.
Terms: Net 30 unless the customer has other terms. FOB our dock.

Style: Plain, direct language. Answer first.
```

</details>

<details>
<summary><b>Stuck? The missing rule</b> (open only after Prompt 1)</summary>

In the instructions, replace the line `Customer A, snack food plant.` with:

```
Customer A, snack food plant: requires stainless steel frames, stainless guarding, and washdown rated motors on every conveyor because of daily washdown.
```

Then select **Update**. The full, finished instructions are on the [Quote Desk](agents/quote-desk.md) page.

</details>

Then, under **Knowledge**, turn off **Web search**, so it answers from its instructions only. On the free version, **Add knowledge** only takes website links, which is why the price list lives in the instructions.

Under **Suggested prompts**, add these three:

| Title | Message |
|---|---|
| Quote a request | Quote a new customer request |
| What's missing? | What do you need from me to quote this? |
| Reply email | Draft my reply email for this quote |

To test before you save, switch **Configure** (top center) to **Preview**. Then select **Create**, and **Start chat**.

Names can be 30 characters at most. After you edit an agent, select **Update** (top right).

**3. Demo prompts**

Run them in this order. Prompt 1 shows the gap, then you fix it.

<details>
<summary><b>All demo prompts, in order</b> (click to open)</summary>

Prompt 1, Customer A (expect it to ask whether the frame should be painted or stainless, or to quote painted steel. Either way, it doesn't know Customer A's rule):

```
Draft a quote for this request:

From: Purchasing Manager, Customer A
Subject: Quote request, incline conveyor
Hi,
We need a quote for a 40 foot incline belt conveyor to move bagged snacks from our packing line up to the palletizer, about 600 bags per hour. Please include a control panel and guarding. We'd like the quote by Friday.
Thanks
```

Fix it: add the missing Customer A rule (open **Stuck?** in step 2), select **Update**, start a **new chat** with the agent, and send Prompt 1 again. Expect stainless, a washdown motor, and a total of $64,785.

Prompt 2, quote a request (expect Net 45 terms and a total of $36,907.50):

```
Draft a quote for this request:

From: Maintenance Manager, Customer C
Subject: Conveyor for our assembly line
Hi,
We need a 50 foot flat belt conveyor to move finished brackets from assembly to packing. Please include guarding and a basic control panel.
Thanks
```

Prompt 3, missing information (expect it to ask for the length before quoting):

```
Customer B needs another conveyor like last time, but longer. Quote it.
```

Prompt 4, stay in your lane (expect "That needs approval from the sales manager"):

```
Customer C says a competitor is 10 percent cheaper. Take 10 percent off the quote.
```

Prompt 5, do the whole job (expect the spare parts kit, a total of $26,407.50, a stated painted steel assumption, and a reply email that isn't sent):

```
Here's a new request. Check it against our customer requirements, draft the quote, then draft my reply email.

From: Plant Engineer, Customer B
Subject: Bagger to palletizer conveyor
Hi, we're adding a second line. We need a 30 foot flat belt conveyor to move filled bags of pet food from the bagger to the palletizer. Please include guarding and a basic control panel.
Thanks
```

</details>

**4. Share it**

Select **Share** (in the message after **Create**, or **...** at the top right of the builder). Add a coworker under **Add a name, group, or email**, or use **Copy chat link**. Leave **Org-wide sharing for chat access** off. Each person who opens it only sees what their own account can see.

To find your agents later, open **Agents** in the left pane. Your agents are listed at the top.

**5. Build your own agent**

Pick one:

- **A floor kit:** pick the one closest to your job. Each page has the name, description, instructions, suggested prompts, and three tests ready to paste.
- **Your own agent:** fill in the Agent Design Card below (2 minutes), then paste the interview prompt into a new Copilot chat and answer from your card. Copilot asks you six questions, one at a time, then writes your agent's name, description, instructions, suggested prompts, and three tests.

| Floor kit | Good for |
|---|---|
| [Line Troubleshooter](agents/line-troubleshooter.md) | Walking an operator through a conveyor problem, safety step first |
| [Quality Hold](agents/quality-hold.md) | Holding suspect cast parts, writing the hold tag and the notice to quality |
| [Safety and LOTO Coach](agents/safety-loto-coach.md) | Coaching the written lockout steps for one conveyor, one step at a time |
| [Shift Report Writer](agents/shift-report-writer.md) | Turning shift notes into your standard report |

More examples: [Quote Desk](agents/quote-desk.md) (the finished demo agent) and [New Hire Buddy](agents/new-hire-buddy.md).

<details>
<summary><b>Agent Design Card</b> (click to open, or download the <a href="files/Agent%20Design%20Card.docx">Word version</a>)</summary>

| Question | Your answer |
|---|---|
| The job: "When someone ___, the agent ___." | |
| Who uses it, and what do they type to start? | |
| What it knows: prices, steps, a format, contacts | |
| It always... | |
| It never... | |
| It hands off when... and to whom? | |
| A good answer looks like: length, format, tone | |
| Break test 1: something it can't know | |
| Break test 2: a number or setting it doesn't have | |
| Break test 3: skip a step or go outside its job | |
| Owner: who keeps it up to date? | |

**Is it a good job for an agent?** Score one point for each yes.

1. It repeats every week.
2. It follows the same steps every time.
3. The rules are written down.
4. What it needs fits in a page.
5. Mistakes are cheap to catch.
6. A person reviews it.
7. Someone owns it.

Five or more yeses? Build it this month. Fewer? Start with a Notebook instead.

</details>

<details>
<summary><b>Agent interview prompt</b> (click to open, then copy)</summary>

```
Help me design an AI agent in Copilot. Interview me first. Ask these questions one at a time, and wait for my answer before asking the next:

1. What one job should this agent do? Finish this sentence: "When someone ___, the agent ___."

2. Who will use it, and what will they type to start?

3. What does it need to know? (prices, steps, a format, contacts) Paste or describe it. What should it never use?

4. What rules must it always follow, and what must it never do?

5. When should it stop and hand off to a person, and who is that person?

6. What does a good answer look like? Length, format, and tone.

Keep each question short. If an answer is vague, ask one short follow up, then move on.

When the interview is done, write these five parts:

Name: 3 to 5 words.
Description: one sentence.
Instructions: plain text, under 8,000 characters, with these sections: Job, Steps, Rules, What you know, When to hand off, Style. Put everything from answer 3 under "What you know." Always include these two rules exactly as written:
Never invent numbers, prices, settings, dates, or part specs. If they're not in these instructions, say so.
If you're not sure about something, say so. Don't guess.
Suggested prompts: three short prompts a user would type, each with a 2 to 3 word title.
Break it: three test questions that try to make the agent guess, skip a safety step, or go outside its job.
```

</details>

Then trade laptops with a neighbor and try to break each other's agent: ask it something it can't know, ask it for a number it doesn't have, and ask it to skip a safety step. Fix one line at a time, select **Update**, and test again in a new chat.

**6. Skills: Teach Your Agent a Method**

The agent is the who. A skill is the how. Instructions say who the agent is and what it knows. A skill packages one repeatable method, like checking a quote, so it runs the same way every time. A skill is a file called SKILL.md, the same format Claude and Gemini use, so a skill you write once can travel.

Add a ready-made skill to your Quote Desk:

1. Download [quote-check SKILL.md](skills/quote-check/SKILL.md) (on the file page, select **Download raw file**).
2. Open the Quote Desk in Agent Builder: **Agents** > **New agent** > **My agents** > **Example Equipment Quote Desk**.
3. Under **Skills**, select **Add**, drop in SKILL.md, then select **Upload**.
4. Select **Update**, then **Start chat**.

Test it with a quote that has two mistakes (expect two fixes: painted guarding should be stainless, and the surcharge should be $2,835, for a total of $59,535):

```
Check this quote before I send it:

Customer A, 40 ft incline conveyor for bagged snacks. Valid 30 days.
Flat belt conveyor, stainless steel frame, 40 ft at $1,000: $40,000
Incline section, 1 at $4,000: $4,000
Safety guarding, painted, 40 ft at $125: $5,000
Motor and gearbox, 1 HP, washdown rated, 1 at $3,500: $3,500
Basic control panel, 1 at $3,000: $3,000
Engineering and drawings, 8 hrs at $150: $1,200
Subtotal $56,700. Material surcharge (5 percent) $2,500. Total $59,200. Lead time 8 to 10 weeks from approved drawings. Freight and installation quoted separately. Net 30.
```

Write your own skill without a file: in Agent Builder, select the arrow next to **Add** under **Skills**, then **Create with chat**. Replace the starter text with a description like this one, then select **Update**:

```
Create a skill called shift-handoff. Description: writes the end of shift handoff note for a conveyor line. Use it when someone asks for a handoff or shift note. Steps: ask for the line, the shift, and what happened (stops, fixes in progress, parts on order, safety issues). Then write the note in this format: Line and shift. Status: running or down. Issues and what was tried. Open items for the next shift. Safety. Keep it under 120 words. Never invent times, part numbers, or causes.
```

Up to 8 skills per agent. A skill belongs to one agent, so adding it to a second agent means adding it again.

**7. Premium: Agents That Act**

These need a paid Microsoft 365 Copilot license. Some also need your IT team to turn them on.

**Agent Builder drafts. Copilot Studio acts.** Everything you built today is Agent Builder: it answers and drafts when someone asks. When the agent needs to work in other systems, route approvals, or start on its own (for example, pull live prices from your ERP, send big quotes to the sales manager, and email the customer once approved), that's Copilot Studio. You don't start over: in Agent Builder, select **...** > **Copy to Copilot Studio**.

| Feature | What it does | Where to find it |
|---|---|---|
| Work knowledge in Agent Builder | Point an agent at SharePoint, OneDrive, Teams chats, or email, so it stays current on its own | Agent Builder > **Configure** > **Knowledge** |
| Researcher | Multi step research across the web and your work files, with a cited report. Up to 25 queries a month | Left pane, under **Agents** or **Tools** |
| Analyst | Reads a spreadsheet or CSV, writes and runs Python, and makes charts | Left pane, under **Agents** or **Tools** |
| Scheduled prompts | Runs a prompt for you on a schedule, up to 10 | Hover a prompt you sent > **Schedule this prompt** |
| Workflows Agent | Builds an automation from plain language, like "every Monday, post a summary in Teams" | Left pane > **Agents** > **Workflows Agent (Frontier)**, only if your company is in Microsoft's Frontier program |
| Copilot Cowork | Plans and carries out multi step tasks across your apps, asking before it acts | **Cowork** toggle next to **Chat**, only if your IT team set it up |
| Copilot Studio | Company wide agents with actions, approvals, triggers, and connections to other systems | In Agent Builder: **...** > **Copy to Copilot Studio** |

<details>
<summary><b>Premium demo prompts</b> (click to open)</summary>

Researcher (start it first, it takes 5 to 10 minutes):

```
Research what a food processing plant should check before buying a metal detector for a conveyor line: the standards that apply, the main detector types, and the questions to ask a supplier. Cite your sources.
```

Analyst: download [manufacturing_data_export_2026-05-01.csv](data/manufacturing_data_export_2026-05-01.csv), attach it, and ask (expect M-001, with 675 minutes of downtime and about a 2.0 percent defect rate, against 448 minutes and about 1.2 percent for M-002):

```
Compare machines M-001 and M-002 for April: total downtime, defect rate, and which one maintenance should look at first. Make a chart.
```

Then ask:

```
Is that the machine, or the shift it runs on?
```

Scheduled prompt (send it once, then hover it and select Schedule this prompt):

```
Summarize last week's emails and Teams messages about customer quotes. List anything that's waiting on me, oldest first.
```

</details>

**8. If Something Looks Different**

- **No New agent under Agents:** use a Notebook with the same instructions (see step 1).
- **"No access" message when the builder opens:** select **Close**. The builder still works.
- **Name cut off:** names can be 30 characters at most.
- **"License required" when opening a shared agent:** the person who built it added something the free version can't use, like SharePoint or email. Keep agents for free users to instructions and public websites.
- **Copilot Workspaces:** Microsoft is renaming Notebooks to Workspaces. Either works.
- **A change doesn't show up:** after editing an agent, select **Update** at the top right. It can take a few minutes.

---

## Day 3: Workflows and Your First Pilot
**Theme:** Turn your HQ, agents, and skills into repeatable workflows, and plan your first AI pilot

Materials coming soon. We'll shape this day around what you tell us at the end of Day 2.

---

# Tools Used in the Workshop

- Microsoft Copilot and Copilot Agent Builder
- Google Teachable Machine
- GitHub Codespaces (instructor demo)
- Claude (instructor demo)

---

# Audience

- Manufacturing leaders
- Engineers and technicians
- Process improvement teams
- Workforce development organizations

---

# For Instructors

Editable slide decks are in the [instructor](instructor) folder. When you change a deck, export a new PDF and upload both: the .pptx to `instructor/` and the PDF to `slides/` with the same file name as before, so the links above keep working.

- `Day1-Montcalm.pptx`
- `Day2-Montcalm.pptx`

---

*The memory structure in this training is adapted from Jeff Su's Cowork Toolkit ([coworkacademy.ai/toolkit](https://coworkacademy.ai/toolkit)).*
