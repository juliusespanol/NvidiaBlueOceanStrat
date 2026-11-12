# NVIDIA Deck: Source of Truth (WAC v3, Learning Teams 1, 2 and 9 + Allen's Deck Review)

**Sources:**
1. `WAC - NVIDIA v3.docx` (Learning Teams 1, 2 and 9, received Nov 12, 2026), sections 1–7 below. **What we say:** facts, numbers, problem, questions, options, moves, justification. It replaces both earlier WAC drafts (the Nov 9 paper and the Nov 10 `v3(1)`).
2. `NVIDIA_Deck_Review_vs_Our_Outline.md` (Allen), section 9 below. **How the deck is built:** slide flow, which frameworks go on main slides, plain titles, poll tags, backups, close.

**Adopted:** Nov 13, 2026
**Rules:**
- If the deck disagrees with these two, the deck changes.
- **If the two disagree with each other, the WAC wins.**
- Deck content that neither source covers stays only if it does not contradict them.

**Tags:** GIVEN = in the case · COMPUTED = calculated from case figures · INTERNET = not in the case · OUR PROPOSAL = our idea, not in the case

---

## 1. Case facts

- **FY2024:** revenue **+126% to $60.9B**. Data centers are **78%** of sales. Gross margin **72.7%**.
- CUDA has **300+ code libraries** and **5M+ developers**, and CUDA code **runs only on NVIDIA chips**.
- **Microsoft, Meta, Amazon and Alphabet** are about **40%** of sales **by outside estimates**. All four are developing their own AI chips.
- Open initiatives such as the **UXL Foundation** and frameworks such as **PyTorch** could make switching easier.
- NVIDIA's purchase of **ARM was dropped after objections**.
- **January 2025:** DeepSeek claimed it trained a leading model for **under $5.6M**, which triggered a one-day drop of about **$600B** in NVIDIA's market value.

Still true case facts the WAC no longer mentions (keep on slides as GIVEN if useful): 1999 first GPU, 2007 CUDA, ChatGPT Nov 2022, data center $47.5B, per-company shares (15 / 13 / 6 / 6), AMD 47% and Intel 41% margins, 18-month waits, export rules on China.

## 2. Problem statement

> NVIDIA charges premium prices because its customers are locked into CUDA. Its four biggest customers now have both the reason and the means to leave. **How can NVIDIA protect its pricing power as its largest buyers build their own chips, and where can it create new demand?**

## 3. Analysis: five questions

### Q1. How much rides on AI data centers?
- Data center share of revenue: **39.4% (FY22) → 55.6% (FY23) → 78.0% (FY24)**.
- Operating margin **15.7% → 54.1%** in one year. Operating expenses grew only **2%**, so **about 85 cents of each extra sales dollar** became operating profit.
- Blue Ocean portfolio map: data center is NVIDIA's **only proven pioneer**. If rival chips catch up, it becomes a **migrator**.
- AI Foundry and enterprise AI services **could become the next blue ocean**, but the case gives them **no revenue yet**.

### Q2. Why can NVIDIA charge so much?
- Estimated GPU shipments **+42% (2.64M → 3.76M)** while data center revenue **+217%**. The gap **can reflect chip prices, product mix and networking sales**.
- Gross margin rose **56.9% → 72.7%**, consistent with strong pricing power, although costs and product mix also affect margins.
- H100 costs about **4×** an A100 but, **on NVIDIA's reported training benchmark**, runs **9× faster**: about **2.25× the training speed per dollar** of chip price, although its **raw computing performance per dollar is lower**. Buyers pay for the **finished job, not the chip**.
- Switching is costly, so **demand is less sensitive to price**, and the profit-maximizing price (**MR = MC**) carries a **higher markup**.

### Q3. Who can break the lock-in?
- **Five Forces** points to an unusual threat: NVIDIA's biggest buyers are also building substitutes for its chips.
- **Four Corners:** their drivers are **lower costs and more control over supply**.
- Amazon already has **Inferentia** (running models) and **Trainium** (training).
- **Prediction:** large buyers shift **specific workloads** in-house **where their chips meet performance needs at lower cost**.

### Q4. How much profit is at risk if the largest buyers shift in-house?
- Top four buy about **$24.4B a year** (40% × $60.9B).
- Using the company-wide **72.7%** gross margin as a proxy, that is about **$17.7B** of gross profit.
- If they shift **25%** of purchases in-house, about **$4.4B** of annual gross profit is at risk.
- **Illustrative scenario:** same product mix, unchanged unit costs.
- It supports **testing whether interoperability can preserve profitable networking and systems sales**.
- **No discount and no break-even** in this paper (both earlier drafts had a 10% discount and a 13.8% break-even).

> Check (COMPUTED): 0.40 × 60.9 = 24.36 · 24.36 × 0.727 = 17.71 · 25% × 17.71 = 4.43. Total gross profit 60.9 × 0.727 = 44.27, so $4.4B ≈ 10% of it (deck only, not in the WAC).

