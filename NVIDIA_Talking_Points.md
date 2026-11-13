# NVIDIA Case: Presenter Talking Points

> Working reference for the NVIDIA Case Keynote. Keep slide copy, speaker notes, click cues, and this script aligned when making future changes.

ECO 502 · Group presentation · Nov 14, 2026 · For the deck “NVIDIA Case Keynote” (18 numbered slides + blank opener + 2 backups)

## How to read this script

*Italic text in square brackets* is a delivery cue. Do it, don’t say it.

Plain text is what you say. **Bold** words get extra stress.

Each slide ends with a **Key line**: if you forget everything else on that slide, say this.

## Five delivery rules

- One idea per breath. Every sentence here is short on purpose. Don’t join them together.

- Pause after every big number. Silence is what makes the audience remember it.

- Talk to the room, not the screen. Glance at the slide, then turn back.

- Explain every technical word the first time. The script already does this; don’t skip those lines.

- Hand off out loud. The last line of each group is a question the next speaker answers.

> Rehearsal target: about 20 minutes including clicks, pauses and handoffs (about 1,660 spoken words). Keep the detailed arithmetic and the defense bank for Q&A.

## Who speaks when

| Group | Slides | Part of the story | Time |
| --- | --- | --- | --- |
| 1 | 1–5 | Hook, case facts, the problem | ~8.5 min |
| 2 | 6–11 | Evidence and profit at risk (Q1–Q4) | ~11 min |
| 3 | 12–17 | Q5, options, recommendation, justification, risks, close | ~10 min |
| All | 18 | Thank you / questions | ~0.2 min |

## SLIDE 1 of 18 · Hook · Group 1 · ~1.5 min

**On screen:** On one day in January 2025, NVIDIA lost $600 billion in market value. Was cheaper AI the real threat?
**Clicks:** 5 (meme, DeepSeek comparison, solo question reveal, "It still trained on NVIDIA chips" with three facts, bottom line)

*[Walk to the centre of the room. Say nothing. Let the number sit on screen for three seconds.]*

Six hundred billion dollars.

That’s how much NVIDIA’s market value fell in one day in January 2025.

*[Pause.]*

*[CLICK 1: Jensen Huang meme appears.]*

Even Jensen probably had a difficult morning.

*[Smile. Give the room a moment, then move on.]*

Let’s look at what worried investors.

*[Slow down. Let each fact land.]*

They marked NVIDIA’s shares down by six hundred billion dollars.

*[CLICK 2: The meme leaves. DeepSeek appears with “<$5.6M vs $100M+”.]*

DeepSeek reported a training run under 5.6 million dollars. The GPT-4 estimate was over a hundred million, though those figures cover different things.

Investors wondered whether cheaper AI meant fewer expensive chips.

*[CLICK 3: The question rises in on its own. Look around the room.]*

Was that NVIDIA’s biggest threat?

*[Pause two seconds. Let the question sit.]*

*[CLICK 4: The question moves up. “It still trained on NVIDIA chips.” appears, then three short facts underneath.]*

DeepSeek still used NVIDIA chips.

*[Pause.]*

And that training bill excluded earlier research and experiments.

*[CLICK 5: The bottom line appears.]*

Our view is that another threat sits on NVIDIA’s own customer list.

Let’s rewind.

**Key line:** Some of NVIDIA’s biggest customers are building alternatives to its chips.

**Note for Q&A:** INTERNET — DeepSeek-V3 technical report, https://arxiv.org/html/2412.19437v2. Its estimated compute bill uses an assumed H800 rental rate and excludes earlier research and ablation experiments. The dollar comparison does not measure all-in R&D or the full cost of DeepSeek-R1.

## SLIDE 2 of 18 · Case facts · Group 1 · ~2 min

**On screen:** NVIDIA’s Journey to $3 Trillion
**Clicks:** 3 (1999 → 2007 with the CUDA logo, then ChatGPT, then the market value bars)

*[Point to the timeline and move your hand left to right.]*

Back then, GPUs were mainly used to make video games run better by handling many calculations at once.

*[CLICK 1: The timeline moves to 2007 and the CUDA logo appears.]*

Then in 2007, NVIDIA introduced Compute Unified Device Architecture (CUDA in short), allowing developers to use GPUs for more than just graphics.

