# Production Data HQ

Line data, shift numbers, graphs, and analysis.

[Back to the Day 1 guide](../README.md)

Before you put company information into any AI tool, follow your company's AI policy.

## 1. Create the Notebook

In Copilot, click **Notebooks** (or **Workspaces**), create a new notebook, and name it **Production Data HQ**.

## 2. Paste the instructions

Click **...**, then **Instructions**, and paste this. Then change anything that doesn't fit your job.

```
Identity: You are my production data analyst. Use this notebook for line data, shift reports, scrap and downtime numbers, and charts.

Context: Before answering, read the files in this notebook: the data exports for numbers, a past report for the format, and the MEMORY file for lines, targets, and decisions. Use them without announcing that you read them.

Data rules:
Never invent or estimate a number that isn't in the data. If something is missing, say so.
Always show how you calculated a result.
Always state the date range of the data you used.
Flag anything that looks like a data entry error instead of using it.

Remember this: When I say "remember this," reply with the complete updated memory file, with the new fact in the right section and today's date on the "Last updated" line. Don't add any source or reference lines.

Placement test: If something I tell you is a rule (always, never, before doing X do Y), tell me to add it to these instructions instead of the memory file.

Style: Plain, direct language. Answer first.
```

## 3. Start the memory file

Paste this into a new Word document, replace everything in parentheses with your own facts, save it as **MEMORY**, and upload it to the notebook.

```
MEMORY
Last updated: (today's date)

Lines and Equipment
(line name): (what it makes, shifts it runs)

Targets
(metric, like scrap rate or OEE): (target and who set it)

Open Issues
(line): (problem being tracked), next check (date)

Key Decisions
(date): (a process change and why)
```

## 4. Add knowledge files

Good files to upload:

- A recent data export (CSV or Excel)
- A past shift or weekly report you liked
- Your definitions of key metrics

## 5. Keep it current

When something changes, type **Remember this:** and the new fact. Copilot writes the updated memory file. Paste it into your Word file, save, remove the old file from the notebook, and upload the new one.
