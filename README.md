# Adversarial-attacks

本仓库为个人学习时的论文简要笔记，仅用于个人学习。


## 1. 《**Intriguing properties of neural networks**》[[ICLR2014]](https://arxiv.org/abs/1312.6199)

​	提出<font style="color:red">**对抗样本**</font>概念和<font style="color:red">**Box-constrained L-BFGS**</font>方法，通过最小化回归误差训练得到对抗扰动。

​	1）高维的神经元个体和其线性组合没有区别。

​	2）深度神经网络不是连续的，所以存在对抗样本。

​	3）对抗样本在不用模型间具有迁移性。



## 2. 《EXPLAINING AND HARNESSING》[[ICLR2015]](https://arxiv.org/abs/1412.6572)

​	提出了<font style="color:red">**Fast Gradient Sign Method (FGSM)**</font>方法，第一次将<font style="color:red">**对抗扰动写入损失表达式**</font>进行对抗训练，提升了模型鲁棒性。

​	1）对抗样本是高维空间线性点积的产物，而不非线性导致的。

​	2）不同模型间对抗样本的迁移性可解释为对抗扰动和高位权重向量的对齐效应，不同的模型处理相同任务时权重趋同于学习相似的	函数，这导致对抗扰动可能同时对齐于多个模型权重。

​	3）对抗扰动有正则化效应，甚至强于dropout，weight-decay和L1范数正则。