*[Step toward the screen. Raise your energy.]*

*[CLICK 2: ChatGPT appears on the timeline.]*

Fast forward to 2022. ChatGPT launched, and suddenly everyone wanted to get into AI.

By then, NVIDIA already had the chips and software needed to train AI models.

*[CLICK 3: Market value bars grow. Point to them.]*

And look what happened.

NVIDIA's market value grew from around 400 billion to over 3 trillion dollars.

In fiscal 2024, it earned 60.9 billion dollars in revenue, mostly from data centers.

*[Pause. Ask the room, as if you really want an answer.]*

So, why did so many companies choose NVIDIA?

Well, the answer goes beyond the chips themselves.

**Key line:** NVIDIA's advantage comes from its chips, software, and developer community working together.

**Note for Q&A:** INTERNET — OpenAI’s July 2025 Productivity Note confirms the two-month timeline: https://cdn.openai.com/global-affairs/be0fe9e0-eb97-43d1-9614-99f2bd948bcc/OpenAI_Productivity-Note_Jul-2025.pdf. The build spec’s proposed one-month replacement is not supported by that source. If asked: “fiscal 2024” is NVIDIA’s financial year ending January 2024.

## SLIDE 3 of 18 · Case facts · Group 1 · ~2 min

**On screen:** NVIDIA sells one package that is hard to leave
**Clicks:** 6 (one per loop step, then the switching cost panel)

*[Trace the loop on screen with your hand, one step at a time.]*

Now, let's look at why companies keep choosing NVIDIA.

*[CLICK 1: Step 1 appears.]*

First, NVIDIA develops powerful chips.

*[CLICK 2: Step 2 appears.]*

Second, CUDA supplies reusable code. Someone has already done part of the work. Very helpful when your deadline is Friday.

*[CLICK 3: Step 3 appears.]*

Third, millions of developers already know how to use CUDA.

*[CLICK 4: Step 4 appears.]*

So naturally, companies prefer buying chips their developers are already familiar with. This also allows NVIDIA to charge higher prices.

*[CLICK 5: Step 5 appears.]*

And with those profits, NVIDIA can invest in even better chips. The cycle continues.

*[Stop moving. Lower your voice slightly. This is the key idea of the whole talk.]*

*[CLICK 6: The switching cost panel appears.]*

Now, what if a company wants to switch to another chip?

Your developers may need to rewrite code and learn different tools.

These are called switching costs.

So even if another chip is cheaper, switching could end up costing more.

*[One beat of silence. Then ask.]*

Now, who can actually afford to make that switch?

**Key line:** Switching away from NVIDIA can cost more than the savings from cheaper chips.

## SLIDE 4 of 18 · Case facts · Group 1 · ~1.5 min

**On screen:** NVIDIA's biggest customers are now building their own chips (donut chart: top 4 = 40%, everyone else = 60%)
**Clicks:** 1 (each company’s own chip)

*[Gesture to each company as it lights up.]*

Microsoft, Meta, Amazon, and Alphabet, Google’s parent company.

*[Point to the four colored segments.]* The case’s customer-share estimates put them at about forty percent of sales. Applied to fiscal 2024 revenue, that’s roughly 24.4 billion dollars.

*[Let that number sit for a moment.]*

*[CLICK 1: Each company’s own chip appears next to its name.]*

Microsoft has MAIA. Meta has MTIA. Amazon has Trainium and Inferentia. Google has the TPU.

These companies operate computing infrastructure at enormous scale.

*[Lean in. Make it slightly provocative.]*

They have the engineers and budgets to build alternatives.

Imagine your biggest customer saying, ‘We’ve started making our own.’ You’d probably clear your calendar.

That’s our problem.

**Key line:** NVIDIA’s biggest buyers have the resources to become less dependent on it.

## SLIDE 5 of 18 · Problem · Group 1 · ~1.5 min

**On screen:** How can NVIDIA protect its pricing power as its largest buyers build their own chips, and where can it create new demand?
**Clicks:** 2 (why/how buyers detach; the title moves up and the five questions appear)

*[Slow and deliberate. This is the thesis of the presentation. Let the title sit alone for a beat.]*

Here’s the decision.

