<div align="center">

# Sisir Kausthubh

<a href="https://github.com/captof-omuamua"><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=2800&pause=900&color=7C3AED&center=true&vCenter=true&width=640&lines=Exploring+local-first+AI;RAG+%C2%B7+fine-tuning+(QLoRA)+%C2%B7+RL;NLP+%C2%B7+speech+%C2%B7+vision-language+models;Robotics+%C2%B7+edge+AI" alt="Exploring local-first AI · RAG, fine-tuning (QLoRA), RL · NLP, speech, vision-language models · robotics, edge AI" /></a>

**Applied ML engineer** · B.Tech CSE (AI), 2025

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch" />
<img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" alt="Hugging Face" />
<img src="https://img.shields.io/badge/vLLM-1F2937?style=flat-square" alt="vLLM" />
<img src="https://img.shields.io/badge/Unsloth%20%2F%20LoRA-0EA5E9?style=flat-square" alt="Unsloth / LoRA" />
<img src="https://img.shields.io/badge/Qdrant-DC244C?style=flat-square" alt="Qdrant" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />

</div>

> I build LLM and vision-language systems on local hardware, then score them on public
> benchmarks with verified labels, **next to the published baseline**. Every number below comes
> from a held-out test split and a script you can re-run.

---

## 🏁 Scoreboard

