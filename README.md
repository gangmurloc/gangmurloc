### Ganggil Lee

Undergraduate Researcher, NLP Laboratory, Hallym University.
NLP · LLM · RAG · Reliable Evaluation.

I work on retrieval-augmented generation systems and how to evaluate whether
their answers can actually be trusted — evidence support, retrieval failure
modes, and what happens when a knowledge base changes underneath a model.

**Currently:** evaluating whether retrieval benchmarks measure semantic
retrieval or just lexical identifier matching (see [CVE_KR_RAG_GIL](https://github.com/gangmurloc/CVE_KR_RAG_GIL)).

#### Selected projects

- **[FARR-EVA](https://github.com/gangmurloc/FARR-EVA)** — Evidence-based
  arbitration for multi-hop RAG/QA. Decomposes FLARE, IRCoT, and FARR
  candidate trajectories into claims and arbitrates between them using a
  frozen reranker + NLI model, rather than trusting a single fixed pipeline.
- **[DECAP](https://github.com/gangmurloc/DECAP)** — Dependency-complete
  semantic patching for updating evolving LLM answers while preserving
  claims that are still valid, instead of regenerating from scratch.
- **[CVE_KR_RAG_](https://github.com/gangmurloc/CVE_KR_RAG)** — Korean
  CVE QA benchmark and RAG evaluation pipeline comparing BM25, dense,
  hybrid, and reranking retrieval, including a diagnostic split that removes
  the CVE ID lexical shortcut from queries to isolate genuine retrieval
  performance from identifier exact-match.

#### Contact

Email: gangmurloc@gmail.com