How can NVIDIA protect its pricing power while large buyers build their own chips, and where can it create new demand?

*[CLICK 1: The line under the title appears: “Customers are locked into CUDA. Now the four biggest have the reason and the means to leave.”]*

CUDA gives customers a reason to stay.

These four have the resources to consider leaving.

They want lower costs and dependable supply.

Their engineers and software give them a way to act.

*[CLICK 2: The title moves up and the five questions appear one by one. Point to them one at a time.]*

We’ll use these five questions to guide the recommendation.

*[Handoff. Turn and open your hand toward the Group 2 presenter.]*

My colleague will take us through the evidence, starting with revenue concentration.

**Key line:** Five questions help us decide what NVIDIA should do.

## SLIDE 6 of 18 · Analysis · Q1 · Group 2 · ~2.5 min

**On screen:** 78% of NVIDIA's revenue now comes from AI data centers, its only proven growth engine
**Clicks:** 4 (margin evidence, portfolio map, migration risk, Blue Ocean verdict)

*[The three columns grow left to right. Point to them in order.]*

AI data centers went from thirty-nine percent of NVIDIA's revenue, to fifty-six, then seventy-eight.

Now, four out of five revenue dollars come from that business.

*[CLICK 1: Operating margin appears.]*

Operating margin reached fifty-four percent. Gross margin increased to seventy-three percent. And operating expenses barely changed. Combine that with strong revenue growth and they drive those strong margin gains.

*[CLICK 2: The portfolio map appears.]*

The Blue Ocean map asks what could drive growth next.

We place AI data centers in the pioneer column. AI Foundry could be an opportunity, but we have no revenue figure proving it yet.

*[CLICK 3: The data center box slides into the migrator column.]*

If alternatives catch up, data centers face more direct competition.

*[Pause. Point at the empty pioneer column.]*

And then NVIDIA loses that pioneer position.

To fill that void, NVIDIA can start testing AI Foundry while the current business is strong.

*[Transition. Curious tone.]*

*[CLICK 4: The verdict appears and the earlier visuals dim.]*

Is NVIDIA still in a Blue Ocean? NVIDIA still offers substantial value, but its buyers can now make substitutes.

**Key line:** A strong current business gives NVIDIA room to test its next source of growth.

**Note for Q&A:** GIVEN inputs: case Fig. 2, p. 4. COMPUTED: (60.9 / 27.0 − 1) ≈ 126%; 72.7 − 56.9 = 15.8 percentage points; (11.3 / 11.1 − 1) ≈ 2%. The 85¢ calculation uses the change in company-wide operating profit divided by the change in revenue, with rounding.

## SLIDE 7 of 18 · Analysis · Q2 · Group 2 · ~1.5 min

**On screen:** Data center revenue grew faster than estimated GPU shipments
**Clicks:** 3 (the "not a pure price" note + labels on the NVIDIA tray, the gross margin columns, the NVIDIA tax gap)

*[The two numbers count up. Point to them one at a time.]*

Looking at the numbers, estimated GPU shipments rose forty-two percent.

But data center revenue per GPU shipped rose by one hundred twenty-two percent.

Revenue grew much faster than GPU shipments.

*[CLICK 1: The note appears and the tray gets two labels: GPUs and networking.]*

Because a data center is not just GPUs; it includes other high-value non-GPU components and services like networking. Each GPU did not magically become more profitable.

*[CLICK 2: The gross margin columns grow.]*

Looking at gross margin, NVIDIA is at seventy-three percent, versus AMD's forty-seven and Intel's forty-one.

*[CLICK 3: The gap between NVIDIA and AMD lights up.]*

Buyers call this premium the ‘NVIDIA tax.’

*[Lean in. Provocative.]*

It's good because it rewards NVIDIA, but it incentivizes customers to investigate alternatives.

So what makes NVIDIA worth paying for?

**Key line:** The premium rewards NVIDIA and encourages buyers to look for alternatives.

## SLIDE 8 of 18 · Analysis · Q2 · Group 2 · ~1.5 min

**On screen:** Buyers pay for the finished AI job, not for raw chip speed

*[Playful. This slide surprises people. Set it up like a puzzle.]*

Imagine you’re approving this purchase.

