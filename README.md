# NanoGPT curriculum experiment

An attempt to use the process in https://arxiv.org/pdf/2310.09518.pdf, Instruction Tuning with Human Curriculum 

## how does it work?

 - take a curriculum/content dataset
 - sep. it all into the different topics
 - generate questions, then filter it from easy to hard

to use this approach the plan is

a. bulid an eval setup with common benchmarks for gpt-2, acc/acc_norm

b. train 2 models
    - gpt 2 small with random shuffled oh-2.5
    - gpt 2 small with an oh-2.5 filtered through with this method

c. check loss plots, perf. etc?

## citations
```
@misc{lee2024instruction,
      title={Instruction Tuning with Human Curriculum}, 
      author={Bruce W. Lee and Hyunsoo Cho and Kang Min Yoo},
      year={2024},
      eprint={2310.09518},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```