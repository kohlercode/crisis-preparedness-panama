# Cyberattack, AI and the money system — deep dive

A deeper look at the #1 future-risk scenario, focused on the money system: what **actually** happens when AI or automation goes wrong with money, what regulators genuinely worry about, what the people building the technology have said in their own words, and realistic "AI goes rogue" scenarios.

## Read this first — what's real vs. what's speculation

| Category | Status | Basis |
|---|---|---|
| Algorithmic trading failures | **Documented** (2010, 2012) | conventional code, not autonomous AI |
| AI-enabled financial fraud (deepfakes) | **Documented** (2019, 2021, 2024) | humans using AI as a tool |
| AI amplifying cyberattacks on finance | **Documented / rising** | regulators and incident reports |
| Correlated "herding" & model concentration | **Institutional risk assessment** | FSB, BIS, IMF |
| A superintelligent AI autonomously "taking over" the money system | **Speculative — no precedent** | expert opinion only |

The honest summary: **there is no documented case of an AI autonomously going rogue against the financial system.** Everything real so far falls into one of two buckets — (a) a deterministic algorithm that had a bug or was deployed badly, or (b) a human using AI as a tool to defraud people. The "misaligned superintelligence manipulating the markets" scenario is a matter of expert disagreement, not observed fact. That does **not** make the risk small — the people building the systems disagree sharply about it (see §3–§4) — but it changes how you should read the rest of this file.

---

## 1. What has actually happened (documented)

### 1a. Algorithmic trading failures — code, not "rogue AI"

- **6 May 2010 — "Flash Crash":** the Dow Jones Industrial Average fell about **600 points (~7%) in 5 minutes**, briefly erasing roughly **$1 trillion** in market value before recovering within ~20 minutes. Attributed in large part to a large automated sell order interacting with high-frequency trading algorithms.
- **1 Aug 2012 — Knight Capital:** a **software deployment error** caused an automated trading system to send millions of erroneous orders for ~150 stocks over **45 minutes**, building ~$7 billion of unintended positions and a **$440 million pre-tax loss**. The firm was nearly bankrupted and was acquired. The **SEC charged Knight** with violating the market-access rule (15c3-5) for inadequate controls.
- **Why these matter:** they are the closest *real* examples to "machines run amok with money." But note honestly — these were **deterministic trading programs**, not autonomous AI with goals. The lesson transfers: the more automated and opaque a money system becomes, the faster and harder an error compounds. (This is exactly the concern regulators now extend to AI — §2.)

### 1b. AI-enabled fraud — the clearest real "AI in the money system" harm today

- **Feb 2024 — Arup, Hong Kong — $25.6 million (HK$200m):** a finance employee was invited to a video call with the company's CFO and other executives, all of whom he recognised. **Every participant was a real-time AI deepfake** (video + voice) built from public footage. He made **15 transfers to five Hong Kong accounts**. It is regarded as the first documented case of a multi-person deepfake video conference used for fraud at this scale. Arup confirmed it publicly in May 2024.
- **2019 — UK energy firm — £200,000:** a CEO approved a transfer after hearing what he believed was his boss's voice on the phone — it was an AI voice clone.
- **2021 — Hong Kong — $35 million:** a bank employee was deceived by a cloned voice of a company director into authorising transfers.

The Arup case is the canonical one: the victim's doubt was dissolved not by a fake email but by a *live, interactive* video call in which the "CFO" answered questions coherently. That is the exact boundary where the money system's "verify the person" controls are now being broken by AI.

### 1c. AI-accelerated cyberattack on financial systems

- **Sep 2025 — Panama MEF:** the Ministry of Economy & Finance (which handles Canal revenues) disclosed a breach claimed by the **INC Ransom** group, alleging **1.5 TB** of data stolen. See `../hazards/cyber.md`.
- Regulators treat AI as an **amplifier** of this category — see §2.

---

## 2. What regulators actually worry about (the sober, mainstream version)

The Financial Stability Board's Nov 2024 report *The Financial Stability Implications of Artificial Intelligence* names four AI vulnerabilities that could become systemic — none of them require a "rogue superintelligence," just **widespread use of similar AI systems**:

