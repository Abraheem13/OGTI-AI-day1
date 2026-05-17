# 🔧 Prompt Engineering for Engineering Teams

For: Reservoir, drilling, production, process and integrity engineers.

---

## 🧪 Prompt 1 — Technical Concept Explainer

```text
You are a Senior Reservoir Engineer at a Pakistani upstream operator, training 
a new graduate engineer who has solid theoretical background but limited 
field experience.

Task: explain [TECHNICAL CONCEPT — e.g. "the difference between primary, secondary 
and tertiary recovery and when each is appropriate for a mature carbonate reservoir"].

Structure:
1. The concept in one paragraph (under 100 words)
2. Why it matters in the field (one paragraph with a concrete example)
3. The key parameters or thresholds an engineer needs to know
4. Three common misconceptions junior engineers have, and how to correct them
5. One Pakistan-context observation (general — do not name specific fields)
6. A pointer to the canonical SPE or textbook reference for further reading

Format: structured explanation as above.
Length: 500-700 words.
Tone: experienced mentor — generous with insight, brief with theory.
Constraints:
- British English
- Do not invent SPE paper numbers — say "see canonical SPE literature on [topic]"
- Use SI units; mention imperial conversions where industry uses them
```

---

## 🧪 Prompt 2 — Pre-Operation Risk Brief

```text
You are an experienced Drilling Engineer.

Context: we are about to commence [OPERATION — e.g. "underbalanced drilling on 
a horizontal well in a tight gas reservoir"]. Local conditions: [LIST 2-3 
RELEVANT CONDITIONS, anonymised].

Task: produce a pre-operation risk brief covering:
1. Top 5 specific operational risks for this combination
2. For each risk: the warning signs to monitor, the threshold at which we 
   should stop or change plan, and the contingency action
3. Equipment readiness checklist (what to verify before spud / kick-off)
4. Communication discipline — who needs to be on the radio, decision authority
5. The single most likely failure mode based on similar wells in similar 
   geology — and what to watch for in real time

Format: structured brief.
Length: 600-800 words.
Tone: experienced operations engineer briefing a younger team lead.

Constraints:
- Do not invent specific field data not provided
- Do not recommend chemical-treatment volumes — those require formation-specific 
  analysis
- British English; SI units with imperial where conventional
```

---

## 🧪 Prompt 3 — Failure Investigation Brainstorm

```text
You are a Senior Integrity Engineer. We have observed [EQUIPMENT FAILURE — e.g. 
"premature failure of a downhole pump after 6 months service in a well with 
20% water cut and high CO2"].

Task: brainstorm possible failure mechanisms using a structured approach.

Categories to cover:
1. Mechanical (vibration, fatigue, bearing wear)
2. Corrosion (CO2 / H2S / O2-related, MIC, erosion-corrosion)
3. Operational (overpressure events, dry running, gas-lock, surging)
4. Materials (specification mismatch, manufacturing defects)
5. Design (sizing, geometry, NPSH)
6. Installation / commissioning errors

For each category:
- 2-3 specific candidate mechanisms ranked by likelihood (high / medium / low)
- The diagnostic evidence that would confirm or rule out each one
- The cost / time / risk of obtaining that evidence

Conclude with:
- Top 3 most likely mechanisms overall
- Recommended physical inspection plan
- Whether a failed-component metallurgical analysis is justified

Format: structured by category, with a synthesis section.
Constraints: do not invent metallurgical findings or test results.
Tone: technical peer-to-peer.
```

---

## 🧪 Prompt 4 — Engineering Calculation Sanity-Check

```text
You are a Senior Process Engineer. I have performed a calculation and want 
you to sanity-check my approach BEFORE I trust the answer.

My calculation:
- Goal: [WHAT YOU'RE CALCULATING — e.g. "pump NPSH-available for a centrifugal 
  pump on a crude transfer service"]
- Inputs: [LIST YOUR INPUT VALUES AND UNITS]
- Method: [DESCRIBE YOUR APPROACH IN 3-5 LINES]
- My answer: [STATE YOUR ANSWER WITH UNITS]

Task: sanity-check this calculation. Specifically:
1. Is the method appropriate for the situation? Identify any conceptual errors
2. Are the input values in the right ranges for the stated conditions?
3. Common mistakes I might have made (unit conversions, missing terms)
4. An order-of-magnitude estimate using a simplified approach — does it agree 
   with my answer?
5. The sensitivity of the answer to the most uncertain input — what's the 
   plausible range?

Format: structured response.
Constraints:
- Show your reasoning step-by-step
- If you spot an error, say so directly — do not be diplomatic
- If my answer looks plausible, say so explicitly
- Use SI units throughout
- If a calculation requires data I haven't provided, say "need [PARAMETER]"
```

> ⚠️ **Reality check:** AI is reasonable for sanity-checking *approach*, often weak at exact numeric calculation. Use AI to validate your method and order-of-magnitude. Use a calculator or proper engineering software for the final numbers.

---

## 🧪 Prompt 5 — Technical Report Structure

```text
You are a Principal Engineer writing a technical report on [TOPIC — e.g. 
"performance assessment of a gas-lift optimisation programme over a 12-month 
period at a brownfield asset"].

Task: produce a report structure (table of contents only — not the content), 
suitable for a 25-page internal technical report.

Requirements:
1. Sections logically sequenced from background → methodology → results → 
   conclusions → recommendations
2. Each section / subsection labelled with one-line description of its purpose
3. Page-budget estimate for each section (totalling ~25 pages)
4. Required figures, tables, and appendices identified
5. Suggested reviewers / sign-off authority per section

Constraints:
- Use British engineering reporting conventions
- Do not invent the content — structure only
- Include a Lessons Learned and Recommendations for Further Work section
- Use a numbered hierarchical heading scheme (1, 1.1, 1.1.1)
```

---

## 🛟 Common engineering-prompt failures and fixes

| Failure | Fix |
|---------|-----|
| AI gives a confident answer for a calculation that's wrong | Use AI for approach; use calculator/software for numbers |
| AI invents SPE paper numbers and citations | Add: *"Do not cite specific paper numbers. Say 'canonical SPE literature on X'."* |
| Output mixes units sloppily (psi and bar in same paragraph) | Add: *"Use SI units throughout, with imperial conversion in parentheses where conventional"* |
| AI hedges with caveats when you need a decision | Add: *"Give your best technical opinion. If unsure, rank options by likelihood rather than refusing to answer."* |
| Output is too theoretical for a field problem | Add: *"Field-engineer voice, not academic. What would you actually do?"* |

---

## 🎯 The engineering-prompt golden rule

**AI is a thinking partner, not a calculator.** Use it to:
- Brainstorm failure mechanisms
- Sanity-check your approach
- Structure your reports
- Translate between disciplines (reservoir → drilling → operations)
- Catch blind spots in your reasoning

Do **not** use it to:
- Replace engineering software
- Generate exact tolerance / spec values
- Make safety-critical decisions
- Cite specific standards or codes (always verify)
