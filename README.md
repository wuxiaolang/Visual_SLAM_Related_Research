# Mark

+ [**1.论文（及代码）**](https://github.com/wuxiaolang/Mark/blob/master/README.md#1-%E8%AE%BA%E6%96%87%E5%8F%8A%E4%BB%A3%E7%A0%81)
  + [**1.1 传统视觉 SLAM (侧重前端)**](https://github.com/wuxiaolang/Mark/blob/master/README.md#smile-11-%E4%BC%A0%E7%BB%9F%E8%A7%86%E8%A7%89-slam-%E4%BE%A7%E9%87%8D%E5%89%8D%E7%AB%AF)
  + [**1.2 语义相关**](https://github.com/wuxiaolang/Mark/blob/master/README.md#smile-12-%E8%AF%AD%E4%B9%89%E7%9B%B8%E5%85%B3)
  + [**1.3 深度学习相关**](https://github.com/wuxiaolang/Mark/blob/master/README.md#smile-13-%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E7%9B%B8%E5%85%B3)
  + [**1.4 稠密建图相关**](https://github.com/wuxiaolang/Mark/blob/master/README.md#smile-14-%E7%A8%A0%E5%AF%86%E5%BB%BA%E5%9B%BE%E7%9B%B8%E5%85%B3)
+ [**2. 算法、知识点与代码**](https://github.com/wuxiaolang/Mark/blob/master/README.md#2-%E7%AE%97%E6%B3%95%E7%9F%A5%E8%AF%86%E7%82%B9%E4%B8%8E%E4%BB%A3%E7%A0%81)
+ [**3. 工具**](https://github.com/wuxiaolang/Mark/blob/master/README.md#3-%E5%B7%A5%E5%85%B7)
+ [**4. 优秀作者与实验**](https://github.com/wuxiaolang/Mark/blob/master/README.md#4-%E4%BC%98%E7%A7%80%E4%BD%9C%E8%80%85%E4%B8%8E%E5%AE%9E%E9%AA%8C)
+ [**5.资料**](https://github.com/wuxiaolang/Mark/blob/master/README.md#5-%E8%B5%84%E6%96%99)
  

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
  
#### :white_check_mark: **Gomez-Ojeda R 点线SLAM**
  + **点线SVO**
      + 论文：Gomez-Ojeda R, Briales J, Gonzalez-Jimenez J. [**PL-SVO: Semi-direct Monocular Visual Odometry by combining points and line segments**](http://mapir.isa.uma.es/rgomez/publications/iros16plsvo.pdf)[C]//Intelligent Robots and Systems (IROS), 2016 IEEE/RSJ International Conference on. IEEE, **2016**: 4211-4216.
      + 代码：https://github.com/rubengooj/pl-svo
  + **双目点线里程计**
      + 论文：Gomez-Ojeda R, Gonzalez-Jimenez J. [**Robust stereo visual odometry through a probabilistic combination of points and line segments**](https://riuma.uma.es/xmlui/bitstream/handle/10630/11515/icra16rgo.pdf?sequence=1&isAllowed=y)[C]//**2016** IEEE International Conference on Robotics and Automation (**ICRA**). IEEE, 2016: 2521-2526.
      + 代码：https://github.com/rubengooj/stvo-pl
  + **双目点线SLAM**
      + 论文：Gomez-Ojeda R, Zuñiga-Noël D, Moreno F A, et al. [**PL-SLAM: a Stereo SLAM System through the Combination of Points and Line Segments**](https://arxiv.org/pdf/1705.09479.pdf)[J]. arXiv preprint arXiv:1705.09479, **2017**.
      + 代码：https://github.com/rubengooj/pl-slam
      
#### :white_check_mark: **基于滑动窗口滤波的R-VIO**
   + 论文：Zheng Huai and Guoquan Huang, [**Robocentric visual-inertial odometry**](https://arxiv.org/pdf/1805.04031.pdf), The International Journal of Robotics Research, Nov 2018
   + 代码：https://github.com/rpng/R-VIO

      
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
+ 其实就是 **meaningf maps** 这篇文章的魔改版. 论文大体思路和meaningf maps相同, SLAM部分用的orb-slam2, **目标检测换成了yolo-V3**, 点云分割没变. 论文的实验部分也写得比较简单, 只有定量结果, 没有定性结果, 并且不能实时运行.论文发表在IOP Conference Series Materials Science and Engineering, EI检索, 是一个**OA会议论文集**.
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

#### :white_check_mark: DynamicSemanticMapping
+ 基于**分割**和orbslam2 完成**动态场景**的**稠密重建**
+ **论文**：Kochanov D, Ošep A, Stückler J, et al. [**Scene flow propagation for semantic mapping and object discovery in dynamic street scenes**](http://web-info8.informatik.rwth-aachen.de/media/papers/paper_compressed.pdf)[C]//Intelligent Robots and Systems (IROS), 2016 IEEE/RSJ International Conference on. IEEE, **2016**: 1785-1792.
+ **代码**：https://github.com/ganlumomo/DynamicSemanticMapping
+ wiki有详细记录：https://github.com/ganlumomo/DynamicSemanticMapping/wiki
![](https://raw.githubusercontent.com/ganlumomo/DynamicSemanticMapping/master/wiki_materials/snapshot_Area_1_office_1.jpg)

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

#### :white_check_mark: **单目稠密建图的几篇文章**
  + Tateno K, Tombari F, Laina I, et al. [**CNN-SLAM: Real-time dense monocular SLAM with learned depth prediction**](http://openaccess.thecvf.com/content_cvpr_2017/papers/Tateno_CNN-SLAM_Real-Time_Dense_CVPR_2017_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition (**CVPR**). **2017**, 2.
  + Brasch N, Bozic A, Lallemand J, et al. [**Semantic Monocular SLAM for Highly Dynamic Environments**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8593828)[C]//2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (**IROS**). IEEE, **2018**: 393-400.
  + Hosseinzadeh M, Li K, Latif Y, et al. [**Real-Time Monocular Object-Model Aware Sparse SLAM**](https://arxiv.org/pdf/1809.09149.pdf)[J]. arXiv preprint arXiv:1809.09149, **2018**.
  + Sünderhauf N, Pham T T, Latif Y, et al. [**Meaningful maps with object-oriented semantic mapping**](https://arxiv.org/pdf/1609.07849.pdf)[C]//Intelligent Robots and Systems (**IROS**), 2017 IEEE/RSJ International Conference on. IEEE, **2017**: 5079-5085.
  + Yang X, Chen J, Wang Z, et al. [**Monocular Camera Based Real-Time Dense Mapping Using Generative Adversarial Network**](http://delivery.acm.org/10.1145/3250000/3240564/p896-yang.pdf?ip=219.216.73.1&id=3240564&acc=ACTIVE%20SERVICE&key=BF85BBA5741FDC6E%2E4183B12E3311CD37%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&__acm__=1548299726_a21229f36359160e246c0c03d8ffd0c0)[C]//2018 ACM Multimedia Conference on Multimedia Conference. ACM, **2018**: 896-904.

#### :white_check_mark: **orb_slam2-ElasticFusion**
  + 代码：https://github.com/mp3guy/ElasticFusion
```
一种离线SLAM获取三维图的方法(linux平台，ubuntu14.04测试）
1.在线跑orb_slam2,录制成oni格式的录像
2.离线对oni录像逐帧处理得到相机的位姿数据
3.将oni文件转换成为ElasticFusion支持的klg格式
4.将klg文件和位姿数据传递给ElasticFusion，fusion成图
编译
下载orb_slam2,(https://github.com/gaoxiang12/ORBSLAM2_with_pointcloud_map)，
添加两个cpp文件和一个yaml文件，修改CMakeLists.txt，编译ORBSLAM2_with_pointcloud_map。
下载ElasticFusion（https://github.com/mp3guy/ElasticFusion），替换两个cpp文件后编译ElasticFusion。
编译FormatConverter。
使用
cd ×××/ORB_SLAM2_modified
./Examples/RGB-D/rgbd_xtion_cc Vocabulary/ORBvoc.txt Examples/RGB-D/xtion.yaml 
./Examples/RGB-D/rgbd_xtion_cc_offline Vocabulary/ORBvoc.txt Examples/RGB-D/xtion.yaml test.oni
FormatConverter test.oni test.klg
cd ×××/ElasticFusion-master/GUI/build
./ElasticFusion -l test.klg -p trajectory.txt -ocl
```
#### :white_check_mark: **单目稠密建图-沈邵劼**
  + **论文**：Yang Z, Gao F, Shen S. [**Real-time monocular dense mapping on aerial robots using visual-inertial fusion**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7989529)[C]//2017 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2017: 4552-4559.
  + **代码**：https://github.com/dvorak0/VI-MEAN

#### :white_check_mark: **苏黎世单目稠密建图**
  + **论文**：Pizzoli M, Forster C, Scaramuzza D. [**REMODE: Probabilistic, monocular dense reconstruction in real time**](https://files.ifi.uzh.ch/rpg/website/rpg.ifi.uzh.ch/html/docs/ICRA14_Pizzoli.pdf)[C]//2014 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2014: 2609-2616.
  + **代码**：https://github.com/uzh-rpg/rpg_open_remode
  
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
### :key: 3.1 轨迹误差分析工具
  + 苏黎世大学rpg_trajectory_evaluation：https://github.com/uzh-rpg/rpg_trajectory_evaluation
  + EVO：https://github.com/MichaelGrupp/evo
  
### :key: 3.2 RVIZ 显示不同的可视化图像
  + Github：https://github.com/PickNikRobotics/rviz_visual_tools
  + 参考资料：https://blog.csdn.net/u013834525/article/details/80447931
  
---
## 4. 优秀作者与实验
+ :+1: **Julian Straub MIT,facebook VR 实验室**
  + [**个人主页**](http://people.csail.mit.edu/jstraub/) &emsp; [Google Scholar](https://scholar.google.com/citations?user=49_cCT8AAAAJ)  &emsp; [**Github**](https://github.com/jstraub)
  + 人工 3D 感知方面，曼哈顿世界，很多开源方案

+ :+1: **牛津大学 Duncan Frost（PTAM 课题组）**
  + [**谷歌学术**](https://scholar.google.com/citations?hl=zh-CN&user=P9l4zHIAAAAJ&view_op=list_works&citft=1&citft=3&email_for_op=wuxiaolang2008%40gmail.com&gmla=AJsN-F5JUKaudKfKc2WwYAX2Fi7vY79tDw1lxd5PEz6GCwuhMwGuAKJQWIa3bPQC96HsGSEB0PqkP40E4qZGFGCHTUeubA1gr-wDSGe7d88TQ5lS3FomXSNYeHs497MCaVDi-QL4E4gPHaFcFVgO2sFKeR7LWX0iHCd2O3SXGU50WSLNLpE1Q7imrzefjWOy71Haz9ZSofbFIjUiziPGKOCTa8on8yrkqelT_TD9_z2bxU_8YvuJYsVH5JYuW2aUBltffGPulT5sU80CQnfFyqpe3K-X6KC5uw)
  + **github**：
    + https://github.com/duncanfrost/PSLAM
    + https://github.com/duncanfrost/DenseDepth
  + **论文**：
    + 博士论文：[**Long Range Monocular SLAM 2017**](https://ora.ox.ac.uk/objects/uuid:af38cfa6-fc0a-48ab-b919-63c440ae8774/download_file?file_format=pdf&safe_filename=thesis.pdf&type_of_work=Thesis)
    + [**Recovering Stable Scale in Monocular SLAM Using Object-Supplemented Bundle Adjustment**](https://ora.ox.ac.uk/objects/uuid:74aaa7b5-5b14-4feb-b672-fa1802a804c6/download_file?file_format=pdf&safe_filename=Frost%2Bet%2Bal.pdf&type_of_work=Journal+article)[J]. IEEE Transactions on Robotics, 2018
    + [**Direct Line Guidance Odometry**](https://ora.ox.ac.uk/objects/uuid:f8b6d16e-07b4-4432-bc6e-6dddccaca511/download_file?file_format=pdf&safe_filename=Direct%2Bline%2Bguidance%2Bodometry.pdf&type_of_work=Conference+item)[C]//2018 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2018
    + [**Object-aware bundle adjustment for correcting monocular scale drift**](http://www.robots.ox.ac.uk/~duncan/pdf/frost2016.pdf)[C]//Robotics and Automation (ICRA), 2016 IEEE International Conference on. IEEE, 2016

+ :+1: **Yoshikatsu NAKAJIMA (中島 由勝)**
  + 深度学习状态估计、语义分割、目标检测
  + [**个人主页**](http://hvrl.ics.keio.ac.jp/nakajima/)
  + **论文**
    + Yoshikatsu Nakajima and Hideo Saito, [**Efficient Object-oriented Semantic Mapping with Object Detector**](http://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8579143), IEEE Access, Vol.7, pp.3206-3213, 2019
    + Yoshikatsu Nakajima and Hideo Saito, [**Simultaneous Object Segmentation and Recognition by Merging CNN Outputs from Uniformly Distributed Multiple Viewpoints**](http://search.ieice.org/bin/summary.php?id=e101-d_5_1308&category=D&year=2018&lang=E&abst=), IEICE Transactions on Information and Systems, Vol.E101-D, No.5, pp.1308-1316, 2018
    + Yoshikatsu Nakajima and Hideo Saito, [**Robust camera pose estimation by viewpoint classification using deep learning**](http://link.springer.com/article/10.1007/s41095-016-0067-z), Computational Visual Media (Springer), DOI 10.1007/s41095-016-0067-z, Vol.3, No.2, pp.189-198, 2017 [**Best Paper Award**]
    ![](http://hvrl.ics.keio.ac.jp/nakajima/img/access.png)

+ :+1: **Alejo Concha（苏黎世Oculus VR）**
  + 介绍：单目稠密建图，布局平面，超像素，曼哈顿世界
  + [**个人主页**](https://sites.google.com/view/alejoconcha/) &emsp; [**谷歌学术**](https://scholar.google.com/citations?user=GIaG3CsAAAAJ&hl=zh-CN&oi=sra)
  + [**Github**](https://github.com/alejocb)
  + 论文：
    + Marta Salas, Wajahat Hussain, Alejo Concha, Luis Montano, Javier Civera, J. M. M. Montiel.**Layout Aware Visual Tracking and Mapping (**[**pdf**](http://www.google.com/url?q=http%3A%2F%2Fwebdiis.unizar.es%2F~jcivera%2Fpapers%2Fsalas_etal_iros15.pdf&sa=D&sntz=1&usg=AFQjCNG-5QcfQ8D3PTPonvE9K9xpTtur7A)**) (**[**video 1**](https://youtu.be/Qor9dVRqrpQ)**) (**[**video 2**](https://youtu.be/TsEbJMmR348)**).** IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS15), Hamburg, Germany, 2015.
    
+ :+1: **波兹南理工大学移动机器人实验室**
  + 有很多基于**RGB-D平面**的稠密建图工作（但我想搞单目啊！！！）
  + **论文**：
      + Wietrzykowski J, Skrzypczyński P. [**A probabilistic framework for global localization with segmented planes**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8098672)[C]//Mobile Robots (ECMR), 2017 European Conference on. IEEE, **2017**: 1-6.
      + Wietrzykowski J, Skrzypczyński P. [**PlaneLoc: Probabilistic global localization in 3-D using local planar features**](https://www.sciencedirect.com/science/article/pii/S0921889018303701)[J]. Robotics and Autonomous Systems, **2019**.
      ![](https://ars.els-cdn.com/content/image/1-s2.0-S0921889018303701-gr9.jpg)
  + **开源代码**：
      + https://github.com/LRMPUT/PlaneSLAM
      + https://github.com/LRMPUT/PUTSLAM
      + https://github.com/LRMPUT/PlaneLoc

+ :+1: **Xiaohu Lu**
  + 俄亥俄州立大学在读博士
      + github：https://github.com/xiaohulugo
      + 相关作者：[Yahui Liu](https://scholar.google.com/citations?user=P8qd0rEAAAAJ&hl=zh-CN&oi=sra)
  + **消失点**检测
      + Lu X, Yaoy J, Li H, et al. [**2-Line Exhaustive Searching for Real-Time Vanishing Point Estimation in Manhattan World**](https://www.computer.org/csdl/proceedings/wacv/2017/4822/00/07926628.pdf)[C]//Applications of Computer Vision (WACV), 2017 IEEE Winter Conference on. IEEE, **2017**: 345-353.
      + 代码：https://github.com/xiaohulugo/VanishingPointDetection
  + **点云分割聚类**
      + Lu X, Yao J, Tu J, et al. [**PAIRWISE LINKAGE FOR POINT CLOUD SEGMENTATION**](https://www.isprs-ann-photogramm-remote-sens-spatial-inf-sci.net/III-3/201/2016/isprs-annals-III-3-201-2016.pdf)[J]. ISPRS Annals of Photogrammetry, Remote Sensing & Spatial Information Sciences, **2016**, 3(3).
      + 代码：https://github.com/xiaohulugo/PointCloudSegmentation
  + 点云中 **3D 线检测**
      + Lu X, Liu Y, Li K. [**Fast 3D Line Segment Detection From Unorganized Point Cloud**](https://arxiv.org/pdf/1901.02532.pdf)[J]. arXiv preprint arXiv:1901.02532, **2019**.
      + 代码：https://github.com/xiaohulugo/3DLineDetection
  + 曼哈顿结构化环境的**单目 SLAM**
      + Li H, Yao J, Bazin J C, et al. [**A monocular SLAM system leveraging structural regularity in Manhattan world**](http://cvrs.whu.edu.cn/projects/Struct-PL-SLAM/source/file/Struct_PL_SLAM.pdf)[C]//2018 IEEE International Conference on Robotics and Automation (**ICRA**). IEEE, **2018**: 2518-2525.

+ :+1: **澳大利亚机器人视觉中心 Yasir Latif**
  + [**机器人视觉中心**](https://www.roboticvision.org/)
  + 团队代表作：SLAM 的过去现在和未来，Meaningful Maps，平面物体路标，Rat SLAM，SeqSLAM
  + **Yasir Latif**：[**作者主页**](http://ylatif.github.io/) &emsp; [**谷歌学术**](https://scholar.google.com/citations?user=pGsO6EkAAAAJ&hl=zh-CN) 
  + **Lachlan Nicholson**：二次平面作为物体SLAM的路标  &emsp; [**谷歌学术**](https://scholar.google.com/citations?user=DkyLABAAAAAJ&hl=zh-CN&oi=sra) 
  + **Michael Milford**：Rat SLAM，SeqSLAM &emsp; [**谷歌学术**](https://scholar.google.com/citations?user=TDSmCKgAAAAJ&hl=zh-CN&oi=sra) 
  + **论文**：
      + Cadena C, Carlone L, Carrillo H, et al. [**Past, present, and future of simultaneous localization and mapping: Toward the robust-perception age**](https://arxiv.org/pdf/1606.05830.pdf)[J]. IEEE Transactions on Robotics, **2016**, 32(6): 1309-1332.
      + Sünderhauf N, Pham T T, Latif Y, et al. [**Meaningful maps with object-oriented semantic mapping**](https://arxiv.org/pdf/1609.07849.pdf)[C]//Intelligent Robots and Systems (IROS), 2017 IEEE/RSJ International Conference on. IEEE, **2017**: 5079-5085.
      + Hosseinzadeh M, Li K, Latif Y, et al. [**Real-Time Monocular Object-Model Aware Sparse SLAM**](https://arxiv.org/pdf/1809.09149.pdf)[J]. arXiv preprint arXiv:1809.09149, **2018**.实时单目目标-模型感知的稀疏SLAM
      + Hosseinzadeh M, Latif Y, Pham T, et al. [**Towards Semantic SLAM: Points, Planes and Objects**](https://arxiv.org/pdf/1804.09111.pdf)[J]. arXiv preprint arXiv:1804.09111, **2018**.基于二次曲面和平面的结构感知SLAM

+ :+1: **西班牙马拉加大学博士生：RubénGómezOjeda**
  + 计算机视觉和移动机器人专业，**点线 SLAM**；
  + [个人主页](http://mapir.isa.uma.es/mapirwebsite/index.php/people/164-ruben-gomez) &emsp; [谷歌学术](https://scholar.google.com/citations?user=7jne0V4AAAAJ&hl=zh-CN) &emsp; [Github](https://github.com/rubengooj)
  + 代表作：PL-SVO，stvo-pl，pl-slam
  
---
## 5. 资料
+ SLAM 最新研究更新 Recent_SLAM_Research ：https://github.com/YiChenCityU/Recent_SLAM_Research
+ 西北工大智能系统实验室 SLAM 培训：https://github.com/zdzhaoyong/SummerCamp2018
+ 
