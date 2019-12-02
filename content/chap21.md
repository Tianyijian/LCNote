# 第一章 深度学习绪论

### 一. 深度学习介绍

深度学习三步：定义一个函数集合、函数的质量、挑选最好的函数

#### 定义一个函数集合

- 神经元：权重、偏置、激活函数
- 全连接前馈神经网络
- 给定参数定义一个函数，给定网络架构定义一个函数集合
- Deep意味着许多隐藏层，通用函数近似定理
- 输出层：softmax
- 应该用多少层，每层多少神经元：不断试错+直觉

#### 函数的质量

- 带标签的训练集、训练目标、Loss、Total Loss

#### 挑选最好的函数

- 找到网络参数最小化 Total loss：梯度下降
- 局部最小值：平坦区更新缓慢，陷入鞍点、陷入局部最小值
- 反向传播

### 二. 深度学习示例

准备数据——配置网络——训练网络——模型评估——模型预测

### 三. 深度学习技巧

- 训练集表现不佳：选择合适的loss，Mini-batch，新激活函数，调节学习率，增加冲量
- 测试集表现不佳(过拟合)：及时停止、dropout、正则化、网络架构