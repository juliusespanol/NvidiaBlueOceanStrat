# NVIDIA Deck: Handoff (Nov 10, 2026, updated after slide 13)

Read this first in a new chat. It covers what is done, how we work, and exactly what to do on each remaining slide.

**Presentation:** ECO 502 NVIDIA group presentation, Nov 14, 2026, ~30 min, 3 speaker groups.
**Git:** clean at commit `cd8cc9f` ("slide 13 added images"). Everything below marked done is committed. Julius commits himself.

**▶ Next up: slide 14, the justification trace (`<!-- 14 TRACE -->`)** (see §6). Then 15, 16, the backups, and the leftovers in §7.

**Slide numbers in this file = the deck as it is now: 16 main slides + B1, B2.** The planned new Q5 slide was **not** inserted (see §8, decision 1).

---

## 1. Files

| File | What it is |
|---|---|
| `index.html` | **The deck.** One HTML file, 1920×1080 stage, slides are `<section class="slide">`. Speaker notes are in `<aside class="notes">` inside each slide. Rebuilt slides have an `id` (e.g. `slide-13-rec`) and their own scoped `<style>` block. |
| `NVIDIA_Talking_Points.md` | Speaker script. **Restyled like Julius's old docx:** one header line per slide (`## SLIDE 13 of 16 · Recommendation · Group 3 · ~2.5 min`), then **On screen**, **Clicks**, the script with *[italic cues]*, **Key line**, optional **Note for Q&A**. **Update it with every slide change**, same words as the deck notes. |
| `/Users/espanoljulius/Downloads/WAC - NVIDIA v3(1).docx` | **The new WAC (Nov 10). This is now the source of truth for content.** |
| `WAC_Update_Diff.md` | Section-by-section diff: new WAC vs our old source-of-truth MD, with the slide impact and 5 decisions. **Read it before touching slides 14–16.** |
| `WAC_v3_Source_of_Truth.md` | Built from the **old** WAC. ⚠️ Outdated where the diff says so. Not rewritten yet (§8). Its §9 (Allen's review rules) still applies. |
| `/Users/espanoljulius/Downloads/NVIDIA_Talking_Points.docx` | Julius's **old** talking points. Older than our MD; every line is already in the MD. Only use it as a format reference. |
| `Kim_Deck_Diff.md`, `/Users/espanoljulius/Downloads/NVIDIA_Case_Keynote(1).html` | Kim's deck and its diff. Copy text in only where it matches the **new** WAC. Never replace `index.html` with Kim's deck (no images). |
| `/Users/espanoljulius/Downloads/NVIDIA_Deck_Review_vs_Our_Outline.md` | Allen's deck review (structure rules). |
| `nvidia_assets/_picks/…` + `nvidia_assets/01_…08_…` | Images. `_picks/moat_system/compute_tray_cut.webp` is a transparent cut-out made for slide 7. |
| `.claude/launch.json` | Preview config `deck` → `http://127.0.0.1:8765` (attaches to an already-running server). |

## 2. Source-of-truth rules

1. **New WAC (`WAC - NVIDIA v3(1).docx`) = what we say.** If the deck or the old MD disagree with it, the new WAC wins.
2. **Allen's review = how the deck is built** (Five Forces + Four Corners on main slides, ERRC, no weighted scorer, Microsoft close + NVLink Fusion, plain titles), unless the new WAC removed the content.
3. What the new WAC **dropped** (see `WAC_Update_Diff.md`): antitrust in the problem statement, AMD 47% / Intel 41% in the facts, "NVIDIA tax", AMD $4.5B vs $76B, 65% cloud share, "DeepSeek is a smaller worry", "never tie it to a promise not to build chips", governments / sovereign AI, "sell the whole AI system", "We give up", "a substitute becomes a complement", the timing weak point. Don't add these to new slides; existing ones are listed in §8.
4. What the new WAC **changed:** "purchase commitment" (not "volume commitment"); 72.7% is a **company-wide proxy**, unit costs unchanged; Move 2 = "**Keep selling systems when customers build their own chips**"; Move 3 = "**Test demand from first-time enterprise buyers**"; Q5 pilot = a partner-delivered **standard package for one manual task**, insurer "could be the first test", two pilot questions (do savings justify the price? can it be delivered profitably across customers?).

## 3. How we work (Julius's preferences)

- **One slide at a time.** Change it → check it → show Julius → he says "Go, next slide" → next.
- **Titles: one plain, natural sentence.** No AI-sounding comma lists. Numbers go in the visual, not the title. Julius approves each new title.
- **Less text, more NVIDIA images, more clicks.** Each extra fact gets its own click or goes to the notes (as a "Q&A note" if it is a detail). Julius dislikes things that "look AI": little tag codes (M1/M2), "We give up" bars, dense tables.
- **Don't repeat images across slides** (see §4 image list).
- **Always update the deck notes AND `NVIDIA_Talking_Points.md`** for the same slide. The deck notes for every slide are now the full script with cues (slides 8–16 were synced from the MD on Nov 10).
- **Check every change on the local server**, `http://127.0.0.1:8765/index.html#sN`. Never the `file://` preview (images don't load).
- **Checking routine:** resize the pane to 1920×1080, reload, step with `dispatchEvent(new KeyboardEvent('keydown',{key:'ArrowRight'}))`, check `scrollHeight == clientHeight`, measure element bottoms (content must end ≤ ~930px), screenshot. ⚠️ If `document.visibilityState` is `hidden`, screenshots are stale: verify with computed styles/positions instead and say so.
- **CSS gotchas found this round:** global classes clash with slide classes. `.row` (flex), `.b` (build-in animation), `.a` (amber text), `.errc` (old 2×2 grid) are global. Scope new classes under the slide id and avoid those names. A step-only slide needs hidden `<i data-frag="1" hidden></i>` markers so the deck counts its clicks. Elements with an entry `animation … forwards` ignore later opacity/transform changes: wrap them and animate the wrapper.
- Inline SVG: use `style="fill:var(--x)"`, not `fill="var(--x)"`.
- Julius commits himself. Don't commit unless asked.
- Julius and Kim write in Taglish. Reply in kind is fine.

## 4. Global changes already made

- Small top headers (`.eyebrow`) removed from all slides. Footers show the page number only.
- **No monospace font anywhere** (`--mono` points to IBM Plex Sans). Don't bring one back.
- **On-screen buttons:** only ← → remain. Notes / titles / full-screen buttons are `hidden`; the keys still work. **Shortcuts:** ← → move · **N** notes · **I** titles · **F** full screen · **B** backups.
- **Backups behind B:** slide 16 is the last slide unless **B** is pressed. B unlocks B1–B2 after 16; B again locks them and jumps back to 16. Opening `#s17`/`#s18` by URL or from the titles list unlocks them. Code: `let backups`, `lastIdx()`, `updBar()` in the main script.
- **Progress bar:** counts 16 slides when backups are off (slide 16 = 100%), 18 when on.
- **Break-even calculator JS fixed:** `costA = mv/100*SALES`, `lossB = lv/100*GP`, `be = mv/GM*100`, plus `≈ 1 in N dollars`.
- **Images already used** (avoid reusing): `ai_factory/data_center_row`, `ai_factory/ai_factory_hall` (slides 12 faint + 13), `company/deepseek_logo`, `geforce_chip_1999`, `jensen_opentowork_meme`, `nvidia_logo_stacked` (1, 9), `moat_software/cuda_libraries` (3, 12), `cuda_logo`, `moat_system/blackwell_chip` (5, 10), `compute_tray` (12), `compute_tray_cut` (7), `gb200_rack` (12), `04_cuda_software/nvidia-cuda-x-og` (13), `05_networking/infiniband-switches-2c50-d-2x` (13). Save `_picks/threat_response/nvlink_fusion_*` for slide 16.

## 5. Done: slides 1–13

| # | Title (on screen) | Status / what it is now |
|---|---|---|
| 1 | Hook: −$600B | Done (DeepSeek "claimed… <$5.6M"). |
| 2 | "NVIDIA's Journey to $3 Trillion" | Done. Shows 1999 / 2007 / ChatGPT / $47.5B, which the new WAC dropped (§8). |
| 3 | "NVIDIA sells one package that is hard to leave" | Done. |
| 4 | "NVIDIA's biggest customers are now building their own chips" | Done (donut). |
| 5 | "How can NVIDIA keep its pricing power and keep growing?" | Done, but **conflicts with the new WAC problem** + has the "Without… antitrust" box (§8). |
| 6 | "78% of NVIDIA's revenue now comes from one business…" | Done. Long title still awaiting Julius. Notes say AI Foundry pilot "on slide 12", which is now Options (§8). |
| 7 | "Data center revenue grew faster than estimated GPU shipments" | **Rebuilt.** Count-up +42% vs +122% bars, floating compute tray (`compute_tray_cut.webp`) with shine. Click 1: "Not a pure price…" note + GPU / Networking pins. Click 2: tray recedes, gross-margin columns 73/47/41. Click 3: amber "+26 pts" NVIDIA-tax band. |
| 8 | "Buyers pay for the finished AI job, not for raw chip speed" | **Not touched yet.** Only the notes were synced to the full script. Planned: add "Switching is costly, so demand is less sensitive to price; the profit-maximizing price (MR = MC) carries a higher markup"; notes "in the case example, it trains about nine times as fast". "18 months" is no longer in the WAC (§8). |
| 9 | "NVIDIA's biggest buyers are also its biggest substitutes" | **Rebuilt.** NVIDIA-logo hub (rivalry) with spinning ring, five short force cards with 3-bar meters. Click 1: entrants/suppliers dim, buyers + substitutes amber with flowing lines. Click 2: Microsoft/Meta/Amazon/Google + MAIA/MTIA/Trainium/TPU pills, "Same four firms" arc. Cut details are a Q&A note. |
| 10 | "The big buyers will move work to their own chips wherever it is cheaper" | **Rebuilt** (title approved implicitly, not explicitly). Big 2×2 Four Corners around a "Top 4 buyers" badge. Click 1: corners fold into the badge, the label hides, and a large flow takes their place: Each AI workload → "Can their own chip do it well enough, for less?" → Yes: move in-house / No: keep it on NVIDIA, with moving workload dots. Click 2: Amazon Inferentia + Trainium strip. Still shows 65% cloud; script still says "NVIDIA tax" (§8). |
| 11 | "A 10% discount pays for itself if it keeps 1 in 7 dollars from leaving" | **Rebuilt** to the new WAC. Sliders (discount 1–30, default 10; volume lost 5–50, default 25), 13.8% break-even with "≈ 1 in 7 dollars" and 7 tiles. Click 1: A $2.4B vs B $4.4B bars + verdict. Click 2: "Tie any discount to a purchase commitment." Notes use Kim's $100 example. |
| 12 | "We tested the case's five options, plus one of our own" | **Rebuilt** as cards with faint NVIDIA images: E / B + "our addition" / C in Move 1-2-3 columns, A and D in a bottom strip. Values from the new WAC table. Click 1: A and D struck out with reasons. Click 2: "Move 1 · Approve now / Move 2 · Test first / Move 3 · Pilot first" headers, kept cards turn green. |
| 13 | "Invest in CUDA now, and test the other two moves before scaling them" | **Rebuilt.** Three move cards with photos: 1 Approve now (CUDA-X image), 2 Test first (InfiniBand switches), 3 Pilot first (AI factory hall). One card per click, then a one-line ERRC strip (Eliminate exclusive deals · Reduce discounts without a commitment · Raise CUDA ease of use · Create a plug-in path · an AI Foundry package). No M-tags, no "We give up". |

Titles of 7, 9–13 were written by Claude; Julius said "Go" on each slide but did not comment on the titles individually.

## 6. To do: slides 14–16 + backups (deck numbering)

### Slide 14: Justification trace (`<!-- 14 TRACE -->`), REBUILD  ← **START HERE**
Currently a 5-row table with outdated content ("move inference in-house", "~17.5%", "Q1 + Q3", Lerner/Porter jargon). Text-heavy, will look "AI" to Julius. Rebuild to the **new WAC justification**:
- **Move 1 ← Q2:** CUDA's switching costs make customers less sensitive to price and support NVIDIA's pricing power.
- **Move 2 ← Q3 + Q4:** the four buyers are ~40% of sales, so even a partial shift in-house matters. A buyer's chip can replace an NVIDIA GPU while still using NVIDIA networking and racks. The test: does the gross profit NVIDIA keeps justify the integration cost and any discount? Keep the plug-in path at racks, networking and system software, **keeping CUDA tied to NVIDIA hardware**.
- **Move 3 ← Q1 + Q5:** 78% of revenue from data centers and ~40% from four buyers, so NVIDIA needs another source of growth. The pilot tests whether companies that put off custom AI will pay for a package NVIDIA and a partner can deliver profitably.
- **Rejected:** exclusive contracts (regulators already watch NVIDIA closely); selling design know-how (helps rivals copy it).
- Idea in the same style as 12–13: three finding → move links revealed one per click (finding card on the left, arrow draws, move card on the right), rejected pair last. Short phrases on screen, full logic in the notes.
- Drop: 17.5%, "inference", "a substitute becomes a complement", the antitrust/export "how, not what" row (fold "no exclusive deals" into the rejected line).
- Open: Allen's review wants one line "**Passes the Session 1 seven tests** (details in backup)". Ask Julius.
- New title idea: "**Every move comes from one finding in our analysis**" (ask).

### Slide 15: Risks (`<!-- 15 RISKS -->`), REBUILD
Currently a 5-row table + "Our weak spot" box (old timing argument, INTERNET 75% margin).
- Row 1 signal → "More top-4 workloads move to their own chips; outside AI labs sign up for TPU or Trainium" (not "inference").
- Replace the TSMC row with: "**The AI Foundry pilot does not convert, or costs too much to deliver**" · few first-time buyers move to paid use · stop, or switch to another first-time segment. Keep TSMC in the notes.
- Add the WAC **watch metrics**: top-4 share of sales · gross-margin trend · any big buyer moving its **training** off NVIDIA.
- Weak spot → the new WAC close: "Strong revenue growth gives NVIDIA room to act while the core business is still performing well." Whether to keep the post-case 75% margin (INTERNET) is a decision (§8).
- Fewer words: one risk per click or a compact card layout.

### Slide 16: Close (`<!-- 16 CLOSE -->`), SMALL
- Keep Allen's question and NVLink Fusion (May 18, 2025, INTERNET · AFTER THE CASE).
- Change "It shows NVIDIA chose a move close to our Move 2." → "**It shows NVIDIA pursuing a similar approach.** It does not yet prove the move works." (slide + notes + MD).
- Move 2's new name ("keep selling systems when customers build their own chips") fits; consider echoing it.
- Image: `_picks/threat_response/nvlink_fusion_rack_infra.jpg` or `nvlink_fusion_board.png` (not used anywhere yet).
- Closing line in the script ("Make staying the best option…") is from the old WAC one-liner; consider the new one.

### B1: polling answers, SMALL
- Q14 → "E, C, B · B = the case's custom-chip option". Q15 → "D, E, F, [__]" (letter from Kim). Footnote: "Q14: the plug-in path and targeted pricing are our proposals, not one of the case's options."
- Check the "Slide" column against the current numbering (no Q5 slide).

### B2: frameworks in reserve, SMALL
- Check slide references against the current numbering.

## 7. Leftovers on done slides (do after 16, or when Julius asks)

- **Slide 8** planned edits (§5 row 8).
- **Slide 5** to the new problem statement: "How can NVIDIA protect its pricing power as its largest buyers build their own chips, and where can it create new demand?" The old docx title "Can NVIDIA keep its pricing power when its biggest customers are building their own chips?" is a good base. Remove or move the "Without… antitrust" box to the notes.
- **Slide 6 notes:** "We will test it with a pilot … on slide 12" no longer true.
- `NVIDIA_Talking_Points.md` "Who speaks when" table and group split (Group 3 = 11–16 is heavy; consider moving 11 to Group 2).
- Rewrite `WAC_v3_Source_of_Truth.md` from the new WAC once the §8 decisions are made.
- Final pass: every slide, every click, no overflow, all images load, B toggle, progress bar.

## 8. Open decisions / waiting on

1. **Q5 slide.** The new WAC still has Q5 (new demand). Insert a Q5 slide after 11 (deck becomes 17, `const MAIN=16` → 17, renumber notes/MD/B1/B2), or leave Q5 inside slide 13's Move 3? Not decided.
2. **Case facts the new WAC dropped but slides still show:** slide 2 (1999/2007/ChatGPT/$47.5B), slide 7 (AMD 47% / Intel 41%), slide 8 (18 months). Keep as GIVEN case facts or remove?
3. **Slide 7 numbers:** keep Kim's "+122% revenue per GPU" or switch to the WAC's "+42% shipments vs +217% revenue"?
4. **"NVIDIA tax"** on slide 7 (click 3) and in the slide 10 script, and the **65% cloud** figure on slide 10: keep or drop?
5. **Seven tests** line on slide 14 (Allen's review)?
6. **Post-case 75% margin** (INTERNET) in the slide 15 weak spot?
7. Q15 missing letter (Kim).
8. Titles of 6, 7, 9–13 still need Julius's explicit OK.
