# Jeyson Dagondon, RPh

**Healthcare workflow automation** — I run the operations layer of a US telehealth clinic, and I build the tools that remove manual work from it.

I'm a Registered Pharmacist (PRC, board rating 91.07%) working remotely for a US peptide/GLP-1 telehealth clinic. My day job is the full patient and prescription pipeline in Zoho CRM — records, refills, and order coordination with US compounding pharmacies. The other half of the job is a **45+ script Tampermonkey userscript and Chrome extension suite** that automates intake, order queues, tracking, and address validation across the clinic's CRM, patient portal, and pharmacy portals.

I read protocols, catch dosing discrepancies, and build the systems that keep them from recurring.

---

### The pattern in everything below

I don't have a favourite platform. A CRM, a pharmacy portal, a job board, a spreadsheet, an exam — it doesn't matter. **If something is inefficient, I will spend disproportionate time making sure it can never become a problem again.**

So each project below is written as **problem → what was manual → the fix → the impact**. The tool was never the interesting part.

---

### What I work with

| | |
|---|---|
| **Clinical operations** | Zoho CRM · EHR/EMR workflows · HIPAA · ADR reporting · GxP/cGMP · ICD coding |
| **Automation** | Tampermonkey userscripts · Chrome extensions (MV3) · Chrome DevTools Protocol · Google Apps Script · n8n · Excel VBA |
| **Data & code** | Python · JavaScript · SQL · Google Sheets · dashboards & KPI reporting |
| **AI** | LLM prompt engineering · API integration · batch pipeline design · local inference |

---

### Selected work

**[userscript-showcase](https://github.com/anki-boi/userscript-showcase)** · 40 production userscripts
- **Problem:** one prescription meant re-typing the same patient data into whichever pharmacy portal the order needed, finding its tracking number by hand, then writing the patient SMS from scratch — 15–20 manual actions per order.
- **Fix:** 40 scripts that each do one job. Deliberately *not* one extension: these portals change their DOM constantly, so isolation is what keeps a one-file selector fix from breaking patient messaging.
- **Impact:** ~6 min → ~40 s per order, roughly **40–60 h/month** returned; wrong-patient and wrong-vial classes designed out.
- **Read the full log:** [PROBLEMS.md](https://github.com/anki-boi/userscript-showcase/blob/master/PROBLEMS.md) — every script, its pain point, and its failure history.

**[True-Anki-MCQ-Note-Template](https://github.com/anki-boi/True-Anki-MCQ-Note-Template)** ★ 15
- **Problem:** Anki's default is pure active recall, but the pharmacy board exam is 100% multiple choice. Full recall is overkill for a recognition test — same study minute, harder task, less exam-relevant yield.
- **Fix:** a card template that trains recognition under exam conditions: randomised choice order, single and multi-answer, immediate correct/wrong/missed feedback.
- **Impact:** familiarity with the real question format instead of picture-perfect recall.

**[datecard](https://github.com/anki-boi/datecard)** · open source (MIT)
- **Problem:** there's no good way to show someone who you are when you meet them in public. A social handle is an all-or-nothing broadcast, and dating apps put an algorithm between two people who already met.
- **Fix:** a QR dating card — scan, read the profile, *apply to connect*; you approve or decline, and only then do they get your socials. One account, up to three profiles, each with its own card and inbox.
- **Impact:** an exchange you control, works in public with no app installed, and socials are never scrapeable from the page.

**[ojph-cleaner](https://github.com/anki-boi/ojph-cleaner)** · Chrome MV3
- **Problem:** job listings arrive unfiltered — salary buried in the description body, keyword hits that don't mean what you searched for.
- **Fix:** a rules engine that deep-scans full descriptions against your own salary and keyword rules.
- **Impact:** days of scrolling collapse into a shortlist.

**[Anki-MCQ-Importer-AI-Batch-Generator](https://github.com/anki-boi/Anki-MCQ-Importer-AI-Batch-Generator)**
- **Problem:** every exam block arrived as hundreds of lecture-slide images, each needing a hand-written question with plausible distractors.
- **Fix:** an Anki add-on that batch-processes those folders through Gemini into structured MCQ cards with automatic subdecks.
- **Impact:** ~1 minute of thinking-and-typing per card → a batch job.

**[onlinejobs.ph-suite](https://github.com/anki-boi/onlinejobs.ph-suite)** · Job Hunter Dashboard
- **Problem:** no way to score r&eacute;sum&eacute; fit across thousands of listings, salaries quoted in mixed currencies, applications tracked in a spreadsheet you forget to update.
- **Fix:** local FastAPI + SQLite dashboard — live SSE scrape console, ATS scoring per listing, one-click r&eacute;sum&eacute; tailoring, FX-normalized salaries.
- **Impact:** a multi-hour manual sweep becomes one scoped, pre-scored run.

**[PH-Pharmacy-Setup-Guide](https://github.com/anki-boi/PH-Pharmacy-Setup-Guide)**
- **Problem:** standing up a community pharmacy in the Philippines is a maze of licensing, layout and compliance steps with no published order — so people stall on the wrong phase, and a goal measured in months loses momentum when progress is invisible.
- **Fix:** a single-page quest board with phases, priorities and progress tracking.
- **Impact:** "where do I start / what's next?" becomes a glance.

---

📄 [Portfolio](https://anki-boi.github.io/) · 💼 [LinkedIn](https://www.linkedin.com/in/donjeysonmd) · ✉️ [donjeysonofficial@gmail.com](mailto:donjeysonofficial@gmail.com)
