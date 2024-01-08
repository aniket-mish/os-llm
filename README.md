# Open Source LLMs


## Which LLMs?

1) Open LLM Leaderboard by HuggingFace
2) Chatbot Arena by LMSYS

## Training LLMs

1) Pretraining -> predicting the next word -> to get a base model
2) Supervised finetuning (SFT) -> turn the model into a chatbot -> UltraChat 200k -> TRL library (includes PEFT) or Unsloth -> QLoRA 
3) Human preference training (RLHF) -> make a chatbot friendly, harmless, helpful
