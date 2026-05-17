# 🦺 Prompt Engineering for HSE

For: HSE managers, safety officers, incident investigators, training coordinators.

---

## 🧪 Prompt 1 — Monsoon Safety Alert

```text
You are a Senior HSE Manager at a Pakistani refinery.

Context: heavy monsoon rain is forecast at the site for the next 72 hours. 
Risk of waterlogging around live electrical equipment, slippery walkways, 
and reduced visibility during night shift.

Task: draft a 10-point safety alert for the operating crew. Cover:
- Electrical hazards (waterlogging, exposed wiring, earthing)
- Slip-and-fall risks (walkways, stairs, ladders)
- Heat stress (humidity adds to heat load)
- Communication discipline in poor visibility
- Emergency response readiness
- PPE checks
- Personnel rotations
- Reporting threshold for near-misses
- Coordination with control room
- Pre-shift briefing requirement

Format: numbered bullets for a WhatsApp broadcast. Each bullet under 25 words.
Length: under 200 words total.
Tone: directive, professional. Second-language-English-friendly.
End with: "Stay alert. Stay safe. — HSE Manager."
```

---

## 🧪 Prompt 2 — Root-Cause 5-Whys

```text
You are a senior HSE investigator. I will describe an incident in 2-3 sentences. 
Your job is to walk me through the 5-Whys methodology rigorously.

Rules:
- Each "Why" must logically follow from the previous answer
- Do not skip to root cause prematurely
- After the 5th "Why", state whether you have reached a true root cause 
  (procedural, behavioural, or systemic) or whether more investigation is needed
- Do not invent facts not in my description

Incident:
[DESCRIBE THE INCIDENT IN 2-3 SENTENCES]

Format:
Why 1: ... → Answer: ...
Why 2: ... → Answer: ...
Why 3: ... → Answer: ...
Why 4: ... → Answer: ...
Why 5: ... → Answer: ...

Root Cause Statement: [single sentence]
Cause Type: [Procedural / Behavioural / Systemic / Equipment / Environmental]
Confidence: [High / Medium / Low — and one sentence why]
Additional investigation needed: [Yes / No — and if yes, what]
```

---

## 🧪 Prompt 3 — CAPA (Corrective and Preventive Actions) Plan

```text
You are an HSE Compliance Officer. I have just completed root-cause analysis 
on an incident. Now I need a CAPA plan.

Root cause: [PASTE THE ROOT-CAUSE STATEMENT FROM PROMPT 2]
Contributing factors: [LIST FROM YOUR INVESTIGATION]

Produce a CAPA plan with two clearly labelled sections:

CORRECTIVE ACTIONS (fix what went wrong right now):
- Action / Owner / Target completion date / Verification method

PREVENTIVE ACTIONS (stop it happening again — systemic):
- Action / Owner / Target completion date / Verification method

Each section: 3-5 actions, prioritised by urgency.

Constraints:
- Actions must be SMART: specific, measurable, achievable, relevant, time-bound
- Owners are roles, not named individuals (e.g. "Maintenance Superintendent")
- Verification method is concrete — "audit checklist X" not "review"
- Format as two markdown tables.
- Conclude with a one-line statement on whether this incident should trigger 
  a broader policy review.
```

---

## 🧪 Prompt 4 — Regulator Disclosure Draft (OGRA Section 26)

```text
You are an HSE Compliance Officer at a Pakistani downstream operator. I need a 
draft disclosure for OGRA Section 26 reporting based on the following facts:

[PASTE ANONYMISED INCIDENT FACTS — no real names, dates, or sensitive 
identifiers. Use placeholders.]

Draft a formal disclosure covering:
1. Incident classification (severity, on-site / off-site impact)
2. Sequence of events (chronological, factual, no interpretation)
3. Personnel affected (use roles, not names)
4. Environmental impact (quantified where possible, with placeholders if not)
5. Immediate actions taken
6. Status of ongoing investigation

Tone: third person, formal, regulator-facing register. British English.
Length: under 400 words.

Constraints:
- Do not include opinions, blame attribution, or speculation
- Do not cite specific OGRA section numbers UNLESS I have provided them — if 
  unsure, write "[verify Section reference]"
- Do not invent any facts not in my input
- End with placeholder fields: [REPORTING OFFICER], [DESIGNATION], [DATE], 
  [SIGNATURE]

REMINDER TO ME: this is a draft only. Manual legal review required before filing.
```

---

## 🧪 Prompt 5 — Training Programme Design

```text
You are a Senior HSE Trainer at a Pakistani O&G operator. I want to design a 
half-day refresher training on [TOPIC — e.g. "confined space entry"] for our 
maintenance technicians.

Produce a training plan covering:
1. Learning objectives (3-4, in measurable language)
2. Audience profile (assumed prior knowledge)
3. Session breakdown — table with: time slot, topic, format (lecture / hands-on 
   / drill / quiz), trainer, materials
4. Practical exercise design (one detailed exercise of 30-45 minutes)
5. Assessment method (how we'll know they actually learned it)
6. Refresher cadence recommendation

Total duration: 4 hours including a 20-minute tea break.

Constraints:
- Mix of theory and practice — at least 50% hands-on
- Include one real-world Pakistani O&G case study (you may use a generic 
  description — do not invent a specific incident)
- Final assessment must be observable behaviour, not just a written test
- British English. Suitable for technicians whose English is a second language.
```

---

## 🛟 Common HSE-prompt failures and fixes

| Failure | Fix |
|---------|-----|
| AI cites a specific OGRA section that doesn't exist | Always add: *"Do not cite specific section numbers unless I provide them. If unsure, write 'verify reference'."* |
| Tone is too informal for a regulator | Add: *"Third-person, formal, regulator-facing register. No first-person pronouns."* |
| Action items are vague ("review process") | Add: *"All actions must be SMART. Owners are roles. Verification methods are concrete."* |
| Output includes blame language | Add: *"Factual only. No blame attribution. No speculation about intent."* |
| Output reveals confidential context | **You included it in the prompt** — go back and anonymise before re-running |

---

## ⚠️ The HSE-prompt golden rule

**For any document that may be filed with a regulator, used in a legal proceeding, 
or shared outside the company: AI produces the draft, a qualified human signs the 
final.** AI cannot be held liable. You can.
