### [A Dual Reinforcement Learning Framework for Unsupervised Text Style Transfer](https://arxiv.org/pdf/1905.10060.pdf)

非平行数据。通过从x转换到y'，再从y'转换到x'。使用了两个loss，一个衡量y'与目标风格的相似度（风格迁移），另一个衡量x'与x的相似度（内容保留）。

训练方式：1）从x开始，得到y'来评价style，从y'转回来，评价content。2）类似1，但是是从y'开始

其中，style classifer是pretrain的二分类器，在训练过程中固定。content的做法：*Therefore, we can estimate how much the content preserved in y0 by means of the probability that the model g reconstructs x when taking y0
as input.*

### [Controllable Unsupervised Text Attribute Transfer via Editing Entangled Latent Representation](https://arxiv.org/pdf/1905.12926.pdf)

分为3个部分。z=Encoder(x)；y=Classifier(z);x'=Decoder(z)。encoder是基于transformer的。
