<p align="center">
  <img src="assets/profile-header-v2.svg" alt="Wenjie Zhou — Applied Statistics · Graph Learning · Risk Modeling" width="100%" />
</p>

<p align="center">
  <a href="README.md">English</a> · <a href="README_CN.md">中文</a> · <a href="mailto:zhouwenjie_0617@163.com">Email</a>
</p>

I am **Wenjie Zhou (周文杰)**, a master's student in Applied Statistics at **Shanghai University of Finance and Economics**, expecting to graduate in 2027. My interests lie at the intersection of statistical learning, graph representation learning, and financial risk modeling.

My current work asks how relational information can improve risk prediction when strong company-level signals are already available—and how to evaluate that contribution under temporal change.

## Research interests

- **Multi-source representation learning:** combining financial variables, text, and company history while retaining source-specific information.
- **Graph learning for risk prediction:** selective use of heterogeneous relations, risk-relative messages, and residual correction.
- **Temporal evaluation:** separating model selection from future-year testing, studying negative transfer, and reporting uncertainty alongside aggregate performance.

## Selected work

### [MSAR-HGRN · Financial Statement Fraud Detection](https://github.com/RookieZhou0617/risk-aware-financial-fraud-detection)

*Master's thesis project · Model development completed; manuscript in preparation.*

The framework first builds a **Multi-Source Deviation Risk Anchor (MDRA)** by comparing a company's current and historical states. A heterogeneous graph branch then learns a hidden-state residual while the anchor encoder and classifier remain frozen.

The study emphasizes **relational increment over a strong anchor**, rather than unrestricted graph propagation. Rolling development evaluations and a fixed-protocol 2022 out-of-time test show that the contribution is year-dependent: the final mean AUC-PR improves, but bootstrap intervals cross zero and negative transfer remains visible in 2019.

[Method & architecture](https://github.com/RookieZhou0617/risk-aware-financial-fraud-detection/blob/main/docs/methodology.md) · [Evaluation & limitations](https://github.com/RookieZhou0617/risk-aware-financial-fraud-detection/blob/main/docs/experiments.md) · [Synthetic PyTorch example](https://github.com/RookieZhou0617/risk-aware-financial-fraud-detection/tree/main/examples)

<sub>The repository provides a compact implementation, reviewed aggregate evidence, and synthetic examples—not private data, trained checkpoints, or a full reproduction package.</sub>

## Research practice

I aim to make the relationship between a modeling choice and its supporting evidence explicit:

- **Respect the information boundary.** Fit transformations within the permitted temporal window and state data-availability assumptions.
- **Use informative controls.** Compare against the intrinsic anchor and matched shuffled relations to examine what the graph adds.
- **Keep mixed results visible.** Report preset-seed summaries, adverse years, metric trade-offs, and uncertainty rather than selecting the most favorable outcome.
- **Make scope clear.** Distinguish a runnable demonstration from a complete experimental reproduction.

## Background

Before my master's studies, I completed a B.S. in Data Science and Big Data Technology at the University of Jinan. Internships at **Duxiaoman, Baidu, and Xinfei Technology** have given me experience in risk strategy, content safety, speech classification, and LLM-assisted analysis. These applications inform my interest in evaluation that remains meaningful beyond the training setting.

I work primarily with **Python, PyTorch, scikit-learn, LightGBM, and SQL**, using Linux and Git for development and experiment organization.

---

I welcome discussions about graph learning, financial risk modeling, and applied machine learning, as well as related research and industry opportunities.

[zhouwenjie_0617@163.com](mailto:zhouwenjie_0617@163.com)
