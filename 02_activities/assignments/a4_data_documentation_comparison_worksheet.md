# Assignment: Data Documentation Comparison Worksheet

For each of the three sources listed, find any and all available documentation for the data gathered and identify and describe the survey features indicated in the table below. Some may not be available for all sources.

Sources: - Canadian General Social Survey on Giving, Volunteering, and Participating, 2018 (cycle 33), conducted by Statistics Canada - Canadian Election Study Online Survey, 2019, conducted by Laura Stephenson, Allison Harell, Daniel Rubenson and Peter Loewen - Trophic niche flexibility in Glossophaga soricina: how nectar seeker sneaks an insect snack, conducted by Elizabeth Clare et al.

|                                                       | Canadian General Social Survey on Giving, Volunteering, and Participating, 2018 (cycle 33) | Canadian Election Study Online Survey, 2019 | Trophic niche flexibility in Glossophaga soricina: how nectar seeker sneaks an insect snack |
|----------------|-----------------------------------------------|----------------------------------------|--------------------------------------------------------------------------------------------|
| Sample type     | Stratified sampling, combined with random sampling and reject sampling | Stratified sampling and quota sampling | Sample of Glossophaga soricina bats                                                         |
| Sample size     | 50,000 | Pre-election survey: 37,822; Post-election survey: 10,337 | Specific to the study, usually indicated in the paper                                        |
| Target population | Canadian residents, aged 15 and over living in private households, excluding residents of the Yukon, Northwest Territories and Nunavut and full time residents of institutions         | Canadian citizens and permanent residents, aged 18 or older    | Glossophaga soricina bats in specific regions                                                |
| Sampling frame  | A frame that combines landline and cellular telephone numbers from the Census and various administrative sources with Statistics Canada's dwelling frame | All individuals in the Qualtrics database who meet the criteria for the survey | Locations where Glossophaga soricina bats are found                                         |
| Survey mode(s)  | Electronic questionnaire or CATI (computer assisted telephone interviewing) | Online survey | Field observations and experiments                                                         |
| Timeline        | Every 5 years, from September to December | Campaign Period Survey: September 13th to October 21st, 2019; Post-election survey: October 24th to November 11th, 2019 | Duration of field study, specific to the research                                           |
| Response rate   | 41.9% | Less than 50% | Not applicable in the traditional survey sense                                              |
| Weights         | 1. Basic Weight (WGHT_PER): used for calculating estimates at the individual level; 2. Adjusted Weight: The basic weight is multiplied by a factor to adjust for the proportion of non-volunteers; 3. Adjusted Weight (Income Distribution Adjustment): to ensure that the income distribution matches the 2017 CIS distribution by province; 4. Bootstrap Weights: created using the bootstrap method to estimate sampling error and variance; 5. Non-Response Adjustment Weight: to account for nonresponse, using administrative source data to model and correct for nonresponse bias. | Weight variables are provided; weights must be used to ensure that the data is representative of the population. | Not applicable                                                                               |
| Data processing |  Utilized SSPE set of generalized processing steps and utilities to ensure high-quality outputs| Not mentioned in the documentation | Detailed methods of observation and analysis                                               |
| Cleaning, imputation, etc. | 1. Imputation Method: Donor Records and Mean Imputation; 2. Imputation steps: personal and family income, formal/informal volunteering variables in the master file, variables in the donation file and the solicitation methods in the master file; 3. Missing income data were obtained by linking to tax data (T1FF) | Incomplete responses, duplicate responses of previous respondents, speeders, those who “straight-lined” grid questions (“straightliners”), and respondents whose postal code didn’t match their province have all been removed from the data file, and are excluded from numbers reported in the documentation. | Cleaning methods and data treatment described                                              |
| Sources of error | Sampling Error; Non-sampling Error (including Coverage Error, Non-response, response errors and processing errors) | Not mentioned in the documentation | Observation error, environmental variability                                                |
| Limitations, known biases | Non-response bias         | Not mentioned in the documentation  | Specific to study conditions and methods                                                     |
| Citation        | Statistics Canada. (2018). "Canadian General Social Survey on Giving, Volunteering, and Participating, 2018 (cycle 33)." | Stephenson, Laura B., Allison Harell, Daniel Rubenson and Peter John Loewen. The 2019 Canadian Election Study – Online Collection. [dataset] | Clare, E., et al. (Year of publication). "Trophic niche flexibility in Glossophaga soricina: how nectar seeker sneaks an insect snack." |
| Links to any documentation or additional sources used | [Statistics Canada](https://www23.statcan.gc.ca/imdb/p2SV.pl?Function=getSurvey&amp;SDDS=4430) | [Canadian Election Study](https://dataverse.harvard.edu/file.xhtml?persistentId=doi:10.7910/DVN/DUS88V/HRZ21G&version=1.0) | Typically accessed via academic journals or databases                                      |

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
