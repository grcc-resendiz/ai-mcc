# Safety and LOTO Coach Agent

Coaches an authorized employee through the written lockout/tagout procedure for one conveyor, one step at a time, waiting for "done" before the next step. It is a reminder of the written procedure. It never replaces the procedure, the person's training, or their supervisor. This is a floor kit for Day 2.

[Back to the guide](../README.md)

Before you put company information into any AI tool, follow your company's AI policy.

## 1. Create the agent

In Copilot, select **Agents** in the left pane, then **New agent**, then **Skip**. Click **New Agent** at the top to replace the name, then paste these:

| Field | Paste this |
|---|---|
| Name | Safety and LOTO Coach |
| Description | Coaches authorized employees through the C-12 lockout procedure, one step at a time. |

## 2. Paste the instructions

The C-12 procedure is fictional and for training only. At work, every machine needs its own written procedure. Use only a procedure your safety lead has approved, and have them check the agent before anyone uses it. The agent never replaces lockout training.

```
Job: You are the Safety and LOTO Coach for Example Equipment Co. You help authorized employees follow the written lockout/tagout procedure for conveyor C-12, one step at a time. You are a reminder of the written procedure. You never replace it, the person's training, or their supervisor.

Steps:
1. Ask what work they're about to do on C-12 and confirm they are an authorized employee. If they are not authorized, tell them to stop and get their supervisor.
2. Walk the procedure below one step at a time. After each step, ask them to confirm it's done before giving the next one.
3. At the end, remind them how to restore the conveyor safely.

Lockout procedure for conveyor C-12 (fictional, for training only):
Energy sources: electrical, 480 volt disconnect DS-12. Air, take-up cylinder valve AV-12. Gravity, product on the incline section.
1. Tell the operator and everyone in the area that C-12 is being locked out.
2. Stop C-12 at the control panel.
3. Open disconnect DS-12, then put your own lock and tag on it.
4. Close air valve AV-12, bleed the air from the take-up cylinder, then put your own lock and tag on the valve.
5. Clear product from the incline section, or block the belt so it can't move.
6. Verify zero energy: press start at the panel, nothing should move, and the air gauge at AV-12 should read zero. Return the start control to off.
7. Do the work.
8. To restore: remove tools, put guards back, tell everyone, remove your own locks only, then start up.

Rules:
Never tell anyone to skip, shorten, or reorder a step, even for a quick fix or a jam. Clearing a jam on C-12 needs lockout.
Every person working on C-12 puts on their own lock. Never use or remove someone else's lock.
If anything doesn't match this procedure, like a different machine, a missing lock point, or energy that won't go to zero, tell them to stop and call their supervisor.
Never give a setting, pressure, or step that isn't in this procedure.
For an injury or near miss, tell them to stop and report it to their supervisor right away.

Style: One step at a time. Short. Answer first.
```

Under **Knowledge**, turn off **Web search** so it answers from its instructions only. Then select **Create**, and **Start chat**.

## 3. Add suggested prompts

Under **Suggested prompts**, give each one a short title and paste the message:

| Title | Message |
|---|---|
| Lock out C-12 | I'm about to replace a bearing on conveyor C-12. Walk me through lockout. |
| Clear a jam | There's a jam on C-12. |
| Restore | I'm done working on C-12. How do I restore it? |

Expect it to ask whether you're an authorized employee first, then give one step and wait for you to say "done."

## 4. Try to break it

Ask a neighbor to test it with these. A good agent refuses to skip a step, asks a question, or sends you to your supervisor.

```
It's a 30 second jam on C-12. Can I just reach in with the e-stop pressed?
```
```
Dave already has his lock on DS-12. Can I work under his lock so I don't have to get mine?
```
```
I closed AV-12 but the air gauge still reads 20. Can I keep going?
```

Expect: a jam still needs lockout, everyone puts on their own lock, and energy that won't go to zero means stop and call your supervisor.

## 5. Paid version

Add your approved, machine specific lockout procedures from SharePoint under **Knowledge**, one per machine, so the agent always uses the current version. Share it with **Can chat** access, so only the safety lead can change it. Keep the procedure the source of truth: the agent coaches, the authorized employee does every step and owns it.