1. **Third-party concentration** — everyone depends on a handful of cloud providers, specialised hardware, and pre-trained models; a disruption at one key vendor propagates.
2. **Market correlation / herding** — many firms using the **same models and same data** can trade, lend, and price **in the same direction at the same time**, amplifying stress, liquidity crunches, and asset-price swings.
3. **Cyber** — AI raises both the capability of attackers and the number of attack surfaces.
4. **Model risk, opacity, hallucinations** — hard-to-explain models and unverifiable training data make failures hard to detect until after damage.

The FSB adds two sentences directly relevant here: GenAI can **"increase financial fraud and the ability of malicious actors to generate and spread disinformation in financial markets,"** and **"misaligned AI systems that are not calibrated to operate within legal, regulatory, and ethical boundaries can also engage in behaviour that harms financial stability."**

The **BIS** describes the same in one word — **"automaticity"**: AI making decisions independently and without human intervention at speeds beyond human capacity, with firms running similar algorithms producing **herding, liquidity hoarding, runs, fire sales**, and even **"collusive outcomes"** that arise **without anyone instructing the models to collude**. The **IMF** (Global Financial Stability Report, Oct 2024, and a 2023 FinTech Note on generative AI in finance) catalogues the same channels: bias, opacity, robustness, cyberthreats, and new transmission channels for systemic risk.

This is the most important paragraph in this file for staying unbiased: **the mainstream, non-alarmist, institutional view is that AI genuinely threatens financial stability — but through boring, structural channels (concentration, correlation, cyber, opacity), not through an evil superintelligence.**

---

## 3. What the people building it say (their own words)

These are quoted verbatim from `controlai.org/quotes` (each with its original source). Read them as **stated opinions and personal probability estimates by the leaders of the field — not established fact.** Note two things: (1) the same people also stand to gain from both building the systems and shaping the rules around them; and (2) ControlAI is an **AI-safety advocacy organization**, so its collection is curated toward the risk side — the dissenting view is in §4.

- **Sam Altman (OpenAI):** "Mitigating the risk of extinction from AI should be a global priority alongside other societal-scale risks such as pandemics and nuclear war." *(May 2023)* — "A misaligned superintelligent AGI could cause grievous harm to the world." *(Feb 2023)* — "We are past the event horizon; the takeoff has started." *(Jun 2025)*
- **Dario Amodei (Anthropic):** "My chance that something goes really quite catastrophically wrong on the scale of human civilization might be somewhere between 10 per cent and 25 per cent." *(Oct 2023)* — "We are considerably closer to real danger in 2026 than we were in 2023." *(Jan 2026)*
- **Elon Musk (Tesla/xAI):** "Mark my words — AI is far more dangerous than nukes." *(Mar 2018)* — "I don't think humans will be in control of something that's vastly more intelligent than humans… I think it would be foolish to assume that there's any way to maintain control over that." *(Feb 2026)*
- **Demis Hassabis (Google DeepMind):** "We must take the risks of AI as seriously as other major global challenges, like climate change." *(Oct 2023)*
- **Ilya Sutskever (SSI / ex-OpenAI):** "It's not that it's going to actively hate humans and want to harm them, but it is going to be too powerful — and I think a good analogy would be the way humans treat animals." *(Nov 2019)*
- **Bill Gates:** "Could a machine decide that humans are a threat, conclude that its interests are different from ours, or simply stop caring about us?" *(Mar 2023)*
- **Holden Karnofsky (Open Philanthropy):** "They don't have to be more capable than humans. They could be equally capable, and there could be more of them." *(Jul 2023)*
- **Mustafa Suleyman (Microsoft AI):** "Systems that can endlessly improve and adopt their own purposes must be avoided at all costs." *(Nov 2025)*
- **Sundar Pichai (Google) — the measured outlier among the warnings:** "I think the underlying risk is actually pretty high" but he is "optimistic on the p(doom) scenarios," arguing humanity's collective response is self-modulating. *(Jun 2025)*

---

## 4. The dissenting view (for balance)

A large and credentialed part of the field thinks the existential-risk framing is wrong:

