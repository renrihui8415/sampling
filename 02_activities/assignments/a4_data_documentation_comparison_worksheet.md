# Assignment: Data Documentation Comparison Worksheet

For each of the three sources listed, find any and all available documentation for the data gathered and identify and describe the survey features indicated in the table below. Some may not be available for all sources.

Sources: - Canadian General Social Survey on Giving, Volunteering, and Participating, 2018 (cycle 33), conducted by Statistics Canada - Canadian Election Study Online Survey, 2019, conducted by Laura Stephenson, Allison Harell, Daniel Rubenson and Peter Loewen - Trophic niche flexibility in Glossophaga soricina: how nectar seeker sneaks an insect snack, conducted by Elizabeth Clare et al.

|                                                       | Canadian General Social Survey on Giving, Volunteering, and Participating, 2018 (cycle 33) | Canadian Election Study Online Survey, 2019 | Trophic niche flexibility in Glossophaga soricina: how nectar seeker sneaks an insect snack |
|----------------|-----------------------------------------------|----------------------------------------|--------------------------------------------------------------------------------------------|
| Sample type     | Stratified sampling, combined with random sampling and reject sampling | Stratified sampling and quota sampling | Convenience sampling                                                       |
| Sample size     | 50,000 | Pre-election survey: 37,822; Post-election survey: 10,337 | 1. Dietary Analysis： 38 fecal samples from 112 G. soricina caught by mist nets in the Area de Conservación de Guanacaste, Costa Rica; 2. Behavioural Experiments: 23 synchronized video and call sessions of 5 males and 10 females of G. soricina from a captive colony at the University of Bristol; 3. Model of Maximum Detection Distances: echolocation call intensity from  7 free-flying G. soricina and moths surface area measurements                                     |
| Target population | Canadian residents, aged 15 and over living in private households, excluding residents of the Yukon, Northwest Territories and Nunavut and full time residents of institutions         | Canadian citizens and permanent residents, aged 18 or older    | The Neotropical bat Glossophaga soricina (Pallas, 1766)                                                |
| Sampling frame  | A frame that combines landline and cellular telephone numbers from the Census and various administrative sources with Statistics Canada's dwelling frame | All individuals in the Qualtrics database who meet the criteria for the survey | Locations where Glossophaga soricina bats are found                                        |
| Survey mode(s)  | Electronic questionnaire or CATI (computer assisted telephone interviewing) | Online survey | Field observations and experiments                                                         |
| Timeline        | Every 5 years, from September to December | Campaign Period Survey: September 13th to October 21st, 2019; Post-election survey: October 24th to November 11th, 2019 | 1. Dietary Analysis: 7-week period from late May to early July 2009; 2. Behavioural Experiments: D1–1·5 h on nine consecutive days; 3. Model of Maximum Detection Distances: 7 individual bats flying for up to 2.5 hours                                          |
| Response rate   | 41.9% | Less than 50% | Not applicable in the traditional survey sense                                              |
| Weights         | 1. Basic Weight (WGHT_PER): used for calculating estimates at the individual level; 2. Adjusted Weight: The basic weight is multiplied by a factor to adjust for the proportion of non-volunteers; 3. Adjusted Weight (Income Distribution Adjustment): to ensure that the income distribution matches the 2017 CIS distribution by province; 4. Bootstrap Weights: created using the bootstrap method to estimate sampling error and variance; 5. Non-Response Adjustment Weight: to account for nonresponse, using administrative source data to model and correct for nonresponse bias. | Weight variables are provided; weights must be used to ensure that the data is representative of the population. | Not applicable                                                                               |
| Data processing |  Utilized SSPE set of generalized processing steps and utilities to ensure high-quality outputs| Not mentioned in the documentation | Calculate the average maximum detection distance of the bat and estimate the upper and lower limits of the detection distance using the standard errors of source level, peak frequency, call duration, and target strength                                               |
| Cleaning, imputation, etc. | 1. Imputation Method: Donor Records and Mean Imputation; 2. Imputation steps: personal and family income, formal/informal volunteering variables in the master file, variables in the donation file and the solicitation methods in the master file; 3. Missing income data were obtained by linking to tax data (T1FF) | Incomplete responses, duplicate responses of previous respondents, speeders, those who “straight-lined” grid questions (“straightliners”), and respondents whose postal code didn’t match their province have all been removed from the data file, and are excluded from numbers reported in the documentation. | Not mentioned in the documentation                                             |
| Sources of error | Sampling Error; Non-sampling Error (including Coverage Error, Non-response, response errors and processing errors) | Not mentioned in the documentation | Observation error, environmental variability                                                |
| Limitations, known biases | Non-response bias         | Not mentioned in the documentation  | When building the Model of Maximum Detection Distances: 1. Model Bias: Using the lowest hearing thresholds for moths may bias the model in favor of moths; 2. Threshold Bias: Using the low hearing threshold of Noctua pronuba may lead to overestimation of detection distances for moths; 3. Duration Correction Bias: Adjusting hearing thresholds for shorter call durations may further bias the model towards moths.                                                     |
| Citation        | Statistics Canada. (2018). "Canadian General Social Survey on Giving, Volunteering, and Participating, 2018 (cycle 33)." | Stephenson, Laura B., Allison Harell, Daniel Rubenson and Peter John Loewen. The 2019 Canadian Election Study – Online Collection. [dataset] | Clare, E. L., Goerlitz, H. R., Drapeau, V. A., Holderied, M. W., Adams, A. M., Nagel, J., Dumont, E. R., Hebert, P. D. N., & Fenton, M. B. (2013). Trophic niche flexibility in Glossophaga soricina: How a nectar seeker sneaks an insect snack. Functional Ecology. 10.1111/1365-2435.12192 |
| Links to any documentation or additional sources used | [Statistics Canada](https://www23.statcan.gc.ca/imdb/p2SV.pl?Function=getSurvey&amp;SDDS=4430) | [Canadian Election Study](https://dataverse.harvard.edu/file.xhtml?persistentId=doi:10.7910/DVN/DUS88V/HRZ21G&version=1.0) | [Functional Ecology](https://besjournals.onlinelibrary.wiley.com/doi/full/10.1111/1365-2435.12192)

## Criteria

|Criteria|Complete|Incomplete|
|--------|----|----|
|Population of the data table|The table has been correctly populated from the sources.|The table has been populated, but the information provided is incorrect.|

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `HH:MM AM/PM - DD/MM/YYYY`
* The branch name for your repo should be: `data-documentation`
* What to submit for this assignment:
     * This markdown file (data_documentation_comparison_worksheet.md) should be populated and should be the only change in your pull request.
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/sampling/pull/<pr_id>`
     * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `data-documentation`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack at `#cohort-3-help`. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
