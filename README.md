# Invoice exceptions: decision memo and fact base

A work sample: a one-page steerco memo on supplier invoice exceptions, and the fact base behind it.

**Fictional company and data.** Kestrow Grocers Ltd and every figure on the page are invented.

Live page: https://saeedfzn.github.io/process-insight-memo/

## The answer the memo gives

Approve a six-week agent pilot, in two moves:

1. Set the ERP match tolerance to the written procedure first. That alone removes about 18% of exceptions and needs no agent.
2. Pilot the agent on what is left, judged on control and cash: no price above tolerance paid without a buyer's decision on record. Released clerk time is a by-product.

## What is on the page

1. **Decision memo.** The decision, the recommendation, three numbers with baselines and ranges (cash exposure, clerk capacity, cycle time), four kill criteria with thresholds and sources, and five asks of the steerco. It prints on one A4 page; nothing else prints.
2. **Fact base.**
   - As-is process map: seven steps and three exception loops, each with its system, owner, volume, time and finding.
   - Value at stake by lever (cost, cash, cycle time, service, control), with a sensitivity panel and a flag when the scenario differs from the base case.
   - Capacity and cash are never added into one £ figure.
3. **Hypothesis log.** Three hypotheses, each with a kill criterion written before the test, evidence for and against, and what changed. Two did not survive as first written.
4. **Agent versus person.** What the agent does by rule, what goes to a named person with the evidence attached, and what is logged. Pilot scope, a primary control metric, a cash measure, cycle time, a balancing measure on late payment and a volume gate.
5. **Handover.** Next actions with owner and date, open questions, and an evidence trail with caveats.

## How the numbers stay consistent

- The sized figures, including those quoted in the memo, are calculated from one model in the page script. Each input is tagged measured, sampled or assumption and has a low, base and high value. A few descriptive facts (the interquartile range, the thresholds in the kill criteria) are stated directly.
- Ranges are computed from the low and high inputs, not typed in.
- Twelve model checks run on load and are shown on the page: for example, the sample classes sum to 400, the hours reconcile, and each range is confirmed as the true envelope across every low/high combination.

## Build

A single `index.html` with system fonts and no external requests. Light and dark themes follow the OS setting; a toggle overrides it.