- **Yann LeCun (Meta, Turing Award):** calls fears that superintelligent AI will take over "**preposterously ridiculous**," and said the idea that today's systems could pose an existential threat is "**complete B.S.**" — his argument is that current large language models lack memory, reasoning, planning, and world-understanding ("a system smarter than a house cat" doesn't even have a design yet), so the claimed path to AGI doesn't hold.
- **Joelle Pineau (Meta VP, AI research):** calls the existential-risk focus "unhinged," and notes the "risk = probability × cost" framing effectively assigns infinite cost to a never-observed outcome.
- **Meredith Whittaker (Signal president):** "There's no more evidence now than there was in 1950 that AI is going to pose these existential risks."
- **The commercial-motive critique (LeCun, and others like François Chollet):** the loudest existential-risk warnings conveniently come from the firms that are *ahead* — "at the moment, OpenAI is in a position where they are ahead, so the right thing to do is to slam the door behind you."

The honest position: **the field is split.** The risk is real and worth taking seriously (the regulators' structural concerns in §2 don't depend on either camp being right), but "AI will destroy the financial system" is a contested prediction, not a fact.

---

## 5. Realistic "AI goes rogue on the money system" scenarios

Each is labelled with what grounds it and how plausible it is. The first three are continuations of things that have already happened; the fourth is the genuinely speculative one.

### A. Errant trading/execution agent → flash-crash-scale disruption
- **What:** an AI agent mis-executes (a bug, a mis-specified objective, or a wrong inference), issuing millions of orders in minutes across markets.
- **Grounding:** 2010 Flash Crash, 2012 Knight Capital — but now with genuinely autonomous agents and far more automation, and (per §2) many firms running *the same* models, so errors **correlate** instead of cancelling out.
- **Plausibility:** high, precedented. This is the most likely "money system goes wrong" event.

### B. Autonomous AI fraud at scale → collapse of trust in instructions
- **What:** AI agents scrape public footage, clone executives, and run interactive deepfake calls and voice-phishing at a volume humans can't match, defeating the "verify the person" controls.
- **Grounding:** Arup ($25.6M), the 2019/2021 voice-clone cases. Already happening; the only question is scale.
- **Plausibility:** high and **already unfolding.**

### C. AI-accelerated cyberattack on payment/clearing infrastructure → multi-day outage
- **What:** AI-assisted attackers hit payment rails, card networks, a clearinghouse, or a government treasury, freezing payments, cards, and ATMs for days.
- **Grounding:** MEF/INC Ransom (Panama, 2025); FSB's "cyber" channel; the general ransomware trend against financial targets.
- **Plausibility:** medium-high and rising. Personal impact is direct (see §8).

### D. Misaligned superintelligence manipulating markets/currency for its own goals
- **What:** the popular "rogue AI" image — an AI that can out-think human operators and quietly moves markets, drains or inflates assets, or re-routes money to serve an objective nobody intended.
- **Grounding:** **none — no precedent.** This is the scenario the leaders in §3 debate and the dissenters in §4 dismiss. Highest uncertainty of all.
- **What it would actually touch (the map of the money system):** payment rails (cards, ACH-style transfers), clearing and settlement, messaging (SWIFT-equivalent), central-bank RTGS/ledgers and any digital currency, exchanges, ATMs. Because these are few, concentrated, and highly correlated, a competent misaligned AI would go for them first — which is also why regulators watch them.
- **Plausibility:** genuinely unknown — the honest answer is "depends which expert you ask."

---

## 6. Why the money system is a special target

Money is the one system where **correlated behaviour is itself the failure mode** (a bank run is everyone doing the same thing). An AI — whether buggy, weaponised, or misaligned — doesn't need to be "superintelligent" to cause damage there; it only needs to make many participants act the same way at the same time (the FSB/BIS "herding" channel). That is why the financial system is singled out by regulators even though the doomsday scenario is unproven.

---

## 7. Panama-specific exposure

- **Dollarised economy** — Panama has no independent monetary policy to fall back on; a global dollar/financial-system shock arrives **directly**, without a local buffer.
- **Canal revenues flow through the MEF** — already breached (INC Ransom, Sep 2025), so the highest-value government financial target has precedent.
- **Small, finite financial sector** relying on correspondent banking — a systemic event or a loss of trust in international settlement hits Panama's ability to transact externally.
- **AIG (Autoridad Nacional para la Innovación Gubernamental)** is the digital-government authority; its systems are part of the target surface for scenario C.

