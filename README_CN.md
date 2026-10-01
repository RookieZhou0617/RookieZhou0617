<p align="center">
  <img src="assets/profile-header-v2.svg" alt="周文杰 — 应用统计 · 图学习 · 风险建模" width="100%" />
</p>

<p align="center">
  <a href="README.md">English</a> · <a href="README_CN.md">中文</a> · <a href="mailto:zhouwenjie_0617@163.com">邮件联系</a>
</p>

我是**周文杰（Wenjie Zhou）**，目前就读于**上海财经大学应用统计硕士**，预计于 2027 年毕业。我的研究兴趣位于统计学习、图表示学习与金融风险建模的交叉领域。

当前研究关注：当企业自身信息已能提供较强的风险信号时，关系信息如何进一步改善预测，以及如何在时间变化下评价这种贡献。

## 研究兴趣

- **多源表示学习：** 融合财务变量、文本和企业历史，同时保留各信息来源的特点。
- **面向风险预测的图学习：** 有选择地利用异构关系，构建相对风险消息与残差修正。
- **时序评价：** 区分模型选择与未来年度测试，分析负迁移，并在汇总性能之外报告不确定性。

## 代表研究

### [MSAR-HGRN · 财务造假检测](https://github.com/RookieZhou0617/risk-aware-financial-fraud-detection)

*硕士论文课题 · 模型开发已完成，论文撰写中。*

框架首先比较企业当前状态与历史状态，构建**多源偏差风险锚点模型（MDRA）**；随后冻结锚点编码器及分类器，由异构图分支学习隐藏表示残差。

研究重点是**较强风险锚点之上的关系增量**，而非无约束的图传播。滚动开发评价与 2022 年固定协议跨期测试表明，关系贡献存在年度差异：最终平均 AUC-PR 有所改善，但 Bootstrap 区间跨零，2019 年也出现了负迁移。

[方法与架构](https://github.com/RookieZhou0617/risk-aware-financial-fraud-detection/blob/main/docs/methodology.md) · [评价与局限](https://github.com/RookieZhou0617/risk-aware-financial-fraud-detection/blob/main/docs/experiments.md) · [PyTorch 合成示例](https://github.com/RookieZhou0617/risk-aware-financial-fraud-detection/tree/main/examples)

<sub>公开仓库提供精简实现、经核对的汇总证据与合成示例，不含私有数据、训练检查点，也不是完整实验的一键复现包。</sub>

## 研究实践

我希望让建模选择与支持它的证据之间的关系更加清楚：

- **遵守信息边界。** 在允许的时序窗口内拟合变换，并明确数据可用性假设。
- **设置有效对照。** 与企业内生风险锚点及匹配随机关系比较，检验图信息的额外贡献。
- **保留混合结果。** 报告预设种子汇总、负向年度、指标取舍与不确定性，不只呈现最有利的结果。
- **明确公开范围。** 区分可运行的方法演示与完整的实验复现。

## 背景

本科毕业于济南大学数据科学与大数据技术专业。在**度小满、百度和信飞科技**的实习中，我接触了风控策略、内容安全、语音分类及大模型辅助分析。这些应用经历也促使我关注模型离开训练环境之后，评价结论是否仍有实际意义。

主要使用 **Python、PyTorch、scikit-learn、LightGBM 和 SQL**，通过 Linux 与 Git 开展开发和实验组织。

---

欢迎交流图学习、金融风险建模与应用机器学习，也欢迎联系相关研究和业界机会。

[zhouwenjie_0617@163.com](mailto:zhouwenjie_0617@163.com)
