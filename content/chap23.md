# 第三章 Attention

- 传统encoder-decoder结构
- 传统的RNN结构的缺陷：编译器在翻译时仅依赖最后的隐藏状态，原句子很长时，编译器很难将所有信息编码成一个向量，可能无法捕捉所有细节。
- Attention机制的来源：对所摄入的场景的局部具有强烈的注意，而对其周围的场景进行弱化
- Encoder-Attention-Decoder：原先相同的语义中间表示C将会被替换会根据当下生成单词而不断变化的Ci
- Attention的本质思想：给定目标语言的元素query，计算和各个key之间的相关性，得到每个key对应value的权重系数，然后对value进行加权求和。
- Soft attention：在t时刻输出yt求上下文向量Ct时，为输入句子中的每一个单词都给出一个注意力概率
- Hard Attention：试图直接找到与输出yt多对应的源语言单词，而认为源语言其余单词对其概率为0
- Global attention：考虑编码器的所有隐藏层状态
- local attention：选择性关注于上下文所在的一个小窗口
- Self attention：内部元素之间的Attention机制，更容易捕捉句子中长距离的相互依赖特性，增加计算并行性
-  multi-head attention：多个self-Attention结合，每个head学到在不同表示空间的特征。