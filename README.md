# fastest-llm-apis

A package to explore the fastest LLM APIs from Groq, Cerebras, and Sambanova

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]()

A simple benchmark comparing the performance of Llama 3.3 70B model across different API providers.

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
| Provider   | Tokens/sec | First Token | Latency |
|------------|------------|-------------|---------|
| Groq       | 1,734.4/s  | 0.005s     | 0.72s   |
| Cerebras   | 1,678.9/s  | 0.005s     | 1.01s   |
| Sambanova  | 323.5/s    | 0.212s     | 4.33s   |


## Key Findings
- Groq leads with the highest tokens/sec at 1,734.4
- Groq and Cerebras have similar first token latency (0.005s)
- Sambanova has higher latency but maintains consistent output
- All providers successfully handle long-form generation

