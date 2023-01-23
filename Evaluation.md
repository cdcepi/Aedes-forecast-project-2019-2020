### Evaluation

All forecasts will be scored by comparison to data reported by participating counties in each year. Those data will be collected from participating counties when the data are complete for the year. Forecasts will be ranked by average logarithmic score (see below) across all counties and months for each species separately. If reported trapping effort for the year is substantially different from previous year for some counties/months, those counties/months may be removed from the analysis. Forecasts for counties without trapping data for a given month (e.g. November and December) will not be scored.


**Eligibility**
  
To be eligible for an overall ranking, teams must:
1. Submit forecasts for every county listed on the **Data** page and for every month of the challenge: April, May, June, July, August, September, October, November, and December.
2. Submit forecasts electronically prior to the respective deadline (the day before each new month starts).
3. Submit a model description (see **Participation** page).

Forecasts from teams that do not submit all required forecasts may still be evaluated, but they will not be ranked for overall performance. Teams may consider submitting some naive forecasts (e.g. 0.5) if they have difficulty producing all forecasts by the deadlines.

**Results**
  
Preliminary results will be distributed to all teams. A joint manuscript will be prepared by the project organizers to disseminate all forecasts, findings of this analysis, and the general performance of submitted forecasts. Participants may publish their own forecasts and results at any time.

### Logarithmic Score

All forecasts are probabilistic, a probability, $p$, of the mosquito species being reported in a specific month in a specific county. Reported data from 2019 will be used to classify presence for each species, county, and month combination, $x$, as present (1) or absent (0) following the definition on the **Targets** page. The logarithmic score is calculated as:
  
  $$S(p,x) = x\text{ln}(p) + (1-x)\text{ln}(p - 1)$$
  
  Logarithmic scores ($S$) can be averaged across many different predictions. In this case they will be averaged for all included counties and months for each species separately.

**Example:** A forecast predicts there is a probability of 0.2 (i.e. a 20% chance) that *Ae. aegypti* is reported in County X in June 2019. Collection of an adult *Ae. aegypti* in June is reported later in 2019. The logarithmic score is therefore $\text{ln}(0.2) = -1.6$. Alternatively, if no *Ae. aegypti* were reported, the logarithmic score would be higher, $\text{ln}(1 - 0.2) = \text{ln}(0.8) = -0.22$.

**Notes**
  
  * A 50/50 chance or a probability of 0.5 gives a logarithmic score of -0.69 regardless of whether the species was observed or not. 
* A forecast probability of 0 will give a logarithmic score of -Infiniti if the species is reported. The same is true for a probability of 1 when the species is not reported. Even a small probability for unlikely events can substantially improve average scores. For example, a forecast probability of 0.01 will give a logarithmic score of -4.6 if the species is observed.

**References**
  
  * Gneiting T and AE Raftery. (2007) Strictly proper scoring rules, prediction, and estimation. Journal of the American Statistical Association. 102(477):359-378. Available at: [https://www.stat.washington.edu/raftery/Research/PDF/Gneiting2007jasa.pdf](https://www.stat.washington.edu/raftery/Research/PDF/Gneiting2007jasa.pdf).

* Rosenfeld R, J Grefenstette, and D Burke. (2012) A Proposal for Standardized Evaluation of Epidemiological Models. Available at: [http://delphi.midas.cs.cmu.edu/files/StandardizedEvaluation_Revised_12-11-09.pdf](http://delphi.midas.cs.cmu.edu/files/StandardizedEvaluation_Revised_12-11-09.pdf).
