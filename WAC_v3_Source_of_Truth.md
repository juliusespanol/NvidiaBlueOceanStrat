# NVIDIA Deck: Source of Truth (Allen's WAC v3 + Allen's Deck Review)

**Sources (both from Allen):**
1. `WAC - NVIDIA v3.docx` (Learning Team 2), sections 1–7 below. **What we say:** facts, numbers, problem, questions, options, moves, justification.
2. `NVIDIA_Deck_Review_vs_Our_Outline.md`, section 9 below. **How the deck is built:** slide flow, which frameworks go on main slides, plain titles, poll tags, backups, close.

**Adopted:** Nov 9, 2026
**Rules:**
- If the deck disagrees with these two, the deck changes.
- **If the two disagree with each other, WAC v3 wins.** It was written after the review and fixes the review's break-even math (17.5% → 13.8%).
- Deck content that neither source covers stays only if it does not contradict them.
**Tags:** GIVEN = in the case · COMPUTED = calculated from case figures · INTERNET = not in the case · OUR PROPOSAL = our idea, not in the case

---

## 1. Case facts

- NVIDIA made the first GPU in **1999**. In **2007** it released **CUDA**, software that lets developers use NVIDIA chips for any heavy computing task.
- AI chip demand took off after **ChatGPT launched in November 2022**.
- **FY2024** (year to January 2024): revenue **+126% to $60.9B**; data center revenue **+217% to $47.5B**.
- Gross margin **72.7%** vs **AMD 47%** and **Intel 41%**.
- Customers waited **up to 18 months** for NVIDIA chips rather than buy elsewhere.
- CUDA keeps customers with NVIDIA: **300+ code libraries**, **5M+ developers**, and CUDA code **runs only on NVIDIA chips**.
- Top buyers (share of sales, **by outside estimates**): **Microsoft 15%, Meta 13%, Amazon 6%, Alphabet 6%**, together **about 40%**. All four now build their own AI chips.
- Open initiatives such as the **UXL Foundation** aim to reduce dependence on CUDA. **PyTorch** runs on chips from several makers, which could make switching easier.
- Regulators **blocked NVIDIA's purchase of ARM**, and **export rules** limit its China sales.
- **January 2025:** DeepSeek claimed it trained a leading model for **under $5.6M**. NVIDIA lost **$600B** of market value in one day.

## 2. Problem statement

> NVIDIA charges premium prices because its customers are locked into CUDA. Its four biggest customers now have both the reason and the means to leave. **How can NVIDIA keep its pricing power and keep growing without pushing them out faster or drawing antitrust action?**

## 3. Analysis: five questions

### Q1. How much rides on AI data centers?
- Data center share of revenue: **39.4% (FY22) → 55.6% (FY23) → 78.0% (FY24)**.
- Operating margin **15.7% → 54.1%** in one year. Operating expenses grew only **2%**, so **about 85 cents of each extra sales dollar** became operating profit.
- Blue Ocean portfolio map: data center is NVIDIA's **only proven pioneer**. If rival chips catch up, it becomes a **migrator**.
- AI Foundry and enterprise AI services **could become the next blue ocean**, but the case gives them **no revenue yet**.

### Q2. Why can NVIDIA charge so much?
- Estimated GPU shipments **+42% (2.64M → 3.76M)** while data center revenue **+217%**.
- **Caveat:** the gap is **not a pure price measure**, because data center revenue also includes networking and a richer product mix. It still fits a picture of buyers paying a premium.
- H100 costs about **4×** an A100, but NVIDIA says it trains **9× faster**, so buyers get about **2.25× more training per dollar**. Buyers pay for the **finished job, not the chip**.
- Switching is costly, so **demand is less sensitive to price**, and the profit-maximizing price (**MR = MC**) carries a **higher markup**.

### Q3. Who can break the lock-in?
- **Five Forces:** buyer power and threat of substitutes are both **high**, and both come from **the same four firms**.
- **Rivalry from other chipmakers is weaker.** AMD expects about **$4.5B** of AI chip revenue in 2024 vs NVIDIA's expected **$76B** from data centers, and AMD's software trails CUDA.
- **Four Corners** on the big buyers: their drivers are **cutting the "NVIDIA tax"** and **securing supply**.
- Amazon, Microsoft and Google hold **65% of the cloud market (32% + 23% + 10%)**.
- **Prediction:** they move work in-house wherever their own chips can do it at lower cost. Amazon already has **Inferentia** (running models) and **Trainium** (training).
- **DeepSeek is a smaller worry.** It changes **how much** computing AI needs, not **who supplies it**, and its models were **trained on NVIDIA chips**.

