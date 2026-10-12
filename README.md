# WebOperator Experiments: trajectory viewers

Step-by-step trajectory viewers for WebOperator runs (gpt-4o), browsable on GitHub Pages.
Screenshots are loaded from the dataset on Hugging Face.

**All run data** (search trees, logs, trajectories, evaluations, configs, screenshots and
analysis scripts) is on Hugging Face:
https://huggingface.co/datasets/mahirlabibdihan/weboperator-experiments

| Benchmark | Viewers |
|---|---|
| WebArena (812 tasks) | [`webarena/main/`](webarena/main/) |
| WebArena-lite ablation study (155 tasks, 10 runs) | [`webarena-lite/ablations/`](webarena-lite/ablations/) |

Viewer URL pattern:

```
https://mahirlabibdihan.github.io/WebOperator-Experiments/<benchmark>/tasks/task_<id>/trajectory.html
```
