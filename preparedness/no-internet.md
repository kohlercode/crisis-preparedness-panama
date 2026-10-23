# Weeks without internet — preparing as a person and as a small business

The practical companion to `../events/cyber-ai-finance.md` (the *why* and *what if*). This file is the *how*: what an average person and a small business owner do **now** so that a cyber pandemic — or any event that cuts internet for weeks — is survivable rather than crippling.

## Read this first — the honest framing

A **total, planet-wide internet blackout for weeks is extraordinarily unlikely.** The internet has no single switch; it is millions of independently-run networks, and its routing was designed to route around damage. So read "worldwide attack" realistically: the precedents below are *nation-scale* or *service-scale* outages, not a global off-switch. But **the preparation is almost identical**, and a coordinated attack that degrades payments, DNS, cloud, and government services for weeks in your region is a real, precedented risk.

### The precedents (what "weeks without internet" actually looked like)

| Event | What happened | Duration |
|---|---|---|
| **Tonga, Jan 2022** (Hunga Tonga–Hunga Ha'apai eruption) | Both submarine cables severed; a nation of ~100,000 lost internet, phones, and outside contact almost entirely. Ash blocked satellite phones at first; only HF radio and a few satellite links worked. | Main island ~**5 weeks** offline; one island group ~**16 months** |
| **Tonga, Jun–Jul 2024** (earthquake cable damage) | Northern islands cut off; a third of the population lost internet, and the government ordered Starlink to stop operating (no licence). | **2+ weeks** and counting |
| **Estonia, Apr–May 2007** | Nation-state DDoS campaign took down parliament, banks, newspapers, and ministries in waves; online banking was unusable. | ~**3 weeks** |
| **Egypt, Jan 2011** | The state ordered ISPs to pull the plug; ~88% of the country's internet routes vanished overnight. | ~**5 days**, state-imposed |
| **Dyn / Mirai, Oct 2016** | A botnet of hijacked cameras/routers DDoS'd a core DNS provider, taking down Twitter, Netflix, Reddit, PayPal and more. | ~**8 hours** |
| **CrowdStrike, Jul 2024** | A faulty security update crashed ~8.5 million Windows machines — airlines, hospitals, banks, broadcasters switched to paper/manual. | Recovery ~**10 days** |

The single best analogue for "your whole country loses internet for weeks" is **Tonga 2022**: not an attack, but the effect is the lesson — and note how people coped: door-to-door checks, radio, cash, and patience.

### What actually breaks first

- **Payments** — cards, ATMs, online banking, and mobile-payment apps (Yappy/Clave equivalents) all go dark. This is the single most painful dependency.
- **Messaging** — WhatsApp, email, cloud documents.
- **Government services** — portals, benefits, appointments.
- **Logistics & supply** — ordering, shipping trackers, inventory systems, POS terminals.
- **Information** — news, maps, directions, verification of what's true.

A key nuance worth knowing: **in a partial outage, SMS and ordinary phone calls often keep working when apps and websites die**, because they don't depend on DNS or cloud services. Plan for the worst (nothing works), but know that "data is down, calls/SMS still up" is a common intermediate state.

---

## For the average person

### 1. Cash — your first and most important prep
- Keep a **cash reserve in small bills** (ones, fives, tens). With cards and ATMs down, cash is the only payment that works. In Panama this is straightforward — the currency **is** US dollars.
- Aim for **at least 2–4 weeks of routine spending** in cash, more if you can. Break it into small denominations so small purchases don't require change.

### 2. Documents — offline copies of everything that matters
- **Paper copies** of: ID (cédula/passport), medical records and prescriptions, insurance policies, property/rental documents, bank account numbers, and a written contact list (phone numbers, not just names in a phone).
- A **printed list of emergency numbers** (911, 103/104, SINAPROC, Cruz Roja — see `plan.md`) — your phone's contacts are useless if the phone dies or the account sync fails.

### 3. Communication — how you'll hear and reach people
- A **battery or hand-crank/solar radio** for **AM/FM broadcast** — the one channel that reliably keeps working in an outage (see `supplies.md` for the solar/crank radio already priced). Emergency alerts and official information go out on radio.
- Agree **meeting points and a phone tree** with family/neighbours ahead of time (see `plan.md`). In Tonga, the first response was literally **door-to-door** — know your neighbours.
- If you're serious about resilience, a **satellite messenger or phone** is the strongest fallback — but it's expensive and, as Tonga 2024 showed, can be subject to regulatory/licensing surprises. Don't make it your only plan.

### 4. Information you can't look up later
- **Printed local maps** (roads, plus your neighbourhood), and printed copies of the key pages of this archive (`plan.md`, `water.md`, `first-aid.md`).
- Water, food, and medication are covered in `water.md`, `food.md`, and `first-aid.md` — but note the cross-dependency: if the *power* is also out (a cascade), your stored water/food plan becomes the backbone. Assume some cascade; don't assume internet-only.

### 5. Digital hygiene *now* (so a bad day doesn't lock you out)
- Offline **password manager** (or a written password book kept safe) — don't depend on a cloud sync you can't reach.
- **Local backups** of important files (photos, documents) on a drive you control, not just the cloud.
- Turn on **MFA** everywhere now, so the *attack itself* doesn't cost you your accounts before the outage does.

### 6. Mental health is part of preparedness
- Weeks without internet means **no streaming, no social media, no casual news**. Have offline books, games, cards, and a hobby. Boredom and anxiety are real loads, not luxuries — and they'll hit harder if you're also anxious about the emergency. This is routinely the most under-prepared dimension.

---

## For the small business owner

The business version of the same principle: **the goal is to keep operating (and keep getting paid) when the tools you normally run on are gone.**

### 1. Money & payments
- **Cash reserve** — for payroll, change-making, and supplier payments when cards and bank transfers fail. Decide now, in writing, how staff get paid if direct deposit is down.
- **Know which of your payment tools work offline.** Many POS terminals have an **offline "store-and-forward" mode** that queues transactions and settles when the network returns — check with your provider whether yours does, and enable/test it.
- **Pre-arrange manual fallbacks** with your bank: cheque runs, cash withdrawal limits raised, a branch-contact you can reach by phone.

### 2. Data & systems — the "your whole business is in the cloud" problem
- **Daily offline backups**, stored on-site **and** off-site, of everything: customer records, accounting, contracts, inventory. Test that you can actually *restore* from them.
- **Printed critical records**: customer contact list (with phone numbers), open invoices, account numbers, supplier list, and a one-page summary of who owes you and what you owe.
- If your accounting is cloud-only, keep a **parallel simple ledger** (spreadsheet on a local machine, or even paper) that you update at least weekly.

### 3. Operating without the tools
- Write **offline SOPs**: how to take an order, ring a sale, issue a receipt, and log it when the POS/website/email are all down.
- **Pre-printed forms**: paper order sheets, receipts/invoices, delivery manifests. In the CrowdStrike outage, hospitals and airlines fell back to **paper** — the ones who had it ready functioned; the ones who didn't, didn't.
- **Cross-train staff** so no single person is the only one who knows how to run a manual day.

### 4. Communications with customers & suppliers
- **Don't rely on email as the only channel.** Keep **phone numbers** (and a phone tree) for key customers and suppliers. SMS often survives when apps don't.
- Agree **radio and printed signage** as your customer-facing fallback: "Open — cash only today" on the door, and local radio if you're a larger operation.
- A **satellite link (Starlink or similar)** is the strongest single backup for a business that must stay online — but price it, and remember Tonga 2024: regulatory action can take even that away. Treat it as *one* layer, not the plan.

### 5. Supply chain & inventory
- **Diversify suppliers** so no single vendor's outage (or shipping system) stops you.
- **Hold higher local inventory** of the few things that would stop your operation, and keep **manual re-order triggers** (e.g., "reorder when below X units") written down, since your automated reorder system won't run.

### 6. Insurance & legal
- Check whether your **cyber / business-interruption** coverage actually pays for "no internet" — most policies have narrow definitions and exclusions. Know the gap *before* the event, not after.

---

## Panama-specific notes

- **Cash is US dollars** — the currency works everywhere without any system; keep small bills.
- **Mobile-payment apps (Yappy/Clave/equivalents) and online banking are internet-dependent** — they will fail in an outage. Cash is the fallback, so the cash-reserve advice above is *more*, not less, important here.
- **Official information** flows through **AM/FM radio** and SINAPROC channels; the emergency numbers are already recorded in `plan.md` (911, 103, 104, SINAPROC, Cruz Roja).
- **Panama is a dollarised economy with heavy correspondent-banking dependence** — a global or regional financial-communications disruption transmits here directly (see `../events/cyber-ai-finance.md` §7), so the payment and cash contingencies above are not hypothetical.

## The honest limit

No individual or small business fully insulates against weeks without internet — the point is to **reduce the harm and keep the essentials running**, not to be unaffected. The highest-value, lowest-cost actions are: **cash in small bills, printed documents, a radio, local backups, and knowing your neighbours.** Those five cost almost nothing and cover most of what breaks.

## Sources

- Tonga 2022 cable outage postmortem (ACM): https://dl.acm.org/doi/10.1145/3570748.3570759
- PCMag — "An Underwater Internet Cable Mishap Sent an Entire Country Back to the 1880s": https://pcmag.com/articles/tonga-underwater-internet-cable-cut-disaster
- The Guardian — Tonga without internet (2024, Starlink ordered to cease): https://theguardian.com/world/article/2024/jul/16/parts-of-tonga-without-internet-after-cables-damaged-and-starlink-ordered-to-cease-operations
- Euronews — Tonga back online after 5 weeks: https://euronews.com/next/2022/02/23/tonga-is-finally-back-online-here-s-why-it-took-5-weeks-to-fix-its-volcano-damaged-interne
- Outage Atlas — Dyn (2016) and CrowdStrike (2024): https://outage-archive.jonathanrreed.com
- Wikipedia — 2024 CrowdStrike-related IT outages: https://en.wikipedia.org/wiki/2024_CrowdStrike-related_IT_outages
- Estonia 2007 cyberattacks (syscfg.sh / NATO cyber defence): https://syscfg.sh/research/estonia-2007-cyberattacks-russia-nato
- versus.com — biggest global internet outages (Egypt 2011, Dyn 2016): https://versus.com/en/news/biggest-global-internet-outages
