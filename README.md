# Mark

## 1. 论文及代码
### 1.1 传统视觉 SLAM
+ :white_check_mark: **直接法：LSD-SLAM（TUM）**
  + 论文：Engel J, Schöps T, Cremers D. [**LSD-SLAM: Large-scale direct monocular SLAM**](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.646.7193&rep=rep1&type=pdf)[C]//European Conference on Computer Vision. Springer, Cham, **ECCV 2014**: 834-849.
  + 代码：https://github.com/tum-vision/lsd_slam
  + 资料：
    + 课题组网站：https://vision.in.tum.de/research/vslam/lsdslam?redirect=1
    + [LSD SLAM和ORB SLAM的对比](https://blog.csdn.net/OsgoodWu/article/details/79900277?utm_source=blogxgwz0)
+ :white_check_mark: **直接稀疏里程计：DSO（TUM）**
  + 论文：[**Direct Sparse Odometry**](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7898369) (J. Engel, V. Koltun, D. Cremers), In arXiv:1607.02565, **2016**.
  + 代码：https://github.com/JakobEngel/dso
  + 慕尼黑工业大学：https://vision.in.tum.de/research/vslam/dso
+ :white_check_mark: **高翔：LDSO 具有闭环的 DSO（TUM）**
  + 论文：[**LDSO: Direct Sparse Odometry with Loop Closure**](https://arxiv.org/abs/1808.01111) (X. Gao, R. Wang, N. Demmel, D. Cremers), In International Conference on Intelligent Robots and Systems (**IROS**), **2018**
  + 代码：https://github.com/tum-vision/LDSO
  + 慕尼黑工业大学：https://vision.in.tum.de/research/vslam/ldso
### 1.2 语义相关
+ :white_check_mark: **CNN 稠密三维语义建图**
  + 论文：   
    + **[SemanticFusion: Dense 3D Semantic Mapping with Convolutional Neural Networks](http://wp.doc.ic.ac.uk/bjm113/wp-content/uploads/sites/113/2017/07/SemanticFusion_ICRA17_CameraReady.pdf)**, _J. McCormac, A. Handa, A. J. Davison, and S. Leutenegger_, ICRA '17
    + **[ElasticFusion: Real-Time Dense SLAM and Light Source Estimation](http://www.thomaswhelan.ie/Whelan16ijrr.pdf)**, _T. Whelan, R. F. Salas-Moreno, B. Glocker, A. J. Davison and S. Leutenegger_, IJRR '16 
  + 代码：https://github.com/seaun163/semanticfusion
  + 视频：https://www.youtube.com/watch?v=cGuoyNY54kU
  + 介绍：用了ElasticFusion和caffe合成，实现了三维场景的语义分割，（YouTube的视频展示了它可以回环检测，畸形的椅子正常了，不知道是它的创新还是Elastic本身自带）
    + 仪器：Elastic本身需要Kinect深度图 
    + 软件：caffe 有训练好的model供下载 
    <center>
      <img src="https://github.com/wuxiaolang/Mark/blob/master/pic/paper_semantic/SemanticFusion.PNG?raw=true" title="SemanticFusion" width="500" />
    </center>

---
## 2. 工具
### 2.1 轨迹误差分析工具
  + 苏黎世大学rpg_trajectory_evaluation：https://github.com/uzh-rpg/rpg_trajectory_evaluation
  + EVO：https://github.com/MichaelGrupp/evo
