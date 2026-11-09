# Kim's Deck vs Our Deck: Differences

**Compared:** `NVIDIA_Case_Keynote(1).html` (Kim) vs `index.html` (ours, commit `a46b320`)
**Checked against:** `WAC_v3_Source_of_Truth.md` (WAC wins)
**Verdict key:** **ADOPT** = take Kim's version · **KEEP OURS** = ours is newer or matches WAC better · **DECIDE** = team call

> ⚠️ **Do not replace `index.html` with Kim's file.** Kim's file has **zero images**: no NVIDIA logo, Jensen meme, DeepSeek logo, data center photo, CUDA logo, 1999 chip photo or CUDA library background. It is also based on an **older version** of slides 1–4 (before our logo, meme, slide-2 title and slide-1/3 WAC fixes). Port Kim's changes **into** our file, one slide at a time.

---

## Slide-by-slide

| # (Kim) | Slide | Ours | Kim | Matches WAC? | Verdict |
|---|---|---|---|---|---|
| 1 | Hook | NVIDIA logo, Jensen meme, DeepSeek card: "Claimed it trained a leading model for **<$5.6M**" vs "Big US labs: $100M+" | No images. Header "ECO 502 · NVIDIA case · Group presentation · Nov 14, 2026". One sentence: "DeepSeek had said it trained… under $5.6 million". Shorter notes, no meme | Both OK | **KEEP OURS**. Optional: add Kim's course/date line |
| 2 | Timeline | Title "NVIDIA's Journey to $3 Trillion"; +126%, +217% | Old title "How NVIDIA got here / ChatGPT turned a gaming-chip company…"; adds **$60.9B** and **$47.5B** under the % figures | Kim adds WAC's $ figures | **KEEP OURS** title · **ADOPT** the $60.9B / $47.5B labels |
| 3 | Loop | "The cost of leaving", **5M+ developers**, switching-cost panel (3 items) | Old version: "Faster GPUs", "R&D funding", **5M developers**, "code runs **best** on NVIDIA" | Ours (WAC: "more than 5M", "runs **only** on NVIDIA") | **KEEP OURS** |
| 4 | Top 4 | Title "Their biggest customers are building their own chips"; "~$24B a year" | Title "Four customers that make up 40% of NVIDIA's sales are now building their own AI chips"; "**$24.4B** of FY2024 revenue" | Kim ($24.4B) | **ADOPT** $24.4B · DECIDE on title |
| 5 | Problem | "Can NVIDIA keep its pricing power?" + reason/means/antitrust boxes; **4 questions** | Problem rewritten close to WAC: "…protect its pricing power **and growth** without speeding up their exit or triggering antitrust action?"; still **4 questions** | Kim's wording ≈ WAC. Neither has **Q5** | **ADOPT** wording · **DECIDE** on Q5 (see below) |
| 6 | Q1 | "AI Foundry: potential pioneer, no revenue in case" | "AI Foundry: potential pioneer, **tested by a pilot (slide 13)**" + same line in notes | Kim (links Q1 to the pilot) | **ADOPT** |
| 7 | Q2 price | Title "growth came mostly from higher prices, not more chips"; "Chips shipped"; "paid more than twice as much per chip" | Title "**Data center revenue grew faster than estimated GPU shipments**"; "Estimated GPU shipments"; "Revenue per GPU shipped"; **caveat: product mix + networking, not a pure price** | Kim = WAC exactly | **ADOPT** |
| 8 | Q2 finished job | Same | Same on screen; notes say "in the case example, it trains about nine times as fast" | Kim (more careful) | **ADOPT** notes line. Neither has WAC's **MR = MC** line → add |
| 9 | Five Forces | Same | Same | Neither has WAC's "rivalry weaker, AMD $4.5B vs $76B" | Same in both → still add from WAC |
| 10 | Four Corners | Title "move their own **inference** … keep NVIDIA for the most advanced training" | Title "likely to move **workloads** in-house where their own chips can do the job at lower cost"; next move names **Inferentia + Trainium** | Kim = WAC | **ADOPT**. Neither has "DeepSeek is a smaller worry" → add from WAC |
| 11 | Q4 break-even | Margin slider 72.7% → 60%, **$3.1B**, break-even **17.5%** (math is off) | **10% discount** slider, **$2.4B vs $4.4B**, break-even **13.8%** (= discount ÷ 72.7%), "tie any discount to a volume commitment", $100 worked example in notes | Kim = WAC exactly, math correct | **ADOPT** fully |
| 12 | Options | B = "Semi-custom products, a plug-in path, targeted pricing" | B = "Semi-custom products for hyperscalers (case option)" + new row "**Our addition** · plug-in path + targeted pricing · NOT A POLL OPTION" | Kim = WAC | **ADOPT** |
| 13 | Recommendation | Move 3 Create cell: "enterprises via AI Foundry, governments, neo-clouds, inference and edge" | Move 3 Create cell: **AI Foundry pilot for mid-sized insurers**, claims assistant via a cloud partner, track paid conversions + cost to serve | Kim ≈ WAC, but **drops governments** (WAC keeps them as "our proposal") | **ADOPT** + add back governments flagged OUR PROPOSAL |
| 14 | Justification trace | Q4 row "~17.5%", "volume pricing reviewed yearly"; Move 3 "grow customers who cannot build their own chips" | Q4 row "**10% discount breaks even at 13.8%**", "**tied to volume commitments**"; Move 3 "…**starting with an AI Foundry pilot**"; Q3 row says "workloads" | Kim = WAC | **ADOPT**. Still missing from both: "a substitute becomes a complement", "we don't port CUDA" |
| **15** | **NEW: "What Jensen approves first"** | — | **Approve now** Move 1 (CUDA) · **Test** Move 2 (one buyer's chip in NVIDIA racks, discount only for volume commitment) · **Pilot** Move 3 (insurers) · a "Watch:" metric for each · **scale gate** | Kim = WAC's "approved in order" | **ADOPT** (new slide) |
| 16 | Risks | 5 rows incl. "**Supply runs short at TSMC**"; inference wording | TSMC row **replaced** by "**AI Foundry pilot does not convert or costs too much**" → stop or switch segment; TSMC moved to notes; "workloads" wording | Kim fits WAC better | **ADOPT**. Add WAC's 3 watch metrics |
| 17 | Close | Question: "If you were Microsoft, would you still build your own chip if it could plug into NVIDIA's systems?" + NVLink Fusion | Question: "**If Microsoft builds its own AI chip, what can NVIDIA still sell it?**" + 3 cards: **Networking · Racks and systems · Software** + NVLink as "an example"; "pursuing a similar approach" | Kim's version shows WAC's "substitute becomes a complement" | **DECIDE**. Leaning ADOPT: it explains Move 2 in one picture |
| B1 | Poll answers | Q14 "E, C, B"; Q15 "D, E, F" | Q14 "E, C, B · B = case's custom-chip option"; Q15 "**D, E, F, [__]** · diversification"; footnote on Q14/Q15 | Kim's Q14 note OK | **ADOPT** Q14 note · ⚠️ **Q15 has a blank `[__]` placeholder. Kim needs to fill in the letter** |
| B2 | Frameworks | "slides 13–15" | "slides 13–16" | — | **ADOPT** (renumber after final order) |

---

## Kim's deck vs WAC v3 (direct check)

✅ = matches WAC · ⚠️ = partly / worded differently · ❌ = missing or conflicts

| WAC v3 point | Kim's deck | Status |
|---|---|---|
| **Facts:** DeepSeek "under $5.6M" | On screen ✅. **Notes say "less than six million dollars"** | ⚠️ |
| 1999 first GPU, 2007 CUDA, Nov 2022 ChatGPT, +126% to $60.9B, +217% to $47.5B | All there, with $ labels | ✅ |
| 72.7% vs AMD 47% / Intel 41%; 18-month wait | Slides 7–8 | ✅ |
| 300+ libraries | Slide 3 | ✅ |
| **More than** 5M developers | "5M developers" / "about five million" | ⚠️ |
| CUDA code runs **only** on NVIDIA | "Their code runs **best** on NVIDIA chips" | ❌ |
| Top-4 shares are **outside estimates** | Not labelled | ⚠️ |
| UXL, PyTorch, ARM blocked, export rules | Five Forces, risks, ERRC, trace | ✅ |
| **Problem:** keep pricing power **and growth** without speeding exit or antitrust | Slide 5, nearly word for word | ✅ |
| **Five** questions | **Four** questions ("we need four answers") | ❌ |
| **Q1:** 39 → 56 → 78%, op. margin 15.7 → 54.1%, 85 cents | Slide 6 | ✅ |
| Q1: opex grew only 2% | Missing | ⚠️ minor |
| Q1: only proven pioneer → migrator; AI Foundry no revenue yet | Slide 6 + pilot link | ✅ |
| **Q2:** +42% shipments vs +217% revenue, **not a pure price** caveat | Slide 7, exact | ✅ |
| Q2: 4× price, 9× faster, 2.25× training per $; pay for the finished job | Slide 8 | ✅ |
| Q2: switching cost → less price-sensitive → **MR = MC higher markup** | Only "inelastic demand… markup (Lerner)" on trace slide | ⚠️ |
| **Q3:** buyer power + substitutes high, same four firms | Slide 9 | ✅ |
| Q3: **rivalry weaker**, AMD **$4.5B vs $76B**, software trails CUDA | "Rivalry · **Medium, rising**", no $4.5B vs $76B | ❌ |
| Q3: Four Corners drivers (NVIDIA tax, supply); 65% cloud | Slide 10 | ✅ |
| Q3: move work in-house where cheaper; Inferentia + Trainium | Slide 10, exact | ✅ |
| Q3: **DeepSeek is a smaller worry** (how much compute, not who supplies; trained on NVIDIA) | Missing | ❌ |
| **Q4:** $24.4B, $17.7B GP, 10% → $2.4B, quarter lost → $4.4B, **13.8%** | Slide 11, exact, math correct | ✅ |
| Q4: illustrative | Labelled ASSUMPTION | ✅ |
| Q4: tie discount to volume commitments | Slides 11, 14, 15 | ✅ |
| Q4: **never** tied to a promise not to build own chips (antitrust) | Missing | ❌ |
| **Q5:** noncustomers with shelved AI projects; Blue Ocean noncustomer logic | Only "insurers have put off building an AI tool" in notes. No Q5 question | ⚠️ |
| Q5: mid-sized insurers, claims staff + policy documents, cloud partner | Slides 13, 15 | ✅ |
| Q5: built on **NIM and NeMo** so demand stays on NVIDIA chips | Missing | ❌ |
| Q5: small on purpose | "Keep it small" (scale gate) | ✅ |
| **Options:** E adopt, B within Move 2, our addition row, C adopt, A/D reject | Slide 12 | ✅ |
| Option B wording: "low-cost custom chips", keeps lock-in = **Partly** | "Semi-custom products for hyperscalers", keeps lock-in = **Yes** | ⚠️ |
| Option C: "enterprise **and sovereign** AI" | "Broaden the customer base" | ⚠️ |
| **Recommendation one-liner:** make staying cheapest and fastest | Slide 13 | ✅ |
| "Sell the whole AI system"; chips → AI infrastructure | Missing (close slide's 3 cards come closest) | ⚠️ |
| Move 1 approve now · Move 2 test first · Move 3 pilot first | Slide 15 "What Jensen approves first" | ✅ |
| Move 2: plug-in racks/networking, semi-custom, volume discounts, check profit | Slides 13, 15 | ✅ |
| Move 3: **governments** as a second target (our proposal) | Missing, dropped | ❌ |
| Move 3: scale only if paid conversion + revenue covers onboarding | Scale gate | ✅ |
| Gives up: exclusive deals, large acquisitions, top margins on top 4 | Slide 13 | ✅ |
| **Watch:** top-4 share of sales · gross margin trend · big buyer moving **training** off NVIDIA | Different "Watch" lines per move; these 3 not named | ⚠️ |
| **Justification:** M1 ← Q2, M2 ← Q3+Q4, M3 ← Q1+**Q5** | M3 ← Q1+**Q3** (no Q5) | ⚠️ |
| **A substitute becomes a complement** | Close slide shows the idea (networking / racks / software), phrase not used | ⚠️ |
| **We would not port CUDA** to rival chips | Missing | ❌ |
| Rejections: exclusive (regulators), design know-how (helps rivals) | Slide 12 notes | ✅ |
| **Weak point:** margins before sales, chips take years, act now | Slide 16 | ✅ |

**Score (45 points):** ✅ 25 · ⚠️ 12 · ❌ 8. Kim's deck is close to WAC on the analysis numbers and the recommendation. The gaps are the Q5 structure, a few one-liners from WAC (DeepSeek smaller worry, AMD vs NVIDIA, no-build promise, NIM/NeMo, governments, don't port CUDA), and older slide 3 wording.

---

## Still missing from **both** decks (from WAC)

| WAC item | Where it goes |
|---|---|
| **Q5 "Where can NVIDIA create new demand?"** as an analysis question | Problem slide + its own slide, **or** Kim's approach (pilot only in recommendation + approve-first slide). **DECIDE** |
| MR = MC → higher markup line | Slide 8 |
| Rivalry is weaker: AMD $4.5B vs NVIDIA $76B | Slide 9 |
| DeepSeek is a smaller worry (how much compute, not who supplies it; trained on NVIDIA) | Slide 10 |
| Discount **never** tied to a promise not to build own chips | Slide 11 or 15 |
| "A substitute becomes a complement" + "we don't port CUDA" | Trace slide (or Kim's close) |
| Governments / sovereign AI flagged as OUR PROPOSAL | Recommendation |
| "Sell the whole AI system", "from chips to AI infrastructure" | Recommendation one-liner |
| Top-4 shares labelled "outside estimates" | Slide 4 |

## Decisions for the group

1. **Q5:** a separate Q5 slide (WAC structure, 5 questions), **or** Kim's way (keep 4 questions, put the insurer pilot in the recommendation and the new approve-first slide)?
2. **Close:** keep the "would you still build your own chip…?" question, or Kim's "what can NVIDIA still sell it?" with 3 cards?
3. **Q15 blank:** Kim to give the missing option letter.

## Final order if we adopt Kim's changes (17 slides, or 18 with a Q5 slide, + 2 backup)

1 Hook · 2 Timeline · 3 Loop · 4 Top 4 · 5 Problem · 6 Q1 · 7 Q2 price · 8 Q2 finished job · 9 Five Forces · 10 Four Corners · 11 Q4 break-even · *(12 Q5 insurer pilot, only if decision 1 = separate slide)* · Options · Recommendation · Trace · **Approve first (new)** · Risks · Close · B1 · B2
