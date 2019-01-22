# Mark

## 1. 论文（及代码）
### :smile: 1.1 传统视觉 SLAM (侧重前端)
#### :white_check_mark: **PTAM**
  + 论文：Klein G, Murray D. [**Parallel tracking and mapping for small AR workspaces**](http://www.robots.ox.ac.uk/ActiveVision/Publications/klein_murray_ismar2007/klein_murray_ismar2007.pdf)[C]//Mixed and Augmented Reality, 2007. ISMAR 2007. 6th IEEE and ACM International Symposium on. IEEE, **2007**: 225-234.
  + 代码：https://github.com/Oxford-PTAM/PTAM-GPL
  + 工程地址：http://www.robots.ox.ac.uk/~gk/PTAM/
  + 作者其他研究：http://www.robots.ox.ac.uk/~gk/publications.html
    
#### :white_check_mark: **直接法：LSD-SLAM（TUM）**
  + 论文：Engel J, Schöps T, Cremers D. [**LSD-SLAM: Large-scale direct monocular SLAM**](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.646.7193&rep=rep1&type=pdf)[C]//European Conference on Computer Vision. Springer, Cham, **ECCV 2014**: 834-849.
  + 代码：https://github.com/tum-vision/lsd_slam
  + 资料：
    + 课题组网站：https://vision.in.tum.de/research/vslam/lsdslam?redirect=1
    + [LSD SLAM和ORB SLAM的对比](https://blog.csdn.net/OsgoodWu/article/details/79900277?utm_source=blogxgwz0)
#### :white_check_mark: **直接稀疏里程计：DSO（TUM）**
  + 论文：[**Direct Sparse Odometry**](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7898369) (J. Engel, V. Koltun, D. Cremers), In arXiv:1607.02565, **2016**.
  + 代码：https://github.com/JakobEngel/dso
  + 慕尼黑工业大学：https://vision.in.tum.de/research/vslam/dso
#### :white_check_mark: **高翔：LDSO 具有闭环的 DSO（TUM）**
  + 论文：[**LDSO: Direct Sparse Odometry with Loop Closure**](https://arxiv.org/abs/1808.01111) (X. Gao, R. Wang, N. Demmel, D. Cremers), In International Conference on Intelligent Robots and Systems (**IROS**), **2018**
  + 代码：https://github.com/tum-vision/LDSO
  + 慕尼黑工业大学：https://vision.in.tum.de/research/vslam/ldso

### :smile: 1.2 语义相关
#### :white_check_mark: **CNN 稠密三维语义建图**
  + 论文：   
    + **[SemanticFusion: Dense 3D Semantic Mapping with Convolutional Neural Networks](http://wp.doc.ic.ac.uk/bjm113/wp-content/uploads/sites/113/2017/07/SemanticFusion_ICRA17_CameraReady.pdf)**, _J. McCormac, A. Handa, A. J. Davison, and S. Leutenegger_, ICRA '17
    + **[ElasticFusion: Real-Time Dense SLAM and Light Source Estimation](http://www.thomaswhelan.ie/Whelan16ijrr.pdf)**, _T. Whelan, R. F. Salas-Moreno, B. Glocker, A. J. Davison and S. Leutenegger_, IJRR '16 
  + 代码：https://github.com/seaun163/semanticfusion
  + 视频：https://www.youtube.com/watch?v=cGuoyNY54kU
  + 介绍：用了ElasticFusion和caffe合成，实现了三维场景的语义分割，（YouTube的视频展示了它可以回环检测，畸形的椅子正常了，不知道是它的创新还是Elastic本身自带）
    + 仪器：Elastic本身需要Kinect深度图 
    + 软件：caffe 有训练好的model供下载 
    <center>
      <img src="https://github.com/wuxiaolang/Mark/blob/master/pic/paper_semantic/SemanticFusion.PNG?raw=true" title="SemanticFusion" width="400" />
    </center>

#### :white_check_mark: ORB-SLAM2 + 语义标签
+ 论文：Qi X, Yang S, Yan Y. [**Deep Learning Based Semantic Labelling of 3D Point Cloud in Visual SLAM**](http://iopscience.iop.org/article/10.1088/1757-899X/428/1/012023/pdf)[C]//IOP Conference Series: Materials Science and Engineering. IOP Publishing, **2018**, 428(1): 012023.
+ 代码：https://github.com/qixuxiang/orb-slam2_with_semantic_label
+ 视频：http://v.youku.com/v_show/id_XMzYyOTMyODM2OA

#### :white_check_mark: Semantic SLAM(法国ENSTA学校)
+ 介绍：法国ENSTA学校的学生做的研究项目 , 做的基于ros的稠密语义建图, slam部分用的**orbslam**, **分割部分用的PSPNet50**, **地图表达有OctoMap和PCL两种**形式
+ 代码：https://github.com/floatlazer/semantic_slam
+ 视频：https://www.youtube.com/watch?v=IwQaRnFmRuU&feature=youtu.be
![](https://github.com/floatlazer/semantic_slam/raw/master/docs/images/rgb.png)

#### :white_check_mark: ORB_SLAM2_SSD_Semantic
+ 介绍：**动态**语义SLAM **目标检测** + VSLAM+光流/多视角几何动态物体检测+ **octomap地图** + 目标数据库 **orbslam2** 基础上做**语义地图**
+ 代码：https://github.com/Ewenwan/ORB_SLAM2_SSD_Semantic
![](https://github.com/Ewenwan/ORB_SLAM2_SSD_Semantic/blob/master/global-pcl.png?raw=true)

#### :white_check_mark: DS-SLAM
+ 介绍：文章提出了一种实时的动态语义SLAM系统, DS-SLAM, 可以减少运动目标对位姿估计的影响, 同时提供**基于八叉树的3D稠密语义地图**. 在DS-SLAM中, 一共有5个并行运行的线程: **跟踪、语义分割、局部建图、闭环检测和密集语义地图构建**。文章结合实时的语义分割网络SegNet和基于光流的运动一致性检验, 剔除场景中动态的部分, 比如行走的人. 然后将匹配的特征点从检测到的动态区域中剔除，从而提高动态场景的鲁棒性和准确性。基于八叉树的3D稠密语义地图使用 log-odds score 方法剔除不稳定的体素, 可用于机器人的导航和复杂任务。在TUM RGB-D数据集和现实环境中进行了实验。结果表明，在高动态环境下， DS-SLAM在精度和鲁棒性方面明显优于orb - slam。
+ 代码：https://github.com/ivipsourcecode/DS-SLAM

### :smile: 1.3 深度学习相关
#### :white_check_mark: **LayoutNet：从单张 RGB 图像中恢复室内 3D 环境**
  + 论文：Zou C, Colburn A, Shan Q, et al. [**LayoutNet: Reconstructing the 3D Room Layout from a Single RGB Image**](http://openaccess.thecvf.com/content_cvpr_2018/papers/Zou_LayoutNet_Reconstructing_the_CVPR_2018_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. **CVPR 2018**: 2051-2059.
  + **代码**：https://github.com/zouchuhang/LayoutNet
  <center>
  <img src="https://github.com/zouchuhang/LayoutNet/raw/master/figs/teasor.jpg" title="SemanticFusion" width="400" />
  </center>
  
### :smile: 1.4 稠密建图相关
#### :white_check_mark: **BundleFusion：识别表面 3D 重建**
  + 论文：Dai A, Nießner M, Zollhöfer M, et al. [**Bundlefusion: Real-time globally consistent 3d reconstruction using on-the-fly surface reintegration**](https://arxiv.org/pdf/1604.01093.pdf)[J]. ACM Transactions on Graphics (TOG), 2017, 36(4): 76a.
  + **代码**：https://github.com/niessner/BundleFusion
  + 工程地址：http://graphics.stanford.edu/projects/bundlefusion/
  + 简介：
  
#### :white_check_mark: **FlashFusion：CPU下实时稠密三维重建**
  + 论文：Han L, Fang L. [**FlashFusion: Real-time Globally Consistent Dense 3D Reconstruction using CPU Computing**](http://www.roboticsproceedings.org/rss14/p06.pdf)[C]. RSS, 2018.
  + **代码**：
  + 工程地址：http://www.luvision.net/FlashFusion/?tdsourcetag=s_pctim_aiomsg
  + 简介：清华-伯克利深圳学院

#### :white_check_mark: **单目稠密分段平面跟踪与建图：DPPTAM**
  + 论文：Concha Belenguer A, Civera Sancho J. [**DPPTAM: Dense piecewise planar tracking and mapping from a monocular sequence**](https://zaguan.unizar.es/record/36752/files/texto_completo.pdf)[C]//Proc. IEEE/RSJ Int. Conf. Intell. Rob. Syst. **2015** (ART-2015-92153).    
  + 代码：https://github.com/alejocb/dpptam
  + 相关研究：基于超像素的单目 SLAM：[**Using Superpixels in Monocular SLAM**](http://webdiis.unizar.es/~jcivera/papers/concha_civera_icra14.pdf) ICRA 2014
  + 谷歌学术：https://scholar.google.com/citations?user=GIaG3CsAAAAJ&hl=zh-CN&oi=sra
  
---
## 2. 算法、知识点与代码
+ :coffee: **消失点检测 vanishing point detection**
  + ！！！！论文：Lu X, Yaoy J, Li H, et al. [**2-Line Exhaustive Searching for Real-Time Vanishing Point Estimation in Manhattan World**](https://xiaohulugo.github.io/papers/Vanishing_Point_Detection_WACV2017.pdf)[C]//Applications of Computer Vision (WACV), **2017** IEEE Winter Conference on. IEEE, 2017: 345-353.
      + 代码：https://github.com/xiaohulugo/VanishingPointDetection
  + https://github.com/ankitdhall/Vanishing-Point-Detector

+ :coffee: **曼哈顿世界**
  + [CVPR 2014: A Mixture of Manhattan Frames: Beyond the Manhattan World](http://people.csail.mit.edu/jstraub/pub/A-Mixture-Of-Manhattan-Frames-Beyond-the-Manhattan-World/) 开源 MIT Julian Straub
  + [IROS 2015: Real-time Manhattan World Rotation Estimation in 3D](http://people.csail.mit.edu/jstraub/pub/A-Dirichlet-Process-Mixture-Model-for-Spherical-Data/) 开源 MIT Julian Straub
  + [TPAMI 2017: The Manhattan Frame Model-Manhattan World Inference in the Space of Surface Normals](http://people.csail.mit.edu/jstraub/pub/The-Manhattan-Frame-Model-Manhattan-World-Inference-in-the-Space-of-Surface-Normals/) 开源 MIT Julian Straub
+ :coffee: **倒角匹配**
  + 代码：https://github.com/s-trinh/Chamfer-Matching
+ :coffee: **无穷小平面姿态估计**
  + 代码：https://github.com/tobycollins/IPPE
+ :coffee: **3D 物体识别**
  + 代码：https://github.com/AmeyaWagh/3D_object_recognition
+ :coffee: **实时目标检测 YOLO**
  + 代码：https://github.com/qixuxiang/real_time_object_detect
+ :coffee: **ORB-SLAM2 地图保存**
  + 代码：https://github.com/BoomFan/ORB_SLAM2
  + 博客：https://blog.csdn.net/qq_34254510/article/details/79969046
  
---
## 3. 工具
### 3.1 轨迹误差分析工具
  + 苏黎世大学rpg_trajectory_evaluation：https://github.com/uzh-rpg/rpg_trajectory_evaluation
  + EVO：https://github.com/MichaelGrupp/evo
---
## 4. 优秀作者与实验
+ :+1: **Julian Straub MIT,facebook VR 实验室**
  + [个人主页](http://people.csail.mit.edu/jstraub/) &emsp; [Google Scholar](https://scholar.google.com/citations?user=49_cCT8AAAAJ)  &emsp; [Github](https://github.com/jstraub)
  + 人工 3D 感知方面，曼哈顿世界，很多开源方案

+ :+1: **牛津大学 Duncan Frost（PTAM 课题组）**
  + [谷歌学术](https://scholar.google.com/citations?hl=zh-CN&user=P9l4zHIAAAAJ&view_op=list_works&citft=1&citft=3&email_for_op=wuxiaolang2008%40gmail.com&gmla=AJsN-F5JUKaudKfKc2WwYAX2Fi7vY79tDw1lxd5PEz6GCwuhMwGuAKJQWIa3bPQC96HsGSEB0PqkP40E4qZGFGCHTUeubA1gr-wDSGe7d88TQ5lS3FomXSNYeHs497MCaVDi-QL4E4gPHaFcFVgO2sFKeR7LWX0iHCd2O3SXGU50WSLNLpE1Q7imrzefjWOy71Haz9ZSofbFIjUiziPGKOCTa8on8yrkqelT_TD9_z2bxU_8YvuJYsVH5JYuW2aUBltffGPulT5sU80CQnfFyqpe3K-X6KC5uw)
  + github：
    + https://github.com/duncanfrost/PSLAM
    + https://github.com/duncanfrost/DenseDepth
  + 论文：
    + 博士论文：[**Long Range Monocular SLAM 2017**](https://ora.ox.ac.uk/objects/uuid:af38cfa6-fc0a-48ab-b919-63c440ae8774/download_file?file_format=pdf&safe_filename=thesis.pdf&type_of_work=Thesis)
    + [**Recovering Stable Scale in Monocular SLAM Using Object-Supplemented Bundle Adjustment**](https://ora.ox.ac.uk/objects/uuid:74aaa7b5-5b14-4feb-b672-fa1802a804c6/download_file?file_format=pdf&safe_filename=Frost%2Bet%2Bal.pdf&type_of_work=Journal+article)[J]. IEEE Transactions on Robotics, 2018
    + [**Direct Line Guidance Odometry**](https://ora.ox.ac.uk/objects/uuid:f8b6d16e-07b4-4432-bc6e-6dddccaca511/download_file?file_format=pdf&safe_filename=Direct%2Bline%2Bguidance%2Bodometry.pdf&type_of_work=Conference+item)[C]//2018 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2018
    + [**Object-aware bundle adjustment for correcting monocular scale drift**](http://www.robots.ox.ac.uk/~duncan/pdf/frost2016.pdf)[C]//Robotics and Automation (ICRA), 2016 IEEE International Conference on. IEEE, 2016

+ :+1: **Yoshikatsu NAKAJIMA (中島 由勝)**
  + 深度学习状态估计、语义分割、目标检测
  + [个人主页](http://hvrl.ics.keio.ac.jp/nakajima/)
  + 论文
    + Yoshikatsu Nakajima and Hideo Saito, [**Efficient Object-oriented Semantic Mapping with Object Detector**](http://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8579143), IEEE Access, Vol.7, pp.3206-3213, 2019
    + Yoshikatsu Nakajima and Hideo Saito, [**Simultaneous Object Segmentation and Recognition by Merging CNN Outputs from Uniformly Distributed Multiple Viewpoints**](http://search.ieice.org/bin/summary.php?id=e101-d_5_1308&category=D&year=2018&lang=E&abst=), IEICE Transactions on Information and Systems, Vol.E101-D, No.5, pp.1308-1316, 2018
    + Yoshikatsu Nakajima and Hideo Saito, [**Robust camera pose estimation by viewpoint classification using deep learning**](http://link.springer.com/article/10.1007/s41095-016-0067-z), Computational Visual Media (Springer), DOI 10.1007/s41095-016-0067-z, Vol.3, No.2, pp.189-198, 2017 [**Best Paper Award**]
    ![](http://hvrl.ics.keio.ac.jp/nakajima/img/access.png)

+ :+1: **Alejo Concha（苏黎世Oculus VR）**
  + 介绍：单目稠密建图，布局平面，超像素，曼哈顿世界
  + [个人主页](https://sites.google.com/view/alejoconcha/)  [谷歌学术](https://scholar.google.com/citations?user=GIaG3CsAAAAJ&hl=zh-CN&oi=sra)
  + [Github](https://github.com/alejocb)
  + 论文：
    + Marta Salas, Wajahat Hussain, Alejo Concha, Luis Montano, Javier Civera, J. M. M. Montiel.**Layout Aware Visual Tracking and Mapping (**[**pdf**](http://www.google.com/url?q=http%3A%2F%2Fwebdiis.unizar.es%2F~jcivera%2Fpapers%2Fsalas_etal_iros15.pdf&sa=D&sntz=1&usg=AFQjCNG-5QcfQ8D3PTPonvE9K9xpTtur7A)**) (**[**video 1**](https://youtu.be/Qor9dVRqrpQ)**) (**[**video 2**](https://youtu.be/TsEbJMmR348)**).** IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS15), Hamburg, Germany, 2015.
---
## 5. 资料
+ SLAM 最新研究更新 Recent_SLAM_Research ：https://github.com/YiChenCityU/Recent_SLAM_Research
+ 西北工大智能系统实验室 SLAM 培训：https://github.com/zdzhaoyong/SummerCamp2018
+ 
