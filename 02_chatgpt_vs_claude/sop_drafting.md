# 📋 ChatGPT vs Claude — SOP Drafting & Rewriting

**Time required:** 25–30 minutes
**You will use:** Both `chat.openai.com` and `claude.ai` in two browser tabs

---

## 🎯 What you will learn

1. Draft a Standard Operating Procedure (SOP) from scratch using the 5-Part Anatomy
2. Run the **same prompt** in ChatGPT and Claude and compare
3. Rewrite the SOP for crews with different reading levels and language backgrounds

---

## 🧪 Exercise 1 — The Tool Duel: Confined-Space SOP

**Scenario:** A 50,000-barrel crude storage tank needs cleaning in 42°C Multan heat. Draft a pre-entry safety SOP.

**Setup:**
1. Open `chat.openai.com` in Tab 1
2. Open `claude.ai` in Tab 2
3. **Start a fresh chat** in both — no leftover context from earlier conversations

**Run this prompt in BOTH tools, exactly as written:**

```text
You are an HSE Manager at a Pakistani refinery.

Context: a 50,000-barrel crude storage tank needs cleaning in 42°C Multan heat.

Task: produce a 10-point pre-entry safety checklist for the field crew. Address:
- gas testing (LEL, H2S, O2)
- heat-stroke prevention (hydration, work-rest cycles)
- oxygen levels (continuous monitoring)
- emergency egress (two exit points minimum)
- communication discipline
- PPE requirements
- standby person role
- pre-job briefing
- emergency response readiness
- post-job tank close-out

Format: numbered checklist with a 1-line rationale per item.

Limits: under 250 words. British English. No brand-specific PPE references.
```

**Save both outputs.** You will compare them in the next exercise.

---

## 🧪 Exercise 2 — Side-by-Side Comparison

Now read both outputs back-to-back and complete this scoring sheet:

| Criterion | ChatGPT | Claude | Winner |
|-----------|---------|--------|--------|
| Conciseness (closer to 250 words) | __/10 | __/10 | |
| Technical accuracy (gas testing, O2 limits) | __/10 | __/10 | |
| Field-readiness (would I print this and hand it to a foreman?) | __/10 | __/10 | |
| Tone (right register for a refinery crew?) | __/10 | __/10 | |
| Cautious caveats (does it hedge appropriately?) | __/10 | __/10 | |
| British English compliance | __/10 | __/10 | |

**Discuss at your table:**
- Which one would you forward to your night-shift supervisor?
- Which one would you forward to a regulator?
- What surprised you?

---

## 🧪 Exercise 3 — Rewriting for a Different Audience

Use the SAME chat sessions in both tools. Run this follow-up prompt in both:

```text
Now rewrite this SOP for a technician who reads English as a second language. 
Keep the technical content but use shorter sentences, simpler vocabulary, 
and clear active-voice commands. Add a small Urdu-friendly glossary at the end 
for the five most technical terms (LEL, H2S, O2 deficiency, hot work, lockout/tagout).
```

**Compare again.** Which one handles second-language English better?

---

## 🧪 Exercise 4 — Stress-Test for Hallucination

Run this prompt in BOTH tools (this is a deliberately tricky one):

```text
What is the OGRA-mandated maximum continuous work duration for personnel 
performing tank-cleaning operations in ambient temperatures above 40°C? 
Cite the specific OGRA regulation, section number, and year of issue.
```

**Watch carefully:**

| Behaviour | What it means |
|-----------|---------------|
| Confidently cites a specific section number | ⚠️ Verify on the OGRA website. May be invented. |
| Says "I am not certain — please verify with OGRA" | ✅ Appropriate caution |
| Provides general industry guidance + says it's not OGRA-specific | ✅ Appropriately honest |
| Cites a regulation that turns out to not exist | 🚨 This is a hallucination. Never quote it. |

**This is the single most important lesson of the day.** Both ChatGPT and Claude can sound completely authoritative while being completely wrong about specific regulations, section numbers, and dates. **For regulatory citations, always verify on the original source.**

---

## 📝 Build your personal cheat sheet

Fill this in based on what you observed:

| Task | I will use… | Because… |
|------|-------------|----------|
| Quick first-draft SOP | | |
| Final-version SOP for regulator | | |
| Rewrite for technicians (ESL) | | |
| Checking a specific OGRA rule | | |
| Brainstorming hazard scenarios | | |

---

## ➡️ Next step

Move on to [`long_document_analysis.md`](long_document_analysis.md) to push the comparison into long-document territory — where the differences become much sharper.
