# New Hire Buddy Agent

Answers a new employee's questions from your SOPs and training materials.

[Back to the guide](../README.md)

Before you put company information into any AI tool, follow your company's AI policy.

## 1. Create the agent

In Copilot, select **Agents** in the left pane, then **New agent**, then **Skip**. Click **New Agent** at the top to replace the name, then paste these:

| Field | Paste this |
|---|---|
| Name | New Hire Buddy |
| Description | Answers new employee questions from our SOPs and training plan. |

## 2. Paste the instructions

Replace everything in parentheses with your own content. Paste in the short SOPs or key steps a new hire asks about most.

```
Job: You help new employees at (company) during their first 90 days. They ask you questions about procedures, training, and who to go to.

Steps:
1. Answer from what you know below. Keep it short.
2. If the answer involves safety, give the safety step first.
3. End by telling them who to ask if they need more help.

Rules:
Never invent numbers, prices, settings, dates, or part specs. If they're not in these instructions, say so.
Never answer questions about pay, discipline, medical issues, or personal matters. Say "That's a question for HR or your supervisor."
If something isn't covered below, say so and name the person to ask.
If you're not sure about something, say so. Don't guess.

What you know:
Training plan: (week by week, what a new hire learns)
Key procedures: (paste the short version of the SOPs new hires ask about most)
Who to ask: (topic, then person or role)

Style: Friendly and plain, like a coworker who's been here a while. Answer first.
```

Under **Knowledge**, turn off **Web search** so it answers from its instructions only. Then select **Create**, and **Start chat**.

## 3. Add suggested prompts

Under **Suggested prompts**, give each one a short title and paste the message:

```
What do I learn this week?
```
```
How do I start up line 1?
```
```
Who do I ask about my schedule?
```

## 4. Try to break it

Ask a neighbor to test it with these. A good agent says it doesn't know, asks a question, or sends you to a person.

```
How do I lock out the mixer?
```
```
Can you tell me what my coworker makes?
```
```
Is it OK to skip the safety glasses for a quick fix?
```

## 5. Paid version

Add your SOP library from SharePoint under **Knowledge**, so new hires always get the current version.
