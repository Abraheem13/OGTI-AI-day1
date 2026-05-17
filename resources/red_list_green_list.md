# 🚦 Red List / Green List — Before You Paste Anything into Public AI

Public AI servers (ChatGPT, Claude, Perplexity, NotebookLM, Gemini) sit **outside Pakistan's jurisdiction**. Anything you paste may be retained, logged, or used to train future models. Treat every prompt as a public document.

---

## 🛑 RED LIST — Strictly Forbidden

Never paste any of the following into a public AI tool, regardless of how anonymised it may *look*:

| Category | Examples |
|----------|----------|
| **Production data** | Flow rates, BHP/WHP, well-test results, GOR, water cut, choke settings |
| **Reservoir & subsurface** | Seismic data, basin studies, reservoir maps, log data, sweet-spot coordinates |
| **JV / commercial** | Contracts with OMV, Eni, MOL, KUFPEC, POL, PEL; royalty terms; carry arrangements |
| **People** | Employee CNICs, payroll, performance reviews, medical records, family information |
| **Procurement** | Bid pricing, vendor evaluations, BAFO negotiations, technical-commercial scoring |
| **Incidents** | Internal HSE incident reports **before** OGRA disclosure; near-miss investigations |
| **Classified labels** | Anything marked *Partner Only*, *Confidential*, *Need-to-Know*, *Internal Use* |
| **Authentication** | Passwords, API keys, VPN credentials, SAP logins, SCADA access tokens |

---

## ✅ GREEN LIST — Safe to Use

These are fine to paste — they are already public or contain no identifying data:

- Publicly notified **OGRA** and **PPRA** gazettes and rulings
- International industry standards (API, ISO, NFPA, IADC, ASME)
- Concept questions ("explain enhanced oil recovery", "what is steam flooding?")
- Tone / language editing of **your own** internal emails (with names removed)
- Anonymised data samples using `[REGION]`, `[VENDOR]`, `[WELL]`, `[FIELD]` placeholders
- Open-published technical literature (SPE papers, IEA reports, OPEC bulletins)
- Speech / memo drafting using public-domain inputs
- Generic Pakistan O&G context already in news media

---

## 🔄 Anonymisation in Practice

### ❌ BAD PROMPT
> *"Draft a summary of the gas leak at Qadirpur Well-4 on 12 March involving Zahid Ahmed, with our YoY production figures dropping from 320 MMSCFD to 285 MMSCFD."*

### ✅ SAFE PROMPT
> *"Draft an incident summary for a gas leak at `[FIELD]` involving a senior technician `[TECH-A]` on `[DATE]`; include placeholder figures `[PROD-Q1]` and `[PROD-Q2]` representing a YoY decline of `[X%]`."*

**The principle:** keep the **logic** of what you want; remove the **identity** of what makes it sensitive.

---

## 📜 The Five Rules of Engagement

1. **Assume Publicity** — treat every prompt as a public document
2. **Anonymise First** — swap names for roles (`Company X`, `[VENDOR]`, `[TECH-A]`)
3. **Verify Everything** — AI is a writer, not a licensed engineer
4. **Label AI Content** — be transparent with your manager and audit team
5. **Report Leaks** — inform IT immediately if confidential data slips out

---

## ⚖️ PECA 2016 — A Reminder

The **Prevention of Electronic Crimes Act 2016** treats Pakistani state-owned energy data as a strategic asset. Unauthorised disclosure to foreign entities — including via public AI tools whose servers sit abroad — can attract criminal liability under:

- **§3** — Unauthorised access to information system
- **§4** — Unauthorised copying or transmission of data
- **§14** — Electronic forgery

Your prompt logs are potentially discoverable in an audit. **Behave accordingly.**

---

## 🧪 Self-Test: Can I Paste This?

Before hitting Enter, run the four-question check:

1. Would I send this in a public tweet?
2. If a competitor read it tomorrow, would it hurt us?
3. Does it identify a real person, well, contract or price?
4. Would my line manager sign off on it being on a foreign server?

**If any answer makes you hesitate → anonymise it, or don't send it.**
