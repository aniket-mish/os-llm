# Open Source LLMs


## Which LLMs?

1) Open LLM Leaderboard by HuggingFace
2) Chatbot Arena by LMSYS

## Training LLMs

1) Pretraining -> predicting the next word -> to get a base model
2) Supervised finetuning (SFT) -> turn the model into a chatbot -> UltraChat 200k dataset -> TRL library (includes PEFT) or Unsloth -> QLoRA 
3) Human preference training (RLHF) -> make a chatbot friendly, harmless, and helpful -> human chooses a preferred answer from LLMs, so you will have a collection of chosen and rejected pairs -> hh-rlhf dataset -> TRL -> DPO (direct preference optimization) -> DPO combines reward modeling and reinforcement learning -> previously PPO -> https://github.com/huggingface/alignment-handbook


## Deploying LLMs

1) Serverless compute -> chat completion apis -> charged per token -> together.ai
2) Dedicated compute -> TGI (Text Generation Inference), vLLM -> There are inference endpoints (charged not for the amount of data we send but the amount of time we use) from huggingface, together.ai -> can scale down to zero
