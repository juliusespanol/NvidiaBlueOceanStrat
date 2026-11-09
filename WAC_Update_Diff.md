# WAC Update: New vs Our Current Source of Truth

**Compared:** `WAC - NVIDIA v3(1).docx` (new, Nov 10, 2026) vs `WAC_v3_Source_of_Truth.md` (ours, built from the old `WAC - NVIDIA v3.docx`).
**Status:** For review only. Nothing in the deck or the source-of-truth MD has been changed yet.

**Legend:** 🔴 changes a slide that is already done · 🟠 changes the plan for a slide not yet done · ⚪ wording only / no deck impact · ✅ same

---

## 1. Section by section

### Case facts

| Item | Ours (old WAC) | New WAC | Impact |
|---|---|---|---|
| 1999 first GPU, 2007 CUDA, ChatGPT Nov 2022 | In | **Removed** | 🔴 Slide 2 timeline. Still case facts (GIVEN), just no longer in the paper |
| Revenue +126% to $60.9B, data center 78% | In | In (new opening paragraph) | ✅ |
| Data center +217% to **$47.5B** | In | +217% kept (in Q2), **$47.5B removed** | ⚪ Slide 2 sub-label |
| Gross margin 72.7% | In | In, now explained: "strong demand and the value of CUDA, which makes switching chips costly for developers" | ✅ |
| **AMD 47%, Intel 41%** gross margin | In | **Removed** | 🔴 Slide 7 margin columns + "NVIDIA tax" (still GIVEN in the case) |
| Waited **up to 18 months** for chips | In | **Removed** | 🟠 Slide 8 bottom line (still GIVEN in the case) |
| CUDA 300+ libraries, 5M+ devs, runs only on NVIDIA | In | In | ✅ |
| Top 4 = MSFT 15 / Meta 13 / AMZN 6 / Alphabet 6 ≈ 40%, outside estimates | In | In (said twice) | ✅ |
| UXL, PyTorch, ARM blocked, export rules, DeepSeek <$5.6M / −$600B | In | In | ✅ |

### Problem statement 🔴

| Ours (old WAC) | New WAC |
|---|---|
| "How can NVIDIA **keep its pricing power and keep growing without pushing them out faster or drawing antitrust action**?" | "How can NVIDIA **protect its pricing power as its largest buyers build their own chips, and where can it create new demand**?" |

First two sentences (premium prices, locked into CUDA, reason and means to leave) are unchanged.
**Impact:** Slide 5 title ("…keep its pricing power and keep growing?") and the click-3 amber box "**Without** pushing them out faster or drawing antitrust action". The antitrust condition is gone from the problem.

### Q1. How much rides on AI data centers? ✅

No change. 39.4 → 55.6 → 78.0%, margin 15.7 → 54.1%, opex +2%, 85¢, pioneer → migrator, AI Foundry no revenue yet. Slide 6 is fine.

### Q2. Why can NVIDIA charge so much?

