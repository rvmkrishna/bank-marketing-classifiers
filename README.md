# Bank telemarketing | Comparing classifiers

[Open the analysis notebook](comparing_classifiers.ipynb)

## Campaign findings

K-nearest neighbors led expanding-window validation (mean AP 0.075). On 8,238 later records its AP was 0.487, against a constant-score baseline of 0.308. Calling the first 824 ranked records would have reached 63.1% subscribers per call versus 30.8% under random priority, or 2.05 times the expected yield. This list captured 20.5% of observed subscribers.

Pilot the ranked list against random priority at equal call capacity. Track subscriptions per 100 calls, agent time, opt-outs and net margin. Validate across new months and customer groups. Use a randomized no-call group to measure incremental subscriptions before expanding the campaign.

## Reproduce

Install requirements.txt, open the notebook from the repository root and run all cells. It reads bank-additional-full.csv locally or downloads the UCI archive. The last cell updates this summary.

Source: [UCI Bank Marketing](https://archive.ics.uci.edu/dataset/222/bank+marketing), Moro, Cortez and Rita.
