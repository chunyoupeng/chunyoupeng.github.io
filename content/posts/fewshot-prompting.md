# Few-Shot LLM

## Summary

Summarize the papers in this section. You should not simply list the reviewed papers. A good practice is to discuss the
connections between them, e.g., paper 1 proposes a xxx method, which solves xxx problems, but it cannot do xxx; while paper 2 improves paper 1’s theory/algorithm/approach/dataset, and it can solve xxx problems, and thus it can achieve xxx
effect. But there are still some other limitations, e.g., xxx and xxx. Paper 3 has proposed xxx, and it addresses the limitations
of paper 2. When referencing contents from the papers, e.g., putting a screenshot of paper’s figures or tables in your review paper (as shown in Figure 1), you should clearly write some text like this ”the table/figure is obtained from [2]” in the figure/table’s caption, otherwise it is plagiarism.

Brown et al. (2020) demonstrated that increasing the scale of language models significantly enhances their performance and efficiency in sample usage, leading to the widespread adoption of few-shot prompting techniques. However, this approach exhibits limitations in tasks requiring advanced reasoning skills and shows marginal improvements with larger model scales, as observed by Wei et al. (2022). To address these shortcomings, Wei et al. (2022) integrated previous methodologies that enable models to articulate intermediate steps in natural language, as initially proposed by Ling et al. (2017), with Brown’s few-shot prompting, achieving superior results compared to conventional prompting strategies. Despite these advances, the approach necessitates labor-intensive fine-tuning and complex sample engineering, a challenge highlighted by Kojima et al. (2023). Kojima and colleagues propose a novel solution to this issue by incorporating a straightforward prompting strategy, "Let's think step by step," effectively overcoming the previously mentioned constraints without the need for extensive tuning or sample manipulation.


## Results
Describe the paper’s experimental results (both quantitative and qualitative). What methods does this paper compare with?
Can the results support the paper’s claim? Do you find any inspiration from the results in Table 1?


In the study of problem-solving capabilities across various methodologies applied to the GSM8K dataset, we observe a gradation in performance contingent upon the complexity and sophistication of the prompting strategies employed. Initially, the Few-shot prompting approach, as delineated by Cobbel et al. in 2021, demonstrated a modest success rate of 18%, underscoring the challenges inherent in leveraging limited examples to guide model inference. Contrastingly, the Chain of Thought (CoT) prompting paradigm marked a substantial improvement, achieving a 57% problem-solving rate. This method benefits from its ability to mimic a more natural problem-solving process, sequentially breaking down complex tasks into manageable steps.

Notably, the Zero-Shot-CoT technique, innovated by Kojima et al. in 2023, has significantly advanced the field by achieving a 70.1% success rate on the same GSM8K dataset. This method stands out not only for its effectiveness but also for its simplicity and efficiency. It eschews the need for extensive sample engineering, a process often characterized by its resource-intensive nature. Instead, Zero-Shot-CoT relies on a simple yet powerful modification: the inclusion of a prompt that encourages a step-by-step analytical approach. By instructing the model to "Let's think step by step," it fosters a more deliberate and structured exploration of the problem space, thus enhancing the model's ability to derive solutions. This innovation represents a significant leap forward in our pursuit of more adept and efficient problem-solving methodologies within the realm of artificial intelligence.

## Contributions
Summarize the theoretical, experimental or dataset contributions of the papers. Usually you can find a contribution list at the end of a paper’s introduction section. But do not copy and paste it 

Brown et al.(2020) demonstrates that large language models, specifically GPT-3, can perform a wide range of tasks with minimal task-specific training data, often just a few examples. This is a significant departure from traditional models that require extensive fine-tuning on large datasets for each new task.

Wei et al.(2022) introduces the Chain-of-Thought prompting technique that guide the language model to articulate its reasoning step-by-step, much like a human would when solving complex problems. This is a shift from traditional prompting methods that typically aim for the shortest possible path to a correct answer.

Kojima et al.(2023) demonstrates that large language models possess an inherent ability to perform zero-shot reasoning. This means that these models can tackle novel tasks or answer questions they weren't explicitly trained on, without needing any additional fine-tuning or examples.

## Critiques

While LLMs can perform impressively across a range of tasks without specific training (zero-shot), their performance can be inconsistent. They might excel in some areas but perform poorly in others, particularly in tasks requiring deep domain-specific knowledge or nuanced understanding. Second, the Zero-Shot-CoT prompting method is so simple that it's suspect of being filler.



