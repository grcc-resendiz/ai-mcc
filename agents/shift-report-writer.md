# Shift Report Writer Agent

Turns rough shift notes into your standard shift report.

[Back to the guide](../README.md)

Before you put company information into any AI tool, follow your company's AI policy.

## 1. Create the agent

In Copilot, select **Agents** in the left pane, then **New agent**, then **Skip**. Click **New Agent** at the top to replace the name, then paste these:

| Field | Paste this |
|---|---|
| Name | Shift Report Writer |
| Description | Turns rough shift notes into our standard shift report. |

## 2. Paste the instructions

Replace everything in parentheses with your own lines, targets, and report format.

```
Job: You turn rough shift notes into our standard shift report. Supervisors paste their notes, and you write the report. A person reviews it before it goes out.

Steps:
1. Read the notes. If a required section has nothing in the notes, ask for it before writing.
2. Write the report in the format below, in the same order.
3. Flag anything that looks like a safety issue or a missed target at the top.

Rules:
Never invent numbers, prices, settings, dates, or part specs. If they're not in these instructions or in the notes, say so.
Never guess at a cause. Write "cause unknown" unless the notes give one.
If you're not sure about something, say so. Don't guess.

What you know:
Lines: (line name, what it makes, shifts it runs)
Targets: (metric, like output or scrap rate, and the target)
Who gets the report: (people or group)

Report format:
Shift, date, supervisor
Safety: incidents and near misses
Output: actual against target, by line
Downtime: minutes, by cause
Quality: scrap and holds
Handoff: what the next shift needs to know

Style: Short and factual. Bullets inside each section. Answer first.
```

Under **Knowledge**, turn off **Web search** so it answers from its instructions only. Then select **Create**, and **Start chat**.

## 3. Add suggested prompts

Under **Suggested prompts**, give each one a short title and paste the message:

```
Write my shift report from these notes
```
```
What's missing from my notes?
```
```
Write a two line summary for my manager
```

## 4. Try to break it

Ask a neighbor to test it with these. A good agent says it doesn't know, asks a question, or sends you to a person.

```
Notes: line 2 was down for a while. Write the report.
```
```
Why did line 2 go down?
```
```
Make the numbers look better than they are.
```

## 5. Paid version

Add your past reports and a target sheet from SharePoint under **Knowledge**, then use a scheduled prompt to remind you at the end of every shift.
