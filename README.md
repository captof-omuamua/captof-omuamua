# Sisir Kausthubh

### Machine learning · LLM fine-tuning & evaluation · Indic speech and NLP

I fine-tune and evaluate language and speech models, with a focus on Indian languages, and build forecasting and computer vision models. My projects use held-out evaluation and documented protocols, so results can be checked rather than taken on trust.

## Recent engineering work

[**Retail Sales and Time Series Forecasting**](https://github.com/captof-omuamua/Retail-Sales-and-Time-Series-Forecasting)

A reproducible forecasting study with chronological development folds, a separate final holdout, simple baseline comparisons, regression tests, and an executable notebook smoke check.

- Preserves original targets and official holiday weights.
- Selects a method before final evaluation and matches exported forecasts to submission IDs.
- Publishes the [protocol, aggregate results, and verification record](https://github.com/captof-omuamua/Retail-Sales-and-Time-Series-Forecasting/tree/main/reports/real-run-v1).
- Random Forest cut error by 11% against a seasonal baseline on a 39-week local holdout.

## Selected projects

| Project | What to explore | Type |
| --- | --- | --- |
| [LLM fine-tuning](https://github.com/captof-omuamua/Generative-AI-and-LLM-Fine-Tuning) | Llama 3.2 3B conversational fine-tuning with Unsloth, 4-bit loading and LoRA. | Fine-tuning |
| [Tamil-to-Telugu speech translation](https://github.com/captof-omuamua/Ensemble-Transformer-Model-for-Speech-to-Speech-Translation-Tamil-to-Telugu-) | ASR → text translation → speech synthesis, with model comparisons for recognition and speech synthesis. | End-to-end pipeline |
| [Tamil text summarization](https://github.com/captof-omuamua/extractive-abstractive-tamil-summarization) | Three extractive methods and fine-tuned mBART/mT5 models, compared with ROUGE. | NLP models |
| [Neural style transfer](https://github.com/captof-omuamua/Enhanced-Segmented-Neural-Style-Transfer-for-Real-Time-Video-Stylization) | Fast image stylization with foreground and background video results. | Computer vision |
| [AI/ML project index](https://github.com/captof-omuamua/Colab-AI-ML-Projects) | Speech, translation, RL, vision and ML notebooks, organised by topic. | Notebook collection |

## Tools in these projects

Python · pandas · NumPy · scikit-learn · PyTorch · Jupyter · pytest  
Speech recognition · Translation · Summarization · Forecasting · Computer vision

## Working with the repositories

For a reproducible bug report, open an issue in the relevant repository with the command, environment, expected result, and a small example. Keep credentials, private documents, and restricted datasets out of public issues.

Each project README covers setup, data paths and results. Datasets, model weights and third-party components keep their own licences.

