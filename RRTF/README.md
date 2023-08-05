# Rank Responses to align Test & Teacher Feedback (RRTF)

1. leverages preferences to align LLMS without the complexity of PPO
2. **Uses ranking rather than rewards to guide models.**
3. Three-step framework - sampling, ranking (test), and training.
4. Sampling: Responses are sampled with prompts generated via Evol-Instruct.
5. Ranking: Results are ranked by running unit tests and filtering via heuristics. (not included)
6. Training: Train Student on Triplets of Inputs + chosen/rejected + score using ranking loss
7. Built on 15B parameter StarCoder.
8. Trained on 68K Evol-Instruct problems
9. Achieves SOTA 62.20% on HumanEval
10. Still a gap between Code LLMs (< 15B) and LLMs like GPT-4 ( > 100B).

![image](https://github.com/DrishtiShrrrma/LLMs/assets/129742046/cbd71602-e8d6-46d4-b48b-61f78e3d84df)