### Q4. What is it worth to keep them?
- Top four buy about **$24.4B a year** (40% × $60.9B), which earns about **$17.7B gross profit**.
- **A 10% discount** to them costs about **$2.4B a year** (assuming unit costs stay the same).
- **Holding the price** while they move **a quarter** of purchases in-house loses about **$4.4B**.
- **Break-even: 13.8%** (10% ÷ 72.7%). The discount pays for itself if it keeps more than 13.8% of their business. That is about **1 in 7 dollars**.
- These numbers are **illustrative**.
- **Antitrust condition:** tie any discount to **volume commitments**, **never** to a promise not to build their own chips, because regulators would read that as an exclusive deal.

> Check (COMPUTED): 0.40 × 60.9 = 24.36 · 24.36 × 0.727 = 17.71 · 10% × 24.36 = 2.44 · 25% × 17.71 = 4.43 · 10 ÷ 72.7 = 13.76%. After a 10% discount the top-4 gross margin would be about 69.7%.

### Q5. Where can NVIDIA create new demand?
- Many companies have **put off custom AI projects** because they lack the staff or infrastructure to build and run them.
- Blue Ocean: growth comes from turning **noncustomers into buyers**. AI Foundry and its enterprise services could do that.
- **Proposed pilot: mid-sized insurers.** NVIDIA packages a tool that helps **claims staff find answers in their own policy documents**, **hosted by a cloud partner**, built on **NVIDIA's own software (NIM and NeMo)** so the demand stays on NVIDIA chips.
- The pilot is **small on purpose**. It tests whether making AI easier to start turns shelved projects into paying customers.

## 4. Options screen (case Q14 + our addition)

| Option | Keeps lock-in? | Less reliance on top 4? | Antitrust risk | Decision |
|---|---|---|---|---|
| E. Strengthen CUDA and developer support | Yes | Indirectly | Medium | **Adopt (Move 1)** |
| B. Low-cost custom chips for big buyers | Partly | No | Low | **Adopt within Move 2** |
| *Our addition, not a case option:* Profitable interoperability (plug-in path, volume pricing) | Yes | No | Low | **Adopt (Move 2)** |
| C. Broaden the customer base (enterprise and sovereign AI) | Yes | Yes | Low | **Adopt (Move 3)** |
| A. Exclusive contracts | Short term | No | High | **Reject** |
| D. Sell design know-how to chip builders | No | No | Low | **Reject** |

## 5. Recommended strategy

**One line:** NVIDIA should **make staying with it the cheapest and fastest option** for its customers instead of trying to make leaving impossible. Over time this also means **selling the whole AI system** (racks, networking, software, services), so NVIDIA depends less on chip sales alone.

Three moves, **approved in order**:

| Move | Approval | What it is |
|---|---|---|
| **1. Strengthen CUDA and developer support** | **Approve now** | Keep improving libraries, models and tools so customers can build and run AI more easily. Make sure NVIDIA hardware stays the **fastest choice when developers work in PyTorch**. |
| **2. Support profitable interoperability** | **Test first** | Let the big buyers' own chips **plug into NVIDIA's high-bandwidth racks and networking**, offer **semi-custom products**, and give **volume discounts to the top four where the break-even supports it**. Check each arrangement to confirm it still earns enough profit. This moves NVIDIA **from selling chips into selling AI infrastructure**. |
| **3. Expand enterprise and sovereign AI** | **Pilot first** | Help companies that cannot afford their own AI infrastructure deploy AI through **AI Foundry**, **starting with the insurer pilot**. **Governments** building national AI capacity are a second target (**OUR PROPOSAL, not covered in the case**). **Scale only if** first-time buyers move to paid use and revenue covers onboarding and support. |

**NVIDIA gives up:** exclusive deals · large acquisitions · its top margins on sales to the four biggest buyers.

**We would watch:** the top four's share of sales · the gross margin trend · any big buyer moving its **training** off NVIDIA.

## 6. Justification

| Move | Comes from | Logic |
|---|---|---|
| Move 1 | **Q2** | Switching costs make demand less sensitive to price, which protects the **73% margin**. |
| Move 2 | **Q3 + Q4** | The buyers who can leave are **40% of sales**, and losing their volume costs more than a targeted discount once **more than 13.8%** would go. The plug-in path changes what their chips mean: today a buyer's chip **replaces** NVIDIA's; running inside NVIDIA's racks and software, it **adds to** what NVIDIA sells. **A substitute becomes a complement.** |
| Move 3 | **Q1 + Q5** | With **78% of revenue from one business** and **40% from four buyers**, NVIDIA needs growth that does not rest on a few chip buyers. The pilot tests one at low cost. |

