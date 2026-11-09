# NVIDIA Deck: Handoff (Nov 9, 2026, updated after slide 6)

Read this first in a new chat. It covers what is done, how we work, and exactly what to do on each remaining slide.

**Presentation:** ECO 502 NVIDIA group presentation, Nov 14, 2026, ~30 min, 3 speaker groups.
**Git:** clean at commit `584e2cd` ("slide 6 updates"). Slides 1–6 and the font change are committed.

**▶ Next up: slide 7** (see §6). Slides 1–6 are done.

---

## 1. Files

| File | What it is |
|---|---|
| `index.html` | **The deck.** One HTML file, 1920×1080 stage, slides are `<section class="slide">`. Speaker notes are in `<aside class="notes">` inside each slide. |
| `NVIDIA_Talking_Points.md` | Speaker script per slide ("Slide N of 16" headings, "On screen", "Clicks", script, key line). **Update it with every slide change.** |
| `WAC_v3_Source_of_Truth.md` | Allen's WAC v3 written out section by section, plus the slide plan (§8) and Allen's review rules (§9). |
| `Kim_Deck_Diff.md` | Kim's deck vs ours vs WAC v3, slide by slide, with a 45-point scorecard. |
| `/Users/espanoljulius/Downloads/NVIDIA_Case_Keynote(1).html` | **Kim's deck.** Has good WAC fixes for slides 5–17. ⚠️ It has **no images** and old versions of slides 1–4. **Never replace `index.html` with it.** Copy text in slide by slide. |
| `/Users/espanoljulius/Downloads/WAC - NVIDIA v3.docx` | Allen's paper (source of truth for content). |
| `/Users/espanoljulius/Downloads/NVIDIA_Deck_Review_vs_Our_Outline.md` | Allen's deck review (source of truth for structure). |
| `nvidia_assets/_picks/…` | Curated images. Full library in `nvidia_assets/01_…08_…`, list in `nvidia_assets/README.md`. |
| `.claude/launch.json` | Preview config `deck` → `http://127.0.0.1:8765` (attaches to an already-running server). |

## 2. Source-of-truth rules

1. **Allen's WAC v3 = what we say** (facts, numbers, problem, 5 questions, options, moves, justification).
2. **Allen's review = how the deck is built** (logic chain, Five Forces + Four Corners on main slides, other frameworks in backup, PMS map, ERRC grid, no weighted scorer, Microsoft close + NVLink Fusion, plain titles).
3. **If WAC and the review disagree, WAC wins** (break-even is 13.8% not 17.5%; **5 questions** not 4).
4. **Kim's deck:** copy in what matches WAC. Not adopted from Kim: the separate "What Jensen approves first" slide (its content goes on slides 14 and 16 instead) and Kim's new close question (keep Allen's Microsoft question).

## 3. How we work (Julius's preferences)

- **One slide at a time.** Change it → check it → show Julius → he says "Go, slide N" → next.
- **Titles: one plain, natural sentence.** No AI-sounding comma lists like "Four customers, 40% of sales, all building their own chips". Put numbers in the visual, not the title.
- **Less text, more NVIDIA images.** Text that gets cut goes into the speaker notes.
- **Always update the speaker notes in `index.html` AND `NVIDIA_Talking_Points.md`** for the same slide.
- **Check every change on the local server**, `http://127.0.0.1:8765/index.html#sN` (preview config `deck`). **Do not use the `file://` preview**: images don't load there, which once caused a false "logos are gone" alarm.
- Checking routine: reload, press → to reveal all clicks, check `scrollHeight > clientHeight` for overflow, take a screenshot.
- Inline SVG gotcha: `fill="var(--x)"` attributes don't work. Use `style="fill:var(--x)"`. A global rule also turns SVG text grey unless overridden.
- Julius commits himself. Don't commit unless asked.
- **Style direction from this round:** fewer words on screen, more things revealed by clicks/transitions (each extra fact gets its own click or goes to the notes). Mockups from Julius/Kim are guides, not pixel specs. Keep the deck's dim chip-grid background on every slide.
- Julius and Kim often write in Taglish. Reply in kind is fine.

## 4. Global changes already made

- **The small top headers** (`<div class="eyebrow">`, e.g. "Analysis · Q1") are **removed from all slides**. The `.eyebrow` CSS is left in but unused.
- **Footers show the page number only** ("07 / 16", bottom right). "NVIDIA case · ECO 502" and the green "Case poll Q…" tags are gone (all poll answers still on B1). Built in JS: `ft.innerHTML='<span class="pg"></span>'`.
- **No monospace font anywhere.** Kim said JetBrains Mono (the small uppercase labels, tags, Q-numbers, page numbers, chart labels) looked "too AI". `--mono` now points to **IBM Plex Sans** (the body font), so every `var(--mono)` use changed at once; JetBrains Mono is removed from the Google Fonts link and the two inline SVG uses. `.k` labels are weight 500, letter-spacing .08em. **Don't bring a mono font back.** (The variable is still called `--mono`; that's only a name.)
- **Framework labels** (small green text, since the headers are gone):
  - Slide 9: "Porter's Five Forces", top-left of the diagram.
  - Slide 10: "Four Corners · Microsoft, Meta, Amazon, Google", above the grid.