### Q5. Where can NVIDIA create new demand?
- Use **AI Foundry** to reach companies that **evaluated custom AI and decided it costs too much to implement**.
- Through a **partner**, test a **standard package for one task these companies still do manually**.
- The pilot answers two questions: **(1)** do the savings justify the price for a first-time buyer? **(2)** can NVIDIA and its partner deliver the same package **profitably across several customers**?

## 4. Options screen (case Q14 + our addition)

"We compared the options in Question 14 with our proposed approach to interoperability."

| Option | Strategic effect | Reduces reliance on top four? | Antitrust risk | Decision |
|---|---|---|---|---|
| E. Strengthen CUDA and developer support | Gives developers a reason to keep choosing NVIDIA | No direct effect | Lower | **Approve now (Move 1)** |
| B. Offer low-cost custom chips to large buyers | Could retain selected chip orders | No | Depends on deal terms | **Test selectively within Move 2** |
| *Our addition:* Support customer-designed chips in NVIDIA systems | Could retain networking and systems sales when buyers use their own chips | No | Depends on deal terms | **Test first (Move 2)** |
| C. Broaden the customer base | Tests whether AI Foundry can attract first-time enterprise buyers | Potentially, if the pilot scales | Lower | **Pilot first (Move 3)** |
| A. Use exclusive contracts | Could retain purchases during the contract term | No | Higher | **Reject** |
| D. Sell design know-how to chip builders | Could generate fees while helping customers develop competing chips | Unclear | Lower | **Reject** |

## 5. Recommended strategy

**One line:** NVIDIA should **protect the value of CUDA, keep selling networking and systems when large buyers use their own chips, and test whether AI Foundry can bring in first-time enterprise buyers**. Invest in CUDA now and test the other two moves before expanding them.

| Move | Approval | What it is |
|---|---|---|
| **1. Strengthen CUDA and developer support** | **Approve now** | Keep improving NVIDIA's libraries, models and tools so developers can build and run AI more easily. Prioritize performance and ease of use for developers who already work in PyTorch. |
| **2. Keep selling systems when customers build their own chips** | **Test first** | Test whether **one large buyer** can connect its own chips to NVIDIA's networking and racks. Compare expected gross profit **with what NVIDIA would earn without the arrangement**, counting integration costs and any additional GPU sales it would displace. **Expand only if it improves expected profit.** |
| **3. Test demand from first-time enterprise buyers** | **Pilot first** | Use AI Foundry and an implementation partner to offer a standard package for one task companies still do manually, using NVIDIA software and computing infrastructure. **A mid-sized insurer could be the first test.** Expand only if customers **pay to keep using it** and the package **earns a profit for NVIDIA and its partner**. |

The strategy relies on stronger software, continued networking and systems sales, and demand from first-time enterprise buyers. Expand each pilot only if expected returns justify the cost.

**We would track:** gross profit from interoperability deals · AI Foundry's conversion to paid use · the top four buyers' share of sales.

**Removed from earlier drafts:** discounts and purchase commitments · semi-custom products in Move 2 · governments / sovereign AI · "sell the whole AI system" · the "NVIDIA gives up" line · gross margin trend and training-off-NVIDIA as watch metrics.

## 6. Justification

| Move | Comes from | Logic |
|---|---|---|
| Move 1 | **Q2** | CUDA's switching costs make customers less sensitive to price and help support NVIDIA's pricing power. |
| Move 2 | **Q3 + Q4** | The four buyers are about **40% of sales**, so even a partial shift in-house matters. The pilot tests whether NVIDIA can keep networking and systems sales when a buyer uses its own chips, and whether that beats proceeding without it after integration costs and any further loss of GPU gross profit. |
| Move 3 | **Q1 + Q5** | With **78%** of revenue from data centers and about **40%** of sales from four buyers, NVIDIA needs another source of growth. The pilot tests whether companies that put off custom AI will pay for a package NVIDIA and its partner can deliver profitably. |

- Keep the plug-in path to **racks, networking and system-level software**, while **keeping CUDA tied to NVIDIA hardware**.
- **Rejected:** exclusive contracts, because regulators already watch NVIDIA closely; selling design know-how, because it would help rivals copy NVIDIA.

## 7. Conclusion

NVIDIA can sustain its advantage if customers keep getting enough value from its software and systems to keep buying, while AI Foundry attracts profitable new demand. **Invest in CUDA now and expand the two pilots only when their results justify the cost.**

---

## 8. Slide map (as of Nov 13)