On the case’s raw computing comparison, the H100 gives about fourteen percent fewer calculations per dollar.

And it costs roughly four times as much. Finance is gonna ask hard questions.

*[Ask the room. Wait one beat.]*

So why would the buyer approve it?

On NVIDIA’s reported training benchmark, it finishes the job about nine times faster.

Nine times the speed for four times the chip price gives about two and one-fourth times the training speed per dollar.

The hardware and software work together to deliver that result.

Customers even waited up to eighteen months, suggesting demand exceeded the available supply .

*[Transition. Firmer voice.]*

Let’s look at who has a realistic alternative.

**Key line:** Compare the cost of completing the job as well as the chip’s purchase price.

## SLIDE 9 of 18 · Analysis · Q3 · Group 2 · ~1.5 min

**On screen:** NVIDIA’s biggest buyers are also its biggest substitutes
**Clicks:** 2 (the other forces fade and buyers + substitutes turn amber, then the four names and their chips with “Same four firms”)

*[The NVIDIA hub appears, then the five forces pop out around it.]*

Five Forces helps us locate the pressure.

Here, buyers are developing another way to get the work done.

*[Pick up the pace. Move quickly past the other forces.]*

AMD and Intel compete too, but CUDA makes switching harder.

On supply, dependence on TSMC can constrain deliveries.

*[CLICK 1: The other forces fade. Buyers and substitutes turn amber.]*

*[Slow down. This is the main insight of the analysis.]*

For our strategy, the key relationship is here.

*[CLICK 2: The four names and their four chips appear, joined by “Same four firms”.]*

The same four firms are major buyers and developers of competing chips.

*[Firm.]*

A customer relationship can become a competitive relationship, sometimes during the same meeting.

What will they do next?

**Key line:** Major customers are also developing alternatives.

**Note for Q&A (details taken off the slide):** New entrants: $8.8 billion of venture money went into chip startups in 2023, but CUDA and scarce TSMC capacity hold them back. Suppliers: TSMC alone mass-produces 3-nanometer chips and is booked to 2026; ASML is the only maker of the EUV machines. Rivals: AMD MI300X, Intel Gaudi 3, Huawei Ascend. Substitutes: Amazon’s Trainium trains at about half the cost; open software such as PyTorch and UXL makes switching easier.

## SLIDE 10 of 18 · Analysis · Q3 · Group 2 · ~2 min

**On screen:** The big buyers will move work to their own chips wherever it is cheaper
**Clicks:** 2 (the corners fold away and the prediction flow takes their place, then the Amazon example)

*[The four corners fly in. Walk through them in order.]*

Four Corners helps us think through that.

Their motives are lower costs, supply security, and control.

Their chip programs show the strategy in action.

Google’s CEO argues that spending too little on AI is the bigger risk.

Google’s reported chip manufacturing cost is two to three thousand dollars, versus an A100 selling price around ten thousand. Design, software, and job performance still matter.

*[CLICK 1: The four corners fold into the Top 4 badge, and the prediction takes their place. Workloads start flowing. Say it clearly.]*

We expect a workload-by-workload decision.

If their own chip meets the performance need at lower overall cost, they have a reason to switch.

*[CLICK 2: The Amazon example appears.]*

Amazon has Inferentia for running models and Trainium for training. The case reports training at about half the cost. That’s a make-versus-buy decision.

*[Continue to the profit-at-risk calculation.]*

How much profit could a partial shift put at risk?

**Key line:** Buyers will assess each workload on performance and overall cost.

**Note for Q&A:** Current strategy detail taken off the slide: they rent their chips through their clouds rather than sell them, and Amazon tied Anthropic to its chips.

## SLIDE 11 of 18 · Analysis · Q4 · Group 2 · ~2 min

**On screen:** If the top four move a quarter of their purchases in-house, about $4.4 billion of gross profit is at risk
**Clicks:** 3 (gross profit, then the red at-risk slice with the count-up, then the Move 2 line)

*[Point to the first number.]*

Here’s our scenario.

Estimated annual sales to the four are about 24.4 billion dollars.

*[CLICK 1: Gross profit appears. The bar turns green.]*

Using the company-wide margin as a proxy gives about 17.7 billion in gross profit, assuming unchanged product mix and unit costs.