| Item | Ours (old WAC) | New WAC | Impact |
|---|---|---|---|
| Shipments vs revenue | +42% (2.64M → 3.76M) vs data center revenue **+217%** | Same | 🔴 Slide 7 shows **revenue per GPU +122%** (Kim's computed ratio). The paper compares **+42% vs +217%** directly |
| Caveat | "The gap is **not a pure price measure**… networking and a richer product mix. It still fits a picture of buyers paying a premium." | "The gap **can reflect chip prices, product mix, and networking sales**." | 🔴 Slide 7 note ("Not a pure price…") |
| Link to H100 | "The case shows why they would." | "The H100 comparison gives **a more direct reason** buyers **might** pay a premium." | ⚪ Slide 7 → 8 transition |
| H100 4× price, 9× faster, 2.25× per dollar, "finished job" | In | Same | ✅ |
| MR = MC, higher markup | In | Same | ✅ (slide 8 still adds this line) |

### Q3. Who can break the lock-in? (much shorter now)

| Item | Ours (old WAC) | New WAC | Impact |
|---|---|---|---|
| Five Forces | Buyer power + substitutes both **high**, from the same four firms | "Points to an **unusual threat**. NVIDIA's biggest buyers are also building substitutes." | ⚪ Same idea, simpler |
| Rivalry weaker: AMD **$4.5B** vs NVIDIA **$76B** | In | **Removed** | 🟠 Slide 9: the planned rivalry edit has no WAC basis now |
| Four Corners drivers | "Cutting the **'NVIDIA tax'** and securing supply" | "**Lower costs and more control over supply**" | 🔴 The phrase "NVIDIA tax" is gone from the paper (slide 7 click 3; slide 10 wording) |
| Cloud share 65% (32+23+10) | In | **Removed** | 🟠 Slide 10 if it shows 65% |
| Prediction | Move work in-house **wherever** own chips do it cheaper | Shift **specific workloads** in-house **where their chips meet performance needs** at lower cost | 🟠 Slide 10 title / "likely next move" |
| Inferentia + Trainium | In | Same | ✅ |
| **DeepSeek is a smaller worry** | In | **Removed** | 🟠 Slide 10: drop the planned DeepSeek line |

### Q4. What is it worth to keep them?

| Item | Ours (old WAC) | New WAC | Impact |
|---|---|---|---|
| $24.4B, $17.7B, 10% discount = $2.4B, lose a quarter = $4.4B | In | Same | ✅ |
| Break-even wording | "Pays for itself if it keeps **more than 13.8%** of their business (10% ÷ 72.7%)" | "A 10% discount **that retains all eligible volume** breaks even if holding the price would cost NVIDIA **13.8% of that volume**" | ⚪ Same math, clearer wording for slide 11 caption |
| Assumption | "These numbers are illustrative." | "Uses NVIDIA's **company-wide 72.7% as a proxy** and assumes unchanged unit costs." | 🟠 Slide 11 hint text |
| Commitment | Tie to **volume** commitments | Tie to a **purchase** commitment | 🟠 Slides 11, 15 wording |
| "**Never** tie it to a promise not to build their own chips (exclusive deal)" | In | **Removed** | 🟠 Slide 11: drop the planned line |
| "About 1 in 7 dollars" | In our MD only (our math) | Not in either paper | ⚪ OK to keep as plain-language help |

### Q5. Where can NVIDIA create new demand? 🟠 (biggest content change)

| Item | Ours (old WAC) | New WAC |
|---|---|---|
| Who | Companies that **put off custom AI** because they **lack staff or infrastructure** ("noncustomers") | Companies that **evaluated custom AI and decided it costs too much to implement** |
| What | Insurer **claims assistant** that finds answers in **policy documents** | A **standard package for one task these companies still do manually** (task not named) |
| Who delivers | Hosted by a **cloud partner**, built on **NIM + NeMo** | "Through a **partner**" / "**implementation partner**". NIM + NeMo **removed** |
| Insurer | Named as **the** pilot | "A mid-sized insurer **could be** the first test" (only in Move 3) |
| Pilot purpose | "Small on purpose", tests whether easier start → paying customers | Answers **two questions**: (1) do the savings justify the price for a first-time buyer? (2) can NVIDIA + partner deliver it **profitably across several customers**? |

**Impact:** New slide 12 should be built around the two pilot questions, not the claims-assistant detail. Slide 14 Move 3 cell and slide 16 pilot risk row follow from this.

### Options screen 🟠 (new columns and new values)

**Columns changed:** "Keeps lock-in?" is **gone**. New column **"Strategic effect"**. Decisions now use **Approve now / Test / Pilot first / Reject** instead of "Adopt".

| Option | Strategic effect (new) | Less reliance on top 4? old → new | Antitrust risk old → new | Decision old → new |
|---|---|---|---|---|
| E. Strengthen CUDA and developer support | Gives developers a reason to keep choosing NVIDIA | Indirectly → **No direct effect** | Medium → **Lower** | Adopt (Move 1) → **Approve now (Move 1)** |
| B. **Offer** low-cost custom chips to large buyers | Could retain selected chip orders | No → No | Low → **Depends on deal terms** | Adopt within Move 2 → **Test selectively within Move 2** |
| Our addition. ~~Profitable interoperability~~ → **Support customer-designed chips in NVIDIA systems and offer targeted volume pricing** | Could retain **networking and systems sales** when buyers use their own chips | No → No | Low → **Depends on deal terms** | Adopt (Move 2) → **Test first (Move 2)** |
| C. Broaden the customer base ~~(enterprise and sovereign AI)~~ | Tests whether AI Foundry can attract first-time enterprise buyers | Yes → **Potentially, if the pilot scales** | Low → **Lower** | Adopt (Move 3) → **Pilot first (Move 3)** |
| A. Use exclusive contracts | Could retain purchases during the contract term | No → No | High → **Higher** | Reject |
| D. Sell design know-how to chip builders | Could generate fees **while helping customers develop competing chips** | No → **Unclear** | Low → **Lower** | Reject |

**Impact:** The slide 13 plan in HANDOFF (columns "Protects lock-in? · Margin cost", "enterprise and sovereign AI") no longer matches. Rebuild the table from the new one.

### Recommended strategy

| Item | Ours (old WAC) | New WAC | Impact |
|---|---|---|---|
| One line | "Make staying with NVIDIA **the cheapest and fastest option** instead of making leaving impossible." + "**sell the whole AI system**" | "**Protect the value of CUDA, keep selling networking and systems when large buyers use their own chips, and test whether AI Foundry can bring in first-time enterprise buyers.** Invest in CUDA now and test the other two before expanding." | 🟠 Slide 14 one-liner. "Sell the whole AI system" is **gone** |
| Move 1 name | Strengthen CUDA and developer support · Approve now | Same | ✅ |
| Move 1 PyTorch | "NVIDIA hardware stays the **fastest choice** when developers work in PyTorch" | "**Prioritize performance and ease of use** for developers who already work in PyTorch" | ⚪ |
| Move 2 name | **Support profitable interoperability** · Test first | **Keep selling systems when customers build their own chips** · Test first | 🟠 Slides 14, 15 |
| Move 2 content | Big buyers' chips plug into **high-bandwidth** racks + networking; semi-custom; discounts **where break-even supports it**; "from selling chips into **AI infrastructure**" | Test whether **one large buyer** can connect its chips to NVIDIA networking and racks; semi-custom **where there is a clear need**; discount tied to a **purchase commitment**, **compare expected gross profit with holding the price** | 🟠 Slide 14 |
| Move 3 name | **Expand enterprise and sovereign AI** · Pilot first | **Test demand from first-time enterprise buyers** · Pilot first | 🟠 Slides 14, 15 |
| Move 3: governments / sovereign AI | "Second group to target (OUR PROPOSAL)" | **Removed** | 🟠 Slide 14: drop governments |
| Move 3 scale gate | First-time buyers move to paid use + revenue covers onboarding and support | Companies that put off custom AI **pay to keep using it** AND NVIDIA + partner deliver it **profitably across customers** | 🟠 Slides 14, 16 |
| Pricing rule | (none) | **New:** "Relies on better products and selective discounts. Accept a lower margin on a deal **only if the purchase commitment yields more gross profit than holding the price**." | 🟠 Slide 14 or 15 |
| "**NVIDIA gives up:** exclusive deals · large acquisitions · top margins on sales to the four biggest" | In | **Removed** | 🟠 Slide 14 "We give up" line (Allen's review asks for it; see decisions) |
| Watch: top-4 share · gross margin trend · big buyer moving **training** off NVIDIA | In | Same | ✅ Slide 16 |

### Justification

| Move | Ours (old WAC) | New WAC | Impact |
|---|---|---|---|
| Move 1 ← Q2 | Switching costs → less price-sensitive → **protects the 73% margin** | CUDA's switching costs → less price-sensitive → **help support pricing power** | ⚪ |
| Move 2 ← Q3 + Q4 | 40% of sales; losing volume costs more than a discount **once >13.8% would go**; "**A substitute becomes a complement**" | 40% of sales, **so even a partial shift matters**. A buyer's chip can replace an NVIDIA GPU **while still using NVIDIA networking and racks**. **Test: does the gross profit kept justify the integration cost and any discount?** | 🟠 Slide 15. "A substitute becomes a complement" is **gone**; the 13.8% link is **gone** from this row |
| CUDA porting | "We would **not port CUDA** to rival chips" | "Keep the plug-in path focused on racks, networking, system-level software **while keeping CUDA tied to NVIDIA hardware**" | ⚪ Same idea, new wording |
| Move 3 ← Q1 + Q5 | Needs growth not resting on a few buyers; pilot tests one at low cost | Same idea; pilot tests whether companies **will pay** for a package NVIDIA + partner can **deliver profitably** | ⚪ |
| Rejected A and D | Regulators watch NVIDIA; design know-how helps rivals copy | Same | ✅ |

### Weak point / closing 🟠

| Ours (old WAC) | New WAC |
|---|---|
| "**The weak point is timing.** The threat doesn't show yet; competition hurts margins before sales; in-house chips take years. **Act now, while NVIDIA is strong.**" | "Strong revenue growth gives NVIDIA **room to act while the core business is still performing well**. Invest in CUDA now, expand interoperability **where the economics work**, and scale AI Foundry **when first-time buyers pay and the package can be delivered profitably**." |

**Impact:** Slide 16 weak-spot box. Same "act now" spirit, but the "margins before sales / years to mature" argument is gone.

---

## 2. What this means for the slides

### Done slides that now disagree with the new WAC

| # | Slide | What disagrees | Size |
|---|---|---|---|
| 2 | Timeline | 1999 / 2007 / ChatGPT / $47.5B no longer in the paper (still true case facts) | Probably keep. Decide |
| 5 | Problem | Title and the "Without… antitrust" box vs the new problem question | **Edit** |
| 7 | Q2 price vs volume | +122% per GPU vs paper's +42% vs +217%; caveat wording; AMD/Intel + "NVIDIA tax" no longer in the paper | **Edit**. Decide on margins |
| 1, 3, 4, 6 | | No conflict | ✅ |

### Slides not done yet: HANDOFF plan items that change

| # | Slide | HANDOFF plan item | Now |
|---|---|---|---|
| 8 | Finished job | MR = MC line; "18 months" | MR = MC still in. 18 months no longer in the paper |
| 9 | Five Forces | Rivalry "Lower" with AMD $4.5B vs $76B | **Drop** (not in the paper). Use "unusual threat: biggest buyers build substitutes" |
| 10 | Four Corners | DeepSeek "smaller worry" line; "NVIDIA tax" driver. **Slide now shows** "cut the NVIDIA tax" and "65% of cloud (Amazon 32, Microsoft 23, Google 10)" | **Drop** DeepSeek line. Decide on the 65% cloud figure (no longer in the paper). Drivers → "lower costs, more control over supply". "Specific workloads… meet performance needs" |
| 11 | Break-even | "Never tie it to a promise…" line; "volume commitment" | **Drop** the never-line. "Purchase commitment". Proxy-margin caveat |
| 12 | Q5 (new) | Claims assistant, cloud partner, NIM + NeMo | **Rebuild idea:** firms that found custom AI too costly → partner-delivered standard package for one manual task → 2 pilot questions. Insurer = "could be the first test" |
| 13 | Options | Old columns and values | **Rebuild** from the new table (Strategic effect column, new risk/decision values) |
| 14 | Recommendation | "Sell the whole AI system"; governments; "We give up" | New one-liner; new move names; **no governments**; pricing rule; decide on "We give up" |
| 15 | Trace | "Substitute becomes a complement"; 13.8% in Move 2 row | Use the new Move 2 logic (retained gross profit vs integration cost + discount). Keep "CUDA tied to NVIDIA hardware" |
| 16 | Risks | Weak-spot box "already WAC-correct" | **No longer.** Use "room to act while the core still performs" |
| 17 | Close | Microsoft question + NVLink Fusion | Not in either paper (from Allen's review). Fits the new Move 2 even better |

---

## 3. Decisions for Julius

1. **Case facts the paper dropped** (1999/2007/ChatGPT, AMD 47% / Intel 41%, 18-month wait, $47.5B). Keep them on slides as GIVEN case facts, or strip the deck down to what the paper says?
2. **Slide 7 numbers.** Keep Kim's "revenue per GPU +122%", or switch to the paper's direct comparison "shipments +42% vs data center revenue +217%"?
3. **"NVIDIA tax".** The paper no longer uses the phrase. Keep it on slide 7 as the buyers' nickname, or drop it?
4. **"We give up" line on slide 14.** Allen's review asks for it, but the new paper removed it. Keep or drop?
5. **Allen's deck review** (Five Forces + Four Corners on main slides, ERRC, Microsoft close, etc.). Does it still apply alongside the new WAC?
6. After you approve: I'll rewrite `WAC_v3_Source_of_Truth.md` from the new paper and update the HANDOFF plan for slides 8–17.
