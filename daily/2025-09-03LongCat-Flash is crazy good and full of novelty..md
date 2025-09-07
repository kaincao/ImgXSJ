---
title: 2025-09-03LongCat-Flash is crazy good and full of novelty.
tags: 新建,模板,小书匠
category: /小书匠/日记/2025-09
grammar_cjkRuby: true
---

<!--StartFragment-->

<span class="css-1jxf684 r-bcqeeo r-1ttztb7 r-qvutc0 r-poiln3">The technical report of </span>
<div class="css-175oi2r r-xoduu5">
  <span class="r-18u37iz"><a dir="ltr" href="https://x.com/Meituan_LongCat" role="link" class="css-1jxf684 r-bcqeeo r-1ttztb7 r-qvutc0 r-poiln3 r-1loqt21">@Meituan_LongCat</a>
  </span>
</div>
<span class="css-1jxf684 r-bcqeeo r-1ttztb7 r-qvutc0 r-poiln3"> LongCat-Flash is crazy good and full of novelty. The model is a 560B passive ~27B
  active MoE with adaptive number of active parameters depending on the context
  thanks to the Zero-Computational expert. 1) New architecture &gt; Layers have
  2 Attention blocks and both FFN and MoE, that way you can overlap the 2 all-to-all
  coms. (also it's only 28 layers but you have to take into account the 2 attention
  blocks). &gt; They add the zero-computational expert that tokens can choose and
  do nothing, kinda like a "sink" for easy tokens. &gt; For load balancing, they
  have a dsv3-like aux loss free to set the average real/fake expert per token.
  They apply a decay schedule to this bias update. They also do loss balance control.
  2) Scaling &gt; They made changes to MLA/MoE to have variance alignment at init.
  The gains are pretty impressive in Figure 5, but i don't know to what extent
  this has impact later on. &gt; Model growth init is pretty cool, they first train
  a 2x smaller model and then "when it's trained enough" (a bit unclear here how
  many B tokens) they init the final model by just stacking the layers of the smaller
  model. &gt; They used </span>
<div class="css-175oi2r r-xoduu5">
  <span class="r-18u37iz"><a dir="ltr" href="https://x.com/_katieeverett" role="link" class="css-1jxf684 r-bcqeeo r-1ttztb7 r-qvutc0 r-poiln3 r-1loqt21">@_katieeverett</a>
  </span>
</div>
<span class="css-1jxf684 r-bcqeeo r-1ttztb7 r-qvutc0 r-poiln3"> </span>
<div class="css-175oi2r r-xoduu5">
  <span class="r-18u37iz"><a dir="ltr" href="https://x.com/Locchiu" role="link" class="css-1jxf684 r-bcqeeo r-1ttztb7 r-qvutc0 r-poiln3 r-1loqt21">@Locchiu</a>
  </span>
</div>
<span class="css-1jxf684 r-bcqeeo r-1ttztb7 r-qvutc0 r-poiln3"> and al. paper to have hyperparameter transfer with SP instead of muP for the 2x
  smaller model ig. 3) Stability &gt; They track Gradient Norm Ratio and cosine
  similarity between experts to adjust the weight of the load balancing loss (they
  recommend Gradient Norm Ratio &lt;0.1). &gt; To avoid large activations, they
  apply a z-loss to the hidden state, with a pretty small coef (another alternative
  to qk-clip/norm). &gt; They set Adam epsilon to 1e-16 and show that you want
  it to be lower than the gradient RMS range. 4) Others &gt; They train on 20T
  tokens for phase 1, "multiple T of tokens" for mid training on STEM/code data
  (70% of the mixture), 100B for long context extension without yarn (80B for 32k,
  20B for 128k). The long context documents represent 25% of the mixture (not sure
  if it's % of documents or tokens, which changes a lot here). &gt; Pre-training
  data pipeline is context extraction, quality filtering, dedup. &gt; Nice appendix
  where they show they compare top_k needed for different benchmarks (higher MMLU
  with 8.32, lower GSM8K with 7.46). They also compare token allocation in deep/shallow
  layers. &gt; They release two new benchmarks Meeseeks (multi-turn IF) and VitaBench
  (real-world business scenario). &gt; Lots of details in the infra/inference with
  info on speculative decoding acceptance, quantization, deployment, kernel optimization,
  coms overlapping, etc. &gt; List of the different relevent paper in thread </span>
<img
alt="🧵" draggable="false" src="https://abs-0.twimg.com/emoji/v2/svg/1f9f5.svg"
title="Thread" class="r-4qtqp9 r-dflpy8 r-k4bwe5 r-1kpi4qh r-pp5qcn r-h9hxbl">
  <!--EndFragment-->![enter description here](./images/1756837284384.png)
  
  relevant paper: -zero-computation expert: [https://arxiv.org/abs/2410.07348](https://t.co/qESOr7H2cr) - adaMoE: [https://aclanthology.org/2024.findings-emnlp.361/](https://t.co/V3xRLTOT8O) - Shortcut-connected Expert Parallelism: [https://arxiv.org/abs/2404.05019](https://t.co/JjUGCgHJpT) - hyperparm transfer: [https://arxiv.org/abs/2407.05872](https://t.co/pgyUJvuTqk) tech report: [https://github.com/meituan-longcat/LongCat-Flash-Chat/blob/main/tech_report.pdf](https://t.co/QGZbEMOMLl) model:
  
  ![enter description here](./images/1756837345613.png)
  
  