# OoD-papers
A place for storing thoughts on OoD papers.

###### 数据集

1. [OoD-Bench: Benchmarking and Understanding Out-of-Distribution Generalization Datasets and Algorithms](./notes/OoD-Bench.md) 对常见OoD数据集的分析, 给出了diversity/correlation shift两个评价指标
2. [The Many Faces of Robustness: A Critical Analysis of Out-of-Distribution Generalization](./notes/TheManyFacesofRobustness.md) 语义层面的OoD数据集 (材质, 拍摄过程, 模糊), 对现有方法的经验分析, DeepAugment (对自编码器过程进行随机扰动)

###### 数据增强

1. [The Many Faces of Robustness: A Critical Analysis of Out-of-Distribution Generalization](./notes/TheManyFacesofRobustness.md) 语义层面的OoD数据集 (材质, 拍摄过程, 模糊), 对现有方法的经验分析, DeepAugment (对自编码器过程进行随机扰动)
2. [RobustNet: Improving Domain Generalization in Urban-Scene Segmentation via Instance Selective Whitening](./notes/RobustNet.md) Whitening, 只考虑颜色/模糊程度的变化, 认为covariance矩阵中随augmentation变化较大的是style信息, 从而设计了一个whitening loss, 在segmentation任务上有较好性能
3. [Improve Unsupervised Domain Adaptation with Mixup Training](./notes/ImproveUnsupervisedDomainAdaptationwithMixupTraining.md) Mixup