*[CLICK 2: The red slice grows out of the green bar and the number counts up to $4.4 billion. Let it finish before you speak.]*

A quarter of purchases moving in-house would put about 4.4 billion in annual gross profit at risk. Roughly a tenth of NVIDIA’s total.

The quarter is illustrative.

*[CLICK 3: The Move 2 line appears.]*

That exposure supports testing whether NVIDIA can retain networking and systems sales.

*[Handoff to Group 3.]*

My colleague will now explore new demand.

**Key line:** Even a partial shift can put billions in gross profit at risk.

## SLIDE 12 of 18 · Analysis · Q5 · Group 3 · ~2 min

**On screen:** NVIDIA’s next customers are companies that found custom AI too costly.
**Clicks:** 3 (the offer, the insurer workflow, the two pilot gates).

*[Point to the highlighted middle tier.]*

Let’s turn to companies that haven’t started buying yet.

This map helps us explore groups outside the existing market.

We’d start with companies that evaluated custom AI but found implementation too expensive.

*[CLICK 1: Tiers 1 and 3 fold away. The offer appears.]*

This is our proposed offer: Test a standard package for one manual task, delivered through a partner using AI Foundry, NeMo, and NIM.

*[CLICK 2: The insurer appears, and a dot lands on the tier 2 ring.]*

For example, consider an insurer searching policy documents. First, we check the time spent and willingness to pay.  And if they say ‘Let’s add AI’, well that's time for a business case.

*[CLICK 3: The gates appear.]*

We need two confirmations. One, do savings justify the price? And two, can NVIDIA and its partner deliver profitably? Otherwise, revise or stop.

Now let’s choose the responses.

**Key line:** Start with one task and prove that the offer pays for both sides.

**Note for Q&A:** GIVEN anchors supplied by the build spec: enterprise market, p. 16; Jetson price and December 2024 timing, p. 17. Tier mapping is OUR JUDGMENT; the insurer, package and pilot gates are OUR PROPOSAL based on WAC v3.

## SLIDE 13 of 18 · Options · Group 3 · ~1.5 min

**On screen:** We tested the case’s five options, plus one of our own
**Clicks:** 2 (A and D are struck out, then the Move 1/2/3 labels and the kept cards light up)

*[The six cards come in. Steady and quick. Don’t read the cards.]*

We screened the five case options and added one more, interoperability: connecting customer chips to NVIDIA networking and systems.

We looked at competitive value, customer concentration, and risk.

*[CLICK 1: The two bottom options are struck out.]*

We rejected two of the options.

Exclusive purchasing contracts may raise regulatory concerns and could make customers feel more constrained.

Meanwhile, selling chip design know-how could strengthen competing chips.

*[CLICK 2: The move labels drop in and the four kept cards light up.]*

That leaves us with three moves: CUDA gets investment now. Custom products and interoperability need testing. New enterprise demand starts with a pilot.

**Key line:** Invest in CUDA now and test the other promising options.

**Note for Q&A:** GIVEN, case pp. 5, 14 and 17: large buyers can build whole systems themselves. Our proposal targets mixed fleets; Meta still planned about 350,000 H100s in 2024. We must demonstrate that integration keeps enough gross profit to cover its cost. We used no weighted scores. The weights would be our own guesses, and changing them could change the winner.

## SLIDE 14 of 18 · Recommendation · Group 3 · ~2 min

**On screen:** Invest in CUDA now, and test the other two moves before scaling them
**Clicks:** 3 (Move 2, Move 3, then the ERRC strip)

*[Stand tall. Slow down. This is the answer.]*

Here’s what we would ask Jensen, I mean the CEO, to approve.

*[Move 1 is on screen.]*

Move one. Invest in CUDA now. Keep improving the tools and performance for developers, including those using PyTorch.

*[CLICK 1: Move 2 appears.]*

Move two. Test interoperability with one buyer. Compare expected profit with proceeding without it, including integration costs and any additional loss of GPU gross profit. Expand only if the comparison improves.

*[CLICK 2: Move 3 appears.]*

Move three. Pilot a standard AI Foundry package for first-time buyers, delivered on NVIDIA software and computing infrastructure. Scale when customers keep paying and delivery earns a profit.

*[CLICK 3: The ERRC strip appears.]*

