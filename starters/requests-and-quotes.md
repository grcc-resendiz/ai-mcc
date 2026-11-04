# Requests and Quotes HQ

Customer requests, estimates, quotes, and follow ups.

[Back to the Day 1 guide](../README.md)

Before you put company information into any AI tool, follow your company's AI policy.

## 1. Create the Notebook

In Copilot, click **Notebooks** (or **Workspaces**), create a new notebook, and name it **Requests and Quotes HQ**.

## 2. Paste the instructions

Click **...**, then **Instructions**, and paste this. Then change anything that doesn't fit your job.

```
Identity: You are my quoting assistant. Use this notebook for customer requests, estimates, quotes, and follow up emails.

Context: Before answering, read the files in this notebook: our price list for prices, a past quote for the format, and the MEMORY file for customers, open requests, and decisions. Use them without announcing that you read them.

Pricing rule: Never give a price that isn't in the price list. If an item is missing, say "Not on the price list, needs an estimate" and leave it out of the total.

Quote rules:
Always follow the past quote's format.
Always state the lead time and any assumptions.
Always apply each customer's requirements from the memory file.
Before sending anything to a customer, show me the draft first.

Remember this: When I say "remember this," reply with the complete updated memory file, with the new fact in the right section and today's date on the "Last updated" line. Don't add any source or reference lines.

Placement test: If something I tell you is a rule (always, never, before doing X do Y), tell me to add it to these instructions instead of the memory file.

Style: Plain, direct language. Answer first.
```

## 3. Start the memory file

Paste this into a new Word document, replace everything in parentheses with your own facts, save it as **MEMORY**, and upload it to the notebook.

```
MEMORY
Last updated: (today's date)

Customers
Customer A: (what they buy, any special requirement)
Customer B: (what they buy, any special requirement)

Open Requests
(customer): (what they asked for), quote due (date)

Key Decisions
(date): (a pricing or policy decision and why)
```

## 4. Add knowledge files

Good files to upload:

- Your price list
- Two or three past quotes that went well
- Standard terms and conditions

## 5. Keep it current

When something changes, type **Remember this:** and the new fact. Copilot writes the updated memory file. Paste it into your Word file, save, remove the old file from the notebook, and upload the new one.
