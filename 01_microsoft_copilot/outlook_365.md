# 📧 Microsoft Copilot — Outlook 365

**Time required:** 20–25 minutes
**You will use:** Outlook for the web or Outlook desktop (M365 Copilot licence required)
**Sample data:** [`sample_data/sample_email_thread.txt`](sample_data/sample_email_thread.txt)

---

## 🎯 What you will learn

1. Triage a long email thread without reading every message
2. Extract action items by person
3. Draft a professional reply in your own tone
4. Compose an escalation email when a deadline slips

---

## 🧭 How to access Copilot in Outlook

1. Open **Outlook on the web** at `outlook.office.com` and sign in with your work account
2. Open any email thread
3. Look for the **Copilot icon** (a small badge with diagonal lines) near the top-right of the message or in the ribbon
4. Click it to open the side pane

If you don't see the icon:
- Confirm your licence with IT (you need M365 Copilot add-on, not just basic M365)
- Try the **mobile Outlook app** — Copilot is rolled out there too

---

## 🧪 Exercise 1 — Summarise a Long Thread

**Scenario:** A pipeline-delay thread from SNGPL has 14 emails over 3 days. You need to brief your GM in 60 seconds before the 10:30 meeting.

**Setup:**
1. Open `sample_data/sample_email_thread.txt`
2. Copy the contents into a draft email (or use a real long thread you've handled)
3. Open Copilot in the side pane

**Run this prompt:**

```text
Summarise this thread for my GM. Highlight:
1. What is the original problem?
2. What decisions have been taken so far, and by whom?
3. What is still outstanding?
4. Who is the bottleneck right now?
Keep it under 120 words.
```

**Critical check:**

- ✅ Does the summary attribute actions to the correct person?
- ✅ Does it surface the *real* bottleneck, not just the last sender?
- ❌ Does it invent a deadline or a name not in the thread? → flag it and re-run

---

## 🧪 Exercise 2 — Extract Action Items

**Same thread. Run this prompt:**

```text
Extract all action items from this thread. For each:
- Who is responsible (full name)
- What they must do (one sentence)
- By when (only if explicitly mentioned)
- Status: pending / in-progress / blocked

Format as a markdown table.
```

**What to verify:** Copilot occasionally **invents** deadlines that look reasonable but were never in the thread. Read every row.

---

## 🧪 Exercise 3 — Draft a Professional Reply

**Run this prompt:**

```text
Draft a reply from me confirming our next steps. Tone: senior manager, polite but firm. 
Length: 80–120 words. Structure:
1. Acknowledge the delay
2. Reiterate our two non-negotiables (safety clearance, OGRA compliance)
3. Propose a Friday 4 PM call with all parties
4. Sign off professionally

Do not invent any data. Use placeholders [PROJECT] and [DATE] if details are missing.
```

---

## 🧪 Exercise 4 — Compose an Escalation

**Scenario:** The vendor has missed the deadline twice. You need to escalate to the Director (Operations) — copying your GM — but without burning the relationship.

**Run this prompt:**

```text
Draft an escalation email from me to the Director (Operations), with my GM in CC. Context: the contractor [VENDOR-X] has missed the pipeline integrity inspection deadline twice. 

Required tone: serious but professional — this is a relationship I want preserved.
Required content:
1. Factual recap of missed dates
2. Operational risk of further delay
3. Specific ask: Director's intervention to convene a meeting this week
4. Offer of three time slots

Length: under 200 words. British English. No emojis.
```

---

## 🚨 Red-flag behaviours to watch for

| Copilot behaviour | What to do |
|-------------------|------------|
| Mentions a person not in the thread | Delete that line; re-run with stricter prompt |
| Invents a date or figure | Replace with `[DATE]` or `[FIGURE]`; re-run |
| Adds an emoji or casual phrase | Rewrite manually — escalations don't joke |
| Quotes someone in a way they didn't say | Never forward without verifying |

---

## 📝 Reflection — write down before moving on

1. What did Copilot do better than I expected?
2. What did Copilot get wrong that I caught?
3. Would I trust this thread summary to brief my GM directly, or would I always edit it first?

---

## ➡️ Next step

Move on to [`word_excel.md`](word_excel.md) for the HSE report and production data exercises.
