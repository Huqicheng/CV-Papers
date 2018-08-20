# CV-Papers

## 1. Consensus Maximization for Semantic Region Correspondence

设计了一个全局最优的Semantic Region Correspondence解的架构，基于MI-SDP以及使用BnB Strategy 来遍历及prune解空间。

## 2. PointNetVlad

使用端到端学习匹配两个3D点阵，设计思路比较巧妙。

triplet loss（anchor, positive, negative）, maximize the distance between anchor and negative and minimize the distance between anchor and positive.

quadruplet loss (anchor, positive, negative, negative*) where negative* is the sample randomly sampled from the dataset at each iteration and is dissimilar to all point clouds in (anchor, positive, negative).

## 3. Convolutional Seq2Seq Model for Human Dynamics

基于 rnn 的人类motion预测结构，loss参考了GAN的策略，所以就有了用seq 生成（g） seq的


#### Note: 2和3的亮点主要在设计了很有效的loss，网络结构上并没有啥很创新的地方。