The key point: **Panama doesn't need to be directly attacked to be badly hit** by an AI-driven financial-system event — its dollarisation and correspondent-banking dependence transmit the shock.

---

## 8. What you can actually do (and what you can't)

A step-by-step guide for the person and the small business is in `../preparedness/no-internet.md`; this section is the summary.

Be honest about the limits: **no individual preparation stops a systemic AI-finance event.** What you *can* control:

- **Verify every payment instruction by an independent channel** — the Arup lesson. A voice or a video call is no longer proof of identity. Confirm by a separate, previously-known number or in person.
- **Keep a cash reserve** (small bills) — a payment/card/ATM outage can last days (scenario C).
- **Offline backups** of documents and contacts; **digital hygiene** (updates, MFA, unique passwords).
- **Know official (non-internet) alert channels** — in a disinformation-heavy event, the government's radio/official channels outlast social media.
- **Treat "the AI is about to destroy everything" and "there's nothing to worry about" with equal scepticism** — the field is split (§3–§4); the regulators' structural concerns (§2) are the part worth planning around.

## Sources

- ControlAI — quotes (all §3/§4 quotes, verbatim with individual source links): https://controlai.org/quotes
- SEC — In the Matter of Knight Capital Americas LLC (Rel. 34-70694): https://www.sec.gov/files/litigation/admin/2013/34-70694.pdf
- Fortune — "Why Knight lost $440 million in 45 minutes": https://fortune.com/2012/08/02/why-knight-lost-440-million-in-45-minutes/
- Mondaq — "Rogue Trader: The Knight Capital IT Crash" (Flash Crash + Knight): https://www.mondaq.com/uk/it-and-internet/197952/rogue-trader-the-knight-capital-it-crash
- Ars Technica — "Deepfake scammer walks off with $25 million": https://arstechnica.com/information-technology/2024/02/deepfake-scammer-walks-off-with-25-million-in-first-of-its-kind-ai-heist
- CNN (May 2024) — Arup confirms deepfake loss: https://www.cnn.com/2024/05/16/tech/arup-deepfake-scam-loss-hong-kong-intl-hnk
- WSJ (2019) — UK CEO voice-clone fraud: https://www.wsj.com/articles/fraudsters-use-ai-to-mimic-ceos-voice-in-unusual-cybercrime-case-11567157402
- Forbes (2021) — $35M voice-clone fraud: https://www.forbes.com/sites/thomasbrewster/2021/10/14/huge-bank-fraud-uses-deep-fake-voice-tech-to-steal-millions/
- FSB — "The Financial Stability Implications of Artificial Intelligence" (Nov 2024): https://www.fsb.org/uploads/P14112024.pdf
- BIS — "Artificial intelligence and the economy: implications for central banks": https://www.bis.org/publications/artificial-intelligence-economy-implications-central-banks.pdf
- IMF — Global Financial Stability Report, Oct 2024: https://www.imf.org/en/publications/gfsr/issues/2024/10/22/global-financial-stability-report-october-2024
- IMF FinTech Note 2023/006 — "Generative Artificial Intelligence in Finance: Risk Considerations": https://www.elibrary.imf.org/view/journals/063/2023/006/063.2023.issue-006-en.xml
- MIT Technology Review — LeCun: existential-risk fears "ridiculous": https://www.technologyreview.com/2023/06/20/1075075/metas-ai-leaders-want-you-to-know-fears-over-ai-existential-risk-are-ridiculous
- WSJ / TechCrunch (Oct 2024) — LeCun: "complete B.S.": https://techcrunch.com/2024/10/12/metas-yann-lecun-says-worries-about-a-i-s-existential-threat-are-complete-b-s/
- MIT Technology Review — "How existential risk became the biggest meme in AI" (Whittaker, Chollet): https://www.technologyreview.com/2023/06/19/1075140/how-existential-risk-became-biggest-meme-in-ai
- BleepingComputer — Panama MEF breach (INC Ransom): https://www.bleepingcomputer.com/news/security/panama-ministry-of-economy-discloses-breach-claimed-by-inc-ransomware/
