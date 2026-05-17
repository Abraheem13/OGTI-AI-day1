# 📦 Prompt Engineering for Procurement

For: Procurement officers, tender committees, contract managers, supply chain leads.

**Special caution:** Procurement data — bid pricing, vendor negotiations, BAFO terms — is **firmly on the Red List**. Anonymise before pasting anything into a public AI.

---

## 🧪 Prompt 1 — Technical Bid Evaluation Framework

```text
You are a Senior Procurement Manager at a Pakistani national oil company, 
preparing a technical evaluation framework for a PPRA-compliant tender.

Context: we are about to issue a tender for [SCOPE-OF-WORK — e.g. "rotating 
equipment maintenance services for a refinery"]. Estimated contract value is 
above the PPRA Rule 36 threshold for full open competition.

Task: design a technical evaluation framework covering:
1. Pre-qualification criteria (5-7 minimum requirements, pass/fail)
2. Technical scoring criteria (max 100 points, broken into categories with 
   weightings — e.g. experience 25, technical proposal 30, key personnel 20, 
   methodology 15, HSE record 10)
3. The minimum technical score to pass (typically 70/100 in PPRA practice)
4. Documentation each bidder must submit for each criterion
5. Common red flags evaluators should watch for

Format: structured framework document with tables for the scoring matrix.
Length: 600-800 words.
Tone: formal, PPRA-aware.

Constraints:
- Do not cite specific PPRA rule numbers unless I provide them
- Do not include commercial / price criteria — this is technical-only
- Do not invent the scope-of-work specifics beyond what I provided
- British English
```

---

## 🧪 Prompt 2 — PPRA Rule 36 Justification

```text
You are a Procurement Compliance Officer. I need to draft a PPRA Rule 36 
justification for [METHOD-OF-PROCUREMENT — e.g. "single-source"], based on 
these facts:

[STATE THE FACTUAL JUSTIFICATION IN 3-4 SENTENCES. Anonymise vendor names. E.g. 
"The required spare part is proprietary to OEM [VENDOR-X]. Only [VENDOR-X] 
holds the design rights. Three alternative suppliers were market-tested and 
found unable to supply genuine OEM-specified parts. Equipment is critical to 
production continuity."]

Draft a justification memo covering:
1. Background and context
2. Specific requirement
3. Why standard open competition is not feasible (with specific reasons)
4. What alternatives were considered and why they were rejected
5. Value-for-money assessment
6. Risk mitigation measures
7. Recommendation

Format: formal memo, ready for internal sign-off.
Length: 400-500 words.

Constraints:
- Do not cite specific PPRA section numbers unless I provided them
- Tone: factual, defensible in audit. No marketing language.
- Avoid words like "preferred", "trusted partner" — focus on objective necessity
- Leave [APPROVING AUTHORITY], [DATE], [REFERENCE NUMBER] as placeholders
- British English
```

---

## 🧪 Prompt 3 — Tender Clarification Reply

```text
You are a Senior Procurement Officer responding to a clarification query from a 
prospective bidder during the question-and-answer window of an open tender.

Context: the bidder has asked: [PASTE THEIR EXACT QUERY]

The tender's relevant clauses are: [PASTE THE RELEVANT TENDER CLAUSES]

Task: draft a clear, professional reply that:
1. Restates the bidder's question in one line (for clarity)
2. Answers based ONLY on the tender clauses provided
3. Does not introduce new requirements not in the tender
4. Does not give any one bidder an advantage
5. Notes if the clarification will be circulated to all bidders (per PPRA fairness rule)

Format: formal letter / email response. Under 250 words.
Tone: neutral, factual, professional. British English.

Constraints:
- If the answer is not clear from the tender clauses, say "the tender does not 
  specify; this matter will be addressed by addendum"
- Do not invent any tender terms
- End with the standard signoff: "[PROCUREMENT OFFICER], [DESIGNATION], 
  [DEPARTMENT], [DATE]"
```

---

## 🧪 Prompt 4 — Vendor Capability Assessment

```text
You are a Senior Category Manager performing market intelligence on potential 
vendors for [CATEGORY — e.g. "downhole well integrity services"].

I will provide three vendors, anonymised. Without inventing facts, produce 
a comparative assessment covering for each:

1. Apparent technical strengths (based ONLY on the information I provide)
2. Apparent technical weaknesses or gaps
3. Regional / Pakistan-specific factors (e.g. local presence, language, 
   knowledge of OGRA / PPRA — only state these if I have confirmed them)
4. Overall fit for our requirement (one paragraph)
5. Key questions we should ask in a clarification call

Vendor A: [PASTE ANONYMISED CAPABILITY STATEMENT]
Vendor B: [PASTE ANONYMISED CAPABILITY STATEMENT]
Vendor C: [PASTE ANONYMISED CAPABILITY STATEMENT]

Format: comparison table, then a one-paragraph synthesis per vendor.
Constraints:
- Do not rank or recommend a winner — that's our committee's job
- Do not invent any capability I haven't given you
- If two vendors look similar, say so honestly rather than over-differentiating
- British English. Neutral, professional tone.
```

---

## 🧪 Prompt 5 — Contract Clause Comparison

```text
You are a Contracts Specialist. I will paste TWO versions of a contract clause:
- Our standard clause (what we want)
- The vendor's proposed amendment (what they want)

Task: produce a side-by-side analysis covering:
1. What has changed (specific words/phrases)
2. The commercial implication of the change for the Pakistani party
3. The legal/risk implication for the Pakistani party
4. Three possible counter-positions, ranked from "easy compromise" to "hard 
   redline"
5. Recommended response and the rationale

Format: structured analysis with clear headers.
Length: 400-600 words.

Constraints:
- Be specific about what each word/phrase change actually means in practice
- Do not invent legal precedent or case law
- Do not recommend signing as-is unless the change is genuinely neutral
- British English. Plain professional language — assume the GM is an engineer, 
  not a lawyer.

Our standard clause:
[PASTE ORIGINAL CLAUSE]

Vendor's proposed clause:
[PASTE PROPOSED CLAUSE]
```

---

## 🛟 Common procurement-prompt failures and fixes

| Failure | Fix |
|---------|-----|
| AI invents PPRA section numbers | Add: *"Do not cite specific PPRA rules unless I provide them"* |
| AI recommends a winner when you asked for analysis | Add: *"Do not recommend or rank. Analysis only."* |
| Tone is too commercial / vendor-friendly | Add: *"Neutral and factual. No marketing language."* |
| Output favours one vendor without justification | Re-prompt: *"Treat all vendors symmetrically. Same number of strengths and weaknesses each."* |
| Real vendor / price data was used | **You broke the Red List.** Anonymise and re-run. Inform IT if necessary. |

---

## 🚨 The single most important rule for procurement

> **Never paste live bid prices, technical-commercial scores, BAFO negotiations, 
> or vendor-specific evaluations into a public AI. Even anonymised, the 
> combination of clauses + your context can fingerprint the deal.**

Use Microsoft 365 Copilot for procurement work where licensing and data 
residency allow — your data stays inside your tenant. For public AI, 
anonymise to the point that even your own team couldn't identify the deal.
