# AdaSeq: An All-in-One Library for Developing State-of-the-Art Sequence Understanding Models

[![license](https://img.shields.io/github/license/modelscope/adaseq.svg)](./LICENSE)
[![modelscope](https://img.shields.io/badge/modelscope-1.1.0-624aff.svg)](https://modelscope.cn/)
![version](https://img.shields.io/github/tag/modelscope/adaseq.svg)
[![issues](https://img.shields.io/github/issues/modelscope/adaseq.svg)](https://github.com/modelscope/AdaSeq/issues)
[![stars](https://img.shields.io/github/stars/modelscope/adaseq.svg)](https://github.com/modelscope/AdaSeq/stargazers)
[![contribution](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](./CONTRIBUTING.md)


## Introduction
***AdaSeq*** (**A**libaba **D**amo **A**cademy **Seq**uence Understanding Toolkit) is an easy-to-use all-in-one library, built on [ModelScope](https://modelscope.cn/home), that allows researchers and developers to train custom models for sequence understanding tasks, including word segmentation, POS tagging, chunking, NER, entity typing, relation extraction, etc.

![](./docs/imgs/task_examples_en.png)

<details open>
<summary>🌟 <b>Features:</b></summary>

- **State-of-the-Art**: we provide plenty of cutting-edge models, training methods and useful toolkits for sequence understanding tasks.
- **Easy-to-Use**: one line of command is all you need to obtain the best model.
- **Extensible**: easily register new tasks, models, modules, criteria, optimizers, lr_schedulers and training methods.
</details>

⚠️**Notice:** This project is under quick development. This means some interfaces could be changed in the future.

## 📢 What's New
- 2022-11: [[EMNLP 2022] Released NPCRF code](./examples/NPCRF)
- 2022-11: [[EMNLP 2022] Released BABERT models](./examples/babert)

## ⚡ Quick Experience
You can try out our models via online demos built on ModelScope:
[[English NER]](https://modelscope.cn/models/damo/nlp_raner_named-entity-recognition_english-large-news/summary)
[[Chinese NER]](https://modelscope.cn/models/damo/nlp_raner_named-entity-recognition_chinese-base-news/summary)
[[CWS]](https://modelscope.cn/models/damo/nlp_structbert_word-segmentation_chinese-base/summary)

All modelcards we released can be found in this [page](.).

## 🛠️ Model Zoo & Dataset Zoo
<details open>
<summary><b>Supported models:</b></summary>

- [Transformer-based CRF](./examples/bert_crf)
- [Partial CRF](./examples/partial_bert_crf)
- [Retrieval Augmented NER](./examples/RaNER)
- [Global-Pointer](./examples/global_pointer)
- [Multi-label Entity Typing](./examples/entity_typing)
- ...
</details>

<details open>
<summary><b>Supported datasets:</b></summary>

- TODO
</details>


## 📦 Installation
AdaSeq project is based on `Python version >= 3.7` and `PyTorch version >= 1.8`.
```
git clone https://github.com/modelscope/adaseq.git
cd adaseq
pip install -r requirements.txt -f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html
```

## 📖 Tutorials
- [Quick Start](./docs/tutorials/quick_start.md)
- Basics
  - [Learning about Configs](./docs/tutorials/learning_about_configs.md)
  - [Customizing Dataset](./docs/tutorials/customizing_datasets.md)
  - [Common Architectures](./docs/tutorials/common_architectures.md)
  - [TODO] Useful Hooks
  - [Hyperparameter Optimization](./docs/tutorials/hyperparameter_optimization.md)
  - [Training with Multiple GPUs](./docs/tutorials/training_with_multiple_gpus.md)
- Best Practice
  - [Training a Model with Custom Dataset](./docs/tutorials/training_a_model.md)
  - [Reproducing Results in Published Papers](./docs/tutorials/reproducing_papers.md)
  - [TODO] Uploading Saved Model to ModelScope
  - [TODO] Customizing your Model
  - [TODO] Serving with AdaLA

## 📝 Contributing
All contributions are welcome to improve AdaSeq. Please refer to [CONTRIBUTING.md](./CONTRIBUTING.md) for the contributing guideline.

## 📄 License
This project is licensed under the Apache License (Version 2.0).