- **We would not port CUDA to rival chips.** That would remove the main reason to buy NVIDIA. Interoperability happens at the level of **racks, networking and software**.
- **Rejected:** exclusive contracts, because regulators already watch NVIDIA closely; selling design know-how, because it would help rivals copy NVIDIA.

## 7. Weak point (timing)

NVIDIA's revenue is still growing fast, so the threat does not yet show in the numbers. But **competition usually hurts margins before it hurts sales**, and **in-house chips take years to mature**. **The time to act is now, while NVIDIA is strong.**

---

## 8. Slide plan (final)

Built from: WAC v3 (content) + Allen's review (structure) + Kim's deck (changes that match both).
Status: **DONE** · **KEEP** = no change · **SMALL** = wording or one line · **EDIT** = content changes · **REBUILD** · **NEW**

| # | Slide | Status | What to do | Source |
|---|---|---|---|---|
| 1 | Hook: −$600B | **DONE** | `<$5.6M`, "claimed" | WAC |
| 2 | Timeline | SMALL | Add **$60.9B** / **$47.5B** under +126% / +217%. Title: see decision 1 | WAC, Kim |
| 3 | Loop + cost of leaving | **DONE** | 5M+ developers, CUDA code runs only on NVIDIA. Title: see decision 1 | WAC |
| 4 | Top 4 build own chips | EDIT | Title → "**Four customers that make up 40% of NVIDIA's sales are now building their own AI chips**". **$24.4B**. Label shares "**outside estimates**" | Review §7, WAC, Kim |
| 5 | Problem + **5 questions** | EDIT | WAC problem question (Kim's wording). Q4 → "What is it worth to **keep them**?". **Add Q5** "Where can NVIDIA create new demand?" | WAC, Kim |
| 6 | Q1: 78% from one business | SMALL | "AI Foundry: potential pioneer, **tested by a pilot (slide 12)**". Optional: opex grew only 2% | WAC, Kim |
| 7 | Q2: price vs volume | EDIT | Kim's version: title "**Data center revenue grew faster than estimated GPU shipments**" + **not-a-pure-price caveat** | WAC, Kim |
| 8 | Q2: finished job | SMALL | Add **MR = MC → higher markup** line. Notes: "in the case example" | WAC, Kim |
| 9 | Q3: Five Forces | SMALL | Rivalry → "**weaker**": AMD **$4.5B** AI chips vs NVIDIA **$76B** data center (~17×), software trails CUDA | WAC, Review §4 #3 |
| 10 | Q3: Four Corners | EDIT | Kim's version: "move **workloads** in-house where cheaper" + **Inferentia / Trainium**. Add "**DeepSeek is a smaller worry**: changes how much compute, not who supplies it; trained on NVIDIA" | WAC, Kim, Review §6 |
| 11 | Q4: break-even | **REBUILD** | Kim's version: **10% discount, $2.4B vs $4.4B, 13.8% (~1 in 7)**, discount slider, $100 example in notes. Add: discount tied to volume commitments, **never to a promise not to build own chips** | WAC, Kim |
| 12 | **Q5: new demand** | **NEW** | Noncustomers with shelved AI projects → AI Foundry → **mid-sized insurer claims assistant**, cloud partner, **NIM + NeMo**, small on purpose | WAC |
| 13 | Options | EDIT | Kim's version (B = case option, separate "**Our addition**" row). B wording/values per WAC: "low-cost custom chips", lock-in **Partly**. C = "enterprise **and sovereign** AI". No weighted scores | WAC, Kim, Review |
| 14 | Recommendation (ERRC) | EDIT | Add **approve now / test first / pilot first** tags per move. "**Sell the whole AI system**". Move 3 = insurer pilot (Kim) + **governments (OUR PROPOSAL)** + scale gate. Keep "We give up" line | WAC, Kim, Review |
| 15 | Justification trace | EDIT | Kim's Q3/Q4 rows (13.8%, volume commitments). Move 3 ← **Q1 + Q5**. Add "**a substitute becomes a complement**", "**we don't port CUDA**". One line: **seven tests** passed (detail in B2) | WAC, Kim, Review §2 |
| 16 | Risks + weak spot | EDIT | Kim's version (pilot-doesn't-convert row; TSMC kept as "monitor, no second source" in notes). Add WAC's **3 watch metrics**: top-4 share of sales · gross margin trend · big buyer moving **training** off NVIDIA | WAC, Kim, Review §4 #10 |
| 17 | Close | KEEP | Allen's question: "**If you were Microsoft, would you still build your own chip if it could plug into NVIDIA's systems?**" + NVLink Fusion (INTERNET). Only Kim's wording fix: "**pursuing a similar approach**" | Review §3, §7 |
| B1 | 15 polling answers | SMALL | Kim's Q14 note. Q15 blank `[__]` → **needs the letter from Kim**. Renumber slides | Review, Kim |
| B2 | Frameworks in reserve | SMALL | Renumber slide references | Review |

