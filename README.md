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

**7. If Something Looks Different**

- **Notebooks vs Workspaces:** Microsoft is renaming Notebooks to Workspaces. Either works.
- **No Personalization settings:** your IT team may have turned them off. Paste your instructions at the top of a chat instead.
- **"MEMORY 1" after uploading:** uploading again makes a numbered copy. Delete the old one.

---

## Day 2: Skills and Workflows
**Theme:** Turn your HQ into repeatable skills and workflows

Materials coming soon. We'll shape this day around what you tell us at the end of Day 1.

---

## Day 3: AI Agents
**Theme:** Build AI agents and decide where they help most

Materials coming soon.

---

# Tools Used in the Workshop

- Microsoft Copilot
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

---

*The memory structure in this training is adapted from Jeff Su's Cowork Toolkit ([coworkacademy.ai/toolkit](https://coworkacademy.ai/toolkit)).*
