<div align="center">
  <h1> NovelQA </h1>
  
  ![Data Version](https://img.shields.io/badge/Data%20Version-1.0.0-blue.svg?style=for-the-badge&logo=appveyor)
  [![License: Apache-2.0](https://img.shields.io/crates/l/Ap?style=for-the-badge)](https://opensource.org/licenses/Apache-2.0)
  [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=for-the-badge)](https://github.com/NovelQA/novelqa.github.io/issues)
</div>

# 📌 Table of Contents
- [📌 Table of Contents](#-table-of-contents)
- [🚀 Introduction](#-introduction)
- [📝 Dataset](#-dataset)
  - [Data Description](#data-description)
  - [Data Scale](#data-scale)
- [🏆 Evaluation \& Submission](#-evaluation--submission)
- [📜 License](#-license)
- [📚 Citation](#-citation)
  - [📮 Contact](#-contact)
  - [Acknowledgement](#acknowledgement)
  
# 🚀 Introduction
  Welcome to our GitHub repository for the "Evaluating Open-QA Evaluation" [paper](https://arxiv.org/abs/2305.12421), a comprehensive study on the evaluating of evaluation methods in Open Question Answering (Open-QA) systems.
  
  Open-QA systems, which generate answers to questions with a vast range of possible topics, have become an increasingly significant research field in recent years. However, accurately evaluating these systems remains challenging, and currently lacks robust, reliable methods.
  
  In response to this, we introduce the QA Evaluation task (QA-Eval), a new task that rigorously tests various evaluation methods for their ability to accurately assess the relevance of machine-generated answers to a set of gold standard answers within an Open-QA context. This task requires the evaluating method to discern whether a machine-generated answer aligns with the gold standard answer, with performance evaluated against human-annotated results.
  
  We sourced our data from the test sets of two well-established QA datasets, Natural Questions (NQ) and TriviaQA. We ask several representative models, including FiD, ChatGPT-(3.5/4), GPT-3.5 and BingChat, to answer the questions. We then manually annotated the correctness of each question-answer pair.
  
  Through this work, we hope to foster a deeper understanding of Open-QA systems, their evaluations, and aid the research community in developing more reliable automatic evaluation tools.
  
# 📝 Dataset
  ## Data Description
  
  Each data point in our dataset is represented as a dictionary with the following keys:
```

```
  Here is an example of a data point:
```json

```
  ## Data Scale
  The scale of our dataset is detailed in the table below:
  
 |models | Natural Questions| TriviaQA |
 |------------------------------|------------------------------|------------------------------|
 |DPR+FiD |3610|2000|
 |GPT-3.5 |3610|2000|
 |ChatGPT-3.5 |3610|2000|
 |ChatGPT-4 |3610|2000|
 |Bing Chat |3610|2000|
 
# 🏆 Evaluation & Submission


  The work flow of our online benchmark is as follows. 

```mermaid

graph LR

    A[[🤗 Huggingface]]  --(Input Data)--> B[[🤖Your Model]]
    B --(Model output)--> C[[⚖️Codabench]]
    C --(Accuracy Score)--> D[[🗳️Google Form]]
    D ----> E[[🏆Leaderboard Website]]

```

# 📜 License

This dataset is released under the [Apache-2.0 License](LICENSE).

# 📚 Citation

If you use this dataset in your research, please cite it as follows:
```bibtex

```
## 📮 Contact
We welcome contributions to improve this dataset! 
If you have any questions or feedback, please feel free to reach out at wangcunxiang@westlake.edu.cn.

## Acknowledgement

This leaderboard adopts the style of [bird-bench](https://github.com/bird-bench/bird-bench.github.io).

[Official Site](https://novelqa.github.io/)