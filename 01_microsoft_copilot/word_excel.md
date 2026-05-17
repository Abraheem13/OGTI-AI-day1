# 📄 Microsoft Copilot — Word & Excel

**Time required:** 30–35 minutes (15 min Word + 15-20 min Excel)
**You will use:** Word and Excel (M365 Copilot licence required)
**Sample data:** 
- [`sample_data/hse_field_notes.txt`](sample_data/hse_field_notes.txt) — for Word exercise
- [`sample_data/well_production_data.csv`](sample_data/well_production_data.csv) — for Excel exercise

---

## Part A — Word: From Rough Notes to a Board-Ready Report

### 🎯 What you will learn

1. Convert raw inspector field notes into a structured 2-page HSE report
2. Auto-generate a Table of Contents
3. Rewrite the same content for different audiences (board, crew, regulator)

---

### 🧭 How to access Copilot in Word

1. Open Word
2. Create a **new blank document**
3. Look for the **Copilot icon** in the ribbon, top-right
4. Click it — you'll see a "Draft with Copilot" prompt box on each new line

---

### 🧪 Exercise 1 — Notes to Report

**Setup:**
1. Open `sample_data/hse_field_notes.txt` and copy the contents
2. In Word, paste the notes into the document
3. Place your cursor at the top of the document
4. Click "Draft with Copilot"

**Run this prompt:**

```text
Using these field inspection notes, draft a formal 2-page HSE incident report. Structure:

1. Executive Summary (3 lines)
2. Incident Overview (date, location, time, severity)
3. Root Cause Analysis (use the 5-Whys framework)
4. Immediate Actions Taken
5. Corrective and Preventive Actions (CAPA) — table format with: action, owner, target date
6. Lessons Learned
7. Recommendations for OGRA filing

Tone: formal, suitable for board review.
Length: approximately 2 pages.
British English.

Do not invent names, dates or quantities. Where the notes are ambiguous, use placeholders like [NAME], [DATE], [QUANTITY].
```

---

### 🧪 Exercise 2 — Add a Table of Contents

Once you have the draft, place your cursor at the top of the document and:

1. **References → Table of Contents → Automatic Table 1**, OR
2. Ask Copilot directly: *"Add a Table of Contents at the top of this document with all my headings."*

---

### 🧪 Exercise 3 — Rewrite for a Different Audience

With the report open, select the **Executive Summary** paragraph and ask Copilot:

```text
Rewrite this Executive Summary for the field crew — plain English, max 80 words, 
read-aloud-able at a toolbox talk. Avoid jargon. End with the one thing the crew 
must do differently tomorrow.
```

Then select it again and ask:

```text
Now rewrite this same summary as a one-paragraph OGRA Section 26 disclosure — 
formal, regulator-facing tone, third person, no first-person pronouns.
```

**Compare all three versions side-by-side.** This is the single most powerful demonstration of why Copilot is valuable for senior managers: same facts, three audiences, three minutes.

---

## Part B — Excel: Production Anomalies in Natural Language

### 🎯 What you will learn

1. Ask Excel questions in plain English — no formulas needed
2. Flag week-on-week pressure drops above a threshold
3. Add trend columns and visual highlights
4. Get a written summary of which wells to investigate

---

### 🧭 Setup

1. Open `sample_data/well_production_data.csv` in Excel
2. **Convert it to a Table:** Select all data → Insert → Table → tick "My table has headers"
3. The Copilot icon appears in the Home ribbon — click it

---

### 🧪 Exercise 4 — Find Anomalies

**Run this prompt:**

```text
Highlight all rows where the Week-on-Week Pressure Change is below -5%. 
Use light red fill for those rows.
```

---

### 🧪 Exercise 5 — Add a Trend Column

```text
Add a new column called "Trend (4 weeks)" that classifies each well as: 
"Declining" (more than -3% average), "Stable" (-3% to +3%), or "Improving" (above +3%).
```

---

### 🧪 Exercise 6 — Investigate

```text
Based on this data, which three wells deserve immediate investigation? 
For each well give:
1. The specific concern (one sentence)
2. The data points supporting it
3. The recommended next action (engineering / well intervention / monitoring)

Format as a numbered list.
```

---

### 🚨 Excel Copilot caveats

| Behaviour | What it really means |
|-----------|---------------------|
| Confident percentage-change figures | Always verify on a sample row — Copilot occasionally rounds inconsistently |
| Trend predictions | These are **pattern recognition**, not reservoir engineering. Treat as triage, not diagnosis. |
| "Insert chart" suggestions | The chart type may not be the most informative; experiment with bar / line / heatmap |

---

## 📝 Self-check — before moving on

- [ ] My HSE report has a Table of Contents
- [ ] The Executive Summary exists in three audience versions (board, crew, regulator)
- [ ] My Excel table highlights wells with material pressure drops
- [ ] I have three named wells to investigate, with one-sentence justifications

---

## ➡️ Next step

Move on to [`teams.md`](teams.md) for the meeting-recap exercise.
