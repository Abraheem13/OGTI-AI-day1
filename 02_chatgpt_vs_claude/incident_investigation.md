# 🚨 ChatGPT vs Claude — Incident Investigation Summaries

**Time required:** 25–30 minutes
**You will use:** Both `chat.openai.com` and `claude.ai`
**Sample data:** [`sample_data/incident_field_notes.txt`](sample_data/incident_field_notes.txt)

---

## 🎯 What you will learn

1. Turn raw inspector field notes into a structured root-cause analysis
2. Apply the **5-Whys** and **fishbone (Ishikawa)** frameworks via AI
3. Generate a regulator-facing disclosure and a crew-facing toolbox talk from the same facts
4. Catch AI hallucination in safety-critical contexts (where it matters most)

---

## ⚠️ Pre-flight: this is the highest-risk module

Incident reports are **legally significant**. They can be subpoenaed, audited, used in court. Mistakes in attribution, sequence, or quantity have professional and legal consequences.

**Three rules for this module:**

1. **Never** paste a real incident report into a public AI before OGRA disclosure
2. **Always** verify every named person, date, and quantity in the AI output
3. **Never** sign or submit an AI-drafted incident report without a human review pass

---

## 🧪 Exercise 1 — From Field Notes to Structured Report

**Setup:**
1. Open `sample_data/incident_field_notes.txt`
2. Copy the contents
3. Paste into both ChatGPT and Claude (new chats in each)

**Run this prompt in both:**

```text
You are a senior HSE investigator at a Pakistani downstream operator. I am pasting 
inspector field notes from a near-miss incident at a refinery. The notes are raw 
and partially anonymised with placeholders.

Produce a structured incident report covering:
1. Incident at a Glance (date, location, severity, persons affected)
2. Sequence of Events (chronological, in 60 seconds of reading)
3. Immediate Actions Taken (what the crew did right; what could be improved)
4. Root Cause Analysis using the 5-Whys framework — show each "Why" explicitly
5. Contributing Factors (procedural, human, environmental, equipment)
6. Corrective and Preventive Actions (CAPA) as a table with: Action / Owner / Target Date
7. Lessons Learned (one paragraph, audience: technical leadership)
8. Recommended Regulatory Disclosure Path (OGRA Section 26 / PEPA / internal only)

Tone: factual, third-person, no first-person pronouns. British English.

CRITICAL: Do not invent names, dates, quantities, or facts that are not in the notes. 
Use [NAME], [DATE], [QUANTITY] placeholders for missing data. If a section cannot 
be completed from the notes, write "Insufficient data — requires additional inspection".
```

---

## 🧪 Exercise 2 — Apply the Fishbone Framework

**Continue in the same chat in both tools:**

```text
Now produce an Ishikawa (fishbone) diagram for this incident, in text format. 
Use the standard 6M categories:
- Manpower (people, training, fatigue)
- Method (procedures, SOPs)
- Machine (equipment, maintenance)
- Material (corrosion, quality)
- Measurement (inspection, monitoring)
- Mother Nature / Environment (weather, working conditions)

For each category list 2–4 specific contributing factors from the field notes.
End with the top 3 factors most likely to be the true cause.
```

**Compare:** Does ChatGPT or Claude do a better job of staying disciplined within the framework?

---

## 🧪 Exercise 3 — Three Audiences, One Incident

This is where the tools' personalities really show. Run this prompt in both:

```text
From the structured report above, produce three different communications using 
the same facts:

A) A 150-word formal disclosure draft for OGRA Section 26 filing. 
   Third person, regulator-facing register. Conservative tone.

B) A 100-word toolbox-talk script the shift supervisor will read aloud to the 
   crew tomorrow morning. Plain English, second-language-friendly, one clear 
   instruction at the end.

C) A 60-word internal note to the GM (Operations) — bullets only — covering 
   what happened, what we did, what's next, and any risk to weekly production.

Clearly label each output A, B, C.
```

**Compare side-by-side:**

| Audience | ChatGPT strength | Claude strength |
|----------|-----------------|-----------------|
| Regulator (A) | Often punchier | Tends to be more careful with hedging |
| Crew (B) | Plain English usually good | Sometimes too formal |
| GM (C) | Tight bullets | Sometimes adds caveats the GM doesn't need |

---

## 🧪 Exercise 4 — The Hallucination Hunt

**This is the most important exercise of the module.** Run this in both tools:

```text
Based on this incident, what specific OGRA notification deadlines and Section 
26 disclosure obligations apply? List the exact section number, the deadline 
in hours, and what must be included in the notification.
```

**Then immediately:**

1. Open `ogra.org.pk` in another tab
2. Search for the section number the AI gave you
3. **Confirm whether it actually says what the AI claims**

You may find:
- ✅ The section exists and the AI got it right → great
- ⚠️ The section exists but says something subtly different → AI partially wrong, dangerous
- 🚨 The section number doesn't exist at all → pure hallucination

**Every single time you cite a regulation in a real document, this verification step is non-negotiable.**

---

## 📝 Sign-off discipline

For any AI-drafted incident document, **adopt this 4-step sign-off**:

1. **Author check** — read every line; replace every placeholder; verify every name
2. **Source check** — verify every quoted regulation, deadline, and figure
3. **Audience check** — would I be comfortable if this exact text appeared in court?
4. **Manual signature** — your signature, your accountability. AI cannot be liable; you can.

---

## ✅ Module 02 complete

1. Take **Quiz 2** in [`../quizzes/quiz_2_chatgpt_claude.html`](../quizzes/quiz_2_chatgpt_claude.html)
2. Move to **Module 03 — Prompt Engineering** in [`../03_prompt_engineering/README.md`](../03_prompt_engineering/README.md)
