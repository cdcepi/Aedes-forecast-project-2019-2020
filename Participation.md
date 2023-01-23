**How to participate**

To participate in the challenge, one team member must register on the predict.cdc.gov website *and*, after logging in, register specifically for the *Aedes* Forecasting Challenge ([instructions for registration](https://predict.cdc.gov/api/v1/attachments/aedes challenge 2019/epi_user_instructions.docx)). The forecast submissions will be made using this account. Only one forecast can be submitted for each deadline per account and the same account must be used for all submissions. If teams wish to submit different forecasts (e.g. from different models), they need to use multiple accounts.

Full participation requires:

1. Electronic submission of forecasts for all included counties and months by the respective deadlines (details below and **Evaluation** page).

2. Submission of a model description document by email (details below).

bp[Download registration instructions](https://predict.cdc.gov/api/v1/attachments/aedes challenge 2019/epi_user_instructions.docx)

### Electronic submission

**Forecast format**

Forecasts should be made for each month in csv files matching the format in this [submission template](https://predict.cdc.gov/api/v1/attachments/aedes_challenge_2019/submission_template.csv). Each csv should contain forecasts for all counties and both species, but only for a single month. For internal record keeping, teams may find it useful to include the month in the file name. 

bp[Download forecast submission template](https://predict.cdc.gov/api/v1/attachments/aedes_challenge_2019/submission_template.csv)

The forecast file includes one line for each forecast. That line includes:

* **location**: “State” and “County” as written in the data files with a hyphen: “State-County”. For example, “California-San Diego” or “Connecticut-Fairfield”. Omit the word “County” and include spaces between words within the county or state name. The template provided above should match the state and county fields in the provided surveillance data. 

* **target**: “Ae. aegypti” or “Ae. albopictus”

* **type**: “binary” for all. Indicates that it is a yes or no forecast.

* **unit**: “present” for all. Indicates the forecasts are for the observation of the species. I.e. a forecast of 0.8 indicates 80% chance of being trapped and reported (and 20% chance of not being trapped and reported). 

* **value**: A probability for the observation of a specific species in that particular month and county. The value indicates the probability on a scale from 0 to 1, where 0 is certain absence, 0.5 is an equal chance of absence or presence (50/50), and 1.0 is certain presence). In the template, the values are 0.5 for all species and counties. These should be changed to reflect the forecast of each team. **Note**: when a forecast has high confidence but not absolute certainty, it may be beneficial to assign a very small probability to the unexpected outcome to prevent a very low score should that occur, e.g. 0.999 instead of 1.0 for presence or 0.001 instead of 0 for absence. See the **Evaluation** page for details on scoring.  

**Submission process**

Registered participants will have access to a **Submit** page. The individual csv files can be uploaded on that page any time before the specific deadlines. Take care to match the forecast time frame as there is no built in check for this. The due dates correspond to 11:59 PM EST the day before the forecasted month begins. For example, forecasts for April are due by 11:59 PM EST on March 31 and should be submitted in the row showing that due date. If you do not see the due date, check the “previous submissions” and “future submissions”. Likewise, forecasts for May have the due date April 30. Forecasts may be submitted and updated at any time prior to the due date. Successful submission can be checked by clicking on the “Open JSON” link (the JSON format is a format used by the server). Note that if you are in a different time zone, the date displayed for each deadline may be one day off, but the deadline is still 11:59 PM on the last day of the month in the Eastern Standard Time Zone.
 
### Model description

Each team should select their best model for forecasts and submit a brief model description (details below) by email to aedeschallenge@cdc.gov prior to the first forecast deadline. Teams may update their model during the challenge provided they submit an updated model description. The description should include the following components:
 
1. **Date**
2. **Team name**: This should match the registration name and may be used in forecast visualizations on the website (predict.cdc.gov).
3. **Team members**: List every person involved with the forecasting effort and their institution. Identify a team leader and include the email address of the team leader.
4. **Agreement**: Include the following statement: “By submitting these forecasts, I (we) indicate my (our) full and unconditional agreement to abide by the project's rules and data use agreements.” See the participation agreement below.
5. **Model description** (no more than 400 words): Is the model mechanistic, statistical? Is it an instance of a known class of models? The description should include sufficient detail for another modeler to understand the approach being applied. It may include equations, but that is not necessary. If multiple models are used, describe each model and how they were combined.
6. **Data sources**: What data were used in the model? Historical case data? Weather data? Other data?
7. **Computational resources**: What programming languages/software tools were used to write and execute the forecasts?
8. **Publications**: Does the model derive directly from previously published work? If so please include references.

### Participation agreement

All participants provide consent for their forecasts to be published in real-time on the CDC’s Epidemic Prediction Initiative website (https://predict.cdc.gov/), GitHub page (https://github.com/cdcepi), and, after the season ends, in a scientific journal describing the results of the challenge. The forecasts can be attributed to a team name (e.g., John Doe University) or anonymous (e.g., Team A) based on individual team preference. Team names should be limited to 25 characters for display online. The team name registered with the EPI website will be displayed alongside a team’s forecasts. Any team may publish results from their forecast at any time, but no participating team may publish the results of another team’s model in any form without the team’s consent. Any mosquito surveillance data used should acknowledge the sources of those data as stated on the **Data** page. The manuscript describing the accuracy of forecasts across teams will be coordinated by a representative from CDC.