## 5. Done: slides 1–6

| # | Title (on screen) | What changed |
|---|---|---|
| 1 | Hook: −$600B, "On one day in January 2025, NVIDIA lost $600 billion in market value." | DeepSeek card: "**Claimed** it trained a leading model for **<$5.6M**" (was "Trained its top model for <$6M"). Number shrunk to 140px to fit. Notes: "claimed… under $5.6 million". Kept: NVIDIA logo, Jensen meme, "Big US labs: $100M+". |
| 2 | "NVIDIA's Journey to $3 Trillion" (Julius's title, **keep**) | Added "**to $60.9B**" under +126% and "**to $47.5B**" under +217% (GIVEN tags). Notes say the dollar amounts. |
| 3 | "**NVIDIA sells one package that is hard to leave**" (was "The cost of leaving") | Loop pill "**5M+ developers**". Notes: "**More than** five million developers… code written for CUDA **runs only on NVIDIA chips**." |
| 4 | "**NVIDIA's biggest customers are now building their own chips**" | Table replaced with a **donut chart** (Kim's request): one amber for Microsoft 15 / Meta 13 / Amazon 6 / **Alphabet** 6, grey for "Every other customer 60%". Centre: **≈40% · $24.4B a year**. Leader lines to labels. Chip names (MAIA, MTIA, Trainium · Inferentia, TPU) appear on click 1. Footnote: "Customer shares are outside estimates. GIVEN · $24.4B = 40% × $60.9B COMPUTED". Notes: "Alphabet, which owns Google", "about 24.4 billion dollars". Four amber shades were rejected because they failed the colour check. |

### Slide 5: problem + roadmap (done)
Built from Julius's mockup: a title shot that animates into the questions.
- **Start:** big title alone on the left (86px, 3 lines, "keep growing?" in green) + short green rule; transparent Blackwell chip (`_picks/moat_system/blackwell_chip.webp`) on the right with a `-webkit-box-reflect` floor reflection. **Background is the normal `dim` chip grid**: Julius asked to keep it (a pure-black version was rejected).
- **Click 1:** line under the rule: "Customers are **locked into CUDA**. Now the four biggest have the reason and the means to leave." (This settled the old "locked into CUDA" open item. The separate reason/means boxes are gone; details are in the notes.)
- **Click 2:** title shrinks and moves to the top left (CSS transitions on `top`/`left`/`font-size`, keyed on `#slide-5-problem[data-step]`), chip eases back, Q1–Q5 rise in one by one as a vertical list.
- **Click 3:** amber dashed box "Without · pushing them out faster or drawing antitrust action".
- Notes + talking points updated with the new clicks.

### Slide 6: Q1 (done)
Kim asked for **vertical columns** so the growth reads left to right, and Julius asked for less text via clicks.
- **Entry:** title + three columns FY22 39% → FY23 56% → FY24 78% that grow one after another (height 4.6px per point; FY24 brightest with a glow). Label "Data center share of revenue · COMPUTED".
- **Click 1:** operating margin "15.7% → 54.1%" + "About 85¢ of each extra sales dollar became profit."
- **Click 2:** Blue Ocean portfolio map (AI Foundry chip says "potential pioneer, tested by a pilot (slide 12)").
- **Click 3:** "if NVIDIA stands still": data center slides to migrator, "No proven pioneer left". (The map's move rules are now scoped to `#slide-6-q1[data-step="3"]`; the old global `section[data-step="1"] .pchip…` rules were removed.)
- Moved to notes: "opex grew only 2%", the gaming dip line, the "Press →" hint.
- **Title still the long one.** Proposed shorter title: "**NVIDIA now depends on AI data centers for almost all of its growth**". Julius hasn't approved yet. Ask.

## 6. To do: slides 7–17 + backups

**Final order is 17 slides + B1, B2.** A new Q5 slide is inserted at 12, so current slides 12–16 become 13–17.

### Slide 7: Q2 price vs volume (`<!-- 7 Q2 -->`), EDIT  ← **START HERE**
- Title → Kim/WAC: "**Data center revenue grew faster than estimated GPU shipments**" (also update `data-label`).
- "Chips shipped" → "**Estimated GPU shipments**" · "Revenue per chip" → "**Revenue per GPU shipped**".
- Replace "Buyers did not just buy more. They paid more than twice as much per chip." with "**Revenue per GPU also reflects product mix and non-GPU sales such as networking, so it is not a pure price. Slide 8 shows why buyers pay a premium.**"
- Keep margins 73/47/41% and "NVIDIA tax".
- Notes (Kim): "Between fiscal 2023 and 2024, estimated data center GPU shipments rose 42 percent, but data center revenue per GPU shipped rose 122 percent. So revenue grew much faster than shipments. Be careful with that ratio: it also reflects a shift to pricier products and non-GPU sales like networking, so it is not a pure price increase. What it does show is that buyers spent far more per chip." Then keep the margins / NVIDIA tax part.

### Slide 8: Q2 finished job, SMALL
- Add one line (WAC): "**Switching is costly, so demand is less sensitive to price. The profit-maximizing price (MR = MC) carries a higher markup.**"
- Notes: "it finishes a training job about nine times faster" → "**in the case example, it trains about nine times as fast**".

### Slide 9: Five Forces, SMALL
- Rivalry node "Rivalry · Medium, rising" → WAC says rivalry is **weaker**: e.g. "**Rivalry · Lower**: AMD expects ~**$4.5B** AI chip revenue in 2024 vs NVIDIA's ~**$76B** from data centers (~17×), and its software trails CUDA." Keep the MI300X / Gaudi 3 / Ascend mention if it fits.
- Don't compare Intel/AMD **total** data center revenue (review §4 #3).

### Slide 10: Four Corners, EDIT
- Title now "The big buyers will move their own inference work to their own chips and keep NVIDIA for the most advanced training" (WAC conflict). Kim: "Big buyers are likely to move workloads in-house where their own chips can do the job at lower cost". Write a **shorter natural** version, e.g. "**The big buyers will move work to their own chips wherever it is cheaper**".
- Likely next move → Kim: "**Move each workload in-house wherever their own chip does it cheaper. Amazon already has chips for both jobs: Inferentia for inference, Trainium for training.**"
- Add WAC line: "**DeepSeek is a smaller worry: it changes how much computing AI needs, not who supplies it, and it was trained on NVIDIA chips.**"
- Notes (Kim): "…They will not move only inference or only training. They will move whichever workload their own chip can do at lower cost. Amazon already has chips for both: Inferentia for inference and Trainium for training, which the case says trains at half the cost."

### Slide 11: Q4 break-even (`<!-- 11 Q4 BREAK-EVEN -->`), REBUILD (copy Kim's)
- Title: "A 10% discount pays for itself if holding the price would lose more than 13.8% of top-buyer volume". Make it natural/shorter, e.g. "**A 10% discount pays for itself if it keeps 1 in 7 dollars from leaving**".
- Slider `#m`: label "**Price discount to the top 4**", `min=1 max=30 step=1 value=10`. Hint "**Starting gross margin 72.7% · unit costs unchanged · $24.4B of top-4 sales**".
- Slider `#l`: `min=5 max=50 value=25`, hint "If NVIDIA holds its price".
- Break-even big number **13.8%**, caption "**Share of top-4 volume that holding the price would have to lose for the discount to pay off: discount ÷ 72.7%.** COMPUTED".
- Bars: A "**Discount, keep volume**" **$2.4B** · B "**Hold price, lose volume**" **$4.4B**.
- Verdict: "At these inputs, the targeted **discount** costs less than the business it protects."
- Bottom line: "**Tie any real discount to a volume commitment. Volume lost to a customer's own chip rarely comes back; a discount can be adjusted next year.**" Add (WAC): "**Never tie it to a promise not to build their own chips (regulators would see an exclusive deal).**"
- JS (`/* break-even calculator */`): `costA=mv/100*SALES, lossB=lv/100*GP, be=mv/GM*100`. The current code is `(GM-mv)/100*SALES`, which is wrong.
- Notes (Kim's $100 example): "Think of 100 dollars of sales to the top four. At a 72.7 percent margin, the chips cost NVIDIA 27.30 and it keeps 72.70. Option A: give a 10 percent discount. The price falls to 90, the cost stays 27.30, so NVIDIA keeps 62.70 and keeps all the volume. Option B: hold the price and lose some volume to their own chips. The two are equal when 13.8 percent of the volume leaves, because 62.70 divided by 72.70 is 86.2 percent… In dollars, a 10 percent discount on 24.4 billion costs about 2.4 billion a year; losing a quarter of the volume would cost about 4.4 billion of gross profit."

### Slide 12: Q5 new demand, NEW SLIDE (insert after slide 11)
- Content (WAC Q5): many companies have **put off custom AI projects** because they lack staff or infrastructure → Blue Ocean: turn **noncustomers** into buyers → AI Foundry. **Pilot: mid-sized insurers**, an assistant that helps **claims staff find answers in their own policy documents**, **hosted by a cloud partner**, built on **NVIDIA NIM + NeMo** so the demand stays on NVIDIA chips. **Small on purpose**: tests whether making AI easier to start turns shelved projects into paying customers.
- Natural title idea: "**Companies that shelved their AI projects are NVIDIA's next customers**".
- Image idea: `nvidia_assets/06_data_center_ai_factory/nvidia-ai-factory-enterprise.jpg` or `04_cuda_software/nvaie-og.jpg` (look at them first).
- Keep it light: 3 steps (noncustomer → pilot → paid), little text.
- Write notes + a talking-points section.

### Slide 13: Options (`<!-- 12 OPTIONS -->`), EDIT
- Current title "Five possible responses, tested against what the analysis showed". Mention "plus our addition".
- Rows (columns: Protects lock-in? · Reduces reliance on top 4? · Antitrust risk · Margin cost · Decision):
  - E · Fortify software/developer ecosystem: Yes, directly · Indirectly · Medium if CUDA stays closed · Low · **Keep · Move 1**
  - B · "**Semi-custom products for hyperscalers (case option)**" (WAC: "low-cost custom chips", lock-in **Partly**) · No · Low · Medium · **Keep · Move 2**
  - **NEW** "**Our addition · Plug-in path for buyers' own chips + targeted pricing**" + tag `NOT A POLL OPTION`: Yes, keeps them on NVIDIA systems · No · Low · Medium, top 4 only · **Keep · Move 2**
  - C · Broaden the customer base (**enterprise and sovereign AI**) · Yes · Yes · Low · Low · **Keep · Move 3**
  - A · Exclusive contracts: Reject · D · Sell design IP: Reject (unchanged)
- Notes (Kim): "…Note option B: in the case it means semi-custom products for hyperscalers. The plug-in path for customers' own chips and the targeted pricing are our own additions, not a poll option, so they get their own row. B plus our addition make Move 2."
- Check vertical fit (one more row).

### Slide 14: Recommendation ERRC (`<!-- 13 RECOMMENDATION -->`), EDIT
- Add move tags: **M1 Approve now · M2 Test first · M3 Pilot first**.
- One-liner add: "**Over time, sell the whole AI system, not just chips.**"
- Create cell M3 → Kim: "**AI Foundry pilot for first-time buyers: mid-sized insurers without a dedicated AI team. Through a cloud partner, an assistant that helps claims staff find answers in policy documents. Track paid conversions and cost to serve.**" + "**Governments building national AI** (OUR PROPOSAL, not in the case)" + "Scale only if first-time buyers move to paid use."
- Drop "neo-clouds, inference and edge" (not in WAC).
- Keep "We give up: exclusive deals · big acquisitions · top margins on sales to the four biggest buyers".
- Image option: `_picks/moat_system/gb200_rack.jpg` (saved for Move 2).
- Text-heavy slide: trim where possible.

### Slide 15: Justification trace (`<!-- 14 TRACE -->`), EDIT
- Q3 row: "…they will move **workloads** in-house where it is cheaper".
- Q4 row → "**A 10% discount breaks even if holding the price would lose 13.8% of top-4 volume**" · "2 · **Discount for the top 4, tied to volume commitments**" · "**Volume lost to an in-house chip is permanent; a discount can be adjusted yearly**".
- Move 3 row: finding → "**Q1 + Q5**", move "3 · Grow customers who cannot build their own chips, **starting with an AI Foundry pilot**".
- Add (WAC): "**A substitute becomes a complement**: their chip inside NVIDIA racks adds to NVIDIA sales" + "**We don't port CUDA to rival chips**".
- Add one line (review): "**Passes the Session 1 seven tests** (details in backup)".
- Notes (Kim): "…Because a 10 percent discount pays off once holding the price would lose more than 13.8 percent of their volume, NVIDIA offers it only to those four, and only against volume commitments…"

### Slide 16: Risks (`<!-- 15 RISKS -->`), EDIT
- Row 1 signal → "**More top-4 workloads move to their own chips; outside AI labs sign up for TPU or Trainium**".
- Replace the TSMC row with: "**The AI Foundry pilot does not convert, or costs too much to serve** · Few insurers move from pilot to paid deployment · **Stop, or switch to another first-time segment**". Keep TSMC in the notes as "a risk to monitor, as on the Five Forces slide; no second source for leading chips".
- Add WAC's **watch metrics**: top-4 share of sales · gross margin trend · any big buyer moving **training** off NVIDIA.
- Weak spot box is already WAC-correct.

### Slide 17: Close (`<!-- 16 CLOSE -->`), KEEP
- Keep Allen's question "If you were Microsoft, would you still build your own chip if it could plug into NVIDIA's systems?" + NVLink Fusion (May 18, 2025, INTERNET).
- Change only "It shows NVIDIA chose a move close to our Move 2." → "**It shows NVIDIA pursuing a similar approach.** It does not yet prove the move works." (slide + notes).
- Image option: `_picks/threat_response/nvlink_fusion_rack_infra.jpg` / `nvlink_fusion_board.png`.

### B1: polling answers, SMALL
- Q14 → "E, C, B · B = case's custom-chip option".
- Q15 → "D, E, F, **[__]**", **waiting on Kim** for the customer-diversification option letter.
- Footnote (Kim): "Q14: the plug-in path and targeted pricing are our proposals, not one of the case's options. Q15: [__] is the customer-diversification option, so the answer reflects Move 3."
- **Renumber the "Slide" column** after the Q5 insert (Q14 → 13, Q15 → 14; check the others).

### B2: frameworks in reserve, SMALL
- "Covered on slides 13–15" → **14–16**. Check the other slide references.

## 7. Wrap-up tasks after slide 17

- JS `const MAIN=16;` → **17** (page numbers "/ 17").
- `NVIDIA_Talking_Points.md`: all "Slide N of 16" → "of 17", renumber 12–16 → 13–17, add the Slide 12 (Q5) section, update the "Who speaks when" table.
- Speaker split (review §7): Group 1 = 1–5 · Group 2 = 6–10 · Group 3 = 11–17 (now heaviest). **Suggest moving slide 11 to Group 2.** Ask Julius.
- Re-run the whole deck on the local server: every slide, every click, no overflow, all images load.

## 8. Open decisions / waiting on

1. ~~Slide 5: "locked into CUDA" on screen~~ Done (line under the title on click 1).
2. Q15 missing letter (Kim).
3. Speaker split with the new slide count.
4. Shorter natural titles for slides 6, 10, 11 (Julius approves each). Slide 6 proposal is in §5.