| # | Slide | WAC section | Status |
|---|---|---|---|
| 1 | Hook: −$600B, DeepSeek <$5.6M | §1 | Matches |
| 2 | Timeline | §1 (plus GIVEN facts the WAC dropped) | Matches |
| 3 | One package that is hard to leave | §1 | Matches |
| 4 | Top 4 build their own chips | §1 | Matches |
| 5 | Problem + 5 questions | §2, §3 | **Updated:** Q4 "How much profit is at risk if the top four go in-house?"; antitrust condition removed from script |
| 6 | Q1: 78% from data centers | §3 Q1 | Matches |
| 7 | Q2: revenue vs shipments | §3 Q2 | Matches |
| 8 | Q2: finished job | §3 Q2 | Matches |
| 9 | Q3: Five Forces | §3 Q3 | Matches |
| 10 | Q3: Four Corners | §3 Q3 | Handoff line updated. **Open:** title says "wherever it is cheaper"; WAC says "specific workloads where their chips meet performance needs at lower cost" |
| 11 | Q4: profit at risk | §3 Q4 | **Rebuilt:** $24.4B → $17.7B → $4.4B at risk, one slider (share moved in-house); no discount, no 13.8% |
| 12 | Q5: new demand | §3 Q5 | Matches |
| 13 | Options | §4 | **Updated:** "Their own chips in NVIDIA systems" (volume pricing removed); ARM "dropped after objections" |
| 14 | Recommendation + ERRC | §5 | **Updated:** Move 2 = with vs without profit test; ERRC Reduce = "Reliance on four big buyers" (OUR PROPOSAL) |
| 15 | Justification trace | §6 | **Updated:** Move 2 = "Scale only if it earns more profit than going without it"; Q3+Q4 finding links to slide 11's $4.4B |
| 16 | Risks + watch metrics | §5, §7 | **Updated:** three WAC watch metrics; closing line = WAC conclusion |
| 17 | Close: Microsoft question + NVLink Fusion | Review §3, §7 | Matches (INTERNET, after the case) |
| B1 | 15 polling answers | Review | Unchanged |
| B2 | Frameworks in reserve | Review | Unchanged |

Speaker notes: `[ … ]` cues, **Key line** and **Note for Q&A** render in red italics in the deck's script panel (press N). `NVIDIA_Talking_Points.md` mirrors the deck notes for every updated slide.

## 9. Allen's deck review: build rules we follow

| Rule | In our deck |
|---|---|
| Logic chain: problem → questions → one finding each → moves → trace | ✅ 5 questions, per WAC |
| **Five Forces + Four Corners** on main slides; PESTLE, SWOT/TOWS, seven tests, CEO actions, motive/means in backup | ✅ slides 9–10, B2 |
| **PMS map** on Q1 | ✅ slide 6 |
| **ERRC grid** for the recommendation | ✅ slide 14 ("We give up" line dropped, since the WAC removed it) |
| **No weighted option scorer**; screen options against findings | ✅ slide 13 |
| Plug-in idea merged into Move 2 | ✅ |
| Risks with early warning signals, compressed | ✅ slide 16 |
| Close: Microsoft question, then **NVLink Fusion** labelled INTERNET / after the case | ✅ slide 17 |
| Poll answers tagged on the slide where the evidence sits + B1 backup | ✅ |
| **Plain, literal titles, no metaphors** | ⚠️ slide 2 is still "NVIDIA's Journey to $3 Trillion" |
| H100 vs A100: lower raw compute per dollar but 2.25× per training job | ✅ slide 8, now also in the WAC |
| DeepSeek = hook, ranked below the hyperscalers | ✅ slide 1 |

### Where the review and the WAC disagree (WAC wins)

| Item | Review says | WAC says | We use |
|---|---|---|---|
| Q4 | Break-even ~17.5%, "1 in 6 dollars" | No discount. Profit at risk: **$4.4B** if 25% moves in-house | **Profit at risk** |
| Number of questions | Four | **Five** (adds Q5 new demand) | **Five** |
| Slide 7 title | "Growth came mostly from higher prices, not more chips" | The gap can reflect prices, mix and networking | **Caveated title** |
| Slide 10 | Move **inference** in-house, keep NVIDIA for frontier training | Shift **specific workloads** where their chips meet performance needs at lower cost | **WAC** |
| What NVIDIA gives up | Top margins on inference | Not in the WAC | **Dropped** |
| Move 3 | Grow customers who cannot build their own chips | AI Foundry pilot with a partner, insurer as possible first test, two scale gates | **WAC** |

### Open questions for the team

1. **Option B vs Move 2.** The options table keeps B as "Test selectively within Move 2", but the Move 2 text no longer mentions custom chips. Should Move 2 name it again, or should B's decision change?
2. **Slide 10 title** still says "wherever it is cheaper" (see slide map).
3. **Slide 15 Move 3 finding** uses "Enterprises were not historically a GPU market (case p. 16)"; the WAC's reason is 78% from data centers + 40% from four buyers. Both are compatible.
4. **Team slide (18):** the WAC now lists Learning Teams 1, 2 and 9.
