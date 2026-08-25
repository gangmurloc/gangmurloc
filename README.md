### Ganggil Lee

Undergraduate Researcher in the NLP Laboratory at Hallym University.
NLP · LLMs · RAG · Reliable Evaluation.

I study how retrieval-augmented generation systems use evidence, why retrieval
and evaluation pipelines fail, and how grounded answers should be updated when
their underlying knowledge changes.

---

## Selected Research Projects

### [FARR-EVA](https://github.com/gangmurloc/FARR-EVA)

**Evidence-based arbitration for multi-hop RAG trajectories**

Performs post-execution arbitration among completed trajectories produced by
local research adaptations of FLARE, IRCoT, and FARR, using claim-level
evidence support rather than relying on a single fixed pipeline.

**Key result**

- Locked 6,000-question Test-C across HotpotQA, 2WikiMultiHopQA, and MuSiQue
- Macro F1: fixed FARR anchor **0.5140** → FARR-EVA **0.5754 (+0.0614)**
- 95% bootstrap CI for the improvement: **[0.0530, 0.0699]**

→ Evidence-based trajectory arbitration improved upon the validation-fixed
FARR anchor on each of the three datasets.

---

### [CVE_KR_RAG](https://github.com/gangmurloc/CVE_KR_RAG)

**Diagnosing retrieval shortcuts in Korean CVE RAG**

Evaluates BM25, dense, hybrid, and reranking retrieval under a fixed
generation model.

**Key result**

- Original benchmark: BM25 Hit@1 = **1.000**
- The result was largely caused by CVE IDs appearing directly in queries
- After removing the identifier shortcut, BM25 lost its lead
- Query-weighted hard split (307 unique queries): Hybrid + Reranker
  Hit@1 = **0.7883**, MRR@10 = **0.8272**

→ Benchmark construction and the choice of evaluation unit can change the
apparent ranking of retrieval strategies.

---

### [ClaimPatch](https://github.com/gangmurloc/ClaimPatch)

**Dependency-complete semantic patching for evolving LLM answers**

Updates claims affected by new evidence while preserving claims that remain
valid, instead of regenerating the entire answer.

**Key result**

- Qwen2.5-7B-Instruct, 100 synthetic instances × 3 evidence updates
- Dependency-complete success: **0.820 vs 0.500** for unstructured selective editing
- DCS improvement: **+0.320**, 95% CI **[0.257, 0.380]**
- Patch recall: **0.926**
- Collateral edit rate: **0.183 vs 1.000** for full regeneration

→ Dependency-aware patching improved required-update coverage relative to
unstructured editing while changing fewer still-valid claims than full
regeneration.

> ClaimPatch is currently evaluated on a controlled synthetic benchmark;
> the result should not be interpreted as evidence of real-world robustness.

---

## Contact

Email: [gangmurloc@gmail.com](mailto:gangmurloc@gmail.com)
