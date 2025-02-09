# DeepSeek Split
## Overview
A utility module designed to separate DeepSeek AI's output into two distinct components: thoughts (internal reasoning enclosed in think tags) and the final answer/response.

## Module Inputs
- **deepseek output**: The complete text output from DeepSeek AI, containing both thought process and final answer

## Module Outputs
- **thoughts**: The extracted internal reasoning/thought process (content between `<think>` tags)
- **answer**: The final response/answer portion of the output (content after the closing `</think>` tag)

## Notes
- Expects DeepSeek output to contain thoughts wrapped in `<think>` tags
- Automatically trims whitespace from both outputs
- Thought process and answer are separated based on the `</think>` tag position
