# Mark

## 1. 论文及代码
### 1.1 语义相关
+ **【CNN 稠密三维语义建图】**
  + 论文：   
    + **[SemanticFusion: Dense 3D Semantic Mapping with Convolutional Neural Networks](http://wp.doc.ic.ac.uk/bjm113/wp-content/uploads/sites/113/2017/07/SemanticFusion_ICRA17_CameraReady.pdf)**, _J. McCormac, A. Handa, A. J. Davison, and S. Leutenegger_, ICRA '17
    + **[ElasticFusion: Real-Time Dense SLAM and Light Source Estimation](http://www.thomaswhelan.ie/Whelan16ijrr.pdf)**, _T. Whelan, R. F. Salas-Moreno, B. Glocker, A. J. Davison and S. Leutenegger_, IJRR '16 
  + 代码：https://github.com/seaun163/semanticfusion
  + 视频：https://www.youtube.com/watch?v=cGuoyNY54kU
  + 介绍：用了ElasticFusion和caffe合成，实现了三维场景的语义分割，（YouTube的视频展示了它可以回环检测，畸形的椅子正常了，不知道是它的创新还是Elastic本身自带）
    + 仪器：Elastic本身需要Kinect深度图 
    + 软件：caffe 有训练好的model供下载 
![](https://github.com/wuxiaolang/Mark/blob/master/pic/paper_semantic/SemanticFusion.PNG?raw=true)
---
## 2. 工具
### 2.1 轨迹误差分析工具
  + 苏黎世大学rpg_trajectory_evaluation：https://github.com/uzh-rpg/rpg_trajectory_evaluation
  + EVO：https://github.com/MichaelGrupp/evo
