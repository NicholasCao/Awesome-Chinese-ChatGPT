# 🧠 Awesome-Chinese-ChatGPT-Implement
收录实现中文版ChatGPT的各种开源技术路线，数据及其他资料

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
![](https://img.shields.io/github/last-commit/NicholasCao/Awesome-Chinese-ChatGPT?color=green)

<img src="assets/chatgpt.jpg" width="44.5%" div align=center /> <img src="assets/chatgpt2.svg" width="45%" div align=center />

Three steps to ChatGPT: 
1. LLM-pretrain
2. Instruction tuning and code continual pretrain
3. RLHF (SFT, RM, PPO-RL)

具体技术可参考 [dalinvip/Awesome-ChatGPT](https://github.com/dalinvip/Awesome-ChatGPT)

## Data
- [Self-instruct](https://github.com/yizhongw/self-instruct)
- [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca)
- [ExpertLLaMA](https://github.com/OFA-Sys/ExpertLLaMA)
- [Evlo-instruct](https://github.com/nlpxucan/evol-instruct)

## 模型
模型更新太快，收录难度较高，提供以下几个榜单作为参考。
- [C-Eval](https://github.com/SJTU-LIT/ceval)
- [Arena](https://chat.lmsys.org/)
- [SuperCLUE](https://github.com/CLUEbenchmark/SuperCLUE); [SuperCLUE琅琊榜](https://www.superclueai.com/)
- [Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)

## 上下文长度
- FlashAttention ([Github](https://github.com/HazyResearch/flash-attention), [Torch 2.0 implementation](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html))
- [Positional Interpolation](https://arxiv.org/pdf/2306.15595.pdf)
- NTK-Aware Scaled RoPE ([Reddit](https://www.reddit.com/r/LocalLLaMA/comments/14lz7j5/ntkaware_scaled_rope_allows_llama_models_to_have/), [Implementation](https://github.com/huggingface/text-generation-inference/issues/512))

## 工具使用
- Toolformer ([Paper](https://arxiv.org/abs/2302.04761), [Implementation](https://github.com/lucidrains/toolformer-pytorch))
- [Toolbench](https://github.com/OpenBMB/ToolBench)
- [Paper List](https://github.com/thunlp/ToolLearningPapers)

## AI Agent
- [Baby AGI](https://github.com/yoheinakajima/babyagi)
- [AutoGPT](https://github.com/Significant-Gravitas/Auto-GPT)
- [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442) 
- [Voyager](https://github.com/MineDojo/Voyager)


## 其他相关开源项目
- [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca): LLAMA-7B SFT
- [Vicuna](https://github.com/lm-sys/FastChat): LLAMA-7b&13B SFT，数据来自ShareGPT
- [Baize](https://github.com/project-baize/baize-chatbot): LLAMA聊天微调，数据采集自ChatGPT self-chat
- [LoRA](https://github.com/microsoft/LoRA): popular低成本LLM参数高效微调方案，已集成到[PEFT](https://github.com/huggingface/peft)


## Contribution
如果你创建或发现了任何关于实现中文ChatGPT的优秀资源，请创建Issue或PR来贡献这个仓库!

If you created or found any awesome resource about Chinese ChatGPT, feel free to create issues or PRs to contribute to this repository!
