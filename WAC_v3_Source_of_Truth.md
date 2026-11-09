# NVIDIA Deck: Source of Truth (Allen's WAC v3)

**Source:** `WAC - NVIDIA v3.docx` (Allen, Learning Team 2)
**Adopted:** Nov 9, 2026
**Rule:** WAC v3 wins. If the deck disagrees with this file, the deck changes. Deck content that WAC does not cover stays only if it does not contradict WAC.
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

## 8. Slide plan (deck → WAC v3)

Status: **KEEP** = no change · **SMALL** = wording or one line · **EDIT** = content changes · **REBUILD** = redo the slide · **NEW** = add a slide

| New # | Current # | Slide | Status | What to do |
|---|---|---|---|---|
| 1 | 1 | Hook: −$600B | SMALL | DeepSeek figure `<$6M` → **`<$5.6M`** (slide + talking points) |
| 2 | 2 | Timeline to $3T | KEEP | Nothing. Matches WAC (1999 GPU, 2007 CUDA, Nov 2022 ChatGPT, +126%, +217%) |
| 3 | 3 | Loop + cost of leaving | KEEP | Nothing. Optional: add "CUDA code runs only on NVIDIA chips" to the switching panel |
| 4 | 4 | Top 4 build own chips | SMALL | Label the 15/13/6/6% as **"outside estimates"** |
| 5 | 5 | Problem + questions | EDIT | Use WAC's problem question ("keep pricing power **and keep growing** without pushing them out faster or drawing antitrust action"). **4 → 5 questions**: Q4 becomes "What is it worth to **keep them**?", add **Q5 "Where can NVIDIA create new demand?"** |
| 6 | 6 | Q1: 78% from one business | KEEP | Already matches WAC. Optional: add "opex grew only 2%" |
| 7 | 7 | Q2: price vs volume | EDIT | Add the caveat: **revenue per chip includes networking and a richer mix, so it's not a pure price measure**. Soften the title to "buyers paid a premium" |
| 8 | 8 | Q2: finished job | SMALL | Add one line: switching is costly → demand less price-sensitive → **MR = MC gives a higher markup** |
| 9 | 9 | Q3: Five Forces | SMALL | Rivalry box: "**weaker**" + **AMD $4.5B vs NVIDIA $76B**, software trails CUDA |
| 10 | 10 | Q3: Four Corners | SMALL | Add **Inferentia / Trainium** as the in-house example + **"DeepSeek is a smaller worry: changes how much compute, not who supplies it; trained on NVIDIA"** |
| 11 | 11 | Q4: break-even | **REBUILD** | Switch to the **10% discount** model: **$2.4B vs $4.4B, break-even 13.8% (~1 in 7)**. Slider becomes "Discount to top 4". Add the **volume-commitment, never no-build-promise** condition. Fix the speaker notes |
| 12 | — | **Q5: new demand (insurer pilot)** | **NEW** | Noncustomers with shelved AI projects → AI Foundry → **mid-sized insurer claims tool**, cloud-hosted, **NIM + NeMo**, small on purpose |
| 13 | 12 | Options screen | EDIT | Use **WAC's table exactly**: B = "low-cost custom chips" (adopt within Move 2), add the **"Our addition: profitable interoperability"** row, use WAC's columns (drop the margin cost column) |
| 14 | 13 | Recommendation (ERRC) | EDIT | Add **approve now / test first / pilot first**. Add "**sell the whole AI system**". Move 3 = AI Foundry **starting with the insurer pilot** + governments (flagged **OUR PROPOSAL**) + "scale only if…". Trim neo-clouds / inference / edge (not in WAC) |
| 15 | 14 | Justification trace | EDIT | Move 1 ← Q2 · Move 2 ← **Q3 + Q4 (13.8%)** · Move 3 ← **Q1 + Q5**. Add "**a substitute becomes a complement**" and "**we don't port CUDA**". Add the two rejection reasons |
| 16 | 15 | Risks + weak spot | SMALL | Add WAC's **three watch metrics**. Weak-spot text already matches WAC |
| 17 | 16 | Close: Microsoft question + NVLink Fusion | KEEP | Nothing. Doesn't contradict WAC |
| B1 | B1 | 15 polling answers | SMALL | Update slide numbers (+1 after slide 11) |
| B2 | B2 | Frameworks in reserve | SMALL | Update slide-number references |

**Also update:** `NVIDIA_Talking_Points.md` for every changed slide ("of 16" → "of 17", and the new Q5 script).
