# CKYC SFTP Log Investigation

## Context

You are supporting an SFTP-based CKYC integration. Over the last few weeks, some customers reported failed transfers and inconsistent behavior. You have been given one anonymized request-level log extract and asked to investigate what happened.

Dataset provided:

- `ckyc.SFTPConnectionLog.anonymized.csv`

Your task is to analyze the dataset and explain the most important patterns, risks, and likely causes.

## Questions

1. What are the main failure patterns in this dataset? Break them down by customer, operation, and error type.
2. Which issues appear customer-specific, and which look more system-wide? Explain the evidence for your conclusion.
3. Identify any major change points over time. What changed, when did it change, and how confident are you?
4. Compare system behavior before and after the biggest change point you identify. Focus on request volume, operation mix, success rate, and error composition.
5. Do the logs suggest the failures were caused only by permission or configuration issues, or is there evidence of an operational pattern contributing to the problem? Defend your answer from the data.
6. Is there evidence that the way the client interacted with the SFTP system changed over time? If yes, describe the likely change and the impact it had.
7. Which customers appear most impacted, and how would you quantify impact fairly? Do not rely on raw failure counts alone.
8. If you had to explain the incident to an engineering manager, what would be your most plausible incident narrative, including timeline, likely mechanism, evidence, and uncertainty?
9. What metrics, alerts, or monitoring would you add so this problem is detected earlier next time?
10. What assumptions did you make, and what additional data would you request before making a final recommendation?

## Deliverables

- Your analysis in SQL, Python, notebook, spreadsheet, or any equivalent format
- A short write-up, 1 to 2 pages max
- At least one chart or table that supports your main conclusion
- A prioritized action plan

## What We Care About

We are not looking only for query writing. We care about:

- analytical thinking
- ability to work with messy operational data
- quality of reasoning
- clarity of communication
- ability to separate evidence from inference
- practical recommendations

## Notes

- You may use AI tools if you want.
- Be explicit about assumptions.
- If you think the data is insufficient to prove a conclusion, say so clearly and explain what would strengthen it.
