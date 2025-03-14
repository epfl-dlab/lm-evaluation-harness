# JSONSchema Bench

## Tasks

- `jsonschema_bench_easy`, corresponding to the `github_easy` split of the original paper
- `jsonschema_bench_medium`, corresponding to the `github_medium` split of the original paper
- `jsonschema_bench_hard`, corresponding to the `github_hard` split of the original paper

Use `jsonschema_bench` tag to run all three tasks.

## ⚠️  Context Window Size
The `easy` task requires a context window of 4K tokens, the `medium` task requires a context window of 28K tokens, and the `hard` task requires a context window of 32K tokens.

If you don't have enough memory to run the `hard` task, you can use the `--max_length` flag to reduce the context window size but this will truncate the schema and will lead to lower performance.

## Paper

JSONSchemaBench: A Rigorous Benchmark of Structured Outputs for Language Models[https://arxiv.org/abs/2501.10868v3]

Homepage: https://github.com/guidance-ai/jsonschemabench


## Citation
```
@misc{geng2025jsonschemabenchrigorousbenchmarkstructured,
      title={JSONSchemaBench: A Rigorous Benchmark of Structured Outputs for Language Models}, 
      author={Saibo Geng and Hudson Cooper and Michał Moskal and Samuel Jenkins and Julian Berman and Nathan Ranchin and Robert West and Eric Horvitz and Harsha Nori},
      year={2025},
      eprint={2501.10868},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2501.10868}, 
}
```



### Checklist

For adding novel benchmarks/datasets to the library:
* [x] Is the task an existing benchmark in the literature?
  * [x] Have you referenced the original paper that introduced the task?
  * [x] If yes, does the original paper provide a reference implementation? If so, have you checked against the reference implementation and documented how to run such a test?


If other tasks on this dataset are already supported:
* [ ] Is the "Main" variant of this task clearly denoted?
* [ ] Have you provided a short sentence in a README on what each new variant adds / evaluates?
* [ ] Have you noted which, if any, published evaluation setups are matched by this variant?
