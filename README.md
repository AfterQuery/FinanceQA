# FinanceQA: A Benchmark for Evaluating Financial Analysis Capabilities of Large Language Models

#### 📄 Read the paper [here](https://github.com/AfterQuery/FinanceQA/blob/main/Finance%20QA.pdf)
#### 🤗 Check out our eval on Hugging Face [here](https://huggingface.co/datasets/AfterQuery/FinanceQA)

[FinanceQA](https://github.com/AfterQuery/FinanceQA/blob/main/Finance%20QA.pdf) is a comprehensive testing suite designed to evaluate LLMs' performance on complex financial analysis tasks that mirror real-world investment work. The dataset aims to be substantially more challenging and practical than existing financial benchmarks, focusing on tasks that require precise calculations and professional judgment.

![Results](https://github.com/AfterQuery/FinanceQA/blob/main/FinanceQA/results_img.png)

**Abstract:** FinanceQA is a testing suite that evaluates LLMs’ performance on complex numerical financial analysis tasks that mirror real-world investment work. Despite recent advances, current LLMs fail to meet the strict accuracy requirements of financial institutions, with models failing approximately 60% of realistic tasks that mimic on-the-job analyses at hedge funds, private equity firms, investment banks, and other financial institutions. The primary challenges include hand-spreading metrics, adhering to standard accounting and corporate valuation conventions, and performing analysis under incomplete information - particularly in multi-step tasks requiring assumption generation. This performance gap highlights the disconnect between existing LLM capabilities and the demands of professional financial analysis that are inadequately tested by current testing architectures. Results show that higher-quality training data is needed to support such tasks, which we experiment with using OpenAI’s fine-tuning API. FinanceQA is publicly released at https://huggingface.co/datasets/AfterQuery/FinanceQA.


### Description

The dataset contains two main categories of questions:
1. <ins>Tactical Questions</ins>: Questions based on financial documents that test calculation accuracy, accounting standards, assumption-making, and real-world practices.
   - Basic questions 
   - Assumption-based questions (requiring inference with incomplete information)

2. <ins>Conceptual Questions</ins>: Questions testing understanding of financial relationships, logical derivations, industry estimations, and accounting principles.

### Fields

The dataset contains the following components:
* `context`: Relevant sections from primary financial documents (e.g., 10-K sections)
* `question`: The specific financial analysis task or query
* `answer`: The correct calculation or response
* `chain_of_thought`: The reasoning logic to arrive at the correct answer
* `question_type`: Categorization as either "basic", "assumption", or "conceptual"
* `company`: The company in question
* `file_link`: The link to the source of the context field
* `file_name`: The file name of the source of the context field

### Hugging Face
[Link](https://huggingface.co/datasets/AfterQuery/FinanceQA)