This ERRC grid makes the choices explicit. Drop exclusive deals, reduce buyer concentration, improve developer ease, and test new offers.

Here’s how those moves connect to the findings.

**Key line:** Approve the CUDA investment and give the two pilots clear profit tests.

## SLIDE 15 of 18 · Justification · Group 3 · ~1.5 min

**On screen:** Every move comes from a finding in our analysis. Three finding cards on the left (73% · ≈40% · a new enterprise market), each move card arrives on the right.

**Clicks:** 4 (Move 1 · Move 2 · Move 3 · the two rejected options)

*[The three findings are on screen. Point to the left column.]*

Let’s follow each row.

CUDA makes switching costly.

*[CLICK 1: Move 1 appears.]*

So keep improving its value to developers.

*[CLICK 2: Move 2 appears.]*

The top four can shift the work in house, which would obviously put a substantial amount of profit at risk.

So test whether retained systems sales improve the overall profit picture. Keep CUDA locked into the NVIDIA hardware.

*[CLICK 3: Move 3 appears.]*

Revenue concentration also gives NVIDIA another reason to be looking for new buyers.

AI Foundry are testing whether previously reluctant customers will prove to be profitable.

*[CLICK 4: The two rejected options are struck out.]*

We rejected the exclusive contracts and the sale of our design know how for the reasons we've already discussed.

*[Firm.]*

Each move is supported by evidence.

What would make us change our minds?

**Key line:** Each move has evidence behind it and a result we can test.

**Note for Q&A:** The 73% is NVIDIA’s company-wide gross margin in fiscal 2024 (72.7%), a GIVEN case figure. We don’t port CUDA to rival chips: the plug-in path is for racks, networking and system software.

## SLIDE 16 of 18 · Risks · Group 3 · ~1.5 min

**On screen:** What could go wrong, and how we would know early. One risk card per move (warning sign + our response), then a "We would watch" strip and the closing line.

**Clicks:** 4 (risk to Move 2 · risk to Move 3 · watch strip · closing line)

*[Brisk. One risk per move.]*

Here's how we keep the recommendation honest.

For CUDA, watch the workloads move to the other chips. Keep earning developer preference.

*[CLICK 1: Risk to Move 2 appears.]*

For interoperability it's watch faster shifts in-house. Test with urgency, but keep the profit gate.

*[CLICK 2: Risk to Move 3 appears.]*

For AI Foundry it's the paid conversion and delivery costs that we're interested in. A nice demo is all very well but it's a paying customer that tells us the real story.

*[CLICK 3: The watch strip appears.]*

Track those alongside customer concentration and total sales.

*[CLICK 4: The closing line appears. Slow down.]*

Invest in CUDA. Expand the pilots when the results warrant it.

Let's test that with the room.

**Key line:** Pilot results should decide whether the strategy expands.

**Note for Q&A:** Other risks we would watch: regulators acting against NVIDIA’s deals (like the Run.ai review in the case), AI getting so cheap that spending slows (Move 3 widens the customer base), and chip supply at TSMC (no real second source for leading chips). After the case, NVIDIA’s revenue kept growing and its margin returned to about 75%; that figure is from outside the case, so say so if asked.

## SLIDE 17 of 18 · Close · Group 3 · ~1.5 min

**On screen:** If you were Microsoft, you’d build your own chip either way. Would you also build the racks, networking and software around it, or plug it into NVIDIA’s? Then the NVLink Fusion board rises in, its chips light up (NVIDIA GPUs green, their own chip blue), and the final line appears.

**Clicks:** 3 (board + NVLink Fusion name · chips light up + caveat · final line)

*[Pause. Look at the room. Ask, then wait.]*

You’re Microsoft, building your own chip. Would you also build the racks and networking, or consider NVIDIA’s? What would decide it?

*[Take two or three answers. Don’t argue. Thank each person.]*

*[CLICK 1: The board rises in.]*

After the case, NVIDIA announced NVLink Fusion in May 2025.

*[CLICK 2: The chips light up.]*

It described ways custom chips could work with NVIDIA infrastructure. The specific configuration still needs testing.

That’s similar to our second move. Commercial results would tell us how well it works.