| Project | Benchmark | My system | Published baseline |
| --- | --- | :---: | :---: |
| [docs-rag-assistant](https://github.com/captof-omuamua/docs-rag-assistant) | FinanceBench, all 84 filings in one index | **61.8%** | 19% (GPT-4-Turbo RAG) |
| [docs-rag-assistant](https://github.com/captof-omuamua/docs-rag-assistant) | FinanceBench, question's filing selected | **66.7%** | 50% (GPT-4-Turbo RAG) |
| [visual-product-tagging](https://github.com/captof-omuamua/visual-product-tagging) | ImplicitAVE, hand-checked labels | **85.3%** | 86.8% (GPT-4V) |

---

## 🚀 Flagship projects

<table>
<tr>
<td width="50%" valign="top">

### 📄 [docs-rag-assistant](https://github.com/captof-omuamua/docs-rag-assistant)
**Chat with your documents, with page citations.**

Answers questions over company filings, cites the page each figure comes from, and says so
when the answer isn't there. Fully local.

- **61.8%** on FinanceBench (GPT-4-Turbo RAG: 19%)
- **98%** correct refusals when the filings are removed
- Every citation checked against its source in code
- One search per needed figure: **+6.9 pts** on test

<sub>Docling · Qdrant · Qwen3 reranker · Gemma 4 26B on vLLM · FastAPI · Gradio</sub>

</td>
<td width="50%" valign="top">

### 🏷️ [visual-product-tagging](https://github.com/captof-omuamua/visual-product-tagging)
**Product attributes from photos, at GPT-4V level.**

A 4B vision-language model, LoRA-tuned in 48 minutes on one laptop GPU, tags sleeve style,
neckline, material and more.

- **85.3%** on ImplicitAVE (GPT-4V: 86.8%)
- **+17.5 pts** over the best fine-tuned model in the paper
- **₹0.67** per 1,000 products
- 79% auto-tagged at **94.6%** accuracy; the rest flagged for review

<sub>Qwen3.5-4B · Unsloth · LoRA · vLLM · Gradio</sub>

</td>
</tr>
<tr>
<td colspan="2" valign="top">

### 🤖 [catalog-automation-agent](https://github.com/captof-omuamua/catalog-automation-agent)
**An AI agent that fills in and checks product attributes from photos, with human review.**

Fetch → tag → auto-approve or pause for a reviewer → write back. Plugs into Shopify, n8n,
Slack, Google Sheets, any REST/CSV catalog, and Claude over MCP.

- **79.2%** of products auto-tagged at **94.6%** accuracy (ImplicitAVE test)
- QC mode catches **67.8%** of wrong listings at **90%** precision
- Crash-safe: **0 lost, 0 duplicate writes** under injected failures and a killed process
- **45 products/s** with FP8 on one laptop GPU, **₹0.35** per 1,000

<sub>LangGraph · MCP server · n8n · vLLM (FP8) · FastAPI · Docker</sub>

</td>
</tr>
</table>

---

## 🧪 More ML work

| | Project | What's inside |
| :---: | --- | --- |
| 📈 | [Retail sales forecasting](https://github.com/captof-omuamua/Retail-Sales-and-Time-Series-Forecasting) | Chronological folds, a separate holdout and baselines; Random Forest cut error 11% vs a seasonal baseline. |
| 🦙 | [LLM fine-tuning](https://github.com/captof-omuamua/Generative-AI-and-LLM-Fine-Tuning) | Llama 3.2 3B conversational fine-tuning with Unsloth, 4-bit loading and LoRA. |
| 🎬 | [AI short video generator](https://github.com/captof-omuamua/ai-short-video-generator) | Next.js app: topic → AI script, images, narration and captions → Remotion preview. Prototype (2024). |
| 🗣️ | [Tamil → Telugu speech translation](https://github.com/captof-omuamua/Ensemble-Transformer-Model-for-Speech-to-Speech-Translation-Tamil-to-Telugu-) | Whisper ASR → transformer translation → MMS speech synthesis, with model comparisons. |
| 📝 | [Tamil text summarization](https://github.com/captof-omuamua/extractive-abstractive-tamil-summarization) | Three extractive methods vs fine-tuned mBART/mT5, compared with ROUGE. |
| 🎨 | [Video style transfer](https://github.com/captof-omuamua/Enhanced-Segmented-Neural-Style-Transfer-for-Real-Time-Video-Stylization) | Fast neural stylization with separate foreground and background video results. |

## 🔬 Research and prototypes

| | Project | What it is | Status |
| :---: | --- | --- | --- |
| 🛡️ | [Tamil multimodal hate speech](https://github.com/captof-omuamua/tamil-multimodal-hate-speech) | IndicBERT text + ViT/ResNet video features, pseudo-labelling and synthetic data. | Research draft |
| 📰 | [Malayalam summarization](https://github.com/captof-omuamua/phase2-summarization) | From-scratch PyTorch Transformer for news-to-headline generation. | Research code |
| 🤖 | [Warehouse navigation (DDPG)](https://github.com/captof-omuamua/warehouse-navigation-ddpg) | Deep RL for goal-directed robot navigation in a Gazebo warehouse. | Report showcase |
| 🔤 | [Indic document OCR](https://github.com/captof-omuamua/indic-document-ocr) | Layout preparation and OCR utilities for Indic-script documents. | Utilities |
| 🏠 | [Smart home security](https://github.com/captof-omuamua/Smart-home-and-Smart-Security-System) | Raspberry Pi camera streaming, motion alerts and Arduino door control. | Hardware prototype |

<details>
<summary><b>📚 Coursework and notebook collections</b></summary>
<br>

- **Index:** [AI/ML project index](https://github.com/captof-omuamua/Colab-AI-ML-Projects): speech, translation, RL, vision and ML notebooks by topic
- **ML notebooks:** [Computer vision & CNNs](https://github.com/captof-omuamua/Computer-Vision-and-CNN-Experiments) · [Traffic sign recognition](https://github.com/captof-omuamua/Traffic-Sign-Recognition-using-CNN) · [NLP & text analytics](https://github.com/captof-omuamua/NLP-and-Text-Analytics) · [Airline sentiment LSTM](https://github.com/captof-omuamua/airline-sentiment-lstm) · [Indic translation](https://github.com/captof-omuamua/Indic-Language-Translation) · [RL experiments](https://github.com/captof-omuamua/Reinforcement-Learning-Experiments) · [RL exercises](https://github.com/captof-omuamua/reinforcement-learning-exercises)
- **Data & systems:** [Movie analytics (Spark)](https://github.com/captof-omuamua/movie-spark-analytics) · [COVID-19 analytics (Spark)](https://github.com/captof-omuamua/covid19-spark-analytics) · [Cloud task scheduling](https://github.com/captof-omuamua/cloud-task-scheduling) · [Web & storage automation](https://github.com/captof-omuamua/Python-Web-and-Storage-Automation) · [FTP/HTTP networking](https://github.com/captof-omuamua/ftp-http-network-programming)
- **Design studies & web:** [Multilingual meeting summarizer](https://github.com/captof-omuamua/multilingual-meeting-summarizer) · [Flask student registration](https://github.com/captof-omuamua/flask-student-registration) · [Tuiter web UI](https://github.com/captof-omuamua/tuiter-web-coursework) · [File encryption tool](https://github.com/captof-omuamua/file-encryption-tool) · [Nand2Tetris](https://github.com/captof-omuamua/Nand2tetris)

</details>

---

## 🧰 What I work with

**Models & training:** PyTorch · Hugging Face · Unsloth/LoRA · vLLM  
**Retrieval & apps:** Qdrant · Docling · FastAPI · Gradio · Docker  
**Agents & automation:** LangGraph · MCP · n8n  
**Quality:** pytest · GitHub Actions · held-out test splits · published baselines  
**Domains:** RAG · AI agents · vision-language models · LLM evaluation · speech · Indic-language NLP · forecasting

<div align="center">
<sub>Each project README covers setup, data and results. Datasets, model weights and third-party components keep their own licences.</sub>
</div>
