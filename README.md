# fastest-llm-apis

Notebook by [Build Fast with AI](https://www.buildfastwithai.com/genai-course)

A simple benchmark comparing the performance of Llama 3.3 70B model across different API providers.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]()

## Providers Tested
- Groq
- Cerebras
- Sambanova

## Metrics Measured
- Tokens per second (generation speed)
- Time to first token (initial latency)
- Total latency
- Token counts (completion & total)

## Results

LLM Performance Comparison:

| Provider | Tokens/sec | First Token | Latency |
|------------|------------|-------------|---------|
| Cerebras | 2,059.9/s | 0.007s | 0.37s |
| Groq | 2,047.2/s | 0.005s | 0.35s |
| Sambanova | 269.0/s | 0.313s | 2.54s |


## Key Findings
- Cerebras leads with the highest tokens/sec at 2,059.9
- Groq and Cerebras have similar first token latency (0.005s)
- Sambanova has higher latency but maintains consistent output
- All providers successfully handle long-form generation

