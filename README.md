# RobustAlpacaEval

This is the repository for our paper [On the Worst Prompt Performance of Large Language
Models](https://arxiv.org/abs/2406.10248).

In this paper, we introduce a new benchmark, **RobustAlpacaEval**, that encompasses semantically equivalent queries of diverse real-world tasks, offering a more holistic assessment compared to existing benchmarks that focus solely on rephrasing task-level instructions.

RobustAlpacaEval is based on [TinyAlpaceEval](https://github.com/felipemaiapolo/tinyBenchmarks), which is a condensed subset of the [AlpacaEval](https://github.com/tatsu-lab/alpaca_eval) benchmark, created to enable efficient assessment of LLMs. We develop **RobustAlpacaEval** by creating ten paraphrases for each query within TinyAlpacaEval. Each paraphrase is manually reviewed and revised to ensure semantic integrity and human-like fluency.

Please see [our paper](https://arxiv.org/pdf/2406.10248) for more details.



## 🚀 Abstract

The performance of large language models (LLMs) is acutely sensitive to the phrasing of prompts, which raises significant concerns about their reliability in real-world scenarios. Existing studies often divide prompts into task-level instructions and case-level inputs and primarily focus on evaluating and improving robustness against variations in tasks-level instructions. However, this setup fails to fully address the diversity of real-world user queries and assumes the existence of task-specific datasets. To address these limitations, we introduce **RobustAlpacaEval**, a new benchmark that consists of semantically equivalent case-level queries and emphasizes the importance of using the worst prompt performance to gauge the lower bound of model performance. Extensive experiments on **RobustAlpacaEval** with ChatGPT and six open-source LLMs from the Llama, Mistral, and Gemma families uncover substantial variability in model performance; for instance, a difference of 45.48% between the worst and best performance for the Llama-2-70B-chat model, with its worst performance dipping as low as 9.38%. We further illustrate the difficulty in identifying the worst prompt from both model-agnostic and model-dependent perspectives, emphasizing the absence of a shortcut to characterize the worst prompt. We also attempt to enhance the worst prompt performance using existing prompt engineering and prompt consistency methods, but find that their impact is limited. These findings underscore the need to create more resilient LLMs that can maintain high performance across diverse prompts.


## 📁 Dataset
### Data Format

## 📊 Main Results

<img width="709" alt="image" src="https://github.com/user-attachments/assets/b1be8ee6-171d-4c7c-be40-0350ac5ad75b">



## 📜 Key Findings
1. There is a significant gap between the worst performance (lower bound) and best performance
(upper bound) for all models.
2. While scaling up models enhances their ability to follow instructions, it does not correspondingly
increase their robustness.
3. The original performance assessment only provides a narrow perspective of a model’s overall
performance.
4. It is difficult to characterize the worst prompts using either model-independent or model-aware features.



## 📬 Contact

For any questions, feel free to open an issue or contact us directly at [bwcao@link.cuhk.edu.hk].
