# WebArena-lite ablation study (gpt-4o): trajectory viewers

Open a task's trajectory at

`https://mahirlabibdihan.github.io/WebOperator-Experiments/webarena-lite/ablations/<row>/tasks/task_<id>/trajectory.html`

For example, task 58 of the full system:
https://mahirlabibdihan.github.io/WebOperator-Experiments/webarena-lite/ablations/12-snapshot-validated-backtracking/tasks/task_58/trajectory.html

| Row | Ablation | `<row>` | SR (%) |
|---|---|---|---|
| 1 | Base ReAct Agent | `01-base-react` | 47.74 |
| 2 | + Dynamic Action Space | `02-dynamic-action-space` | 49.03 |
| 3 | + Action Validation | `03-action-validation` | 53.55 |
| 4 | + Multi-Action | `04-multi-action` | 52.90 |
| 5 | + Action Merging | `05-action-merging` | 54.19 |
| 6 | + Context Variation | `06-context-variation` | 54.84 |
| 7 | + Naive Tree Search | `07-naive-tree-search` | 51.61 |
| 8 | + Checkpoints\* | (derived from row 7) | 51.61 |
| 9 | + Re-rooting | `09-re-rooting` | 51.61 |
| 10 | + Destructive-Action Deferral\* | (derived from row 11) | 56.77 |
| 11 | + Terminating-Action Handling | `11-terminating-action-handling` | 58.71 |
| 12 | + Snapshot-Validated Backtracking | `12-snapshot-validated-backtracking` | **60.00** |

\*Rows 8 and 10 are derived offline from existing runs and have no trajectories of their own.

Run data, full result tables and the analysis scripts:
https://huggingface.co/datasets/mahirlabibdihan/weboperator-experiments/tree/main/webarena-lite
