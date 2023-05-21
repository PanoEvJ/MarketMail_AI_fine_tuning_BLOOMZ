<p align = "center" draggable=”false” ><img src="https://user-images.githubusercontent.com/37101144/161836199-fdb0219d-0361-4988-bf26-48b0fad160a3.png" 
     width="200px"
     height="auto"/>
</p>

# <h1 align="center" id="heading">Fine-tuning BLOOMZ For a Generative Task using LoRA</h1>

This week we'll be fine-tuning [BLOOMZ](https://huggingface.co/bigscience/bloomz) to perform on your desired down-stream generative task. We'll be focusing on "structure" fine-tuning, and won't be teaching BLOOMZ anything new.

We're going to take advantage of [LoRA](https://arxiv.org/abs/2106.09685) through Hugging Face's [PEFT](https://github.com/huggingface/peft) library to fine-tune BLOOMZ in an effecient and manageable manner.

### Objectives 🔍

- [ ] Dataset Preparation
- [ ] Training Prompt Engineering
- [ ] Initializing PEFT/LoRA
- [ ] Fine-tuning
- [ ] Push to Hub

### PRE REQS :warning:
 
Please complete the steps outlined in the `prework` folder.

### 📓 Notebooks

| Notebook | Link |
 --------- | ------- |
| Assignment Notebook: | [Here](https://colab.research.google.com/drive/1RfUuzG11Q8AaZuJIHLzXCVC087xoDeSd?usp=sharing) |
| Completed Notebook: | [Here](https://colab.research.google.com/drive/1ARmlaZZaKyAg6HTi57psFLPeh0hDRcPX?usp=sharing) |
| Synthetic Data Generation Notebook: | [Here](https://colab.research.google.com/drive/1nsyT9ssUWUWTc_TQ2rykuVtedA7QobA-?usp=sharing) |

### APIs and Libraries to Look Into:

- PEFT (linked above)
    - Specifically get_peft_model 
- LoRA (paper linked above)
    - PEFT's LoRAConfig
- Tim Dettmers' [bitsandbytes](https://github.com/TimDettmers/bitsandbytes)
- Hugging Face's [Accelerate](https://huggingface.co/docs/accelerate/index)
- Hugging Face's [transformers](https://huggingface.co/docs/transformers/index)
    - Specifically [AutoTokenizer](https://huggingface.co/docs/transformers/v4.29.1/en/model_doc/auto#transformers.AutoTokenizer), [AutoConfig](https://huggingface.co/docs/transformers/v4.29.1/en/model_doc/auto#transformers.AutoTokenizer), [AutoModelForCausalLM](https://huggingface.co/docs/transformers/v4.29.1/en/model_doc/auto#transformers.AutoTokenizer), [Trainer](https://huggingface.co/docs/transformers/v4.29.1/en/model_doc/auto#transformers.AutoTokenizer), [TrainingArguments](https://huggingface.co/docs/transformers/v4.29.1/en/model_doc/auto#transformers.AutoTokenizer)
- [OpenAI's Python Library](https://github.com/openai/openai-python)
- Hugging Face's [datasets](https://huggingface.co/docs/datasets/index)

### Deep Dive on LoRA Theory:

[Video Here](https://youtu.be/dA-NhCtrrVE)
