---
base_model: pretrain/telechat-7b
library_name: peft
license: other
tags:
- llama-factory
- lora
- generated_from_trainer
model-index:
- name: sft_3
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# sft_3

This model is a fine-tuned version of [pretrain/telechat-7b](https://huggingface.co/pretrain/telechat-7b) on the cmmlu dataset.
It achieves the following results on the evaluation set:
- Loss: 0.9523

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 0.0001
- train_batch_size: 16
- eval_batch_size: 1
- seed: 42
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: cosine
- lr_scheduler_warmup_ratio: 0.1
- num_epochs: 3.0
- mixed_precision_training: Native AMP

### Training results

| Training Loss | Epoch  | Step | Validation Loss |
|:-------------:|:------:|:----:|:---------------:|
| 0.0157        | 2.9806 | 2000 | 0.9524          |


### Framework versions

- PEFT 0.12.0
- Transformers 4.44.0
- Pytorch 2.3.1+cu121
- Datasets 2.20.0
- Tokenizers 0.19.1