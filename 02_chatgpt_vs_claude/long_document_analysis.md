# 📚 ChatGPT vs Claude — Long Document Analysis

**Time required:** 30–35 minutes
**You will use:** Both `chat.openai.com` and `claude.ai`
**Sample data:** [`sample_data/sample_jv_agreement.txt`](sample_data/sample_jv_agreement.txt)

---

## 🎯 What you will learn

1. Upload a long, anonymised document to both tools
2. See where ChatGPT's free-tier context limits hurt you
3. Understand why Claude is the default choice for documents over ~30 pages
4. Extract the top commercial and legal risks from a JV agreement

---

## ⚠️ Important — Red List check before uploading

The sample document in this repo is **fictional and anonymised**. If you are using a real document from your work:

- [ ] Replace all real names with `[NAME]`, `[VENDOR]`, `[COUNTERPARTY]`
- [ ] Replace specific dates with `[DATE]`
- [ ] Replace monetary amounts with `[FIGURE]` or `[AMOUNT-USD]`
- [ ] Remove any classified or partner-only markings
- [ ] **If in doubt: don't upload.** Use NotebookLM with a private Google account instead.

---

## 🧪 Exercise 1 — Upload and Skim

### In ChatGPT:

1. Open `chat.openai.com`, start a new chat
2. Click the paperclip icon to upload `sample_jv_agreement.txt`
3. While it processes, prepare your first prompt

### In Claude:

1. Open `claude.ai`, start a new chat
2. Drag-and-drop the same file into the message box, OR paste the contents directly
3. Claude's free tier handles this size easily

**Run the SAME prompt in both tools:**

```text
You are a senior legal advisor to a Pakistani national oil company. I have just 
uploaded a draft joint-venture agreement with a foreign partner.

Without inventing anything, give me a 200-word executive summary covering:
1. The deal structure (who, what, how long)
2. The financial commitments and their split
3. The governance structure
4. The exit mechanism
5. The dispute resolution forum

If any of these are unclear or missing from the document, say so explicitly.
```

---

## 🧪 Exercise 2 — Top 3 Risks

**Run this in both tools (same chat session, so context is retained):**

```text
Based ONLY on the uploaded document — do not use external knowledge — identify 
the TOP 3 commercial and legal risks for a Pakistani operator entering this agreement.

For each risk:
1. Name the risk in one sentence
2. Cite the EXACT clause or section in the document that creates the risk
3. Explain why this is a problem for the Pakistani side specifically
4. Suggest a mitigating amendment to the clause

Do not invent any clauses. If you are uncertain whether a clause is in the document, 
say "Uncertain — please verify section [X]" rather than guessing.
```

**Watch for:**

- ✅ Claude tends to cite specific clauses; ChatGPT sometimes paraphrases without citing
- ⚠️ Either tool may **invent a clause number** that sounds plausible. Always verify.
- ✅ Claude's free tier usually reads the whole document; ChatGPT's free tier may only read the beginning and end

---

## 🧪 Exercise 3 — The "Hidden Cost" Pressure Test

**Run this in both tools:**

```text
Are there any clauses in this agreement that create hidden costs or hidden 
liabilities for the Pakistani party? Examples to look for:
- Indemnities with no cap
- Tax gross-up clauses
- Currency-risk clauses
- Termination triggers with payment obligations
- Most-favoured-nation pricing clauses
- Foreign jurisdiction litigation forums

For each one you find, quote the exact text from the document.
```

**Verify every quote.** Use Ctrl+F in your text file to confirm the quote actually exists in the document. This is where you'll often catch fabrication.

---

## 🧪 Exercise 4 — Translate for a Non-Lawyer

**Run this in both tools:**

```text
My GM is an engineer, not a lawyer. In 5 bullet points, explain in plain 
English what risks he is signing up to if he approves this agreement as-is. 
Avoid all legal jargon. Each bullet under 25 words. End with one sentence 
on whether you would advise him to sign or to negotiate first.
```

---

## 📊 Compare-and-decide scoresheet

| Criterion | ChatGPT | Claude |
|-----------|---------|--------|
| Did it read the whole document? | ✅ / ❌ | ✅ / ❌ |
| Did it cite specific clauses? | ✅ / ❌ | ✅ / ❌ |
| Did it invent any clause numbers? (Ctrl-F check) | ✅ / ❌ | ✅ / ❌ |
| Did it flag genuine red flags? | ✅ / ❌ | ✅ / ❌ |
| Was the executive summary at the right level? | ✅ / ❌ | ✅ / ❌ |
| Would I share this analysis with my GM? | ✅ / ❌ | ✅ / ❌ |

---

## 💡 The big takeaway

For long documents, **Claude is usually the right starting point**. Once you have a strong shortlist of clauses, you can use ChatGPT for rapid follow-up drafting of amendments or alternative wording.

**For regulated documents** (OGRA filings, PPRA bid evaluations, JV contracts you'll actually sign), **NotebookLM is even safer** because every answer is grounded in the document and cites the exact page. Use NotebookLM for review, then move to ChatGPT or Claude only for drafting fresh language.

---

## ➡️ Next step

Move on to [`incident_investigation.md`](incident_investigation.md).
