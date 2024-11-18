# Data Extraction  
We used **AugmenToolkit** to extract data. Starting with a user manual for an air compressor, we split it into chapters. Using AugmenToolkit, we generated a dataset of 1,000 rows in JSONL format.  

- **Dataset Link**: [Fine-Tune Air Compressor Dataset](https://huggingface.co/datasets/sanket09/finetune_air_compressor)  

---

# Model Fine-Tuning  
We fine-tuned three models using **QLoRA weights**, based on specific requirements and use cases:  

1. **[TinyLLaMA 1.1B](https://huggingface.co/sanket09/TinyLlama-1.1B-Chat-finetune)**  
   - Chosen for its small size, making it the most efficient model for **CPU-based operations**.  

2. **[LLaMA 2 8B](https://huggingface.co/sanket09/Llama-2-7b-chat-finetune-air)**  
   - Selected for its larger parameter count (8B), providing better performance compared to TinyLLaMA.  
   - Requires a **minimum RTX-600 GPU** for optimal performance; otherwise, it may run slower.  

3. **LLaMA 3.2 9B MLLM** *(Under Testing)*  
   - This model was included due to its ability to process **images** effectively.  
   - It is the best-performing model but has a higher requirement of a **T4 GPU with 16GB VRAM**.  
   - **Note:** The fine-tuned version of this model is currently under testing and will be linked once finalized.  

---
