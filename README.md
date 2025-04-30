# dynamo-learnings
Notes for NVIDIA Dynamo - OSS Contribution

## Quick resources:
[Mastering LLM Techniques: Inference Optimization](https://developer.nvidia.com/blog/mastering-llm-techniques-inference-optimization/)

## What's Dynamo?
- Inference framework for GenAI and LLMs.

## How is it different from NVIDIA Nsight?
- Nsight is a suite of performance analysis and profiling tools. It's just for optimizing your code performance. It DOES NOT serve to deploy AI models.

## Other Inference Frameworks:
- NVIDIA Triton Inference Server: Production AI inference at scale.
- TensorRT-LLM, vLLM, SGLang: Inference engines that focus on optimizing the execution of LLMs/other models on GPUs.

## Why Dynamo when you have others?
- Nsight cannot serve or orchestrate models (coordination and mgmt of AI models, systems, and integrations).
- Triton is for general AI inference serving - it's not optimized for distributed LLM workloads.
- TensorRT-LLM, vLLM - For "Engine-level LLM inference acceleration" (basically optimizing core software/hardware/architecture-like using faster kernels, better memory handling, parallelization in the inference engine itself). So it's not a fully distributed serving/orchestration.
- **Dynamo** on the other hand, is for *Distributed, multi-node, LLM-optimized inference*. It's designed for **new scale** and **efficiency demands**.

## Next steps:
- Fork on Mac and old PC (dual-boot Ubuntu). Provision cloud GPU services from Lambda Labs, Vast.ai on demand.
