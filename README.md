# NorQA

NorQA is a collection of multiple-choice and open-ended question answering (QA) datasets for Norwegian Bokmål and Nynorsk: NorOpenBookQA, NorCommonSenseQA, NorTruthfulQA, and NRK-Quiz-QA. The datasets are designed to evaluate the LM’s Norwegian-specific & world knowledge, common sense reasoning abilities, and truthfulness. The 10.5k question-answer pairs are created by a team of native Norwegian speakers through manual translation and localization of the corresponding English-oriented datasets, with a dedicated effort to also create novel Norwegian-specific examples from scratch.

Read more about our dataset creation method, general statistics, and empirical evaluation results in our paper.


## 🤗 HuggingFace

Our datasets are available via the HuggingFace datasets:

- [NRK-Quiz-QA](https://huggingface.co/datasets/ltg/nrk_quiz_qa)
- [NorOpenBookQA](https://huggingface.co/datasets/ltg/noropenbookqa)
- [NorCommonSenseQA](https://huggingface.co/datasets/ltg/norcommonsenseqa)
- [NorTruthfulQA (Multiple Choice)](https://huggingface.co/datasets/ltg/nortruthfulqa_mc)
- [NorTruthfulQA (Generation)](https://huggingface.co/datasets/ltg/nortruthfulqa_gen)

## 🤖 Evaluation

We utilize the [```NorEval```](https://github.com/ltgoslo/noreval/) framework for evaluating Norwegian generative language models. All our datasets are integrated into ```NorEval```, along with a pool of 50 prompts in both Bokmål and Nynorsk designed to represent diverse user requests and answer formats. Please refer to the framework documentation on how to evaluate a model on our datasets.

## 👥 Annotation guidelines

We publicly release our [annotation guidelines](./guidelines/) that are used to create the datasets. The guidelines are tailored to each dataset.

- [Adaptation of NRK-Quiz-QA](./guidelines/nrk_quiz_qa.pdf)
- [Creation of NorOpenBookQA and NorCommonSenseQA](./guidelines/noropenbookqa_and_norcommonsenseqa.pdf)
- [Creation of NorTruthfulQA (Multiple Choice and Generation)](./guidelines/nortruthfulqa.pdf)
- [Data Curation](./guidelines/curation.pdf)

## 🔗 Cite us

```
@article{mikhailov2025collection,
  title={A Collection of Question Answering Datasets for Norwegian},
  author={Mikhailov, Vladislav and M{\ae}hlum, Petter and Lang{\o}, Victoria Ovedie Chruickshank and Velldal, Erik and {\O}vrelid, Lilja},
  journal={arXiv preprint arXiv:2501.11128},
  year={2025}
}
```