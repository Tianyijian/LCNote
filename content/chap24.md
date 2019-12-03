# 第四章 Transformer

- 为什么用Transformer：顺序计算限制了模型的并行能力，长期依赖的存在
- Transformer的结构
  - Input Embedding
  - Position Embedding
  - self-attention
  - multi-head attention
  - add：使网络有效叠加，避免梯度消失
  - norm：不改变矩阵权重的情况下，实现矩阵的独立同分布
  - feed forward
  - output Embedding
  - Masked multi-head attention
- 总结
  - 解决长期依赖，并行性好
  - 粗暴抛弃RNN和CNN丧失了捕捉局部特征的能力
  - 失去的位置信息十分重要，加入位置编码只是权益之计