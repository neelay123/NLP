# NLP — Lab Notebooks

Student lab notebooks for a Natural Language Processing module. Each lab is a self-contained Jupyter notebook covering a core NLP task, built mainly on [HuggingFace Transformers](https://huggingface.co/transformers/), PyTorch, and (in later labs) open LLMs. Notebooks are designed to run on **Google Colab** (a T4 GPU is recommended for several labs).

## Labs

| Notebook | Topic | Key models / datasets |
| --- | --- | --- |
| [Lab1_2_Neural_Machine_Translation_Student.ipynb](Lab1_2_Neural_Machine_Translation_Student.ipynb) | Neural Machine Translation | seq2seq (Sutskever/Cho), attention; English–Vietnamese IWSLT TED corpus; BLEU via `sacrebleu` |
| [Lab3_ABSA_with_BERT_Student.ipynb](Lab3_ABSA_with_BERT_Student.ipynb) | Aspect-Based Sentiment Analysis | BERT as trainable layer; 3-class sentiment (POS/NEU/NEG) per aspect |
| [Lab4_Natural_Language_Generation_Student.ipynb](Lab4_Natural_Language_Generation_Student.ipynb) | Natural Language Generation | GPT-2; decoding strategies — greedy, beam search, sampling, top-k/top-p |
| [Lab5_Social_Media_Processing_Student.ipynb](Lab5_Social_Media_Processing_Student.ipynb) | Social Media Processing | Humour-rating regression; SemEval-2021 HaHackathon Task-1b; preprocessing, data augmentation, ensembling, multi-task |
| [Lab6_Summarisation_and_Data_Generation_Student.ipynb](Lab6_Summarisation_and_Data_Generation_Student.ipynb) | Summarisation & Controlled Generation | T5 fine-tuning; XSum extreme-summarisation dataset; keyword-controlled generation |
| [Lab7_NER_Student.ipynb](Lab7_NER_Student.ipynb) | Named Entity Recognition | Lample et al. (2016) sequence labelling; CoNLL-2003 English; IO tagging; pretrained embeddings |
| [Lab8_Coreference_Resolution_Student.ipynb](Lab8_Coreference_Resolution_Student.ipynb) | Coreference Resolution | Mention-ranking (Lee et al. 2017); word embeddings + coref metrics |
| [Lab9_Dialogue_Act_Tagging_Student.ipynb](Lab9_Dialogue_Act_Tagging_Student.ipynb) | Dialogue Act Tagging | Switchboard Dialog Act Corpus; two DA classification models |
| [Lab10_Seq2seq_Dialogue_Model_Student.ipynb](Lab10_Seq2seq_Dialogue_Model_Student.ipynb) | End-to-End Dialogue System | Generative seq2seq dialogue model |
| [Lab11_LLMs_and_Prompt_Engineering_Student.ipynb](Lab11_LLMs_and_Prompt_Engineering_Student.ipynb) | LLMs & Prompt Engineering | Llama 2 13B-chat via `llama.cpp`; prompting for NLP tasks |

## Running

1. Open a notebook in **Google Colab** (recommended) or a local Jupyter with GPU.
2. Set runtime to **GPU (T4)** — especially for Lab5, Lab6, Lab10, Lab11.
3. Run the setup cells first — each notebook downloads its own data and installs its own dependencies (`transformers`, `datasets`, `sacrebleu`, `sentencepiece`, etc.).
4. `*_Student` notebooks contain **fill-in code blocks**; complete the marked sections (Lab7: 2 blocks, Lab8: 3 blocks).

## Notes

- Notebooks are the student versions — some cells are intentionally left incomplete as exercises.
- Data, embeddings, and model weights are downloaded at runtime and are **not** stored in this repo.
