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
@inproceedings{mikhailov-etal-2025-collection,
    title = "A Collection of Question Answering Datasets for {Norwegian}",
    author = "Mikhailov, Vladislav  and
      M{\ae}hlum, Petter  and
      Lang{\o}, Victoria Ovedie Chruickshank  and
      Velldal, Erik  and
      {\O}vrelid, Lilja",
    editor = "Johansson, Richard  and
      Stymne, Sara",
    booktitle = "Proceedings of the Joint 25th Nordic Conference on Computational Linguistics and 11th Baltic Conference on Human Language Technologies (NoDaLiDa/Baltic-HLT 2025)",
    month = mar,
    year = "2025",
    address = "Tallinn, Estonia",
    publisher = "University of Tartu Library",
    url = "https://aclanthology.org/2025.nodalida-1.43/",
    pages = "397--407",
    ISBN = "978-9908-53-109-0",
    abstract = "This paper introduces a new suite of question answering datasets for Norwegian; NorOpenBookQA, NorCommonSenseQA, NorTruthfulQA, and NRK-Quiz-QA. The data covers a wide range of skills and knowledge domains, including world knowledge, commonsense reasoning, truthfulness, and knowledge about Norway. Covering both of the written standards of Norwegian {--} Bokm{\r{a}}l and Nynorsk {--} our datasets comprise over 10k question-answer pairs, created by native speakers. We detail our dataset creation approach and present the results of evaluating 11 language models (LMs) in zero- and few-shot regimes. Most LMs perform better in Bokm{\r{a}}l than Nynorsk, struggle most with commonsense reasoning, and are often untruthful in generating answers to questions. All our datasets and annotation materials are publicly available."
}
```
