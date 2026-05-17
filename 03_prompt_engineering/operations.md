# 🛢️ Prompt Engineering for Operations

For: Field engineers, production managers, shift supervisors, plant managers.

---

## 🧪 Prompt 1 — Daily Production Briefing

**Use this** to convert raw shift data into a one-page brief for your morning meeting.

```text
You are a Senior Production Engineer at a Pakistani upstream operator. 

Context: I will paste raw shift data from the last 24 hours covering wells, 
flow rates, pressures, and any incidents. Data is anonymised with placeholders.

Task: produce a Morning Production Brief covering:
1. Headline (one sentence — was yesterday a good day or a bad day, and why)
2. Production summary (vs target, in numbers)
3. Top 3 wells of concern (well ID, the specific concern, the proposed action)
4. Any HSE events (severity, status)
5. What I should raise in the 09:00 meeting

Format: markdown with clear headings. Numbers in bold.
Length: under 300 words.

Constraints:
- Do not invent any numbers or wells not present in the data
- Use placeholders [WELL-X] for unclear references
- British English. No emojis.
- End with one specific decision the management team needs to make today.

Here is the data:
[PASTE YOUR ANONYMISED DATA HERE]
```

---

## 🧪 Prompt 2 — Shift Handover Summary

```text
You are a Shift Supervisor at a Pakistani refinery handing over to the incoming 
shift. Context: I will paste my own rough notes from a 12-hour shift.

Produce a shift handover note covering:
1. State of plant at handover (one paragraph)
2. Open issues to monitor (table: issue, severity, location, what was tried)
3. Outstanding maintenance tasks (table: task, location, status, deadline)
4. People-related items (sick, training, contractors on-site)
5. Safety concerns or near-misses
6. What the incoming supervisor MUST check in the first 30 minutes

Format: structured handover document, suitable to print and leave on the desk.
Length: 400-500 words maximum.
Tone: peer-to-peer, professional.

Do not invent any equipment, people or events not in my notes.

My notes:
[PASTE YOUR NOTES HERE]
```

---

## 🧪 Prompt 3 — Anomaly Investigation Plan

```text
You are an experienced Production Engineer. I have observed an anomaly:

[DESCRIBE THE ANOMALY IN 2-3 SENTENCES — e.g. "Well [W-XXX] showed a 7% pressure 
drop week-on-week while neighbouring wells are stable. Water cut also increased 
from 12% to 18% over the same period."]

Produce an investigation plan covering:
1. Five plausible hypotheses, ranked from most to least likely
2. For each hypothesis: the supporting evidence we should look for, and the 
   evidence that would rule it out
3. The diagnostic steps in priority order — what should the well-test engineer 
   check first, second, third
4. Whether this warrants escalation (and to whom)
5. Three documents I should pull before the next technical review

Format: numbered structure as above.
Tone: senior engineer briefing a junior.
Constraints: do not recommend any chemical treatment or intervention that 
requires more data than we currently have.
```

---

## 🧪 Prompt 4 — Vendor Performance Letter

```text
You are a Senior Operations Manager at a Pakistani national operator. 

Context: a service vendor [VENDOR-X] has had three consecutive months of 
sub-target performance on [SERVICE-TYPE]. Their contract is up for renewal in 
two months. I want to send a letter that escalates concerns formally while 
keeping the door open to course-correction.

Task: draft a letter that:
1. Opens professionally — no aggression
2. States the specific KPI shortfalls in numbers (use placeholders [KPI-1], 
   [TARGET-1], [ACTUAL-1])
3. Acknowledges any operating-environment factors fairly
4. Sets out clear expectations for the next 60 days
5. States the contractual consequences if performance does not improve
6. Offers a joint meeting with their senior leadership

Format: letterhead-style, max 400 words.
Tone: firm but professional. British English.
Sign-off: leave [NAME], [TITLE], [DATE] as placeholders.

Do not threaten litigation explicitly. Do not name specific Pakistani regulators 
unless asked.
```

---

## 🧪 Prompt 5 — Toolbox Talk Generator

```text
You are an experienced Field Operations Trainer. 

Task: produce a 5-minute toolbox talk on [TOPIC — e.g. "monsoon electrical 
safety at outdoor switchgear"] for a Pakistani upstream field crew.

Structure:
1. Opening hook (one striking fact or a 2-sentence near-miss story)
2. The three key safety messages — one sentence each
3. Specific behaviours to do today (3 numbered points)
4. Specific behaviours to STOP today (3 numbered points)
5. A quick verbal check — three questions the supervisor can ask the crew at 
   the end to confirm understanding

Tone: spoken language, second-language-English-friendly. Short sentences.
Length: 200-250 words total — reads in 4-5 minutes at a normal pace.
Avoid: jargon, statistics no one will remember, finger-wagging language.
```

---

## 🛟 Common operations-prompt failures and fixes

| Failure | Fix |
|---------|-----|
| Output reads like Wikipedia, not field-ready | Add: *"Output must be ready to print and use today. No theory."* |
| Numbers in output don't match my data | Add: *"Use ONLY the numbers I provided. Do not extrapolate."* |
| Tone is too American / too corporate | Add: *"British English. Pakistani O&G context. Plain professional language."* |
| AI gives a 1000-word answer when I asked for 300 | Add a hard word limit in the Limits section and verify by Ctrl-F before sending |
| AI refuses to give a recommendation | Add: *"Pick the most likely answer. If unsure, say so but still rank your top guess."* |

---

## 🎯 Build your own — fill-in-the-blank template

```text
You are [ROLE — e.g. "a Production Manager at PARCO Multan"].

Context: [WHAT'S HAPPENING — e.g. "our refinery is approaching the monsoon 
season. We had three weather-related incidents last year."]

Task: [WHAT YOU WANT — be specific. E.g. "produce a monsoon-readiness checklist 
covering electrical equipment, slip hazards, and emergency drainage."]

Format: [HOW IT SHOULD LOOK — numbered list / table / memo / letter / paragraph]

Limits:
- [LENGTH — e.g. "under 400 words"]
- [TONE — e.g. "formal, suitable for the GM and board"]
- [LANGUAGE — e.g. "British English"]
- [AVOID — e.g. "no emojis, no marketing language, no jargon"]
- [VERIFICATION — e.g. "do not invent regulations or section numbers"]

[YOUR DATA OR EXTRA CONTEXT, if any]
```
