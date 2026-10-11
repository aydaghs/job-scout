# PROFILE: personal, all projects

## Run mode
Manual only. Run when I type /double-critique or explicitly ask for two critique rounds.
Never run automatically. Otherwise state `two-challenge: exempt` and continue.

## Classes where it applies (when I invoke it)
- Research claims and evaluation results (metrics, comparisons, "X works better than Y")
- Architecture and design decisions for pipelines, agents, or schemas
- Risky code changes: deletes data, touches auth, changes shared interfaces, runs long jobs
- Application material where a wrong claim costs me (CV claims, project descriptions)

## Repo rules a critique must check
- Is every number traceable to a command I can re-run? If not, run it.
- Does the conclusion claim more than the evidence supports (sample size, one dataset, no baseline)?
- What is the rollback if this is wrong?
- Did a fix create a new state no test covers (rule 2b)?

## File location
Write the full history (v1, critique 1, v2, critique 2, v3 FINAL) to
`./critique/<short-name>.md` in the current project. Chat message: v3 summary plus the file path.

## Style
Short sentences. Answer first. No filler. Critiques must name a concrete failure, not "could be clearer".
