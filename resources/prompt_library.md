# 📚 Prompt Library — Copy-Paste Ready

A curated collection of prompts that work consistently for Pakistani O&G professionals. Copy, adapt, paste.

---

## 🧭 How to use this library

1. Find a prompt that matches your task category below
2. Copy the entire prompt block
3. Replace anything in `[BRACKETS]` with your details
4. **Anonymise** any sensitive information first
5. Paste into ChatGPT, Claude, or Copilot
6. Refine the prompt if the first output isn't quite right

---

## 🎤 Communications

### Internal: WhatsApp/Slack announcement

```text
You are a Senior Manager at a Pakistani O&G operator. Draft a short internal 
announcement for the team WhatsApp/Slack group.

Topic: [WHAT'S THE ANNOUNCEMENT?]
Effective date: [WHEN?]
Why it matters: [ONE LINE]

Format: under 80 words, plain professional language, no emojis, ends with a 
specific contact for questions ([CONTACT] placeholder).
```

### External: regulator-facing letter

```text
You are a Compliance Officer at a Pakistani O&G operator. Draft a letter to 
[REGULATOR-AGENCY].

Subject: [WHAT THE LETTER IS ABOUT]
Key points to convey: [3-5 BULLETS]
Desired outcome: [WHAT WE WANT FROM THEM]

Format: formal letter, under 300 words, third person, British English, 
"we" not "I". Leave [ADDRESSEE], [REFERENCE], [DATE], [SIGNATORY] as 
placeholders.
```

### External: vendor escalation

```text
You are a Senior Manager handling a difficult vendor situation. Draft an 
escalation letter to the vendor's senior leadership.

Situation: [ONE PARAGRAPH FACTUAL DESCRIPTION, ANONYMISED]
Specific shortfalls: [LIST WITH DATES AND METRICS, ANONYMISED]
Desired outcome: [WHAT YOU WANT THEM TO DO]

Format: under 400 words, firm but professional, leaves the relationship 
recoverable. No threats of litigation. British English.
```

---

## 📊 Analysis & Synthesis

### Long-document risk scan

```text
I'm pasting a [DOCUMENT TYPE — e.g. JV agreement, OGRA notification, tender 
spec]. Identify the top 3-5 risks or red flags for [PAKISTANI PARTY / OPERATOR].

For each:
1. The risk in one sentence
2. The exact clause/section that creates it
3. Why it's a problem
4. Suggested mitigation

Do not invent clauses. If uncertain, say "verify section [X]".

[PASTE DOCUMENT]
```

### Data summary into briefing

```text
I'm pasting [TYPE OF DATA — e.g. weekly production summary, HSE incident 
log, vendor scorecard]. Synthesise it into a one-page brief for [AUDIENCE].

Output structure:
1. Headline (one sentence — what's the story?)
2. Key numbers (3-5 metrics in bold)
3. What's good / what's bad / what's unclear
4. The single decision the audience needs to make
5. Three follow-up questions worth asking

Length: under 250 words. Format: markdown with headings. British English.

[PASTE DATA]
```

### Multiple sources into one view

```text
I'm pasting [N] separate inputs: [LIST THEM]. Synthesise into a single 
coherent briefing.

Where the sources agree, state the consensus.
Where they disagree, name the disagreement and which source says what.
Where any source is silent on a key point, flag the gap.

Audience: [AUDIENCE]
Output length: [X] words
Tone: [TONE]

[PASTE SOURCES, CLEARLY LABELLED A, B, C, ...]
```

---

## 📝 Drafting

### Toolbox talk

```text
You are an experienced Field Trainer at a Pakistani O&G operator. Write a 
5-minute toolbox talk on [TOPIC] for the morning shift.

Structure:
- Opening hook (one striking fact OR a 2-sentence near-miss story)
- Three key safety messages — one sentence each
- Three behaviours to start today (numbered)
- Three behaviours to stop today (numbered)
- Three verbal check questions for the supervisor to ask at the end

Length: 200-250 words. Plain English, second-language-friendly. 
British English spelling.
```

### HSE incident report draft