*[CLICK 3: The final line appears. Walk back to the spot where you started Slide 1.]*

Back to the opening headline.

Cheaper AI raised questions about demand. We also need to ask what customers will keep buying when they build their own chips.

*[Slow. Final line. Then stop.]*

Make NVIDIA’s systems valuable enough that customers keep choosing them.

Thank you and with that we’ll end with a short video of current happenings in the top management of NVIDIA.

**Key line:** Give customers a reason to keep choosing NVIDIA’s systems.

**Note for Q&A:** GIVEN, case pp. 13 and 15: Amazon bought Annapurna in 2015, launched Inferentia in 2018 and Trainium in 2020, and built the Neuron SDK; Google has developed TPUs since 2015. These are years of chip, software and integration work. We do not assume an NVIDIA partnership eliminates R&D costs. INTERNET — NVLink Fusion launch: https://nvidianews.nvidia.com/news/nvidia-nvlink-fusion-semi-custom-ai-infrastructure-partner-ecosystem. NVLink Fusion is from outside the case (announced May 18, 2025). Partners named at launch included MediaTek, Marvell, Qualcomm and Fujitsu. In NVIDIA’s picture the customer’s chip is drawn as a CPU; Fusion also pairs customers’ own AI chips with NVIDIA’s CPUs and networking.

## SLIDE 18 of 18 · Thank you · All · ~0.2 min

**On screen:** "Thank you" and the members of LT 1, LT 2 and LT 9.

*[Everyone on stage. Smile.]*

We’d be happy to take your questions.

## BACKUP SLIDES B1 and B2 · Group 3 (Q&A captain)

**B1, the 15 poll answers**

*[Use only if the professor asks or runs the case poll. Don’t present it unprompted.]*

“Here’s where we landed on the fifteen case questions. Each answer points back to the slide with our evidence. Which one would you like us to discuss?” Then go to the relevant slide.

The presentation’s analytical Q5 (new demand) is answered on slide 12. Polling Q5 here is a different question: profit model, answered on slide 7.

The 12-question defense bank is in NVIDIA_QA_Defense.md.

**B2, other frameworks**

*[Use only if asked.]*

“We also considered PESTLE and SWOT. They reinforced our focus on the large buyers, so we used Five Forces and Four Corners to keep the main discussion focused. We can talk through the other frameworks if helpful.”

## Quick glossary: every technical term in the script

| Term | Plain meaning |
| --- | --- |
| Market value | What all of a company’s shares are worth together |
| GPU | Graphics processing unit: a chip that does thousands of small calculations at once |
| CUDA | NVIDIA’s software for programming its chips; it only runs on NVIDIA chips |
| Library | Ready-made code that developers can reuse instead of writing it themselves |
| Data center | A building full of computers used to run software at large scale |
| Fiscal 2024 | NVIDIA’s financial year ending January 2024 |
| Pricing power | The ability to charge more without losing customers |
| Switching cost | What a customer loses by changing supplier: rewriting code, retraining staff |
| Lock-in | When switching costs are so high that customers stay |
| Hyperscaler | A company that runs cloud computing at enormous scale (Microsoft, Amazon, Google, Meta) |
| Antitrust | Laws that stop a dominant company from blocking competition |
| Operating profit | What is left after paying to make the product and run the company |
| Gross margin | The share of each sales dollar left after paying to make the product |
| TFLOPS | Trillions of calculations per second; a measure of raw chip speed |
| Training | When an AI model learns from huge amounts of data |
| Inference | When a trained AI model answers a question; happens billions of times a day |
| Pioneer / migrator / settler | Blue Ocean labels: new value / better than rivals / me-too |
| Five Forces | Porter’s tool showing who holds power: buyers, suppliers, rivals, new entrants, substitutes |
| Substitute | A different product that does the same job |
| Four Corners | A tool to predict a competitor’s next move: drivers, strategy, beliefs, capabilities |
| ERRC grid | Blue Ocean tool: what to eliminate, raise, reduce and create |
| PyTorch | Free AI programming software that can run on many companies’ chips |
| TSMC | The Taiwanese company that manufactures NVIDIA’s most advanced chips |
| NVLink Fusion | NVIDIA’s 2025 product that lets customers’ own chips connect into NVIDIA systems (outside the case) |
