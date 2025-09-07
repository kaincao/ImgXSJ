---
title: 2025-09-03无需OCR，基于ColQwen2、Qwen2.5和Weaviate对PDF进行多模态RAG的方法
tags: 新建,模板,小书匠
category: /小书匠/日记/2025-09
grammar_cjkRuby: true
---

<!--StartFragment-->

<span class="css-1jxf684 r-bcqeeo r-1ttztb7 r-qvutc0 r-poiln3">无需OCR，基于ColQwen2、Qwen2.5和Weaviate对PDF进行多模态RAG的方法 此方法用ColQwen2直接将PDF页面截图作为图像进行处理，去除了OCR和分块步骤
  首先嵌入截图，把PDF文档转换为图像截图，用 ColQwen2把截图转为向量表示 把这些向量存入Weaviate向量数据库 查询时，用ColQwen2把文本问题也编成向量，从数据库中检索最相关的PDF页面
  最后用Qwen2.5-VL根据页面内容和问题生成最终答案 这个方法在于用ColQwen2将图像和文本统一到同一个向量空间中，实现跨模态的检索问答，等于是为处理复杂文档以及构建更智能的RAG系统提供了新思路

</span>
<span class="r-18u37iz"><a dir="ltr" href="https://x.com/hashtag/RAG?src=hashtag_click" role="link" class="css-1jxf684 r-bcqeeo r-1ttztb7 r-qvutc0 r-poiln3 r-1loqt21">#RAG</a>
</span>
<span class="css-1jxf684 r-bcqeeo r-1ttztb7 r-qvutc0 r-poiln3"> </span>
<span class="r-18u37iz"><a dir="ltr" href="https://x.com/hashtag/%E5%A4%9A%E6%A8%A1%E6%80%81RAG?src=hashtag_click"
  role="link" class="css-1jxf684 r-bcqeeo r-1ttztb7 r-qvutc0 r-poiln3 r-1loqt21">#多模态RAG</a>
</span>
<!--EndFragment-->![enter description here](./images/1756836556517.png)