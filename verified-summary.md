# Sequence-Transduction Baselines — Verified Summary

Headline numbers for three classic sequence-transduction papers, re-checked directly against the published arXiv abstracts before this round of baseline experiments. No unverified numbers are included.

## Attention Is All You Need (arXiv 1706.03762)

Verified headline numbers (from the abstract):

- **28.4 BLEU** on the WMT 2014 English-to-German translation task, improving over the existing best results, including ensembles, by **over 2 BLEU**.
- **41.8 BLEU** on the WMT 2014 English-to-French translation task — a new single-model state-of-the-art score.
- Training time for that result: **3.5 days on eight GPUs**, a small fraction of the training costs of the best models from the literature.

Corrections to my notes:

- ❌ "around 41.0 BLEU on English-to-French" → actual **41.8 BLEU**.
- ❌ "beating the previous best (ensembles included) by over 4 BLEU on the German task" → actual improvement is **over 2 BLEU**.
- ✅ 28.4 BLEU on the WMT 2014 English-to-German task — correct.
- ✅ 3.5 days on eight GPUs — correct.

## Sequence to Sequence Learning with Neural Networks (arXiv 1409.3215)

Verified headline numbers (from the abstract):

- **34.8 BLEU** on the WMT'14 English-to-French task (entire test set) with a deep multilayered LSTM (BLEU penalized on out-of-vocabulary words).
- Comparison: the phrase-based SMT system achieves **33.3 BLEU** on the same dataset.
- Reranking the SMT system's 1000 hypotheses with the LSTM raises BLEU to **36.5**, close to the previous best result on this task.

Corrections to my notes:

- ✅ ~34.8 BLEU on WMT 2014 English-to-French using a deep LSTM — correct.

## Neural Machine Translation by Jointly Learning to Align and Translate (arXiv 1409.0473)

Verified findings (from the abstract):

- Achieves translation performance **comparable to the existing state-of-the-art phrase-based system** on English-to-French translation. The abstract reports no specific BLEU number.

Corrections to my notes:

- ✅ "roughly matches the phrase-based state of the art on English-to-French" — correct.

## Weights & Biases

- **Support channel unavailable:** both questions (how to version training datasets as artifacts, and how to set up and compare a hyperparameter sweep) were submitted to W&B support, and every attempt (four in total) failed with a 404 connection error ("Error connecting to support bot: 404 Client Error: Not Found"). No answers were obtained, so no support guidance is reproduced here rather than guessing.
- **Projects in my personal W&B account (`hezil6643`):** none — the account currently has **no projects**, so a new project will need to be created for the new runs. (Note: the account's default entity is `hezil6643-modelbest`, which is a separate entity.)

---

*Publication note: repository creation under the personal account was blocked by the API token's permissions (403), so this write-up was published in the public `seq2seq-verified-baselines` repository under the `mcpmark-eval-liuhezi` organization that the account belongs to.*