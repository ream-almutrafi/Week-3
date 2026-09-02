# Model lock (team record)

## The locked model

- Model id: Qwen/Qwen2.5-1.5B-Instruct-AWQ
- Quantisation: awq
- Why this one: Passed function-calling smoke test, holds full quality against fp16, and grants larger KV-cache block allocation.

## The launch flags

- Tool-call parser: hermes

## The smoke score

- Score (valid behaviours out of 10): 10
- Distractor stayed call-free in the majority: yes
- Passed the gate (>= 8/10 and distractor majority clean): yes
- Measured against: AWQ

## Quality spot check note

- The 4-bit AWQ build showed no perceptible text output degradation on any of the five test prompts compared to the baseline fp16 outputs.
