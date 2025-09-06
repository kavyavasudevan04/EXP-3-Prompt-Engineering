# EXP-3-PROMPT-ENGINEERING-

## Aim: 
Evaluation of 2024 Prompting Tools Across Diverse AI Platforms: 
ChatGPT, Claude, Bard, Cohere Command, and Meta
Experiment:
Within a specific use case (e.g., summarizing text, answering technical questions), compare the performance, user experience, and response quality of prompting tools across these different AI platforms.

## Algorithm:

High-level pseudocode
```
for each example in dataset:
    for each prompt_pattern in [zero_shot, few_shot, cot, self_consistency, role, rag]:
        for each platform in platforms:
            request = build_prompt(platform, prompt_pattern, example)
            response, metadata = call_platform_api(platform, request)
            save_response(example_id, platform, prompt_pattern, response, metadata)

### After collection:
compute_auto_metrics(all_responses)
collect_human_ratings(sample_of_responses)
compute_human_metrics()
run_statistical_tests()
generate_plots_and_tables()
```

Algorithm details (reproducible)

Standardize prompt templates (exact same wording across platforms, except where a platform requires a system role vs prompt body).

Control sampling hyperparameters: temperature, top_p/top_k, max_tokens, stop tokens. If a platform does not expose the same settings, choose closest equivalent. Document differences.

Caching: store raw responses and metadata; do not re-query live systems for reproducibility unless necessary.

Human eval: randomize order to prevent rater bias and blind raters to which platform produced which response.

## Prompt
### Chat GPT
Explain detailly about neural network for a beginner, why it is used, how it is used ,what are the future trends of it, advantages,disadvantages,applications explain clearly for a beginner
### Mata AI
Explain the architecture of a Convolutional Neural Network (CNN). Describe how convolution, pooling, and fully connected layers work together for image classification, and provide a simple example with diagrams or pseudocode.
### Claude
Explain how gradient descent works in training a neural network. Include the mathematical formula, an intuitive explanation for beginners, and a simple Python pseudocode example.
### Gemini AI
Explain the difference between supervised, unsupervised, and reinforcement learning in machine learning. Provide real-world examples for each, and summarize the key differences in a comparison table.

## Output
### Chat GPT
<img width="982" height="738" alt="image" src="https://github.com/user-attachments/assets/2e006e8e-496c-4b24-a413-ad2ece7dc2d0" />

### Meta AI
<img width="713" height="755" alt="image" src="https://github.com/user-attachments/assets/f364cc1e-17a0-4efa-9221-3bbe3f7a51cc" />

### Claude
<img width="850" height="623" alt="image" src="https://github.com/user-attachments/assets/68350dba-d964-4d24-87c9-0654deec61d8" />

### Gemini AI
<img width="960" height="597" alt="image" src="https://github.com/user-attachments/assets/2c2a6ef1-3ff7-4c39-9daa-dfc91e4ff622" />






## Result
Thus, the experiment demonstrated that the performance and response quality of prompting tools vary significantly across platforms and prompting patterns.

