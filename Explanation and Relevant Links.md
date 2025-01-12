## Part 1  
**Link**: [https://github.com/ZhaXionghui/llama3-from-scratch-numpy_and_lora-fine-tune](https://github.com/ZhaXionghui/llama3-from-scratch-numpy_and_lora-fine-tune)  
**Video**: [【Llama3和PicoGPT的Numpy复现】](https://www.bilibili.com/video/BV1wf421z7RM)  

In this replication of the **llama3** model, our team utilized **numpy** to recreate the complete inference process of the llama3-8B model. On this basis, we optimized the KVCache by trading space for time to reduce computational costs. Additionally, we encapsulated classes to facilitate subsequent calls, training, and modifications.  

We also compared its runtime on CPUs and GPUs, adopting **pipeline parallelism** to utilize GPUs. By simulating the sequential addition of Transformer layers to the GPU, computations were executed layer by layer with input data, considering the time spent on parameter transmission.  

Furthermore, we performed instruction fine-tuning on the llama3-8B model using **LORA**, a low-memory-cost fine-tuning method that enabled local fine-tuning. As a result, the model could output phrases like “山东大学（威海）数科.”  

We also replicated **PicoGPT**, which implements GPT using only 60 lines of numpy code. Our team added explanations for the replication process and code, providing a comprehensive overview.

---

## Part 2  
**Video**: [【第二部分：大语言模型总结垃圾桶检查项目与进一步科研思路的提出】](https://www.bilibili.com/video/BV1NUYLewEZw)  

In this part, we leveraged large language models (LLMs) to summarize the project **"Low-power Trash Overflow Detection based on Diffusion Data Augmentation and HERD-YOLO"** using tools like GPT4, locally deployed Gemma, and online paper platforms. We documented the **prompt workflows and methods** in detail.  

The video introduces the principles of **llama3** and, targeting the goal of "applying llama3 to trash overflow detection scenarios," proposes three application scenarios, their advantages, and potential implementations.  

We converted the LLM-generated PDF summaries into explanatory PPTs. With further prompting, the LLM generated scripts based on the PPT content. These scripts were later voiced using **CosyVoice** and an online voice platform, and the narration was integrated with the PPT to produce an explanation video.  
