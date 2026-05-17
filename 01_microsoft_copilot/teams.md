# 👥 Microsoft Copilot — Teams

**Time required:** 15–20 minutes
**You will use:** Microsoft Teams desktop or web (M365 Copilot licence required)
**You will need:** Access to a Teams meeting with the **transcript** turned on, or watch the instructor demo

---

## 🎯 What you will learn

1. Get a meeting recap without watching the whole replay
2. Extract decisions attributed to specific named attendees
3. Build an action-item tracker from a meeting you missed

---

## 🧭 Prerequisites — turn on transcription

Copilot in Teams only works if **transcription is enabled** during the meeting. To enable:

1. In a Teams meeting, click **More actions (...)** → **Record and transcribe** → **Start transcription**
2. Inform every participant that transcription is on (consent requirement)
3. After the meeting, the transcript and recording appear in the **Recap** tab

> ⚠️ **Pakistan-specific note:** For sensitive meetings (JV negotiations, vendor selection, internal HSE incidents), discuss with your legal/IT team **before** enabling transcription. The transcript is data — and falls under your tenant's data-residency policy.

---

## 🧪 Exercise 1 — Meeting Recap

After a meeting has ended:

1. Go to the **Recap** tab in the meeting (or Chat → meeting → Recap)
2. Click "Copilot" in the side pane

**Run this prompt:**

```text
Give me a 5-bullet recap of this meeting. Cover:
1. The main topic
2. The two or three key decisions made
3. Any disagreements that surfaced and how they were resolved
4. Action items by named owner
5. The next checkpoint date

Keep it under 150 words.
```

---

## 🧪 Exercise 2 — Decisions by Attendee

```text
List every decision made in this meeting. For each decision:
- The decision (one sentence)
- Who proposed it
- Who agreed or disagreed
- Whether it was finalised or deferred

Format as a markdown table.
```

**Verify:** Does the table attribute statements to the **right** speaker? Speaker identification in Teams is normally good for clear audio but can mis-attribute when two people talk over each other.

---

## 🧪 Exercise 3 — Catch-Up If You Missed the Meeting

```text
I missed this meeting. In 3 minutes of reading, brief me on:
- What I missed that affects MY team
- Any decisions made about my projects (assume my projects are pipeline-integrity and HSE)
- Any commitments made on my behalf, by anyone
- What I need to do before the next meeting
```

---

## 🧪 Exercise 4 — Build an Action Tracker

```text
Extract all action items from this meeting. For each:
- Owner (named person, not "team")
- Action (specific verb-led description)
- Deadline (only if stated; otherwise "TBD")
- Dependency (if it requires someone else to act first)

Output as a markdown table I can paste into a tracking spreadsheet.
```

---

## 🚨 Watch out for these

| Issue | Why it happens | How to handle |
|-------|----------------|---------------|
| Wrong speaker attribution | Two people talking over each other | Verify against video for critical quotes |
| Action with no owner | Generic "the team will…" phrases | Re-prompt: *"For each unowned action, suggest the most likely owner based on context"* |
| Decisions that weren't actually decisions | A senior person musing aloud, not committing | Always confirm critical decisions in writing afterwards |
| Sensitive negotiations leaked into the recap | Anyone with meeting access can read it | Disable transcription for confidential meetings; or restrict Recap access |

---

## 📝 Self-check

- [ ] I can extract a 5-bullet recap of a meeting I didn't attend
- [ ] I can list every named decision with proposer and agreer
- [ ] I have a paste-able action tracker
- [ ] I know **when not** to enable transcription

---

## ✅ Module 01 complete — what's next?

1. Take **Quiz 1** in [`../quizzes/quiz_1_copilot.html`](../quizzes/quiz_1_copilot.html)
2. Move to **Module 02 — ChatGPT vs Claude** in [`../02_chatgpt_vs_claude/README.md`](../02_chatgpt_vs_claude/README.md)
