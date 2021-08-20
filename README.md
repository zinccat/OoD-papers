# OoD-papers
A place for storing thoughts on OoD papers.

###### 数据集

1. [OoD-Bench: Benchmarking and Understanding Out-of-Distribution Generalization Datasets and Algorithms](./notes/OoD-Bench.md) 对常见OoD数据集的分析, 给出了diversity/correlation shift两个评价指标
2. [The Many Faces of Robustness: A Critical Analysis of Out-of-Distribution Generalization](./notes/TheManyFacesofRobustness.md) 语义层面的OoD数据集 (材质, 拍摄过程, 模糊), 对现有方法的经验分析, DeepAugment (对自编码器过程进行随机扰动)

###### 数据增强

1. [The Many Faces of Robustness: A Critical Analysis of Out-of-Distribution Generalization](./notes/TheManyFacesofRobustness.md) 语义层面的OoD数据集 (材质, 拍摄过程, 模糊), 对现有方法的经验分析, DeepAugment (对自编码器过程进行随机扰动)
2. [RobustNet: Improving Domain Generalization in Urban-Scene Segmentation via Instance Selective Whitening](./notes/RobustNet.md) (CVPR 2021) Whitening, 只考虑颜色/模糊程度的变化, 认为covariance矩阵中随augmentation变化较大的是style信息, 从而设计了一个whitening loss, 在segmentation任务上有较好性能
3. [Improve Unsupervised Domain Adaptation with Mixup Training](./notes/ImproveUnsupervisedDomainAdaptationwithMixupTraining.md) 暴力Mixup, intra/inter-domain input/feature都加上了mixup, 外加DANN

###### 探源

1. [Understanding the Failure Modes of Out-of-Distribution Generalization](./notes/UnderstandingtheFailureModesofOut-of-DistributionGeneralization.md)

###### 因果学习

1. [Toward Explainable and Stable Prediction](./notes/TowardExplainableandStablePrediction.md) Talk by Peng Cui

###### 分辨Domain

1. Domain-Adversarial Training of Neural Networks (DANN) 在分类准确的同时尽可能把环境分错, 优化问题可能解的不好
2. DecAug: Out-of-Distribution Generalization via Decomposed Feature Representation and Semantic Augmentation 相比DANN, 说明让模型做更准确的任务(分得更好)比不明确的任务效果更好

###### Pairing

1. DAIR: Data Augmented Invariant Regularization 在能够准确获得不同domain下样本对时, 通过简单的pairing loss即可在CMNIST上做得很好

###### Gradient Alignment

1. Domain Generalization via Gradient Surgery 同AND-mask, 只在各域梯度方向相同时进行更新, 不同时用随机噪声替代以避免神经元不被更新

###### Single Domain

1. Environment Inference for Invariant Learning (EIIL) ICML 2021 环境划分 在ERM易学到虚假特征时, 可以利用其划分环境供OoD算法学习, 在label noise较大的时候效果较好

