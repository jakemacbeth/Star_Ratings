# Medicare Advantage Star Ratings Forecast

Forecasts year end closure rate for the measure controlling blood presure for hypertensive patients to quantify how much outreach is needed to reach or hold a target star rating.

## Contents
- About
- Summary
- Year End Forecast
- Comparison to Previous Years
- Model Reliability
- Limitations and Next Steps

<div align="center">
  
## About
</div>

Medicare Advantage plans are scored on Star measures that affect reimbursement and enrollment. This project forecasts where the measure CBP will finish the year from a May 15th assessment point. The forecast estimates the measure's natural self-closure rate, the share of gaps expected to close without intervention, to determine where it will land relative to its current rating band and the next cut point. The goal is to inform an outreach team so they can determine if the measure is at risk and roughly how much outreach is needed to improve it. The project uses synthetic public health data generated with [Synthea](https://synthetichealth.github.io/synthea/). As a naive target it applies Star cut points drawn from the 2026 [CMS technical specifications](https://www.cms.gov/files/document/2026-star-ratings-technical-notes.pdf ) used to grade 2024 plans.

<div align="center">
  
## Summary
</div>

As of May 15, the forecasted year end Controlling Blood Pressure rate was 80.22% (95% interval: 79.2-81.16%), 1.3 percentage points (184 patients) above the four-year average and .9 percentage points (129 patients) above the previous high in 2025. 33.69% of simulations result in a 3 star rating, 66.25% for 4 stars, and .02% for 5 stars. With respect to the lower bound percentile of simulations reaching 4 stars would take about 150 more controlled members, a 5.2% uplift and 979 more controlled members, a 33.6% uplift for 5 stars. The higher forecast is driven by our strongest May 15 start in four years, while the expected gain over the rest of the year is in line with  prior years. Identifying which members to target and the cost of closing them requires outreach data not yet in the database.

<div align="center">
  
## Year End Forecast
</div>
<div align="center">
  <img src="charts/forecast.png" width="75%" height="auto" />
</div>

<div align="center">
  
## Comparison to Previous Years

</div>
<div align="center">
  <img src="charts/eoy_rates.png" width="75%" height="auto" />
</div>