```text
You are a Senior HSE Investigator. Draft a structured incident report 
based on the field notes below.

Required sections:
1. Incident at a Glance
2. Sequence of Events
3. Immediate Actions Taken
4. Root Cause Analysis (5-Whys, show each step)
5. CAPA table (Corrective Actions | Preventive Actions)
6. Lessons Learned
7. Regulatory Disclosure Recommendation

Tone: factual, third-person, British English. Use [NAME], [DATE], [QUANTITY] 
for missing data. Do not invent facts.

Field notes:
[PASTE ANONYMISED NOTES]
```

### Toolbox SOP

```text
You are a Senior HSE Manager. Produce a pre-job SOP checklist for [ACTIVITY 
— e.g. confined space entry, hot work in classified area, working at height].

Format: numbered checklist, 10-15 items, each with:
- The action
- The reason in one line

Limits: under 250 words. British English. No brand-specific PPE references. 
End with the standby person's responsibilities in 3 bullets.
```

---

## 🤔 Decision Support

### Risk brainstorm

```text
You are an experienced [DISCIPLINE] Engineer. We are about to undertake 
[OPERATION] under these conditions: [CONDITIONS, ANONYMISED].

Brainstorm the top 5 specific risks. For each:
- The risk in one line
- The warning signs to monitor
- The threshold to stop or change plan
- The contingency action

End with the single most likely failure mode based on similar operations.

Constraints: no chemical-treatment volumes; no specific safety-factor numbers 
without the underlying data.
```

### Options analysis

```text
You are a Senior [ROLE] at a Pakistani O&G operator. We are considering 
[N] options for [DECISION]:

Option A: [DESCRIBE]
Option B: [DESCRIBE]
Option C: [DESCRIBE]

For each option, produce:
1. Pros (3 specific)
2. Cons (3 specific)
3. The conditions under which this option is clearly best
4. Risk profile (Low / Medium / High) + one-line justification
5. Estimated decision-reversibility (Easy / Medium / Hard)

Then provide a synthesis: which option fits which strategic objective, 
without picking a single winner. The decision rights remain with the 
committee.
```

---

## 🌐 Translation & Reframing

### English → simplified English for ESL crew

```text
Rewrite the following content for a worker who reads English as a second 
language. Keep the technical accuracy, but use:
- Short sentences (max 15 words)
- Active voice
- Simple vocabulary
- Clear command structure where instructions are involved

Add a brief glossary at the end for the 3-5 most technical terms used.

Content to rewrite:
[PASTE]
```

### Formal → informal (or vice versa)

```text
Rewrite the following from [FORMAL/INFORMAL] to [INFORMAL/FORMAL]. Keep 
all facts and decisions intact. Change only the register, tone, and 
sentence structure.

Audience after rewrite: [WHO IS GOING TO READ IT]

Content:
[PASTE]
```

---

## 🛡️ Universal anti-hallucination block

Add this to ANY prompt where accuracy matters:

```text
IMPORTANT INSTRUCTIONS:
- Do not invent any names, dates, quantities, regulations, section numbers, 
  case citations, or company-specific facts not present in my input
- If something is unclear or missing from my input, use a [PLACEHOLDER] 
  rather than guessing
- If I have asked you to cite a regulation and you are uncertain, write 
  "verify reference" instead of citing a specific number
- If you are confident about a fact but cannot point to a source in my 
  input, prefix it with "general industry practice:" so I know to verify
```

Paste this as the final paragraph of any prompt where the cost of a 
hallucinated fact is high.

---

## 🧠 Meta-prompt: train the AI to know your style

Paste this at the start of any session:

```text
For the rest of our conversation, please adopt these defaults unless I tell 
you otherwise:

- I work at a Pakistani O&G operator
- I write in British English with SI units (imperial in parentheses where 
  industry conventional)
- I prefer outputs under 400 words unless I ask for more
- I want numbered lists for actions, tables for comparisons
- I want explicit [PLACEHOLDERS] for missing data — never invented facts
- I want a one-line verification note when any claim is uncertain
- No emojis
- No "I hope this helps" or "Let me know if you have questions" closers
- Skip preambles like "Great question!" — go straight to the content
- If you cite a regulation, code, or standard, mark it as "verify on source"
- I value brevity over completeness; trim aggressively
```

This works in ChatGPT, Claude, and Copilot. It will follow these defaults 
for the rest of the conversation.
