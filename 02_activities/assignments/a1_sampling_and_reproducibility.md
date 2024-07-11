# ASSIGNMENT: Sampling and Reproducibility in Python

Read the blog post [Contact tracing can give a biased sample of COVID-19 cases](https://andrewwhitby.com/2020/11/24/contact-tracing-biased/) by Andrew Whitby to understand the context and motivation behind the simulation model we will be examining.

Examine the code in `whitby_covid_tracing.py`. Identify all stages at which sampling is occurring in the model. Describe in words the sampling procedure, referencing the functions used, sample size, sampling frame, any underlying distributions involved, and how these relate to the procedure outlined in the blog post.

Run the Python script file called whitby_covid_tracing.py as is and compare the results to the graphs in the original blog post. Does this code appear to reproduce the graphs from the original blog post?

Modify the number of repetitions in the simulation to 5000 (from the original 50000). Run the script multiple times and observe the outputted graphs. Comment on the reproducibility of the results.

Alter the code so that it is reproducible. Describe the changes you made to the code and how they affected the reproducibility of the script file. The output does not need to match Whitby’s original blogpost/graphs, it just needs to produce the same output when run multiple times

# Author: REN Rihui(Julia)

```
## Q1: Identify all stages at which sampling is occurring

1. Initial Infection Sampling:

- Procedure: **Randomly** selects a subset of individuals to be infected based on the ATTACK_RATE.
- Function: np.random.choice(ppl.index, size=int(len(ppl) * ATTACK_RATE), replace=False)
- Sample Size: Determined by ATTACK_RATE which is set to 0.10 (10% of the total population).
- Sampling Frame: All individuals attending the events (wedding and brunch).

2. Primary Contact Tracing Sampling:

- Procedure: **Randomly** decides which infected individuals get traced based on TRACE_SUCCESS.
- Function: np.random.rand(sum(ppl['infected'])) < TRACE_SUCCESS
- Sample Size: Depends on the number of infected individuals and TRACE_SUCCESS, which is set to 0.20 (20% chance of tracing).
- Sampling Frame: Limited to individuals marked as infected from the previous sampling -- the initial sampling.

3. Secondary Contact Tracing Sampling:

- Procedure: Traces contacts of infected individuals who were successfully traced initially, based on event attendance.
- Function: ppl.loc[ppl['event'].isin(events_traced) & ppl['infected'], 'traced'] = True
- Sample Size: Based on the number of individuals successfully traced in the primary stage and meeting the SECONDARY_TRACE_THRESHOLD (set to 2).
- Sampling Frame: Individuals who attended events that were traced in the primary stage.

4. Post-Simulation Sampling:

- Procedure: After simulating the infection and tracing processes, repeat the entire process for multiple times (1000 iterations), plots histograms of proportions of infections and traces attributed to weddings.
- Function: results = [simulate_event(m) for m in range(5000)]
- Sample Size: 1000 iterations (determined by the range in the simulate_event function).
- Sampling Frame: Proportions calculated from the simulation results.

## Q2: Does this code appear to reproduce the graphs from the original blog post?

- No. The graph looks different from the original blog post.

## Q3: Comment on the reproducibility of the results.
- Without a seed or similar setting, the outputted graphs vary each time when running the script due to lack of reproducibility.

## Q4: Describe the changes you made to the code and how they affected the reproducibility of the script file.

- I implemented two approaches to ensure reproducibility. One way is to set a seed for random number generation. The other way is to save the results of random sampling to disk and generated plots using the same data from disk each time. These two methods achieved the same reproducibility of the generated plots.


```


## Criteria

|Criteria|Complete|Incomplete|
|--------|----|----|
|Altercation of the code|The code changes made, made it reproducible.|The code is still not reproducible.|
|Description of changes|The author explained the reasonings for the changes made well.|The author did not explain the reasonings for the changes made well.|

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `HH:MM AM/PM - DD/MM/YYYY`
* The branch name for your repo should be: `sampling-and-reproducibility`
* What to submit for this assignment:
    * This markdown file (sampling_and_reproducibility.md) should be populated.
    * The `whitby_covid_tracing.py` should be changed.
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/sampling/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `sampling-and-reproducibility`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack at `#cohort-3-help`. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
