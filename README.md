# Sisir Kausthubh

### Applied ML · LLM applications (RAG, fine-tuning) · evaluation you can check

I build LLM and vision-language systems that run on local hardware and measure them on public
benchmarks with verified labels, next to published baselines. Every result in these
repositories comes from a held-out test split and a script you can re-run.

## Latest projects

### [docs-rag-assistant](https://github.com/captof-omuamua/docs-rag-assistant): chat with your documents, with citations

Answers questions over company filings, cites the page each figure comes from, and says so
when the answer isn't there. Fully local: Docling, Qdrant, a Qwen3 reranker and Gemma 4 26B on
vLLM, served with FastAPI and a Gradio chat UI.

- **61.8% on FinanceBench** with all 84 SEC filings in one index, and **66.7%** with the
  question's filing selected. The FinanceBench paper reports 19% and 50% for GPT-4-Turbo
  RAG in those two settings.
- **98% correct refusals** when the company's filings are removed; every citation is checked
  against its source in code.
- A gold-page diagnostic showed retrieval was the main gap, so the model now plans one
  search per figure it needs: +6.9 points on test.

### [visual-product-tagging](https://github.com/captof-omuamua/visual-product-tagging): product attributes from photos, at GPT-4V level

A 4B vision-language model, fine-tuned with LoRA in 48 minutes on one laptop GPU, tags
product attributes (sleeve style, neckline, material…) from photos.

- **85.3% on the hand-checked ImplicitAVE benchmark** (GPT-4V: 86.8%), 17.5 points above the
  best fine-tuned model in the benchmark paper.
- **₹0.67 per 1,000 products**, and it flags what it isn't sure about: 79% of products are
  tagged automatically at 94.6% accuracy.

## More projects

| Project | What to explore | Type |
| --- | --- | --- |
| [Retail sales forecasting](https://github.com/captof-omuamua/Retail-Sales-and-Time-Series-Forecasting) | Chronological folds, a separate final holdout and baselines; Random Forest cut error 11% vs a seasonal baseline. | Forecasting |
| [LLM fine-tuning](https://github.com/captof-omuamua/Generative-AI-and-LLM-Fine-Tuning) | Llama 3.2 3B conversational fine-tuning with Unsloth, 4-bit loading and LoRA. | Fine-tuning |
| [Tamil-to-Telugu speech translation](https://github.com/captof-omuamua/Ensemble-Transformer-Model-for-Speech-to-Speech-Translation-Tamil-to-Telugu-) | ASR → text translation → speech synthesis, with model comparisons for recognition and speech synthesis. | End-to-end pipeline |
| [Tamil text summarization](https://github.com/captof-omuamua/extractive-abstractive-tamil-summarization) | Three extractive methods and fine-tuned mBART/mT5 models, compared with ROUGE. | NLP models |
| [Neural style transfer](https://github.com/captof-omuamua/Enhanced-Segmented-Neural-Style-Transfer-for-Real-Time-Video-Stylization) | Fast image stylization with foreground and background video results. | Computer vision |
| [AI/ML project index](https://github.com/captof-omuamua/Colab-AI-ML-Projects) | Speech, translation, RL, vision and ML notebooks, organised by topic. | Notebook collection |

## Tools in these projects

Python · PyTorch · Hugging Face · vLLM · Unsloth/LoRA · Qdrant · Docling · FastAPI · Gradio ·
Docker · pytest · GitHub Actions  
RAG · Vision-language models · LLM evaluation · Speech recognition · Translation · Forecasting

## Working with the repositories

For a reproducible bug report, open an issue in the relevant repository with the command, environment, expected result, and a small example. Keep credentials, private documents, and restricted datasets out of public issues.

Each project README covers setup, data paths and results. Datasets, model weights and third-party components keep their own licences.
