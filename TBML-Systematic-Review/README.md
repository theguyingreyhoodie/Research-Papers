# Toward Privacy-Preserving Detection of Trade-Based Money Laundering

**A Systematic Review of Graph Learning, Federated Learning, and Blockchain Auditing**

Anuj Nanhe, Aniket Shelke, Laiba Shaikh, and S. R. Khonde

📄 [Read the PDF](TBML_Systematic_Review.pdf)

## Abstract

Money laundering through bank transfers and through international trade is hard to detect because the evidence is split across institutions that cannot share raw customer data. Graph learning, federated learning, and blockchain are each proposed as part of the answer, but they are studied by separate communities. This paper presents a systematic review of how these techniques are used to detect laundering and financial fraud, how they protect the data of the participating institutions, and how they make detection auditable.

Following PRISMA 2020, 34 full-text files collected from IEEE Xplore and Emerald Insight in four thematic clusters were screened. After duplicates were removed and one unretrievable report was set aside, 27 studies were assessed in full text, and all were retained and classified against a taxonomy of seven categories. Graph models report strong results on the Elliptic Bitcoin data and on the synthetic IBM transactions, but datasets, splits, and metrics differ so much that the numbers cannot be ranked. Only three studies train fraud detectors across institutions with federated learning. None of them uses laundering data, and the only one that lets institutions keep different columns without matching customers has two clients. Secure aggregation hides individual updates, yet one study shows that it still reveals which classes a participant holds. In a federation of banks this could expose the banks that hold confirmed laundering cases. Blockchain is used for incentives, accountability, policies, and documents, but no study records the updates and alerts of a detection model on a ledger. The literature on trade-based laundering offers price statistics, mirror analysis, and a single classification study.

We synthesize these findings into a taxonomy, ten research gaps, and a reference architecture for privacy-preserving and auditable detection across banks, with trade data as the next step.

**Keywords:** anti-money laundering, trade-based money laundering, federated learning, secure aggregation, graph neural networks, blockchain, explainable AI, financial fraud detection, systematic review.

## Building from source

The paper uses the IEEE `IEEEtran` journal class, TikZ and pgfplots, with the bibliography inline (no `.bib` file needed).

```sh
pdflatex TBML_Systematic_Review.tex
pdflatex TBML_Systematic_Review.tex   # second pass resolves references
```

It also compiles as-is on Overleaf.

## Related code

The prototype built from this review's reference architecture: [Bank-Based-Money-Laundering-Detection](https://github.com/theguyingreyhoodie/Bank-Based-Money-Laundering-Detection).
