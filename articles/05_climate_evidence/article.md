Climate evidence is strongest when independent measurement systems converge. Surface thermometers, satellite observations and atmospheric carbon-dioxide records do not measure the same quantity, use the same instruments or begin in the same decade. Their agreement, visible in the record opening this piece, is valuable precisely because their weaknesses are different.

Across five figures, the evidence forms a chain rather than a collage: the long surface record shows warming, its curvature shows acceleration, satellites confirm the recent direction, atmospheric measurements identify the rising greenhouse-gas background, and the electricity mix shows one system through which societies can respond.

## A century of noise resolves into one direction

The surface-temperature record opening this piece spans 1880 to 2023. Individual years move around, but the rolling average shifts decisively upward, with recent decades well above the earlier baseline. Roughly 1.1°C of warming separates the beginning and end of the record, and much of that increase is concentrated after 1980.

The long time horizon matters. Weather creates short-term variation; climate appears in the movement of the distribution and the baseline across many decades. No single hot year carries the argument. The persistence of the rise does.

## The rate of change is not constant

[[image1]]

*Figure 2. A curved fit to the global surface-temperature anomaly record highlights acceleration rather than a constant linear drift.*

The same surface-anomaly record was refitted with a quadratic term alongside the simple linear trend, so the two models could be compared directly on how well each describes the shape of the late record rather than just its overall direction.

The acceleration view asks a different question from the opening chart. It does not merely show that temperatures rose; it tests whether the pace of warming changed. The upward curve fits the late-record anomalies better than the idea of one constant increase stretched evenly across the full period.

That distinction shapes risk. Systems can adapt more easily to gradual change than to a signal whose rate increases while infrastructure, ecosystems and institutions respond slowly. Acceleration compresses the time available for adjustment.

## Satellites provide an independent recent check

[[image2]]

*Figure 3. AIRS satellite temperature anomalies from 2002 to 2025 show a positive fitted trend despite substantial year-to-year variation.*

A separate satellite-derived anomaly series, built on different instrumentation and physics from the ground-station record, was fitted with its own trend line over its shorter available window, specifically so it functions as an independent check rather than a second view of the same underlying measurements.

Satellite observations cover a much shorter period, so they cannot replace the surface record. Their value is independence: different instruments and physical measurement principles reach a compatible conclusion over the period they observe. The annual anomalies remain noisy, but the fitted direction is positive.

Independent agreement is more persuasive than repeatedly redrawing one dataset. Surface and satellite records can disagree in particular years without undermining the broader result; what matters here is that their long-run directions align.

## The atmospheric background is rising underneath its seasons

[[image3]]

*Figure 4. Cape Grim measurements show carbon-dioxide concentration rising across decades while the normal annual seasonal cycle continues.*

Monthly Cape Grim CO₂ readings were plotted as a continuous time series without smoothing away the seasonal cycle, so the chart shows both the year-to-year oscillation and the underlying multi-decade climb in the same view.

The Cape Grim record adds the forcing side of the evidence chain. Seasonal absorption and release create a regular oscillation, but each cycle occurs on a higher baseline than the one before. Normal variability and structural change coexist in the same chart.

This is a useful visual lesson beyond climate science. A repeating cycle does not imply stability when the centre of that cycle is moving. The long-run concentration trend is the signal; the monthly variation sits around it.

## The response has to be engineered into real systems

[[image4]]

*Figure 5. The NSW fuel mix shows renewable supply growing inside an electricity system that still depends heavily on thermal generation.*

NSW generation was broken down by fuel type over time using the same grouping approach as the other energy pieces in this series, chosen deliberately so the climate evidence and the practical response sit inside one consistent analytical frame rather than two unrelated datasets stitched together.

The energy figure changes the article from diagnosis to response. Electricity is not the whole emissions problem, but it is a major lever because cleaner supply can serve existing demand and support the electrification of transport, buildings and industry. The chart also prevents an easy slogan: renewables grow within a system that must remain reliable through every hour.

The practical program is therefore broader than adding generation. It includes transmission, storage, flexible demand, efficiency and transparent measurement of whether low-carbon supply is actually displacing fossil output.

## A chain of evidence, not a single trend

[[image5]]

*Figure 6. A large-format synthesis board that brings the article's five principal pieces of evidence into one readable argument.*

The synthesis board links observations that are often discussed separately: long-run surface warming, acceleration, satellite measurements, atmospheric carbon dioxide and the energy system that must respond. Their methods and time horizons differ, yet they resolve toward the same underlying direction. Agreement across independent evidence is more informative than the smoothness of any one line.

That convergence changes the burden of proof. Short-term noise can alter a particular year or dataset without dissolving the broader signal. The practical question is therefore how quickly physical systems and policy can react to risk that is already visible across multiple records.

## Converging evidence should produce converging action

The surface record establishes long-run warming. The acceleration curve shows that the change is not evenly distributed through time. Satellites independently confirm the recent direction. Cape Grim records the rising atmospheric background. The electricity mix identifies a concrete system where intervention can reduce future emissions.

Five charts do not remove every scientific or policy uncertainty. What they show is that uncertainty at the margins does not erase agreement at the centre. Different datasets, periods and instruments point toward a warming climate under rising greenhouse-gas concentrations, while the energy system offers a measurable route for response.

The coherent theme is evidence matched to agency: measure the change honestly, then redesign the systems capable of changing its future path. Of everything in this piece, the acceleration chart is the one I find hardest to look away from, because a constant rate is a problem you can plan around and an accelerating one is not, and the fitted curve here says plainly which of those two we are actually living inside.

## Methods and original sources

This is an exploratory synthesis of Australian electricity data, global surface-temperature anomalies, AIRS satellite anomalies and Cape Grim atmospheric CO₂, built in Python with pandas handling the time-series alignment and statsmodels fitting the linear and quadratic trend lines against the surface and satellite records. Different periods and geographies mean it is not a formal attribution study. It shows convergence across independent records and connects that evidence to an actionable energy-system lever.

- [Full Elite analysis notebook](https://github.com/accidentalscientist/elite-analytics-articles-2026/blob/main/notebooks/05_climate_evidence.ipynb)
- [Australian electricity mix](https://github.com/accidentalscientist/daily_data_analytics_august2025/blob/main/week00/climate_change_proof_part5.ipynb)
- [Global surface-temperature anomalies](https://github.com/accidentalscientist/daily_data_analytics_august2025/blob/main/week00/climate_change_proof_part6.ipynb)
- [AIRS satellite-temperature anomalies](https://github.com/accidentalscientist/daily_data_analytics_august2025/blob/main/week00/climate_change_proof_part7.ipynb)
- [Cape Grim atmospheric CO₂](https://github.com/accidentalscientist/daily-data-analytics-may2025/blob/main/day17/climate_change_part1.ipynb)