**Not adopted from Kim:** the separate "What Jensen approves first" slide (its content goes onto slide 14 as tags and slide 16 as watch metrics, which keeps the deck at Allen's ~17–18 slides) · the new close question with 3 cards (Allen's review picks the Microsoft question) · Kim's slides 1–4 (older version, no images).

**Speaker split (Review §7, adjusted for Q5):** Group 1 = slides 1–5 · Group 2 = slides 6–10 (Q1–Q3) · Group 3 = slides 11–17 (Q4, Q5, options, recommendation, justification, risks, close). Group 3 is now the longest. Consider moving slide 11 (Q4) to Group 2.

**Also update:** `NVIDIA_Talking_Points.md` for each changed slide ("of 16" → "of 17", new Q5 script, speaker table).

## 9. Allen's deck review: build rules we follow

| Rule | In our deck |
|---|---|
| Logic chain: problem → questions → one finding each → moves → trace | ✅ (now 5 questions, per WAC) |
| **Five Forces + Four Corners** on main slides; PESTLE, SWOT/TOWS, seven tests, CEO actions, motive/means in backup | ✅ slides 9–10, B2 |
| **PMS map** with the "if NVIDIA stands still" toggle on Q1 | ✅ slide 6 |
| **ERRC grid** + "We give up" line for the recommendation | ✅ slide 14 |
| **No weighted option scorer**; screen options against findings | ✅ slide 13 |
| Plug-in idea merged into Move 2 | ✅ |
| Risks with early warning signals, compressed | ✅ slide 16 |
| Close: Microsoft question, then **NVLink Fusion** labelled INTERNET / after the case | ✅ slide 17 |
| Poll answers tagged on the slide where the evidence sits + B1 backup | ✅ |
| **Plain, literal titles, no metaphors** | ⚠️ see decision 1 |
| H100 vs A100: −14% TFLOPS/$ but 2.25× per training job | ✅ slide 8 |
| Gaming dipped 27% then recovered; **no "98%" share**; no "20× cheaper" headline; 65% cloud labelled COMPUTED; no $91B; no second-sourcing | ✅ |
| DeepSeek = hook, ranked below the hyperscalers | ✅ (add "smaller worry" line on slide 10) |
| Seven tests: one line on the justification slide | ❌ → add on slide 15 |

### Where the review and WAC v3 disagree (WAC wins)

| Item | Review says | WAC v3 says | We use |
|---|---|---|---|
| Break-even | ~17.5%, "1 in 6 dollars" | **13.8%** (10% discount ÷ 72.7%) | **13.8%** |
| Number of questions | Four | **Five** (adds Q5 new demand) | **Five** |
| Slide 7 title | "Growth came mostly from higher prices, not more chips" | Not a pure price measure (networking, mix) | **Kim's caveated title** |
| Slide 10 title | Move **inference** in-house, keep NVIDIA for frontier training | Move **work** in-house wherever cheaper | **WAC** |
| What NVIDIA gives up | Top margins **on inference** | Top margins **on sales to the four biggest buyers** | **WAC** (already in deck) |
| Move 3 | Grow customers who cannot build their own chips | AI Foundry **insurer pilot** + governments, scale gate | **WAC** |

### Decisions still open

1. **Slide 2 and 3 titles.** Allen's review uses plain sentences: "*ChatGPT turned a gaming-chip company into the world's most valuable company in two years*" and "*NVIDIA sells chips, software and a developer community as one package, and that package is hard to leave*". Ours are "NVIDIA's Journey to $3 Trillion" and "The cost of leaving". Keep ours or switch to Allen's?
2. **Q15 letter** for the blank in B1 (from Kim).
