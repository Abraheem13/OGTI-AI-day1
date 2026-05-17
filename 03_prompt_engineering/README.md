# Module 03 — Prompt Engineering for Oil & Gas Functions

**Why this module matters:** A poor prompt returns a Wikipedia-style answer. A great prompt returns an O&G-specific, role-aware, audit-ready output. This module gives you function-specific prompt patterns for the four areas where you will use AI most.

---

## 📦 Sub-modules

Pick the one matching your role first, then explore the others:

| File | For who |
|------|---------|
| [`operations.md`](operations.md) | Field engineers, production managers, shift supervisors |
| [`hse.md`](hse.md) | HSE managers, safety officers, incident investigators |
| [`procurement.md`](procurement.md) | Procurement officers, tender committees, contract managers |
| [`engineering.md`](engineering.md) | Reservoir, drilling, process and integrity engineers |

---

## 🧩 The 5-Part Anatomy — universal framework

Every good prompt has five parts. Learn this once; apply it everywhere.

| Part | What it means | Example (O&G) |
|------|---------------|---------------|
| **Role** | Who should the AI act as? | *"You are a Senior HSE Manager at a Pakistani refinery..."* |
| **Context** | What's the background? | *"...during a monsoon week at a downstream plant..."* |
| **Task** | What exactly do you want? | *"...draft a 10-point worker safety checklist..."* |
| **Format** | How should the output look? | *"...as bullet points suitable for a WhatsApp alert..."* |
| **Limits** | What constraints apply? | *"...focus on heat exhaustion and oxygen levels; max 200 words."* |

**Mnemonic:** **R**ole · **C**ontext · **T**ask · **F**ormat · **L**imits — *"Real Crude Travels Fast Locally."*

---

## 💎 Five power-ups that turn a good prompt into a great prompt

1. **Numbered steps** — *"Use a 5-step structure: 1. ... 2. ..."* — controls the output skeleton
2. **Explicit anti-hallucination** — *"Do not invent any names, dates, or quantities. Use placeholders if missing."*
3. **Audience specification** — *"Tone suitable for a regulator / for a foreman / for a board."*
4. **Negative constraints** — *"Avoid emojis. No marketing language. No first-person pronouns."*
5. **Verification cue** — *"If a clause is unclear, say 'verify clause X' rather than guessing."*

---

## 🎓 Learning outcomes

By the end of this module you will:

1. Write prompts that consistently produce 80% usable output on the first try
2. Build a personal prompt library for your function
3. Recognise and correct the three most common prompt failures
4. Have one master prompt ready to use at your desk tomorrow

---

## 🧪 The 30-second prompt diagnostic

Before you hit Enter, ask:

- [ ] Did I specify a Role?
- [ ] Did I give enough Context for the AI to make smart choices?
- [ ] Is the Task one clear ask (not three at once)?
- [ ] Did I specify Format?
- [ ] Did I give Limits (length, tone, what to avoid)?
- [ ] Did I add an anti-hallucination instruction?

If you ticked all six: 90% chance of a great first output. If you ticked fewer than four: rewrite the prompt before sending.
