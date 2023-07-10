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

- [BELLE指令微调数据集](https://github.com/LianjiaTech/BELLE/tree/main/1.5M)(1.5M)
- [BELLE10M中文数据集](https://github.com/LianjiaTech/BELLE/tree/main/10M), 包含0.25M数学指令数据集和0.8M多轮任务对话数据集
- [InstructionWild](https://github.com/XueFuzhao/InstructionWild): Colossal AI 收集的中英双语数据集(104K)
- [GPT-4-LLM](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM): GPT-4标注的中英双语指令微调数据，prompt来自[Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca)。
- [ShareGPT](https://sharegpt.com/): ChatGPT用户分享的聊天数据，大部分为英文数据，插件维护者目前已经关闭了公开获取数据的接口。
- [CAMEL](https://github.com/lightaime/camel#data-hosted-on-hugging-face): 对话式指令跟随数据集，并将英文数据翻译到10种包含中文的不同语言。
- [OASST1](https://huggingface.co/datasets/OpenAssistant/oasst1): OpenAssistant Conversations，一个人工生成的、人工注释的助理式对话语料库，由 35 种不同语言的 161,443 条消息组成。包含少量中文语料。

## 模型

- [BELLE](https://github.com/LianjiaTech/BELLE)
- [MOSS](https://github.com/txsun1997/MOSS)
- [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B)
- [ChatGLM2-6B](https://github.com/THUDM/ChatGLM2-6B)

## LLM(基座)
- [LLaMA](https://github.com/facebookresearch/llama): Open and Efficient Foundation Language Models，Facebook/Meta开源的LLM，中文词表较小。

- Bloom: Huggingface开源的LLM模型。
  - [BLOOM](https://huggingface.co/docs/transformers/v4.27.2/en/model_doc/bloom#overview)
  - [BLOOMZ](https://huggingface.co/bigscience/bloomz): 指令微调版的BLOOM

- GLM: 清华大学开源的使用自回归填空目标进行预训练的通用语言模型[GLM](https://github.com/THUDM/GLM)
- [更多](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)

## 上下文长度
- FlashAttention ([Github](https://github.com/HazyResearch/flash-attention), [Torch 2.0 implementation](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html))
- [Positional Interpolation](https://arxiv.org/pdf/2306.15595.pdf)
- [NTK-Aware Scaled RoPE] ([Reddit](https://www.reddit.com/r/LocalLLaMA/comments/14lz7j5/ntkaware_scaled_rope_allows_llama_models_to_have/), [Implementation](https://github.com/huggingface/text-generation-inference/issues/512))

## 工具使用
- Toolformer ([Paper](https://arxiv.org/abs/2302.04761), [Implementation](https://github.com/lucidrains/toolformer-pytorch))
- [Toolbench](https://github.com/OpenBMB/ToolBench)

## 其他相关开源项目
其余优秀开源项目，大部分为纯英文

- [Stanford Alpaca](https://github.com/tatsu-lab/stanford_alpaca): LLAMA-7B SFT
- [Vicuna](https://github.com/lm-sys/FastChat): LLAMA-7b&13B SFT，数据来自ShareGPT
- [Baize](https://github.com/project-baize/baize-chatbot): LLAMA聊天微调，数据采集自ChatGPT self-chat
- [LoRA](https://github.com/microsoft/LoRA): popular低成本LLM参数高效微调方案，已集成到[PEFT](https://github.com/huggingface/peft)
- [self-instruct](https://github.com/yizhongw/self-instruct): 低成本收集指令微调数据
- [UltraChat](https://github.com/thunlp/UltraChat): ChatGPT生成的多轮对话数据集，目前只包含英文。
- [Dolly](https://github.com/databrickslabs/dolly): 基于EleutherAI/pythia-12b的指令微调，包含首个开源的人工标注指令微调数据集。
- [Open-Assistant](https://github.com/LAION-AI/Open-Assistant): 一个旨在让每个人都能访问基于聊天的大型语言模型的项目。

## Contribution
如果你创建或发现了任何关于实现中文ChatGPT的优秀资源，请创建Issue或PR来贡献这个仓库!

If you created or found any awesome resource about Chinese ChatGPT, feel free to create issues or PRs to contribute to this repository!
