# Medicare Advantage Star Ratings Forecast

Forecasts year end closure rate for the measure controlling blood presure for hypertensive patients to quantify how much outreach is needed to reach or hold a target star rating.

## Contents
- About
- Summary
- Year End Forecast
- Comparison to Previous Years
- Recommendations and Next Steps
- Model Reliability
- Scope and Limitations

<div align="center">
  
## About
</div>

Medicare Advantage plans are scored on Star measures that affect reimbursement and enrollment. This project forecasts where the measure CBP will finish the year from a May 15th assessment point. The forecast estimates the measure's natural self-closure rate, the share of gaps expected to close without intervention, to determine where it will land relative to its current rating band and the next cut point. The goal is to inform an outreach team so they can determine if the measure is at risk and roughly how much outreach is needed to improve it. The project uses synthetic public health data generated with [Synthea](https://synthetichealth.github.io/synthea/). As a naive target it applies Star cut points drawn from the 2026 [CMS technical specifications](https://www.cms.gov/files/document/2026-star-ratings-technical-notes.pdf ) used to grade 2024 plans.

<div align="center">
  
## Summary
</div>

As of May 15, the forecasted year end Controlling Blood Pressure rate was 80.22% (95% interval: 79.2-81.16%), 1.3 percentage points (184 patients) above the four-year average and .9 percentage points (129 patients) above the previous high in 2025. 33.69% of simulations result in a 3 star rating, 66.25% for 4 stars, and .02% for 5 stars. With respect to the lower bound percentile of simulations reaching 4 stars would take about 150 more controlled members, a 5.2% uplift and 979 more controlled members, a 33.6% uplift for 5 stars. With the 5-star cut point more than 8 standard deviations above the mean forcasted outcome, 5 stars is not a realistic target, and outreach should focus on securing 4 stars. The higher forecast is driven by our strongest May 15 start in four years, while the expected gain over the rest of the year is in line with  prior years. Identifying which members to target and the cost of closing them requires outreach data not yet in the database.

<div align="center">
  
## Year End Forecast
</div>
<div align="center">
  <img src="charts/forecast.png" width="75%" height="auto" />
</div>

The model simulated 10,000 year end outcomes for 2026 based on each member's status at May 15. The median simulated rate is 80.23%, and 95% of simulations fall between 78.92% and 81.44%.

**A 4 star rating is the most likely outcome, but the margin is thin.**
- The 4-star cut point sits almost exactly in the center of the distribution, so the outcome is close to a two-way split: 66.25% of simulations finish at 4 stars and 33.69% at 3 stars.
- At the median, the measure clears 4 stars by about 0.2 percentage points, or roughly 31 of 13,805 members, leaving a thin cushion.
- At the lower end of the 95% interval, reaching 4 stars would take about 150 more controlled members, or 5.2% of the members still expected to be uncontrolled at year end.
- The 3-star floor at 75% is not a realistic concern. It is 7.6 standard deviations below the mean simulated rate, and only 4 of the 10,000 runs fell below it.

**Reaching 5 stars is not realistic without substantial outreach.**
- The 86% cut point is 8.4 standard deviations above the mean simulated rate.
- Only 2 of the 10,000 runs reached it, at 88.06% and 90.30%, which are 11.5 and 14.7 standard deviations above the mean.
- These runs are extreme outliers, roughly 900 and 1,200 more year-end controlled members than the optimistic 97.5th percentile. The 0.02% chance of 5 stars reflects rare tail outcomes rather than a plausible path to 86%.
- Closing the gap would take about 797 more controlled members at the median and 979 at the lower bound, or 33.6% of the members expected to remain uncontrolled.


  
## Comparison to Previous Years

</div>
<div align="center">
  <img src="charts/eoy_rates.png" width="75%" height="auto" />
</div>

**2026 is forecasted to be the first year above the 4 star cut point.**
- Year-end rates rose from 78.1% in 2022 to 79.3% in 2024, then held flat at 79.3% in 2025.
- The 2026 median forecast of 80.2% is 1.3 percentage points (184 members) above the four-year average of 78.9%, and 0.9 percentage points (129 members) above the previous high in 2025.
- Even the lower bound of the 95% interval, 78.9%, matches the four-year average, so the forecast's worst plausible case is an average year rather than a decline.

**The higher forecast comes from a stronger start, not a faster finish.**
- 44.2% of members were controlled at May 15, the highest of any year: 0.6 percentage points above 2025 and 1.4 points above the four-year average of 42.8%.
- The gain from May 15 to year end has been stable, between 35.7 and 36.6 percentage points each year, and the forecast's expected gain of 36.0 points falls within that range.
- That stability also shows how thin the 4-star margin is. A gain at the low end of history, 35.7 points, would put 2026 at 79.9%, just below the cut point.

<div align="center">
  <img src="charts/bp_bands.png" width="75%" height="auto" />
</div>

**The stronger start reflects broad improvement: more members tested and fewer uncontrolled.**
- The share not tested by May 15 fell from 46.7% in 2022 to 45.4% in 2026.
- The share tested but uncontrolled fell every year, from 11.5% to 10.4%.
- Readings shifted toward lower blood pressure: the under-120 band grew from 23.6% to 25.9%, while the 140–149 and 150–159 bands each shrank by about half a point.
- The 160+ band is the exception, holding between 2.6% and 2.9% every year, so the most severely elevated members have not followed the broader improvement.

**Most of the remaining gain has to come from members not yet tested.**
- At May 15, 45.4% of members had no reading, compared with 10.4% who were tested but uncontrolled.
- Even if every tested but uncontrolled member became controlled, a typical 36-point gain would still require about 26 points from members not yet tested.
- Whether 2026 holds 4 stars depends mainly on getting those members a reading before year end.

<div align="center">

## Recommendations and Next Steps
</div>

**Based on current data, protecting 4 stars should take priority over pursuing 5 stars.**
- There is a 33.69% chance the measure finishes at 3 stars, and the median clears the 4-star cut point by only about 31 members.
- A year-end gain at the low end of history would put the rate at 79.9%, just below 4 stars.
- Securing 4 stars at the lower bound takes about 150 more controlled members, while 5 stars takes 797 to 979, about a third of the members expected to remain uncontrolled.
- This could change with outreach success rates and cost-per-closure data, which would show whether the additional members needed for 5 stars can be reached at a reasonable cost.

**Prioritize getting untested members a reading.**
- 45.4% of members had no reading at May 15, and a typical year's gain requires at least 26 points from this group.
- Readings taken earlier in the year leave time for a follow-up reading if the first one is uncontrolled.

**Route members with readings of 160+ to providers rather than general outreach.**
- This band has held between 2.6% and 2.9% every year (about 370 members in 2026) while every other uncontrolled band improved.
- Whatever drove the broader improvement has not reached these members, so more direct involvment is likely needed.

**Refresh the forecast monthly.**
- The 4-star margin is smaller than the year-to-year variation in the gain after May 15, so an early warning matters more than a single May 15 estimate.
- Rerunning the model on each month's data and comparing actual closures with the expected path shows whether 2026 is tracking toward the low or high end of history.

<div align="center">

## Model Reliability
</div>

<div align="center">
  <img src="charts/backtest.png" width="75%" height="auto" />
</div>

**The model forecast past year end rates within half a percentage point and beat a simple benchmark.**
- Each past year was forecasted using only the years before it. Errors were −0.50, +0.05, and +0.49 percentage points for 2023, 2024, and 2025, or 61, 7, and 67 members.
- The mean absolute error was 0.35 points, compared with 0.50 points for a naive forecast that adds the average historical gain to each year's May 15 rate.
- The model beat the benchmark in 2024 and 2025. The benchmark did slightly better in 2023, when the model was trained on a single year.

**Past errors are larger than the 4-star cushion.**
- At the median, the 2026 forecast clears 4 stars by about 31 members, while past errors reached 61 to 67 members.
- A miss the size of 2023's or 2025's could move the result to either side of the cut point.

<div align="center">
  <img src="charts/validation_metrics.png" width="75%" height="auto" />
</div>

**Both underlying models predict well on members they were not trained on.**
- On the 2025 holdout, the closure model predicted 5,109 closures against 5,043 actual, an over forecast of about 1%.
- Its AUC of 0.77 means that 77% of the time, it ranks a randomly chosen member who closed above one who did not. Its predictions are 31% more accurate than always guessing the average closure rate (Brier skill).
- Predicted closure rates matched actual rates within about 3.6 percentage points in every decile.
- The reversion model predicted 143 reversions against 144 actual, with an AUC of 0.93 and 18% Brier skill. Reversions are rare (about 2.4% of members controlled at May 15), so they have a small effect on the final rate.

<div align="center">

## Scope and Limitations
</div>

**Scope:** The 2026 Star Ratings include 45 measures across Part C and Part D. This project models only controlling blood pressure for hypertensive patients. The large majority are out of scope because they cannot be computed from Synthea's claims and clinical output or have unreasonable adherence or closure curves. 
- Patient-experience and survey (CAHPS): Measures like Getting Needed Care, Customer Service, and Rating of Health Plan come from beneficiary surveys, not clinical or claims records. Synthea generates care events, not survey responses, so there is nothing to compute these from.
- Administrative and operations: Measures like Complaints about the Plan, Members Choosing to Leave, Plan Makes Timely Decisions about Appeals, and Call Center availability are properties of the plan's operations and enrollment behavior, not patient health data.
- Part D drug measuresL adherence and pricing measures like Medication Adherence, MPF Price Accuracy, MTM Completion)require pharmacy claims and plan pricing data outside Synthea's scope.
- Dropped after testing: From that computable clinical set, 9 measures were evaluated and dropped for different reasons.
    - COL (Colorectal Cancer Screening): dropped for having no usable within-year closure curve: the qualifying event has a multi-year lookback, so almost nothing closes inside the measurement year and there is no within-year dynamic to forecast.
    - EED (Diabetic Eye Exam): dropped because its closure rate landed roughly 20 percentage points below the 1-star cut point
    - GSD (Diabetes Blood Sugar Controlled): the synthetic A1c distribution ran implausibly low, so almost no members fell in the poor-control band the measure depends on.
    - SPC (Statin Therapy for Cardiovascular Disease) — closure behavior did not reflect a realistic clinical process.
    - Three medication-adherence measures (diabetes, RAS/blood-pressure, cholesterol): dropped for implausible generated adherence - closure rates were unrealistically high.
    - KED (Kindey Health Evaluation for Patients with DIabetes) - Closure Behavior is almost entirely dependent on prior year completetion.

  


