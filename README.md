# Visual_SLAM_Related_Research
> @Author：wuxiaolang    
@E-mail ：wuyanminmax@gmail.com

## 前言
&emsp;&emsp;以下收集的论文、代码等资料主要与本人的学习方向 **视觉 SLAM、增强现实** 相关。    
&emsp;&emsp;目前（2019年3月至今）**重点关注 VO、语义 SLAM**， 传感器融合、稠密建图也略有关注，所以资料的收集范围也与自己的兴趣比较一致，无法涵盖视觉 SLAM 的所有研究，**请谨慎参考**。   
`1. 开源代码` ：经典、优秀的开源工程    
`2. 算法与知识点` ：一些零散的知识点和算法    
`3. 工具` ：论文或实验用到的一些工具    
`4. 优秀作者与团队` ：在自己感兴趣领域比较**优秀的值得关注的团队或个人**    
`5. 资料` ：可供参考的资料或备忘    
`6. 论文` ：自己感兴趣方向的**最新论文**，大概**一个月一更新**（论文不一定好，主要以对现阶段的工作可能有用为收录原则，请谨慎参考）      
&emsp;&emsp;本仓库于 2019 年 3 月（研一下）开始整理（私密）。

## 目录
+ [**1.论文（开源代码）**](https://github.com/wuxiaolang/Mark/blob/master/README.md#1-%E8%AE%BA%E6%96%87%E5%8F%8A%E4%BB%A3%E7%A0%81)
  + [**1.1 传统视觉 SLAM (侧重前端)**](https://github.com/wuxiaolang/Mark/blob/master/README.md#smile-11-%E4%BC%A0%E7%BB%9F%E8%A7%86%E8%A7%89-slam-%E4%BE%A7%E9%87%8D%E5%89%8D%E7%AB%AF)
  + [**1.2 语义相关**](https://github.com/wuxiaolang/Mark/blob/master/README.md#smile-12-%E8%AF%AD%E4%B9%89%E7%9B%B8%E5%85%B3)
  + [**1.3 深度学习相关**](https://github.com/wuxiaolang/Mark/blob/master/README.md#smile-13-%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E7%9B%B8%E5%85%B3)
  + [**1.4 稠密建图相关**](https://github.com/wuxiaolang/Mark/blob/master/README.md#smile-14-%E7%A8%A0%E5%AF%86%E5%BB%BA%E5%9B%BE%E7%9B%B8%E5%85%B3)
  + [**1.5 物体级 SLAM**](https://github.com/wuxiaolang/Mark/blob/master/README.md#smile-15-%E7%89%A9%E4%BD%93%E7%BA%A7%E7%9A%84-slam)
    
+ [**2. 算法、知识点与代码**](https://github.com/wuxiaolang/Mark/blob/master/README.md#2-%E7%AE%97%E6%B3%95%E7%9F%A5%E8%AF%86%E7%82%B9%E4%B8%8E%E4%BB%A3%E7%A0%81)
+ [**3. 工具**](https://github.com/wuxiaolang/Mark/blob/master/README.md#3-%E5%B7%A5%E5%85%B7)
+ [**4. 优秀作者与团队**](https://github.com/wuxiaolang/Mark/blob/master/README.md#4-%E4%BC%98%E7%A7%80%E4%BD%9C%E8%80%85%E4%B8%8E%E5%AE%9E%E9%AA%8C)
+ [**5. 资料**](https://github.com/wuxiaolang/Mark/blob/master/README.md#5-%E8%B5%84%E6%96%99)
+ [**6. 论文（近期论文）**](https://github.com/wuxiaolang/Mark/blob/master/README.md#6-%E8%BF%91%E6%9C%9F%E8%AE%BA%E6%96%87%E6%8C%81%E7%BB%AD%E6%9B%B4%E6%96%B0)
  + [2019 年 03 月论文更新（13 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research/blob/master/README.md#2019-%E5%B9%B4-3-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B013%E7%AF%87)
  + [2019 年 04 月论文更新（17 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research/blob/master/README.md#2019-%E5%B9%B4-4-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B017%E7%AF%87)
  + [2019 年 05 月论文更新（51 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research/blob/master/README.md#2019-%E5%B9%B4-5-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B051%E7%AF%87)
  + [2019 年 06 月论文更新（21 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research/blob/master/README.md#2019-%E5%B9%B4-6-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B021%E7%AF%87)
  + [2019 年 07 月论文更新（36 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2019-%E5%B9%B4-7-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B036%E7%AF%87)
  + [2019 年 08 月论文更新（26 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2019-%E5%B9%B4-8-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B026%E7%AF%87)
  + [2019 年 09 月论文更新（24 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research/blob/master/README.md#2019-%E5%B9%B4-9-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B024-%E7%AF%87)
  + [2019 年 10 月论文更新（22 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research/blob/master/README.md#2019-%E5%B9%B4-10-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B022-%E7%AF%87)

---

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

#### :white_check_mark: **ORB-SLAM2 单目半稠密建图**
   + 博客：https://blog.csdn.net/heyijia0327/article/details/52464278
   + 代码：https://github.com/HeYijia/ORB_SLAM2
![](https://img-blog.csdn.net/20160909121926348)

#### :white_check_mark: **双目 PTAM**
  + 论文：Taihú Pire,Thomas Fischer, Gastón Castro, Pablo De Cristóforis, Javier Civera and Julio Jacobo Berlles. [**S-PTAM: Stereo Parallel Tracking and Mapping**](http://webdiis.unizar.es/~jcivera/papers/pire_etal_ras17.pdf). Robotics and Autonomous Systems, **2017**.
  + 代码：https://github.com/lrse/sptam
  + Castro G, Nitsche M A, Pire T, et al. [Efficient on-board Stereo SLAM through constrained-covisibility strategies](https://www.researchgate.net/profile/Gaston_Castro/publication/332147108_Efficient_on-board_Stereo_SLAM_through_constrained-covisibility_strategies/links/5cacb327a6fdccfa0e7c3e4b/Efficient-on-board-Stereo-SLAM-through-constrained-covisibility-strategies.pdf)[J]. Robotics and Autonomous Systems, 2019.

#### :white_check_mark: **大场景移动视觉跟踪与建图**
  + 论文：Ventura J, Höllerer T. [**Wide-area scene mapping for mobile visual tracking**](https://ieeexplore.ieee.org/abstract/document/6402531)[C]//2012 IEEE international symposium on mixed and augmented reality (ISMAR). IEEE, 2012: 3-12.
  + 代码：https://github.com/jonathanventura/vrlt
  + 作者其他研究 - 多相机：
    + 论文：Ventura J, Arth C, Lepetit V. [**An efficient minimal solution for multi-camera motion**](http://openaccess.thecvf.com/content_iccv_2015/papers/Ventura_An_Efficient_Minimal_ICCV_2015_paper.pdf)[C]//Proceedings of the IEEE International Conference on Computer Vision. 2015: 747-755.
    + 代码：https://github.com/jonathanventura/multi-camera-motion 
  
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

<center>
<img src="https://github.com/floatlazer/semantic_slam/raw/master/docs/images/rgb.png" title="" width="650" />
</center>

#### :white_check_mark: ORB_SLAM2_SSD_Semantic
+ 介绍：**动态**语义SLAM **目标检测** + VSLAM+光流/多视角几何动态物体检测+ **octomap地图** + 目标数据库 **orbslam2** 基础上做**语义地图**
+ 代码：https://github.com/Ewenwan/ORB_SLAM2_SSD_Semantic

<center>
<img src="https://github.com/Ewenwan/ORB_SLAM2_SSD_Semantic/blob/master/global-pcl.png?raw=true" title="" width="650" />
</center>

#### :white_check_mark: DynamicSemanticMapping
+ 基于**分割**和orbslam2 完成**动态场景**的**稠密重建**
+ **论文**：Kochanov D, Ošep A, Stückler J, et al. [**Scene flow propagation for semantic mapping and object discovery in dynamic street scenes**](http://web-info8.informatik.rwth-aachen.de/media/papers/paper_compressed.pdf)[C]//Intelligent Robots and Systems (IROS), 2016 IEEE/RSJ International Conference on. IEEE, **2016**: 1785-1792.
+ **代码**：https://github.com/ganlumomo/DynamicSemanticMapping
+ wiki有详细记录：https://github.com/ganlumomo/DynamicSemanticMapping/wiki

<center>
<img src="https://raw.githubusercontent.com/ganlumomo/DynamicSemanticMapping/master/wiki_materials/snapshot_Area_1_office_1.jpg" title="" width="650" />
</center>

#### :white_check_mark: DS-SLAM
+ 介绍：文章提出了一种实时的动态语义SLAM系统, DS-SLAM, 可以减少运动目标对位姿估计的影响, 同时提供**基于八叉树的3D稠密语义地图**. 在DS-SLAM中, 一共有5个并行运行的线程: **跟踪、语义分割、局部建图、闭环检测和密集语义地图构建**。文章结合实时的语义分割网络SegNet和基于光流的运动一致性检验, 剔除场景中动态的部分, 比如行走的人. 然后将匹配的特征点从检测到的动态区域中剔除，从而提高动态场景的鲁棒性和准确性。基于八叉树的3D稠密语义地图使用 log-odds score 方法剔除不稳定的体素, 可用于机器人的导航和复杂任务。在TUM RGB-D数据集和现实环境中进行了实验。结果表明，在高动态环境下， DS-SLAM在精度和鲁棒性方面明显优于orb - slam。
+ 代码：https://github.com/ivipsourcecode/DS-SLAM

#### :white_check_mark: Co-fusion：融合对物体的实时分割与跟踪
+ **论文**：Rünz M, Agapito L. [**Co-fusion: Real-time segmentation, tracking and fusion of multiple objects**](https://ieeexplore.ieee.org/abstract/document/7989518)[C]//2017 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2017: 4471-4478.
+ **代码**：https://github.com/martinruenz/co-fusion

### :smile: 1.3 深度学习相关
#### :white_check_mark: **LayoutNet：从单张 RGB 图像中恢复室内 3D 环境**
  + 论文：Zou C, Colburn A, Shan Q, et al. [**LayoutNet: Reconstructing the 3D Room Layout from a Single RGB Image**](http://openaccess.thecvf.com/content_cvpr_2018/papers/Zou_LayoutNet_Reconstructing_the_CVPR_2018_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. **CVPR 2018**: 2051-2059.
  + **代码**：https://github.com/zouchuhang/LayoutNet
  <center>
  <img src="https://github.com/zouchuhang/LayoutNet/raw/master/figs/teasor.jpg" title="SemanticFusion" width="400" />
  </center>
  
#### :white_check_mark: **ICRA 2019：Self-Supervised Ego-Motion Estimation**
  + 论文：Shen T, Luo Z, Zhou L, et al. [**Beyond Photometric Loss for Self-Supervised Ego-Motion Estimation**](https://arxiv.org/pdf/1902.09103.pdf)[J]. arXiv preprint arXiv:1902.09103, 2019.
  + **代码**：https://github.com/hlzz/DeepMatchVO
  <center>
  <img src="https://github.com/hlzz/DeepMatchVO/raw/master/data/demo_result.png" title="SemanticFusion" width="600" />
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
#### :white_check_mark: **单目稠密建图-沈邵劼团队**
  + **论文**：Yang Z, Gao F, Shen S. [**Real-time monocular dense mapping on aerial robots using visual-inertial fusion**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7989529)[C]//2017 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2017: 4552-4559.
  + **代码**：https://github.com/dvorak0/VI-MEAN

#### :white_check_mark: **苏黎世单目稠密建图**
  + **论文**：Pizzoli M, Forster C, Scaramuzza D. [**REMODE: Probabilistic, monocular dense reconstruction in real time**](https://files.ifi.uzh.ch/rpg/website/rpg.ifi.uzh.ch/html/docs/ICRA14_Pizzoli.pdf)[C]//2014 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2014: 2609-2616.
  + **原始开源代码**：https://github.com/uzh-rpg/rpg_open_remode
  + **与 ORB-SLAM2 结合版本**：https://github.com/ayushgaud/ORB_SLAM2  https://github.com/ayushgaud/ORB_SLAM2    
  
<center>
<img src="https://cloud.githubusercontent.com/assets/4923897/26147541/7f7feec8-3b11-11e7-8b4c-5458aa922709.png" title="" width="700" />
</center>

#### :white_check_mark: **RTAB-Map**
  + RTAB-Map (Real-Time Appearance-Based Mapping) is a **RGB-D, Stereo and Lidar** Graph-Based SLAM approach based on an incremental appearance-based **loop closure detector**. 
  + 代码：https://github.com/introlab/rtabmap
  + 主页：http://introlab.github.io/rtabmap/

### :smile: 1.5 物体级的 SLAM
#### :white_check_mark: **BundleFusion：识别表面 3D 重建**
  + 论文：Mu B, Liu S Y, Paull L, et al. [**Slam with objects using a nonparametric pose graph**](https://arxiv.org/pdf/1704.05959.pdf)[C]//**2016** IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, 2016: 4602-4609.
  + 需要 caffe-fast-rcnn
  + **代码**：https://github.com/BeipengMu/objectSLAM
  + 视频：https://www.youtube.com/watch?v=YANUWdVLJD4&feature=youtu.be

---
## 2. 算法、知识点与开源库
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
+ :coffee: **关注截断面和欧几里得符号随机场的体素建图开源库**
  + 代码：https://github.com/ethz-asl/voxblox
  
---
## 3. 工具
### :key: 3.1 轨迹误差分析工具
  + 苏黎世大学rpg_trajectory_evaluation：https://github.com/uzh-rpg/rpg_trajectory_evaluation
  + EVO：https://github.com/MichaelGrupp/evo
  
### :key: 3.2 RVIZ 显示不同的可视化图像
  + Github：https://github.com/PickNikRobotics/rviz_visual_tools
  + 参考资料：https://blog.csdn.net/u013834525/article/details/80447931

### :key: 3.3 .obj 文件加载库
  + Github：https://github.com/syoyo/tinyobjloader

### :key: 3.4 .三维点云数据处理库
  + Github：http://geometryhub.net/bgl

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
  + 有很多基于**RGB-D平面**的稠密建图工作
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
  + [**个人主页**](http://mapir.isa.uma.es/mapirwebsite/index.php/people/164-ruben-gomez) &emsp; [**谷歌学术**](https://scholar.google.com/citations?user=7jne0V4AAAAJ&hl=zh-CN) &emsp; [**Github**](https://github.com/rubengooj)
  + 代表作：PL-SVO，stvo-pl，pl-slam

+ :+1: **法国运输，规划和网络科学与技术研究所博士：Nicolas Antigny**
  + 主要研究城市环境下**单目 SLAM**，基于场景和已知物体的**大环境增强现实**，传感器融合
  + [**researchgate**](https://www.researchgate.net/profile/Nicolas_Antigny) &emsp; [**YouTube**](https://www.youtube.com/channel/UC7zmj2Eonwi5kCfoe1r68dA/featured)

+ :+1: **三星 AI 实验室（莫斯科）：Alexander Vakhitov**
  + 点线融合
  + **个人主页**：https://sites.google.com/site/alexandervakhitov/
  + 相关**论文**：
    + Vakhitov A, Lempitsky V. [**Learnable Line Segment Descriptor for Visual SLAM**](https://ieeexplore.ieee.org/abstract/document/8651490/)[J]. IEEE Access, **2019**.
    + Vakhitov A, Lempitsky V, Zheng Y. [**Stereo relative pose from line and point feature triplets**](http://openaccess.thecvf.com/content_ECCV_2018/html/Alexander_Vakhitov_Stereo_relative_pose_ECCV_2018_paper.html)[C]//Proceedings of the European Conference on Computer Vision (ECCV). 2018: 648-663.
    + Pumarola A, Vakhitov A, Agudo A, et al. [**PL-SLAM: Real-time monocular visual SLAM with points and lines**](https://ieeexplore.ieee.org/abstract/document/7989522)[C]//2017 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2017: 4503-4508.
    + Vakhitov A, Funke J, Moreno-Noguer F. [**Accurate and linear time pose estimation from points and lines**](https://link.springer.com/chapter/10.1007/978-3-319-46478-7_36)[C]//European Conference on Computer Vision. Springer, Cham, 2016: 583-599.
  + **Github**：https://github.com/alexander-vakhitov

+ :+1: **苏黎世联邦理工学院计算机视觉与几何实验室：Prof. Marc Pollefeys**
  + 三维语义重建、多相机协同 SLAM 
  + 实验室主页：http://www.cvg.ethz.ch/people/faculty/ 
  + 实验室博士：http://people.inf.ethz.ch/liup/ ， http://people.inf.ethz.ch/sppablo/ ， http://people.inf.ethz.ch/schoepst/publications/ ， https://www.nsavinov.com/ , http://people.inf.ethz.ch/cian/Publications/

+ :+1: **香港中文大学机器人、感知与 AI 实验室**
  + 实验室主页：http://www.ee.cuhk.edu.hk/~qhmeng/research.html
  + 动态 SLAM ，医疗服务型机器人

+ :+1: **微软高级工程师、苏黎世联邦理工：Johannes L. Schönberger**
  + 主要研究：基于图像的 3D 建模、 SFM、立体视觉、语义
  + [**个人主页**](https://demuc.de/)&emsp;[**谷歌学术**](https://scholar.google.com/citations?user=MlcMCd0AAAAJ&hl=zh-CN&oi=sra)
  + 主要文章：
    + [VSO: Visual Semantic Odometry](https://demuc.de/papers/lianos2018vso.pdf)
    + [Semantic Visual Localization](https://demuc.de/papers/schoenberger2018semantic.pdf)
    + [Structure-from-Motion Revisited](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Schonberger_Structure-From-Motion_Revisited_CVPR_2016_paper.pdf)

+ :+1: **美国犹他大学计算机学院：Srikumar Ramalingam**
  + 主要研究：三维重建、语义分割、视觉 SLAM、图像定位、深度学习
  + [**个人主页**](https://www.cs.utah.edu/~srikumar/)&emsp;[**谷歌学术**](https://scholar.google.com/citations?user=6m1ptOgAAAAJ&hl=zh-CN&oi=sra)
  + 主要文章：
    + ICRA 2013 [Point-plane SLAM for hand-held 3D sensors](https://merl.com/publications/docs/TR2013-031.pdf)
    + CVPR 2019 [Minimal Solvers for Mini-Loop Closures in 3D Multi-Scan Alignment](https://arxiv.org/pdf/1904.03941.pdf)

+ :+1: **德国马克斯普朗克智能系统研究所：Jörg Stückler**
  + 主要研究：三维感知、深度学习
  + [实验室主页](https://ev.is.tuebingen.mpg.de/)&emsp;[**谷歌学术**](https://scholar.google.com/citations?user=xrOzfucAAAAJ&hl=zh-CN&oi=sra)
  + 主要文章：
    + 2015:[Large-scale direct SLAM with stereo cameras](https://ieeexplore.ieee.org/abstract/document/7353631)
    + 2019:[EM-Fusion: Dynamic Object-Level SLAM with Probabilistic Data Association](https://arxiv.org/pdf/1904.11781.pdf)

+ :+1: **麻省理工学院航空航天控制实验室**
  + 主要研究：飞机，航天器和地面车辆的自动系统和控制设计相关
  + [实验室主页](http://acl.mit.edu/publications)
  + 主要文章：
    + Mu B, Liu S Y, Paull L, et al. [**Slam with objects using a nonparametric pose graph**](https://arxiv.org/pdf/1704.05959.pdf)[C]//2016 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2016**: 4602-4609.
    + ICRA 2019：Robust Object-Based SLAM for High-Speed Autonomous Navigation    
    + ICRA 2019：[Efficient Constellation-Based Map-Merging for Semantic SLAM](https://arxiv.org/pdf/1809.09646.pdf)    
    + IJRR 2018：[Reliable Graphs for SLAM](http://web.mit.edu/~mrrobot/filez/ijrr17.pdf)    
    + [Resource-aware collaborative SLAM](http://acl.mit.edu/projects/resource-aware-collaborative-slam)    
    
---

## 5. 资料
+ SLAM 最新研究更新 Recent_SLAM_Research ：https://github.com/YiChenCityU/Recent_SLAM_Research
+ 西北工大智能系统实验室 SLAM 培训：https://github.com/zdzhaoyong/SummerCamp2018

---

## 6. 近期论文（持续更新）

### 2019 年 3 月论文更新（13 篇）

+ [ ] **[1]** Han L, Gao F, Zhou B, et al. [**FIESTA: Fast Incremental Euclidean Distance Fields for Online Motion Planning of Aerial Robots**](https://arxiv.org/abs/1903.02144)[J]. arXiv preprint arXiv:1903.02144, **2019**.
    + 基于快速**增量式欧氏距离场**的飞行器实时运动规划
    + 沈邵劼老师团队
+ [x] **[2]** ICRA **2019** ：[**Multimodal Semantic SLAM with Probabilistic Data Association**](https://marinerobotics.mit.edu/multimodal-semantic-slam-probabilistic-data-association)
    + 具有概率数据关联的**多模态语义SLAM**
    + 麻省理工学院海洋机器人团队
+ [x] **[3]** Zhang F, Rui T, Yang C, et al. [**LAP-SLAM: A Line-Assisted Point-Based Monocular VSLAM**](https://www.mdpi.com/2079-9292/8/2/243/htm)[J]. **Electronics**, **2019**, 8(2): 243.
    + **线辅助**的点 SLAM
    + 解放军陆军工程大学
+ [ ] **[4]** Zhang H, Jin L, Zhang H, et al. [**A Comparative Analysis of Visual-Inertial SLAM for Assisted Wayfinding of the Visually Impaired**](https://ieeexplore.ieee.org/abstract/document/8658410)[C]//2019 IEEE Winter Conference on Applications of Computer Vision (**WACV**). IEEE, **2019**: 210-217.
    + **VI-SLAM** 辅助寻径对比分析
    + 弗吉尼亚联邦大学
+ [x] **[5]** Chen Z, Liu L. [**Creating Navigable Space from Sparse Noisy Map Points**](https://arxiv.org/pdf/1903.01503.pdf)[J]. arXiv preprint arXiv:1903.01503, **2019**.
    + 从**稀疏地图点**中创建**可导航**空间
+ [x] **[6]** Antigny N, Uchiyama H, Servières M, et al. [**Solving monocular visual odometry scale factor with adaptive step length estimates for pedestrians using handheld devices**](https://www.mdpi.com/1424-8220/19/4/953)[J]. **Sensors**, **2019**, 19(4): 953.
    + 行人步长估计辅助**单目手持式视觉里程计尺度估计** **城市环境 AR**应用
    + 法国运输\规划和网络科学与技术研究所，[**researchgate**](https://www.researchgate.net/profile/Nicolas_Antigny) &emsp; [**YouTube**](https://www.youtube.com/channel/UC7zmj2Eonwi5kCfoe1r68dA/featured)
+ [x] **[7]** Zhou D, Dai Y, Li H. [**Ground Plane based Absolute Scale Estimation for Monocular Visual Odometry**]()[J]. arXiv preprint arXiv:1903.00912, **2019**.
    + 基于地平面的**单目 SLAM 绝对尺度估计**
    + 百度
+ [ ] **[8]** Duong N D, Kacete A, Soladie C, et al. [**Accurate Sparse Feature Regression Forest Learning for Real-Time Camera Relocalization**](https://ieeexplore.ieee.org/abstract/document/8491017)[C]//2018 International Conference on 3D Vision (3DV). IEEE, **2018**: 643-652.
    + 基于随机森林学习的实时**相机重定位**
    + [视频](https://www.youtube.com/watch?v=2oOL-BSemmQ&feature=youtu.be)
+ [ ] **[9]** Patra S, Gupta K, Ahmad F, et al. [**EGO-SLAM: A Robust Monocular SLAM for Egocentric Videos**](https://ieeexplore.ieee.org/abstract/document/8658783/)[C]//2019 IEEE Winter Conference on Applications of Computer Vision (WACV). IEEE, **2019**: 31-40.
    + **视频序列**鲁棒的**单目 SLAM**
    + 印度理工学院
+ [x] **[10]** Rosinol A, Sattler T, Pollefeys M, et al. [**Incremental Visual-Inertial 3D Mesh Generation with Structural Regularities**](https://arxiv.org/pdf/1903.01067.pdf)[J]. arXiv preprint arXiv:1903.01067, **2019**.
    + 增量式 VI-SLAM **三维网格**生成
    + 麻省理工学院信息与决策系统实验室，[项目主页](https://www.mit.edu/~arosinol/research/struct3dmesh.html)
+ [ ] **[11]** Wang Z. [**Structure from Motion with Higher-level Environment Representations**](https://openresearch-repository.anu.edu.au/handle/1885/157021)[J]. **2019**.
    + 具有**高级环境**表示的 **SFM**
    + 澳大利亚国立大学 硕士学位
+ [x] **[12]** Vakhitov A, Lempitsky V. [**Learnable Line Segment Descriptor for Visual SLAM**](https://ieeexplore.ieee.org/abstract/document/8651490)[J]. IEEE Access, **2019**.
    + 视觉SLAM中的可学习**线段描述**，基于 ORB-SLAM2
    + Samsung AI Center, Moscow
+ [ ] **[13]** Grinvald M, Furrer F, Novkovic T, et al. [**Volumetric Instance-Aware Semantic Mapping and 3D Object Discovery**](https://arxiv.org/abs/1903.00268)[J]. arXiv preprint arXiv:1903.00268, **2019**.
    + **语义**感知建图与**三维物体探索**，基于 mask-RCNN
    + 苏黎世联邦理工学院

---

### 2019 年 4 月论文更新（17 篇）

+ [x] **[1]** Rambach J, Lesur P, Pagani A, et al. [**SlamCraft: Dense Planar RGB Monocular SLAM**](https://www.researchgate.net/profile/Jason_Rambach/publication/331832804_SlamCraft_Dense_Planar_RGB_Monocular_SLAM/links/5c8f6a9a299bf14e7e82d880/SlamCraft-Dense-Planar-RGB-Monocular-SLAM.pdf)[C]. International Conference on Machine Vision Applications MVA **2019**.
    + SlamCraft：**单目平面稠密** SLAM
    + 德国人工智能研究中心 &emsp;[**作者主页**](https://av.dfki.de/members/rambach/) &emsp;[**谷歌学术**](https://scholar.google.com/citations?user=1l4G16AAAAAJ&hl=zh-CN&authuser=1&oi=sra) &emsp;**增强现实**应用
+ [ ] **[2]** Liu C, Yang J, Ceylan D, et al. [**Planenet: Piece-wise planar reconstruction from a single rgb image**](http://openaccess.thecvf.com/content_cvpr_2018/papers/Liu_PlaneNet_Piece-Wise_Planar_CVPR_2018_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. **CVPR 2018**: 2579-2588.
    + **PlaneNet**：从单张 RGB 图像进行**平面重构**
    + 华盛顿大学 &emsp;[**谷歌学术**](https://scholar.google.com/citations?user=Jy3u1_wAAAAJ&hl=zh-CN&authuser=1&oi=sra)  &emsp;[**Github 代码开源**](https://github.com/art-programmer/PlaneNet) 
+ [ ] **[3]** Weng X, Kitani K. [**Monocular 3D Object Detection with Pseudo-LiDAR Point Cloud**](https://arxiv.org/pdf/1903.09847.pdf)[J]. arXiv preprint arXiv:1903.09847, **2019**.
    + 利用伪激光点云进行单目 **3D 物体检测**
    + CMU  &emsp;[**谷歌学术**](https://scholar.google.com/citations?user=yv3sH74AAAAJ&hl=zh-CN&oi=sra) 
+ [ ] **[4]** Hassan M., Mohamed & Hemayed, Elsayed.. [**A Fast Linearly Back-End SLAM for Navigation Based on Monocular Camera**](https://www.researchgate.net/publication/331832850_A_Fast_Linearly_Back-End_SLAM_for_Navigation_Based_on_Monocular_Camera). International Journal of Civil Engineering and Technology **2018**. 627-645. 
    + 单目 SLAM 的快速**线性后端优化**
    + 埃及法尤姆大学
+ [ ] **[5]** Chen B, Yuan D, Liu C, et al. [**Loop Closure Detection Based on Multi-Scale Deep Feature Fusion**](https://www.mdpi.com/2076-3417/9/6/1120/htm)[J]. Applied Sciences, **2019**, 9(6): 1120.
    + 基于多尺度**深度特征融合**的**闭环检测**
    + 中南大学自动化学院
+ [x] **[6]** Ling Y, Shen S. [**Real‐time dense mapping for online processing and navigation**](https://onlinelibrary.wiley.com/doi/pdf/10.1002/rob.21868)[J]. Journal of Field Robotics.
    + 用于在线处理和导航的实时**密集建图**
    + **沈邵劼**老师团队 &emsp;[**Github 代码开源**](https://github.com/ygling2008/dense_mapping) 
+ [x] **[7]** Chen-Hsuan Lin, Oliver Wang et al.[**Photometric Mesh Optimization for Video-Aligned 3D Object Reconstruction**](https://arxiv.org/pdf/1903.08642.pdf)[C].IEEE Conference on Computer Vision and Pattern Recognition (**CVPR**), **2019**
    + 用于视频**三维物体重建**的光度网格优化
    + CMU 在读博士 &emsp;[**个人主页**](https://chenhsuanlin.bitbucket.io/) &emsp;[**Github 代码开源**](https://github.com/chenhsuanlin/photometric-mesh-optim)
+ [x] **[8]** Tang F, Li H, Wu Y. [**FMD Stereo SLAM: Fusing MVG and Direct Formulation Towards Accurate and Fast Stereo SLAM**](https://www.researchgate.net/publication/331198086_FMD_Stereo_SLAM_Fusing_MVG_and_Direct_Formulation_Towards_Accurate_and_Fast_Stereo_SLAM)[J]. **2019**.
    + 融合多视图几何与直接法的快速精准**双目 SLAM**
    + **中科院自动化研究所**，模式识别国家重点实验室，吴毅红团队
+ [ ] **[9]** Duff T, Kohn K, Leykin A, et al. [**PLMP-Point-Line Minimal Problems in Complete Multi-View Visibility**](https://arxiv.org/pdf/1903.10008.pdf)[J]. arXiv preprint arXiv:1903.10008, **2019**.
    + PLMP：多视图中的**点线最小化**
    + 佐治亚理工学院
+ [x] **[10]** Seong Hun Lee, Javier Civera. [**Loosely-Coupled Semi-Direct Monocular SLAM**](https://ieeexplore.ieee.org/abstract/document/8584894)[J] IEEE Robotics and Automation Letters. **2019**
    + 松耦合的**半直接法单目 SLAM**
    + 萨拉戈萨大学，[谷歌学术](https://scholar.google.com/citations?user=FeMFP7EAAAAJ&hl=zh-CN&oi=sra)，[**代码开源**](https://github.com/wuxiaolang/LCSD_SLAM)，[演示视频](https://www.youtube.com/watch?v=j7WnU7ZpZ8c&feature=youtu.be)
    + Lee S H, de Croon G. [**Stability-based scale estimation for monocular SLAM**](https://www.researchgate.net/profile/Seong_Hun_Lee3/publication/322260802_Stability-based_Scale_Estimation_for_Monocular_SLAM/links/5b3def9b0f7e9b0df5f42d67/Stability-based-Scale-Estimation-for-Monocular-SLAM.pdf)[J]. IEEE Robotics and Automation Letters, **2018**, 3(2): 780-787.
    + Lee S H, Civera J. [**Closed-Form Optimal Triangulation Based on Angular Errors**](https://arxiv.org/pdf/1903.09115.pdf)[J]. arXiv preprint arXiv:1903.09115, **2019**.
+ [x] **[11]** Delgado del Hoyo F J. [**Robust and affordable localization and mapping for 3D reconstruction. Application to architecture and construction**](http://uvadoc.uva.es/handle/10324/35078). **2018**.
    + 用于建筑行业稳健的 SLAM 与 **3D 重建**
    + 西班牙巴利亚多利德大学**博士学位论文**，[**代码开源**](https://gitlab.com/fradelg/kn-slam) (基于 ORB-SLAM2)
+ [x] **[12]** Jinyu Li, Bangbang Yang, Danpeng Chen, Nan Wang, Guofeng Zhang*, Hujun Bao*. [**Survey and Evaluation of Monocular Visual-Inertial SLAM Algorithms for Augmented Reality**](http://vr-ih.com/vrih/resource/latest_accept/267415796648960.pdf)[J] Journal of Virtual Reality & Intelligent Hardware **2019**.
    + 应用于**增强现实**的**单目 VI-SLAM** 算法调研与评估
    + 章国锋教授团队，[工程地址](http://www.zjucvg.net/eval-vislam/)，[Github-评估工具](https://github.com/zju3dv/eval-vislam)
+ [x] **[13]** Pablo Speciale, Johannes L. Schonberg, Sing Bing Kang. [**Privacy Preserving Image-Based Localization**](https://arxiv.org/pdf/1903.05572.pdf)[J] **2019**.
    + 利用**线云**进行基于图像的定位
    + **苏黎世**联邦理工、微软，[作者主页](http://people.inf.ethz.ch/sppablo/)，[工程地址](https://www.cvg.ethz.ch/research/secon/)
    + Speciale P, Pani Paudel D, Oswald M R, et al. **Consensus maximization with linear matrix inequality constraints**[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. **CVPR 2017**: 4941-4949. 最大化线性矩阵不等式约束 [[PDF](https://www.cvg.ethz.ch/research/conmax/paper/PSpeciale2017CVPR.pdf)] [[Code](https://www.cvg.ethz.ch/research/conmax/paper/PSpeciale2017CVPR_code_sample.tar.gz)] [[Video](https://www.youtube.com/watch?v=yV1wXknpG1U)] [[Project Page](https://www.cvg.ethz.ch/research/conmax)]
+ [ ] **[14]** Li M, Zhang W, Shi Y, et al. [**Bionic Visual-based Data Conversion for SLAM**](https://ieeexplore.ieee.org/abstract/document/8665130)[C]//2018 IEEE International Conference on Robotics and Biomimetics (**ROBIO**). IEEE, **2018**: 1607-1612.
    + 基于**仿生视觉**的 SLAM 数据转换
    + **北京理工大学**仿生机器人与系统教育部重点实验室
+ [ ] **[15]** Cheng J, Sun Y, Chi W, et al. [**An Accurate Localization Scheme for Mobile Robots Using Optical Flow in Dynamic Environments**](https://ieeexplore.ieee.org/abstract/document/8664893)[C]//2018 IEEE International Conference on Robotics and Biomimetics (**ROBIO**). IEEE, **2018**: 723-728.
    + **动态环境**下使用**光流**的移动机器人精确定位方案
    + **香港中文大学**，[**实验室主页**](http://www.ee.cuhk.edu.hk/~qhmeng/index.html)
+ [x] **[16]** Zichao Zhang, Davide Scaramuzza, [**Beyond Point Clouds: Fisher Information Field for Active Visual Localization**](https://www.ifi.uzh.ch/dam/jcr:5a26a3b4-ce01-4647-8cf6-f6a24e579a85/ICRA19_Zhang.pdf).[C], IEEE International Conference on Robotics and Automation (**ICRA**), **2019**.
    + **超越点云**:用于主动视觉定位的 Fisher 信息
    + 苏黎世大学张子潮，[视频](https://www.youtube.com/watch?v=q3YqIyaFUVE&feature=youtu.be)，[**代码开源**](https://github.com/uzh-rpg/rpg_information_field)，[项目主页](http://rpg.ifi.uzh.ch/research_active_vision.html)
+ [x] **[17]** Georges Younes, Daniel Asmar, John Zelek. [**A Unified Formulation for Visual Odometry**](https://arxiv.org/abs/1903.04253)[J]. arXiv preprint arXiv:1903.04253, **2019**.
    + 一种统一的**视觉里程计**方法
    + 加拿大滑铁卢大学，贝鲁特美国大学； [谷歌学术](https://scholar.google.com/citations?hl=zh-CN&user=4Xy_9NQAAAAJ)
    + Younes G, Asmar D, Shammas E, et al. [Keyframe-based monocular SLAM: design, survey, and future directions](https://www.sciencedirect.com/science/article/pii/S0921889017300647)[J]. Robotics and Autonomous Systems, **2017**, 98: 67-88.
    + 2018：[Fdmo: Feature assisted direct monocular odometry](https://arxiv.org/pdf/1804.05422.pdf)

---

### 2019 年 5 月论文更新（51 篇）

#### 1. Geometric SLAM
+ [x] **[1]** Delmas P, Gee T. [**Stereo camera visual odometry for moving urban environments**](https://content.iospress.com/articles/integrated-computer-aided-engineering/ica190598)[J]. Integrated Computer-Aided Engineering, **2019** (Preprint): 1-14.
    + <font color = blue>用于移动城市环境的双目里程计</font>
    + 奥克兰大学 &emsp; 中科院二区 JCR Q2
+ [ ] **[2]** Guo R, Zhou D, Peng K, et al. [**Plane Based Visual Odometry for Structural and Low-Texture Environments Using RGB-D Sensors**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8679500)[C]//**2019** IEEE International Conference on Big Data and Smart Computing (BigComp). IEEE, 2019: 1-4.
    + <font color = blue>用于结构化低纹理的平面 RGB-D 视觉里程计</font>
    + 国防科大
+ [ ] **[3]** X Wang, F Xue, Z Yan, W Dong, Q Wang, H Zha. [**Continuous-time Stereo Visual Odometry Based on Dynamics Model⋆**](https://www.researchgate.net/profile/Wang_Xin122/publication/332103736_Continuous-time_Stereo_Visual_Odometry_Based_on_Dynamics_Model/links/5ca04e17299bf11169521b1e/Continuous-time-Stereo-Visual-Odometry-Based-on-Dynamics-Model.pdf) **2019**
    + <font color = blue>基于动力学模型的连续时间的双目视觉里程计</font>
    + 北京大学，上海交大
+ [x] **[4]** Strecke M, Stückler J. [**EM-Fusion: Dynamic Object-Level SLAM with Probabilistic Data Association**](https://arxiv.org/pdf/1904.11781.pdf)[J]. arXiv preprint arXiv:1904.11781, **2019**.
    + <font color = blue>具有概率数据关联的**动态物体级 SLAM**</font>
    + 德国马克斯普朗克智能系统研究所 &emsp; [实验室主页](https://ev.is.tuebingen.mpg.de/)
    + Usenko V, Demmel N, Schubert D, et al. [Visual-Inertial Mapping with Non-Linear Factor Recovery](https://arxiv.org/pdf/1904.06504.pdf)[J]. arXiv preprint arXiv:1904.06504, 2019.
    + 奥克兰大学 &emsp; 期刊 Integrated Computer-Aided Engineering 中科院二区，JCR Q1，IF 3.667
+ [ ] **[5]** Guclu O, Can A B. [**k-SLAM: A fast RGB-D SLAM approach for large indoor environments**](https://www.sciencedirect.com/science/article/pii/S107731421930058X)[J]. Computer Vision and Image Understanding, **2019**.
    + <font color = blue>大型室内环境的快速 RGB-D SLAM 方法</font>
    + 土耳其哈西德佩大学 &emsp; JCR Q2，IF 2.776
+ [ ] **[6]** Yokozuka M, Oishi S, Simon T, et al. [**VITAMIN-E: VIsual Tracking And Mapping with Extremely Dense Feature Points**](https://arxiv.org/pdf/1904.10324.pdf)[J]. arXiv preprint arXiv:1904.10324, **2019**.
    + <font color = blue>具有**极度密度的特征点**的视觉跟踪与建图</font>
    + 日本国家先进工业科学技术研究所 &emsp; 
+ [x] **[7]** Zubizarreta J, Aguinaga I, Montiel J M M. [**Direct Sparse Mapping**](https://arxiv.org/pdf/1904.06577.pdf)[J]. arXiv preprint arXiv:1904.06577, **2019**.
    + <font color = blue>**直接法稀疏建图**</font>
    + 西班牙萨拉戈萨大学 &emsp; [代码开源](https://github.com/jzubizarreta/dsm)（还未放出）
    + 作者 2018 年 ECCV 一篇文章：可变形贴图中 SLAM 的相机跟踪 [Camera Tracking for SLAM in Deformable Maps](http://openaccess.thecvf.com/content_ECCVW_2018/papers/11129/Lamarca_Camera_Tracking_for_SLAM_in_Deformable_Maps_ECCVW_2018_paper.pdf)
+ [ ] **[8]** Feng G, Ma L, Tan X. [**Line Model-Based Drift Estimation Method for Indoor Monocular Localization**](https://ieeexplore.ieee.org/abstract/document/8690676)[C]//2018 IEEE 88th Vehicular Technology Conference (VTC-Fall). IEEE, **2019**: 1-5.
    + <font color = blue>基于**线模型**的室内单目定位漂移估计方法</font>
    + 哈工大 &emsp;  VTC 无线通信会议，一年两届
+ [x] **[9]** Castro G, Nitsche M A, Pire T, et al. [**Efficient on-board Stereo SLAM through constrained-covisibility strategies**](https://www.researchgate.net/profile/Gaston_Castro/publication/332147108_Efficient_on-board_Stereo_SLAM_through_constrained-covisibility_strategies/links/5cacb327a6fdccfa0e7c3e4b/Efficient-on-board-Stereo-SLAM-through-constrained-covisibility-strategies.pdf)[J]. Robotics and Autonomous Systems, 2019.
    + <font color = blue>通过约束-合作策略实现高效双目SLAM</font>
    + 阿根廷布宜诺斯艾利斯大学博士 &emsp; 双目 PTAM 作者
+ [ ] **[10]** Canovas B, Rombaut M, Nègre A, et al. [**A Coarse and Relevant 3D Representation for Fast and Lightweight RGB-D Mapping**](https://hal.archives-ouvertes.fr/hal-02068740/document)[C]//VISAPP 2019-International Conference on Computer Vision Theory and Applications. 2019.
    + <font color = blue>应用于快速粗糙的 RGB-D 建图的粗糙的相关 3D 表示</font>
    + 格勒诺布尔计算机科学实验室
+ [x] **[11]** Ziquan Lan, Zi Jian Yew, Gim Hee Lee. [**Robust Point Cloud Based Reconstruction of Large-Scale Outdoor Scenes**](http://219.216.82.193/cache/5/03/www.cvlibs.net/297109a6b31ef7d288d6637f31249bd2/Barsan2018ICRA.pdf)[C], **ICRA 2019**.
    + <font color = blue>**鲁棒的室外大场景点云重建**</font>
    + 苏黎世联邦理工  &emsp; [代码开源](https://github.com/ziquan111/RobustPCLReconstruction)（还未放出）
+ [ ] **[12]** Shi T, Shen S, Gao X, et al. [**Visual Localization Using Sparse Semantic 3D Map**](https://arxiv.org/pdf/1904.03803.pdf)[J]. arXiv preprint arXiv:1904.03803, **2019**.
    + <font color = blue>利用**稀疏语义三维地图**进行可视化定位</font>
    + 中国科学院自动化研究所模式识别国家重点实验室
+ [x] **[13]** Yang S, Kuang Z F, Cao Y P, et al. [**Probabilistic Projective Association and Semantic Guided Relocalization for Dense Reconstruction**](https://cg.cs.tsinghua.edu.cn/papers/ICRA-2019-densemapping.pdf)[C]//**ICRA 2019**.
    + <font color = blue>稠密重建的**概率投影关联**和**语义引导重定位**</font>
    + 清华大学 &emsp; [谷歌学术](https://scholar.google.com/citations?user=50194vkAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[14]** Xiao L, Wang J, Qiu X, et al. [**Dynamic-SLAM: Semantic monocular visual localization and mapping based on deep learning in dynamic environment**](https://www.researchgate.net/profile/Linhui_Xiao/publication/332149941_Dynamic-SLAM_Semantic_monocular_visual_localization_and_mapping_based_on_deep_learning_in_dynamic_environment/links/5cb201d04585156cd7949b7b/Dynamic-SLAM-Semantic-monocular-visual-localization-and-mapping-based-on-deep-learning-in-dynamic-environment.pdf)[J]. Robotics and Autonomous Systems, **2019**.
    + <font color = blue>基于动态环境深度学习的单目 SLAM </font>
    + 中国科学院电子研究所传感器技术国家重点实验室 &emsp; 期刊 中科院三区 JCR Q2
+ [x] **[15]** Zhou L, Wang S, Ye J, et al. [**Do not Omit Local Minimizer: a Complete Solution for Pose Estimation from 3D Correspondences**](https://arxiv.org/pdf/1904.01759.pdf)[J]. arXiv preprint arXiv:1904.01759, **2019**.
    + <font color = blue>不要忽略局部最小化：一种完整的 3D 对应姿态估计解决方案</font>
    + CMU
+ [ ] **[16]** Miraldo P, Saha S, Ramalingam S. [**Minimal Solvers for Mini-Loop Closures in 3D Multi-Scan Alignment**](https://arxiv.org/pdf/1904.03941.pdf)[C]. **CVPR 2019**.
    + <font color = blue>三维多视角对齐中**微型闭环**的最小求解器</font>
    + 美国犹他大学
    + ICRA 2019：[POSEAMM: A Unified Framework for Solving Pose Problems using an Alternating Minimization Method](https://arxiv.org/pdf/1904.04858.pdf)
    
---

#### 2. AR/MR 相关
+ [x] **[17]** Piao J C, Kim S D. [**Real-time Visual-Inertial SLAM Based on Adaptive Keyframe Selection for Mobile AR Applications**](https://ieeexplore.ieee.org/abstract/document/8698793)[J]. IEEE Transactions on Multimedia, **2019**.
    + <font color = blue>基于自适应关键帧选择的**移动增强现实**应用的实时视觉惯性 SLAM</font>
    + 中国延边大学，韩国延世大学 &emsp; 期刊 中科院二区，JCR Q2，IF 4.368
+ [ ] **[18]** Puigvert J R, Krempel T, Fuhrmann A. [**Localization Service Using Sparse Visual Information Based on Recent Augmented Reality Platforms**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8699237)[C]//2018 IEEE International Symposium on Mixed and Augmented Reality Adjunct (ISMAR-Adjunct). IEEE, **2019**: 415-416.
    + <font color = blue>基于最近增强现实平台的稀疏视觉信息定位服务</font>
    + Cologne Intelligence  &emsp; ISMAR：AR 领域顶级会议
+ [ ] **[19]** Zillner J, Mendez E, Wagner D. [**Augmented Reality Remote Collaboration with Dense Reconstruction**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8699225)[C]//2018 IEEE International Symposium on Mixed and Augmented Reality Adjunct (ISMAR-Adjunct). IEEE, **2019**: 38-39.
    + <font color = blue>具有稠密重建的增强现实远程协作</font>
    + DAQRI 智能眼镜：https://daqri.com/products/smart-glasses/  &emsp; ISMAR：CCF 计算机图形学与多媒体 B 类会议
+ [ ] **[20]** Grandi, Jerônimo & Debarba, Henrique & Maciel, Anderson. [**Characterizing Asymmetric Collaborative Interactions in Virtual and Augmented Realities**](https://www.researchgate.net/profile/Jeronimo_Grandi/publication/332353699_Characterizing_Asymmetric_Collaborative_Interactions_in_Virtual_and_Augmented_Realities/links/5cafa2b492851c8d22e51246/Characterizing-Asymmetric-Collaborative-Interactions-in-Virtual-and-Augmented-Realities.pdf). IEEE Conference on Virtual Reality and 3D User Interfaces. **2019**.
    + <font color = blue>表征虚拟现实和增强现实中的非对称协作交互</font>
    + 巴西南里奥格兰德联邦大学 &emsp; [演示视频](https://www.youtube.com/watch?v=6RbXc222spc)
+ [ ] **[21]** Chen Y S, Lin C Y. [**Virtual Object Replacement Based on Real Environments: Potential Application in Augmented Reality Systems**](https://www.mdpi.com/2076-3417/9/9/1797)[J]. Applied Sciences, **2019**, 9(9): 1797.
    + <font color = blue>基于真实环境的虚拟对象替换：在增强现实系统中的潜在应用</font>
    + 台湾科技大学 &emsp; Applied Sciences 开源期刊
+ [ ] **[22]** Ferraguti F, Pini F, Gale T, et al. [**Augmented reality based approach for on-line quality assessment of polished surfaces**](https://www.sciencedirect.com/science/article/pii/S0736584518305131)[J]. Robotics and Computer-Integrated Manufacturing, **2019**, 59: 158-167.
    + <font color = blue>基于**增强现实**的抛光表面在线质量评估方法</font>
    + 意大利摩德纳大学 &emsp; 中科院二区，JCR Q1，IF 4.031
+ [ ] **[23]** Wang J, Liu H, Cong L, et al. [**CNN-MonoFusion: Online Monocular Dense Reconstruction Using Learned Depth from Single View**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8699273)[C]//2018 IEEE International Symposium on Mixed and Augmented Reality Adjunct (ISMAR-Adjunct). IEEE, **2019**: 57-62.
    + <font color = blue>单视图中学习深度的在线单目密集重建</font>
    + 网易 AR 研究所 &emsp; ISMAR：AR 领域顶级会议，CCF 计算机图形学与多媒体 B 类会议
+ [ ] **[24]** He Z, Rosenberg K T, Perlin K. [**Exploring Configuration of Mixed Reality Spaces for Communication**](http://delivery.acm.org/10.1145/3320000/3312761/LBW0222.pdf?ip=219.216.73.1&id=3312761&acc=OPEN&key=BF85BBA5741FDC6E%2E4183B12E3311CD37%2E4D4702B0C3E38B35%2E6D218144511F3437&__acm__=1557107120_3c56b43468e3911f8111789083753416)[C]//Extended Abstracts of the 2019 CHI Conference on Human Factors in Computing Systems. ACM, **2019**: LBW0222.
    + <font color = blue>探索混合现实空间的通信配置</font>
    + 纽约大学 &emsp; CHI：CCF 人机交互与普适计算 A 类会议
#### 3. learning slam
+ [ ] **[25]** von Stumberg L, Wenzel P, Khan Q, et al. [**GN-Net: The Gauss-Newton Loss for Deep Direct SLAM**](https://arxiv.org/pdf/1904.11932.pdf)[J]. arXiv preprint arXiv:1904.11932, **2019**.
    + <font color = blue>GN-Net：高斯牛顿损失的深度直接法 SLAM </font>
    + 慕尼黑工业大学 &emsp; [Google Scholor](https://scholar.google.com/citations?user=jBgFEukAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[26]** Wang R, Yang N, Stueckler J, et al. [**DirectShape: Photometric Alignment of Shape Priors for Visual Vehicle Pose and Shape Estimation**](https://arxiv.org/pdf/1904.10097.pdf)[J]. arXiv preprint arXiv:1904.10097, 2019.
    + <font color = blue>DirectShape：视觉车辆姿态形状估计的形状先验光度对准</font>
    + 慕尼黑工业大学 &emsp; [Google Scholor](https://scholar.google.com/citations?user=buN3yw8AAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[27]** Feng M, Hu S, Ang M, et al. [**2D3D-MatchNet: Learning to Match Keypoints Across 2D Image and 3D Point Cloud**](https://arxiv.org/pdf/1904.09742.pdf)[J]. arXiv preprint arXiv:1904.09742, 2019.
    + <font color = blue>2D3D-MatchNet：学习匹配 2D 图像和 3D 点云的关键点</font>
    + 新加坡国立大学
+ [x] **[28]** Wei Y, Liu S, Zhao W, et al. [**Conditional Single-view Shape Generation for Multi-view Stereo Reconstruction**](https://arxiv.org/pdf/1904.06699.pdf)[J]. arXiv preprint arXiv:1904.06699, **2019**.
    + <font color = blue>多视角立体重建的条件单视图外形生成</font>
    + 清华大学 &emsp; [代码开源](https://github.com/weiyithu/OptimizeMVS)
+ [ ] **[29]** Behl A, Paschalidou D, Donné S, et al. [**Pointflownet: Learning representations for rigid motion estimation from point clouds**](http://ww.cvlibs.net/publications/Behl2019CVPR.pdf)[C]. **CVPR 2019**.
    + <font color = blue>Pointflownet：从点云学习刚体运动估计的表示</font>
    + 图宾根大学 &emsp; 即将[开源代码](https://github.com/aseembehl/pointflownet)（还未放出）
+ [ ] **[30]** Xue F, Wang X, Li S, et al. [**Beyond Tracking: Selecting Memory and Refining Poses for Deep Visual Odometry**](https://arxiv.org/pdf/1904.01892.pdf)[J]. arXiv preprint arXiv:1904.01892, **2019**.
    + <font color = blue>为深度视觉测距选择记忆和细化位姿</font>
    + 北京大学
    
#### 4. learning others
+ [ ] **[31]** Hou J, Dai A, Nießner M. [**3D-SIC: 3D Semantic Instance Completion for RGB-D Scans**](https://arxiv.org/pdf/1904.12012.pdf)[J]. arXiv preprint arXiv:1904.12012, **2019**.
    + <font color = blue>RGB-D扫描的 3D 语义实例</font>
    + 慕尼黑工业大学
+ [ ] **[32]** Phalak A, Chen Z, Yi D, et al. [**DeepPerimeter: Indoor Boundary Estimation from Posed Monocular Sequences**](https://arxiv.org/pdf/1904.11595.pdf)[J]. arXiv preprint arXiv:1904.11595, **2019**.
    + <font color = blue>DeepPerimeter：单目序列室内边界估计</font>
    + Magic Leap &emsp; [Google Scholor](https://scholar.google.com/citations?user=ji6BSBoAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[33]** Yang Z, Liu S, Hu H, et al. [**RepPoints: Point Set Representation for Object Detection**](https://arxiv.org/pdf/1904.11490.pdf)[J]. arXiv preprint arXiv:1904.11490, **2019**.
    + <font color = blue>RepPoints：目标检测的点集表示</font>
    + 北京大学
+ [ ] **[34]** Jiang S, Xu T, Li J, et al. [**Foreground Feature Enhancement for Object Detection**](https://ieeexplore.ieee.org/abstract/document/8684952/authors#authors)[J]. IEEE Access, 2019, 7: 49223-49231.
    + <font color = blue>目标检测的前景特征增强</font>
    + 北京理工大学
+ [ ] **[35]** Zakharov S, Shugurov I, Ilic S. [**DPOD: 6D Pose Object Detector and Refiner**]()[J]. **2019**.
    + <font color = blue>DPOD:6 自由度物体姿态检测与细化</font>
    + 慕尼黑工业大学，西门子
+ [ ] **[36]** Liu C, Yang Z, Xu F, et al. [**Image Generation from Bounding Box-represented Semantic Labels**](https://www.sciencedirect.com/science/article/pii/S0097849319300329)[J]. Computers & Graphics, **2019**.
    + <font color = blue>从边界框表示的语义标签中生成图像</font>
    + 清华大学 &emsp; Computers & Graphics 中科院四区，JCR Q3， IF 1.352
+ [ ] **[37]** Qiu Z, Yan F, Zhuang Y, et al. [**Outdoor Semantic Segmentation for UGVs Based on CNN and Fully Connected CRFs**](https://ieeexplore.ieee.org/abstract/document/8620277)[J]. IEEE Sensors Journal, **2019**.
    + <font color = blue>基于 CNN 和全连通 CRF 的 UGV 室外语义分割</font>
    + 大连理工大学 &emsp; [点云处理代码](https://pan.baidu.com/s/1AofGdJwUSUcsMwgm9IMC-Q#list/path=%2F) &emsp; 中科院三区，JCR Q2，IF 2.698
+ [ ] **[38]** Ma X, Wang Z, Li H, et al. [**Accurate Monocular 3D Object Detection via Color-Embedded 3D Reconstruction for Autonomous Driving**](https://arxiv.org/pdf/1903.11444.pdf)[J]. arXiv preprint arXiv:1903.11444, **2019**.
    + <font color = blue>用于自动驾驶的彩色嵌入式三维重建精准单目三维物体检测</font>
    + 大连理工大学
+ [ ] **[39]** Sindagi V A, Zhou Y, Tuzel O. [**MVX-Net: Multimodal VoxelNet for 3D Object Detection**](https://arxiv.org/pdf/1904.01649.pdf)[J]. arXiv preprint arXiv:1904.01649, **2019**.
    + <font color = blue>用于**三维物体检测**的多模态 VoxelNet</font>
    + 美国约翰斯·霍普金斯大学 &emsp; [个人主页](http://www.vishwanathsindagi.com/)
+ [ ] **[40]** Li J, Lee G H. [**USIP: Unsupervised Stable Interest Point Detection from 3D Point Clouds**](https://arxiv.org/pdf/1904.00229.pdf)[J]. arXiv preprint arXiv:1904.00229, **2019**.
    + <font color = blue>三维点云的无监督稳定兴趣点检测</font>
    + 新加坡国立大学 &emsp; 即将[开源代码](https://github.com/lijx10/USIP)（还未放出）
#### 5. event
+ [x] **[41]** Scheerlinck C, Rebecq H, Stoffregen T, et al. [**CED: Color event camera dataset**](https://arxiv.org/pdf/1904.10772.pdf)[J]. arXiv preprint arXiv:1904.10772, **CVPRW 2019**.
    + <font color = blue>彩色**事件相机**</font>
    + 苏黎世大学 &emsp; [项目主页](http://rpg.ifi.uzh.ch/CED.html) &emsp; [Google Scholor](https://scholar.google.com/citations?user=zveWLBkAAAAJ&hl=zh-CN&oi=sra)
    + 基于事件的视觉研究：[Event-based Vision: A Survey](https://arxiv.org/pdf/1904.08405.pdf). CVPR 2019
    + [Focus is all you need: Loss functions for event-based vision](https://arxiv.org/pdf/1904.07235.pdf). 2019
+ [ ] **[42]** Stoffregen T, Gallego G, Drummond T, et al. [**Event-based motion segmentation by motion compensation**](https://arxiv.org/pdf/1904.01293.pdf)[J]. arXiv preprint arXiv:1904.01293, **2019**.
    + <font color = blue>基于**事件**的运动补偿运动分割</font>
    + 澳大利亚机器人视觉中心，苏黎世大学
    
#### 6. 传感器融合
+ [ ] **[43]** Xiao Y, Ruan X, Chai J, et al. [**Online IMU Self-Calibration for Visual-Inertial Systems**](https://www.mdpi.com/1424-8220/19/7/1624/htm)[J]. Sensors, **2019**, 19(7): 1624.
    + <font color = blue>视觉惯性系统 **IMU 在线标定**</font>
    + 北京工业大学 &emsp; Sensors 开源期刊
+ [x] **[44]** Eckenhoff K, Geneva P, Huang G. [**Closed-form preintegration methods for graph-based visual–inertial navigation**](http://sage.cnpereading.com/paragraph/article/10.1177/0278364919835021)[J]. The International Journal of Robotics Research, 2018.
    + <font color = blue>基于图的视觉惯性导航的**封闭式预积分**方法</font>
    + 特拉华大学 &emsp; [代码开源](https://github.com/rpng/cpi)
+ [ ] **[45]** Joshi B, Rahman S, Kalaitzakis M, et al. [**Experimental Comparison of Open Source Visual-Inertial-Based State Estimation Algorithms in the Underwater Domain**](https://arxiv.org/pdf/1904.02215.pdf)[J]. arXiv preprint arXiv:1904.02215, **2019**.
    + <font color = blue>开源视觉惯导 SLAM 在水下的状态估计比较</font>
    + 美国南卡罗来纳大学哥伦比亚分校 &emsp; [Google Scholor](https://scholar.google.com/citations?user=Izlp7JsAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[46]** Xia L, Meng Q, Chi D, et al. [**An Optimized Tightly-Coupled VIO Design on the Basis of the Fused Point and Line Features for Patrol Robot Navigation**](https://www.mdpi.com/1424-8220/19/9/2004/htm)[J]. Sensors, **2019**, 19(9): 2004.
    + <font color = blue>基于点线特征融合的巡检机器人紧耦合的 VIO </font>
    + 东北电力大学 &emsp; Sensors 开源期刊
+ [ ] **[47]** Ye H, Chen Y, Liu M. [**Tightly Coupled 3D Lidar Inertial Odometry and Mapping**](https://arxiv.org/pdf/1904.06993.pdf)[J]. arXiv preprint arXiv:1904.06993, 2019.
    + <font color = blue>紧耦合的**激光惯性**里程计与建图</font>
    + 香港科技大学 &emsp; [Google Scholor](https://scholar.google.com/citations?user=CdV5LfQAAAAJ&hl=zh-CN&oi=sra)
    + [Focal loss in 3d object detection](https://arxiv.org/pdf/1809.06065.pdf) [J]IEEE Robotics and Automation Letters 4 (2), 1263-1270, **2019**.
+ [ ] **[48]** Usenko V, Demmel N, Schubert D, et al. [**Visual-Inertial Mapping with Non-Linear Factor Recovery**](https://arxiv.org/pdf/1904.06504.pdf)[J]. arXiv preprint arXiv:1904.06504, **2019**.
    + <font color = blue>具有非线性因子恢复的**视觉-惯导建图**</font>
    + 慕尼黑工业大学 &emsp; [Google Scholor](https://scholar.google.com/citations?user=APTNKjoAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[49]** Qiu X, Zhang H, Fu W, et al. [**Monocular Visual-Inertial Odometry with an Unbiased Linear System Model and Robust Feature Tracking Front-End**](https://www.mdpi.com/1424-8220/19/8/1941/htm)[J]. Sensors, **2019**, 19(8): 1941.
    + <font color = blue>具有无偏差线性模型和前端鲁棒特征跟踪的**单目视觉惯导里程计**</font>
    + 多伦多大学 &emsp; [Google Scholor](https://scholar.google.com/citations?user=lSlo1RgAAAAJ&hl=zh-CN&oi=sra) &emsp; Sensors 开源期刊

#### 7. Others
+ [ ] **[50]** Liu Y, Knoll A, Chen G. [**A New Method for Atlanta World Frame Estimation**](https://arxiv.org/pdf/1904.12717.pdf)[J]. arXiv preprint arXiv:1904.12717, **2019**.
    + <font color = blue>亚特兰大世界框架估计的一种新方法</font>
    + 慕尼黑工业大学
+ [x] **[51]** Zhao Y, Qi J, Zhang R. [**CBHE: Corner-based Building Height Estimation for Complex Street Scene Images**](https://arxiv.org/pdf/1904.11128.pdf)[J]. arXiv preprint arXiv:1904.11128, **2019**.
    + <font color = blue>基于角点的复杂街景图像**建筑物高度估计**</font>
    + 墨尔本大学

---

### 2019 年 6 月论文更新（21 篇）

#### 1. Geometric SLAM

+ [x] **[1]** [**A Modular Optimization Framework for Localization and Mapping**](https://ingmec.ual.es/~jlblanco/papers/blanco2019mola_rss2019.pdf). [C] RSS **2019**
    + <font color = blue>用于跟踪与建图的模块化优化框架</font>
    + 西班牙阿尔梅里亚大学 &emsp; [Google Scholor](https://scholar.google.com/citations?hl=zh-CN&user=bhDtzKgAAAAJ)
    + [**代码开源**](https://github.com/MOLAorg/mola)（还未放出） &emsp; [演示视频](https://www.youtube.com/watch?v=Bb92aMBJR44)
+ [x] **[2]** Wang C, Guo X. [**Efficient Plane-Based Optimization of Geometry and Texture for Indoor RGB-D Reconstruction**](https://arxiv.org/pdf/1905.08853.pdf)[J]. arXiv preprint arXiv:1905.08853, **2019**.
    + <font color = blue>用于室内 RGB-D 重建的基于平面的几何和纹理优化</font>
    + 德克萨斯大学达拉斯分校 &emsp; [Google Scholor](https://scholar.google.com/citations?user=PXm3u3gAAAAJ&hl=zh-CN&oi=sra)
    + [**代码开源**](https://github.com/chaowang15/plane-opt-rgbd)
+ [x] **[3]** Wang J, Song J, Zhao L, et al. [**A submap joining algorithm for 3D reconstruction using an RGB-D camera based on point and plane features**](https://www.sciencedirect.com/science/article/pii/S0921889018302033)[J]. Robotics and Autonomous Systems, **2019**.
    + <font color = blue>一种基于点特征和平面特征的RGB-D相机三维重建子地图连接算法</font>
    + 悉尼科技大学 &emsp; [Google Scholor](https://scholar.google.com/citations?user=rf8d0o4AAAAJ&hl=zh-CN&oi=sra) &emsp; 中科院三区，JCR Q2，IF 2.809
+ [x] **[4]** Joshi N, Sharma Y, Parkhiya P, et al. [**Integrating Objects into Monocular SLAM: Line Based Category Specific Models**](https://arxiv.org/pdf/1905.04698.pdf)[J]. arXiv preprint arXiv:1905.04698, **2019**.
    + <font color = blue>将物体集成到单目 SLAM 中：基于线的特定类别模型</font>
    + 印度海德拉巴大学
    + Parkhiya P, Khawad R, Murthy J K, et al. **Constructing Category-Specific Models for Monocular Object-SLAM**[C]//2018 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2018: 1-9.
+ [ ] **[5]** Niu J, Qian K. [**A hand-drawn map-based navigation method for mobile robots using objectness measure**](https://journals.sagepub.com/doi/pdf/10.1177/1729881419846339)[J]. International Journal of Advanced Robotic Systems, **2019**, 16(3): 1729881419846339.
    + <font color = blue>一种基于手绘地图的使用物体度量移动机器人导航方法</font>
    + 东南大学 &emsp; 期刊：中科院四区， JCR Q4，IF 1.0
+ [x] **[6]** [**Robust Object-based SLAM for High-speed Autonomous Navigation**](http://groups.csail.mit.edu/rrg/papers/OkLiu19icra.pdf). **2019**
    + <font color = blue>基于鲁棒的物体 SLAM 的高速导航系统</font>
    + MIT
+ [ ] **[7]** Cheng J, Sun Y, Meng M Q H. [**Robust Semantic Mapping in Challenging Environments**](https://www.cambridge.org/core/journals/robotica/article/robust-semantic-mapping-in-challenging-environments/19F9EA5C806AFC10377F13ABDEDA68EE)[J]. Robotica, 1-15, **2019**.
    + <font color = blue>具有挑战环境下的鲁棒的语义建图</font>
    + 香港中文大学，香港科技大学 &emsp; 期刊：中科院四区， JCR Q4，IF 1.267
+ [x] **[8]** Sun B, Mordohai P. [**Oriented Point Sampling for Plane Detection in Unorganized Point Clouds**](https://arxiv.org/pdf/1905.02553.pdf)[J]. arXiv preprint arXiv:1905.02553, **2019**.
    + <font color = blue>无组织点云中平面检测的定向点采样</font>
    + 美国史蒂文斯理工学院
+ [x] **[9]** Palazzolo E, Behley J, Lottes P, et al. [**ReFusion: 3D Reconstruction in Dynamic Environments for RGB-D Cameras Exploiting Residuals**](https://arxiv.org/pdf/1905.02082.pdf)[J]. arXiv preprint arXiv:1905.02082, **2019**.
    + <font color = blue>ReFusion 利用残差的 RGB-D 相机动态环境下的三维重建</font>
    + 德国波恩大学 &emsp; [**代码开源**](https://github.com/PRBonn/refusion)
    
---

#### 2. Learning SLAM

+ [x] **[10]** Goldman M, Hassner T, Avidan S. [**Learn Stereo, Infer Mono: Siamese Networks for Self-Supervised, Monocular, Depth Estimation**](https://arxiv.org/pdf/1905.00401.pdf)[J]. arXiv preprint arXiv:1905.00401, **2019**.
    + <font color = blue>学习双目，推断单目：用于自我监督，单目，深度估计的连体网络</font>
    + 以色列特拉维夫大学 &emsp; [**代码开源**](https://github.com/mtngld/lsim)（还未放出）
+ [ ] [11] Mukherjee A, Chakaborty S, Saha S K. [**Detection of loop closure in SLAM: A DeconvNet based approach**](https://www.sciencedirect.com/science/article/pii/S1568494619302339)[J]. Applied Soft Computing, **2019**.
    + <font color = blue>基于 DeconvNet 的 SLAM 闭环检测方法</font>
    + 印度贾达普大学 &emsp; 期刊：中科院二区，JCR Q1，IF 4.0

---

#### 3. 传感器融合

+ [ ] **[12]** Huang K, Xiao J, Stachniss C. [**Accurate Direct Visual-Laser Odometry with Explicit Occlusion Handling and Plane Detection**](http://www.ipb.uni-bonn.de/wp-content/papercite-data/pdf/huang2019icra.pdf)[C]//Proceedings of the IEEE International Conference on Robotics and Automation (**ICRA**). **2019**.
    + <font color = blue>具有显式遮挡处理和平面检测的精确直接视觉激光测距</font>
    + 国防科大
+ [x] **[13]** Shan Z, Li R, Schwertfeger S. [**RGBD-Inertial Trajectory Estimation and Mapping for Ground Robots**](https://www.mdpi.com/1424-8220/19/10/2251)[J]. Sensors, **2019**, 19(10): 2251.
    + <font color = blue>用于地面机器人的 RGBD-惯导轨迹估计与建图</font>
    + 上海科技大学 &emsp; [Google Scholor](https://scholar.google.com/citations?user=Y2olJ9kAAAAJ&hl=zh-CN&oi=sra)
    + [代码开源](https://github.com/STAR-Center/VINS-RGBD) &emsp; [演示视频](https://robotics.shanghaitech.edu.cn/datasets/VINS-RGBD) &emsp; 期刊：开源，中科院三区，JCR Q2Q3
+ [ ] **[14]** Xiong X, Chen W, Liu Z, et al. [**DS-VIO: Robust and Efficient Stereo Visual Inertial Odometry based on Dual Stage EKF**](https://arxiv.org/pdf/1905.00684.pdf)[J]. arXiv preprint arXiv:1905.00684, **2019**.
    + <font color = blue>DS-VIO：基于双重 EKF 的稳健高效的双目视觉惯性测距仪</font>
    + 哈工大 &emsp; [Google Scholor](https://scholar.google.com/citations?user=Dhnz264AAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[15]** Xing B Y, Pan F, Feng X X, et al. [**Autonomous Landing of a Micro Aerial Vehicle on a Moving Platform Using a Composite Landmark**](https://www.hindawi.com/journals/ijae/2019/4723869/abs/)[J]. International Journal of Aerospace Engineering, 2019, **2019**.
    + <font color = blue>使用复合路标的在移动平台上自主着陆的微型飞行器</font>
    + 北京理工大学

---

#### 4. AR & MR & VR

+ [x] **[16]** Ozawa T, Nakajima Y, Saito H. [**Simultaneous 3D Tracking and Reconstruction of Multiple Moving Rigid Objects**](https://ieeexplore.ieee.org/abstract/document/8709158)[C]//2019 12th Asia Pacific Workshop on Mixed and Augmented Reality (APMAR). IEEE, **2019**: 1-5.
    + <font color = blue>多运动刚体运动三维跟踪与重建</font>
    + 日本庆应义塾大学 &emsp; [Google Scholor](https://scholar.google.com/citations?user=lX5lY8YAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[17]** Ens B, Lanir J, Tang A, et al. [**Revisiting Collaboration through Mixed Reality: The Evolution of Groupware**](https://www.sciencedirect.com/science/article/pii/S1071581919300606)[J]. International Journal of Human-Computer Studies, **2019**.
    + <font color = blue>通过混合现实重温协作:群件的发展</font>
    + 澳大利亚莫纳什大学，以色列海法大学，加拿大卡尔加里大学 &emsp; 期刊：中科院三区，JCR Q1Q2，IF 2.3

---

#### 5. Learning others

+ [x] **[18]** Song S, Yu F, Zeng A, et al. [**Semantic scene completion from a single depth image**](http://openaccess.thecvf.com/content_cvpr_2017/papers/Song_Semantic_Scene_Completion_CVPR_2017_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. **CVPR 2017**: 1746-1754.
    + <font color = blue>从单个深度图像完成语义场景理解</font>
    + 普林斯顿大学 &emsp; [Google Scholor](https://scholar.google.com/citations?user=5031vK4AAAAJ&hl=zh-CN&oi=sra)
    + [**代码开源**](https://github.com/shurans/sscnet) &emsp;[项目主页](http://sscnet.cs.princeton.edu/)
    + Wang H, Sridhar S, Huang J, et al. [**Normalized Object Coordinate Space for Category-Level 6D Object Pose and Size Estimation**](https://arxiv.org/pdf/1901.02970.pdf)[J]. arXiv preprint arXiv:1901.02970, **2019**.
    + [**A Survey of 3D Indoor Scene Synthesis**](https://www.researchgate.net/publication/333135099_A_Survey_of_3D_Indoor_Scene_Synthesis)[J]. Journal of Computer Science and Technology 34(3):594-608 · May **2019**
+ [ ] **[19]** Howard-Jenkins H, Li S, Prisacariu V. [**Thinking Outside the Box: Generation of Unconstrained 3D Room Layouts**](https://arxiv.org/pdf/1905.03105.pdf)[C]//Asian Conference on Computer Vision. Springer, Cham, **ACCV2018**: 432-448.
    + <font color = blue>跳出边界框的思考：无约束 3D 房间布局的生成</font>
    + 牛津大学

---

#### 6. Others

+ [ ] **[20]** Qian Y, Ramalingam S, Elder J H. [**LS3D: Single-View Gestalt 3D Surface Reconstruction from Manhattan Line Segments**](http://www.elderlab.yorku.ca/wp-content/uploads/2018/12/LS3DACCV18.pdf)[C]//Asian Conference on Computer Vision. Springer, Cham, **ACCV 2018**: 399-416.
    + <font color = blue>LS3D: 单视图格式塔三维表面重建曼哈顿线段</font>
    + 英国约克大学，美国犹他大学  &emsp; [Google Scholor](https://scholar.google.com/citations?user=gmpm0a8AAAAJ&hl=zh-CN&oi=sra)  &emsp; 会议 ACCV：CCF 人工智能 C 类会议
+ [ ] **[21]** Deng X, Mousavian A, Xiang Y, et al. [**PoseRBPF: A Rao-Blackwellized Particle Filter for 6D Object Pose Tracking**](https://arxiv.org/pdf/1905.09304.pdf)[J]. arXiv preprint arXiv:1905.09304, **2019**.
    + <font color = blue>一种用于6D目标姿态跟踪的 Rao-Blackwellized 粒子滤波器</font>
    + 英伟达，华盛顿大学，斯坦福大学  &emsp; [演示视频](https://www.youtube.com/watch?v=lE5gjzRKWuA&feature=youtu.be)

---

### 2019 年 7 月论文更新（36 篇）

#### 1. Geometric SLAM

+ [x] **[1]** Schenk F, Fraundorfer F. [**RESLAM: A real-time robust edge-based SLAM system**](https://pure.tugraz.at/ws/portalfiles/portal/23662547/schenk_icra_2019.pdf)[C]//IEEE International Conference on Robotics and Automation(**ICRA**) 2019. **2019**.
    + <font color = blue>一种实时稳健的基于边缘的SLAM系统</font>
    + 奥地利格拉茨科技大学 &emsp;[Google Scholar](https://scholar.google.com/citations?user=IbK5KvYAAAAJ&hl=zh-CN&oi=sra)
    + [**代码开源**](https://github.com/fabianschenk/RESLAM)  &emsp; [项目主页](https://graz.pure.elsevier.com/en/publications/reslam-a-real-time-robust-edge-based-slam-system)
+ [ ] **[2]** Christensen K, Hebert M. [**Edge-Direct Visual Odometry**](https://arxiv.org/pdf/1906.04838.pdf)[J]. arXiv preprint arXiv:1906.04838, **2019**.
    + <font color = blue>边缘直接法视觉里程计</font>
    + CMU
+ [ ] **[3]** Dong E, Xu J, Wu C, et al. [**Pair-Navi: Peer-to-Peer Indoor Navigation with Mobile Visual SLAM**](https://ieeexplore.ieee.org/abstract/document/8737640)[C]//IEEE **INFOCOM** 2019-IEEE Conference on Computer Communications. IEEE, **2019**: 1189-1197.
    + <font color = blue>使用移动视觉 SLAM 进行点对点室内导航</font>
    + 清华大学 &emsp; [Google Scholar](https://scholar.google.com/citations?user=ZbqGJ_YAAAAJ&hl=zh-CN&oi=sra)
    + 会议：IEEE INFOCOM：CCF 计算机网络 **A 类会议**
+ [ ] **[4]** Zhou H, Fan H, Peng K, et al. [**Monocular Visual Odometry Initialization With Points and Line Segments**](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8728034)[J]. IEEE Access, **2019**, 7: 73120-73130.
    + <font color = blue>利用点线初始化的单目视觉里程计</font>
    + 国防科大、清华大学、港中文
    + IEEE Access：开源期刊
+ [ ] **[5]** He M, Zhu C, Huang Q, et al. [**A review of monocular visual odometry**](https://link.springer.com/article/10.1007/s00371-019-01714-6)[J]. The Visual Computer, **2019**: 1-13.
    + <font color = blue>单目视觉里程计综述</font>
    + 河海大学
    + 期刊 The Visual Computer：中科院四区，JCR  Q3，IF 1.39
+ [ ] **[6]** Bujanca M, Gafton P, Saeedi S, et al. [**SLAMBench 3.0: Systematic Automated Reproducible Evaluation of SLAM Systems for Robot Vision Challenges and Scene Understanding**](https://www.sajad-saeedi.ca/uploads/3/8/5/9/38597021/sb3.pdf)[C]//IEEE International Conference on Robotics and Automation (**ICRA**). **2019**.
    + <font color = blue>用于机器人视觉挑战和场景理解的 SLAM 系统自动可重复性评估</font>
    + 爱丁堡大学，伦敦帝国理工学院
+ [ ] **[7]** Wang Y, Zell A. [**Improving Feature-based Visual SLAM by Semantics**](https://ieeexplore.ieee.org/abstract/document/8708875)[C]//2018 IEEE International Conference on Image Processing, Applications and Systems (IPAS). IEEE, **2018**: 7-12.
    + <font color = blue>利用语义信息提高特征点法的 SLAM</font>
    + 图宾根大学
+ [x] **[8]** Mo J, Sattar J. [**Extending Monocular Visual Odometry to Stereo Camera System by Scale Optimization**](https://arxiv.org/pdf/1905.12723.pdf)[C]. International Conference on Intelligent Robots and Systems (**IROS**), **2019**.
    + <font color = blue>通过尺度优化将单目视觉里程计扩展到双目相机系统</font>
    + [牛津大学交互式机器人和视觉实验室](http://irvlab.cs.umn.edu/publication)
    + [**代码开源**](https://github.com/jiawei-mo/scale_optimization)
+ [ ] **[9]** [**A Modular Optimization framework for Localization and mApping (MOLA)**](http://ingmec.ual.es/~jlblanco/papers/blanco2019mola_rss2019.pdf). **2019**
    + <font color = blue>用于定位和建图的模块化优化框架</font>
    + 西班牙阿尔梅利亚大学
    + [**代码开源**](https://github.com/MOLAorg/mola)
+ [ ] **[10]** Ye W, Zhao Y, Vela P A. [**Characterizing SLAM Benchmarks and Methods for the Robust Perception Age**](https://arxiv.org/pdf/1905.07808.pdf)[J]. arXiv preprint arXiv:1905.07808, **2019**.
    + <font color = blue>表征鲁棒感知时代的 SLAM 基准和方法</font>
    + 乔治亚理工学院
+ [ ] **[11]** Bürki M, Cadena C, Gilitschenski I, et al. [**Appearance‐based landmark selection for visual localization**](https://onlinelibrary.wiley.com/doi/full/10.1002/rob.21870)[J]. Journal of Field Robotics. **2019**
    + <font color = blue>基于外观的用于视觉定位的路标选择</font>
    + ETH，MIT &emsp; 期刊：中科院二区，JCR  Q1，IF 5.0
+ [ ] **[12]** Hsiao M, Kaess M. [**MH-iSAM2: Multi-hypothesis iSAM using Bayes Tree and Hypo-tree**](http://www.cs.cmu.edu/~kaess/pub/Hsiao19icra.pdf)[J]. **2019**.
    + <font color = blue>MH-iSAM2：使用贝叶树和 Hypo 树的多假设 iSAM</font>
    + CMU &emsp; [**代码开源**](https://bitbucket.org/rpl_cmu/mh-isam2_lib/src/master/)
+ [x] **[13]** Schops T, Sattler T, Pollefeys M. [**BAD SLAM: Bundle Adjusted Direct RGB-D SLAM**](http://openaccess.thecvf.com/content_CVPR_2019/papers/Schops_BAD_SLAM_Bundle_Adjusted_Direct_RGB-D_SLAM_CVPR_2019_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. **2019**: 134-144.
    + <font color = blue>直接法 RGB-D SLAM 中的 BA</font>
    + ETH 
    + [**代码开源**](https://github.com/ETH3D) &emsp; [**项目主页**](https://www.eth3d.net/) 
+ [x] **[14]** Wang K, Gao F, Shen S. [**Real-time Scalable Dense Surfel Mapping**](https://wang-kx.github.io/al-folio/assets/pdf/icra2019.pdf)[C]//Proc. of the IEEE Intl. Conf. on Robot. and Autom.(**ICRA**). **2019**.
    + <font color = blue>实时可拓展的表面重建</font>
    + 港科大沈邵劼课题组
    + [**代码开源**](https://github.com/HKUST-Aerial-Robotics/DenseSurfelMapping) 
+ [ ] **[15]** Zhao Y, Xu S, Bu S, et al. [**GSLAM: A General SLAM Framework and Benchmark**](https://arxiv.org/pdf/1902.07995.pdf)[J]. arXiv preprint arXiv:1902.07995, **2019**.
    + <font color = blue>通用SLAM框架和基准</font>
    + 西北工业大学，自动化所 &emsp; [**代码开源**](https://github.com/zdzhaoyong/GSLAM)
+ [ ] **[16]** Nellithimaru A K, Kantor G A. [**ROLS: Robust Object-Level SLAM for Grape Counting**](http://openaccess.thecvf.com/content_CVPRW_2019/papers/CVPPP/Nellithimaru_ROLS__Robust_Object-Level_SLAM_for_Grape_Counting_CVPRW_2019_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition Workshops. **CVPR2019**: 0-0.
    + <font color = blue>用于葡萄计数的鲁棒的物体级 SLAM</font>
    + CMU
+ [ ] **[17]** Nejad Z Z, Ahmadabadian A H. [**ARM-VO: an efficient monocular visual odometry for ground vehicles on ARM CPUs**](https://link.springer.com/article/10.1007/s00138-019-01037-5)[J]. Machine Vision and Applications, **2019**: 1-10.
    + <font color = blue>ARM CPU上地面车辆的高效单目视觉里程计</font>
    + 伊朗德黑兰托西技术大学 
    + [**代码开源**](https://github.com/zanazakaryaie/ARM-VO) &emsp; 期刊：中科院四区，JCR  Q2Q3，IF 1.3
+ [ ] **[18]** Aloise I, Della Corte B, Nardi F, et al. [**Systematic Handling of Heterogeneous Geometric Primitives in Graph-SLAM Optimization**](http://rss2019.informatik.uni-freiburg.de/papers/0285_FI.pdf)[J]. IEEE Robotics and Automation Letters, **2019**, 4(3): 2738-2745.
    + <font color = blue>SLAM 图优化中异构几何基元的系统处理</font>
    + 罗马大学
    + [**代码开源**](https://srrg.gitlab.io/sashago-website/index.html)
+ [ ] **[19]** Guo R, Peng K, Fan W, et al. [**RGB-D SLAM Using Point–Plane Constraints for Indoor Environments**](https://www.mdpi.com/1424-8220/19/12/2721)[J]. Sensors, **2019**, 19(12): 2721.
    + <font color = blue>室内环境中使用点-平面约束的 RGB-D SLAM</font>
    + 国防科大 &emsp; 期刊：开源期刊，中科院三区，JCR Q2Q3，IF 3.0
+ [ ] **[20]** Laidlow T, Czarnowski J, Leutenegger S. [**DeepFusion: Real-Time Dense 3D Reconstruction for Monocular SLAM using Single-View Depth and Gradient Predictions**](https://www.imperial.ac.uk/media/imperial-college/research-centres-and-groups/dyson-robotics-lab/tlaidlow_etal_icra2019.pdf)[J].**2019**.
    + <font color = blue>DeepFusion：使用单视图深度和梯度预测的单眼SLAM实时密集三维重建</font>
    + [帝国理工学院的戴森机器人实验室](https://www.imperial.ac.uk/dyson-robotics-lab/publications/)
+ [x] **[21]** Saeedi S, Carvalho E, Li W, et al. [**Characterizing Visual Localization and Mapping Datasets**](https://www.sajad-saeedi.ca/uploads/3/8/5/9/38597021/saeedi_icra2019.pdf)[C]//2019 IEEE International Conference on Robotics and Automation (**ICRA**). **2019**.
    + <font color = blue>描述可视化定位于建图的数据集</font>
    + [帝国理工学院计算机系](https://www.imperial.ac.uk/computing/research/visual-computing/) &emsp; [数据集地址](http://wbli.me/lmdata/)
+ [ ] **[22]** Sun T, Sun Y, Liu M, et al. [**Movable-Object-Aware Visual SLAM via Weakly Supervised Semantic Segmentation**](https://arxiv.org/pdf/1906.03629.pdf)[J]. arXiv preprint arXiv:1906.03629, **2019**.
    + <font color = blue>通过弱监督语义分割的可移动对象感知视觉SLAM</font>
    + 港科大
+ [x] **[23]** Ghaffari M, Clark W, Bloch A, et al. [**Continuous Direct Sparse Visual Odometry from RGB-D Images**](https://arxiv.org/pdf/1904.02266.pdf)[J]. arXiv preprint arXiv:1904.02266, **2019**.
    + <font color = blue>RGB-D图像连续直接稀疏视觉里程计</font>
    + 密歇根大学 &emsp; [**代码开源**](https://github.com/MaaniGhaffari/cvo-rgbd)
+ [ ] **[24]** Houseago C, Bloesch M, Leutenegger S. [**KO-Fusion: Dense Visual SLAM with Tightly-Coupled Kinematic and Odometric Tracking**](https://www.imperial.ac.uk/media/imperial-college/research-centres-and-groups/dyson-robotics-lab/chouseago_etal_icra2019.pdf)[J]. **2019**
    + <font color = blue>KO-Fusion：具有紧耦合运动和测距跟踪的稠密视觉SLAM</font>
    + 帝国理工学院戴森机器人实验室
+ [x] **[25]** Iqbal A, Gans N R. [**Localization of Classified Objects in SLAM using Nonparametric Statistics and Clustering**](http://comoros.cs.columbia.edu:8080/IROS_2018_proceedings/media/files/1203.pdf)[C]//2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (**IROS**). IEEE, **2018**: 161-168.
    + <font color = blue>在非参数和聚类的 SLAM 中使用类别物体进行定位</font>
    + 德克萨斯大学计算机工程学院
+ [x] **[26]** [**Semantic Mapping for View-Invariant Relocalization**](http://www.cim.mcgill.ca/~jimmyli/pubs/li2019icra.pdf). **2019**
    + <font color = blue>用于视角不变重定位的语义地图</font>
    + 加拿大蒙特利尔麦吉尔大学
+ [ ] **[27]** Hou Z, Ding Y, Wang Y, et al. [**Visual Odometry for Indoor Mobile Robot by Recognizing Local Manhattan Structures**](https://link.springer.com/chapter/10.1007/978-3-030-20873-8_11)[C]//Asian Conference on Computer Vision. Springer, Cham, **ACCV2018**: 168-182.
    + <font color = blue>通过识别曼哈顿结构的室内机器人视觉里程计</font>
    + 南京理工大学
    
---

#### 2. Learning SLAM

+ [ ] [28] Guclu O, Caglayan A, Burak Can A. [**RGB-D Indoor Mapping Using Deep Features**](http://openaccess.thecvf.com/content_CVPRW_2019/papers/WAD/Guclu_RGB-D_Indoor_Mapping_Using_Deep_Features_CVPRW_2019_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition Workshops. **CVPR 2019**: 0-0.
    + <font color = blue>使用深度特征的 RGB-D 室内建图</font>
    + 土耳其 Ahi Evran University
+ [x] [29] Sualeh M, Kim G W. [**Simultaneous Localization and Mapping in the Epoch of Semantics: A Survey**](https://link.springer.com/content/pdf/10.1007%2Fs12555-018-0130-x.pdf)[J]. International Journal of Control, Automation and Systems, **2019**, 17(3): 729-742.
    + <font color = blue>语义时代的 SLAM 综述</font>
    + 韩国忠北国立大学
    
---

#### 3. AR & MR & VR

+ [ ] [30] Guerra W, Tal E, Murali V, et al. FlightGoggles: Photorealistic Sensor Simulation for Perception-driven Robotics using Photogrammetry and Virtual Reality[J]. arXiv preprint arXiv:1905.11377, 2019.
    + <font color = blue>使用摄影测量和虚拟现实感知驱动机器人的逼真传感器模拟</font>
    + MIT  &emsp;[**代码开源**](https://github.com/mit-fast/FlightGoggles) &emsp; [项目主页](https://flightgoggles.mit.edu/)
+ [ ] [31] Stotko P, Krumpen S, Hullin M B, et al. [**SLAMCast: Large-Scale, Real-Time 3D Reconstruction and Streaming for Immersive Multi-Client Live Telepresence**](https://arxiv.org/pdf/1805.03709.pdf)[J]. IEEE transactions on visualization and computer graphics, **2019**, 25(5): 2102-2112.
    + <font color = blue>SLAMCast：用于沉浸式多客户端实时远程呈现的大规模实时3D重建和流媒体</font>
    + 波恩大学 &emsp; [Google Scholar](https://scholar.google.com/citations?user=nMLx_s0AAAAJ&hl=zh-CN&oi=sra)

---

#### 4. Learning others

+ [ ] [32] Jörgensen E, Zach C, Kahl F. [**Monocular 3D Object Detection and Box Fitting Trained End-to-End Using Intersection-over-Union Loss**](https://arxiv.org/pdf/1906.08070.pdf)[J]. arXiv preprint arXiv:1906.08070, **2019**.
    + <font color = blue>单目三维物体检测和使用交叉联合损失的端到端立方框拟合</font>
    + 瑞典查尔姆斯理工大学 &emsp;[演示视频](https://www.youtube.com/watch?v=G3Aqhd5K2GE&list=PL4jJwJr7UjMb4bzLwUGHdVmhfNS2Ads_x)
+ [ ] [33] Wang B H, Chao W L, Wang Y, et al. [**LDLS: 3-D Object Segmentation Through Label Diffusion From 2-D Images**](https://ieeexplore.ieee.org/abstract/document/8735751)[J]. IEEE Robotics and Automation Letters, **2019**, 4(3): 2902-2909.
    + <font color = blue>通过二维图像的标签扩散进行三维物体分割</font>
    + 康奈尔大学
    + [**代码开源**](https://github.com/brian-h-wang/LDLS) &emsp; 期刊：IEEE Robotics and Automation 中科院二区 ，JCR Q1Q2 ，IF 4.8
+ [x] [34] Yang B, Wang J, Clark R, et al. [**Learning Object Bounding Boxes for 3D Instance Segmentation on Point Clouds**](https://arxiv.org/pdf/1906.01140.pdf)[J]. arXiv preprint arXiv:1906.01140, **2019**.
    + <font color = blue>学习点云上三维实例分割的目标 3D 边界框</font>
    + 牛津大学 &emsp; [Google Scholar](https://scholar.google.com/citations?user=VqUAqz8AAAAJ&hl=zh-CN&oi=sra)
    + [**代码开源**](https://github.com/Yang7879/3D-BoNet) 
+ [ ] [35] Ahmed, Mariam. (**2019**). [**Pushing Boundaries with 3D Boundaries for Object Recognition**](https://www.researchgate.net/publication/333676944_Pushing_Boundaries_with_3D_Boundaries_for_Object_Recognition). 10.13140/RG.2.2.33079.98728. 
    + <font color = blue>利用三维边界框推动边界进行物体检测</font>
    + 新加坡国立大学
+ [ ] [36] Wu D, Zhuang Z, Xiang C, et al. [**6D-VNet: End-To-End 6-DoF Vehicle Pose Estimation From Monocular RGB Images**](http://openaccess.thecvf.com/content_CVPRW_2019/papers/WAD/Wu_6D-VNet_End-To-End_6-DoF_Vehicle_Pose_Estimation_From_Monocular_RGB_Images_CVPRW_2019_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition Workshops. **CVPR2019**: 0-0.
    + <font color = blue>6D-VNet：单目 RGB 图像的端到端 6 自由度车辆姿态估计</font>
    + 深圳大学 &emsp; [**代码开源**](https://github.com/stevenwudi/6DVNET)

---

### 2019 年 8 月论文更新（26 篇）

#### 1. Geometric SLAM

+ [ ] **[1]** Wei X, Huang J, Ma X. [**Real-Time Monocular Visual SLAM by Combining Points and Lines**](https://ieeexplore.ieee.org/abstract/document/8784968/authors#authors)[C]//2019 IEEE International Conference on Multimedia and Expo (**ICME**). IEEE, **2019**: 103-108.
    + <font color = blue>点线结合的单目视觉 SLAM</font>
    + 中国科学院上海高等研究院 &emsp; ICME：CCF 计算机图形学与多媒体 B 类会议
+ [ ] **[2]** Fu Q, Yu H, Lai L, et al. [**A Robust RGB-D SLAM System with Points and Lines for Low Texture Indoor Environments**](https://ieeexplore.ieee.org/abstract/document/8756267)[J]. IEEE Sensors Journal, **2019**.
    + <font color = blue>低纹理室内环境的点线联合的鲁棒 RGB-D SLAM 系统</font>
    + 湖南大学机器人视觉感知与控制国家工程实验室 &emsp; 期刊 IEEE Sensors Journal：中科院三区，JCR Q1Q2，IF 2.69
+ [ ] **[3]** Zhao W, Qian K, Ma Z, et al. [**Stereo Visual SLAM Using Bag of Point and Line Word Pairs**](https://link.springer.com/chapter/10.1007/978-3-030-27538-9_56#Footnotes)[C]//International Conference on Intelligent Robotics and Applications. Springer, Cham, **2019**: 651-661.
    + <font color = blue>利用点线词袋对的双目 SLAM</font>
    + 东南大学
+ [x] **[4]** Hachiuma R, Pirchheim C, Schmalstieg D, et al. [**DetectFusion: Detecting and Segmenting Both Known and Unknown Dynamic Objects in Real-time SLAM**](https://arxiv.org/pdf/1907.09127.pdf)[C]//Proceedings British Machine Vision Conference (**BMVC**). **2019**.
    + <font color = blue>**DetectFusion：在实时的 SLAM 中检测和分割已知与未知的动态对象**</font>
    + 日本庆应义塾大学、格拉茨理工大学 &emsp; BMVC：CCF 人工智能 C 类会议
    + 相关论文：
        + [**Co-Fusion: Real-time Segmentation, Tracking and Fusion of Multiple Objects**](https://github.com/martinruenz/co-fusion), Martin Rünz and Lourdes Agapito, 2017 IEEE International Conference on Robotics and Automation (ICRA)
        + Ishikawa Y, Hachiuma R, Ienaga N, et al. [**Semantic Segmentation of 3D Point Cloud to Virtually Manipulate Real Living Space**](https://lclab.org/wp-content/uploads/2019/03/apmar2019_semanticsegmentation.pdf)[C]//2019 12th Asia Pacific Workshop on Mixed and Augmented Reality (APMAR). IEEE, 2019: 1-7.
+ [ ] **[5]** Prokhorov D, Zhukov D, Barinova O, et al. [**Measuring robustness of Visual SLAM**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8758020)[C]//2019 16th International Conference on Machine Vision Applications (MVA). IEEE, **2019**: 1-6.
    + <font color = blue>视觉 SLAM 的鲁棒性评估</font>
    + 三星 AI 研究中心 &emsp; MVA：CCF 人工智能 C 类会议
+ [ ] **[6]** Ryohei Y, Kanji T, Koji T. [**Invariant Spatial Information for Loop-Closure Detection**](https://ieeexplore.ieee.org/abstract/document/8757889/keywords#keywords)[C]//2019 16th International Conference on Machine Vision Applications (MVA). IEEE, **2019**: 1-6.
    + <font color = blue>用于闭环检测的不变空间信息</font>
    + 日本福井大学 &emsp; MVA：CCF 人工智能 C 类会议
+ [ ] **[7]** Yang B, Xu X, Li J. [**Keyframe-Based Camera Relocalization Method Using Landmark and Keypoint Matching**](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8746595)[J]. IEEE Access, **2019**, 7: 86854-86862.
    + <font color = blue>使用路标和关键点匹配基于关键帧的相机重定位方法</font>
    + 东南大学 &emsp; 期刊 IEEE Access：开源期刊

---

#### 2. Learning/Semantic SLAM

+ [x] **[8]** Ganti P, Waslander S. [**Network Uncertainty Informed Semantic Feature Selection for Visual SLAM**](https://ieeexplore.ieee.org/abstract/document/8781616)[C]//2019 16th Conference on Computer and Robot Vision (CRV). IEEE, **2019**: 121-128.
    + <font color = blue>**视觉 SLAM 中网络不确定性语义信息的选择** </font>
    + 滑铁卢大学、多伦多大学 &emsp; [**代码开源**](https://github.com/navganti/SIVO)
    + 相关论文（学位论文）：Ganti P. [**SIVO: Semantically Informed Visual Odometry and Mapping**](https://uwspace.uwaterloo.ca/bitstream/handle/10012/14111/Ganti_Pranav.pdf?sequence=1&isAllowed=y)[D]. University of Waterloo, **2018**.
+ [x] **[9]** Yu H, Lee B. [**Not Only Look But Observe: Variational Observation Model of Scene-Level 3D Multi-Object Understanding for Probabilistic SLAM**](https://arxiv.org/pdf/1907.09760.pdf)[J]. arXiv preprint arXiv:1907.09760, **2019**.
    + <font color = blue>**不仅看到而且还观察：基于场景级三维多目标理解的概率 SLAM 变分观测模型**</font>
    + 首尔国立大学 &emsp;[代码开源](https://github.com/bogus2000/NOLBO)  &emsp; [Google Scholr](https://scholar.google.com/citations?user=pa6RBYkAAAAJ&hl=zh-CN&oi=sra)
+ [x] **[10]** Hu L, Xu W, Huang K, et al. [**Deep-SLAM++: Object-level RGBD SLAM based on class-specific deep shape priors**](https://arxiv.org/pdf/1907.09691.pdf)[J]. arXiv preprint arXiv:1907.09691, **2019**.
    + <font color = blue>**基于特定类深度形状先验的对象级 RGBD SLAM** </font>
    + 上海科技大学 &emsp;
+ [x] **[11]** Torres Cámara J M. Map Slammer. [**Densifying Scattered KSLAM 3D Maps with Estimated Depth**](https://rua.ua.es/dspace/bitstream/10045/94751/1/SLAM_usando_tecnicas_de_deep_learning_Torres_Camara_Jose_Miguel.pdf)[J]. **2019**.
    + <font color = blue>**利用深度估计的加密分散的关键帧 SLAM 三维地图** </font>
    + **西班牙阿利坎特大学学位论文** &emsp;[**代码开源**](https://github.com/jmtc7/mapSlammer)  &emsp;[演示视频](https://www.youtube.com/watch?v=b74P3ykYE34&feature=youtu.be) 
+ [x] **[12]** Cieslewski T, Bloesch M, Scaramuzza D. **Matching Features without Descriptors: Implicitly Matched Interest Points (IMIPs)**[C]// 2019 British Machine Vision Conference.**2018**.
    + <font color = blue>**没有描述符的特征匹配：隐含匹配的兴趣点**</font>
    + 苏黎世理工、帝国理工 &emsp;[**代码开源**](https://github.com/uzh-rpg/imips_open)  &emsp; BMVC：CCF 人工智能 C 类会议
+ [ ] **[13]** Zheng J, Zhang J, Li J, et al. [**Structured3D: A Large Photo-realistic Dataset for Structured 3D Modeling**](https://arxiv.org/pdf/1908.00222.pdf)[J]. arXiv preprint arXiv:1908.00222, **2019**.
    + <font color = blue>用于结构化三维建模的大型照片拟真数据集</font>
    + 上海科技大学 &emsp;[代码、数据集开源](https://github.com/bertjiazheng/Structured3D)  &emsp; [项目主页](https://structured3d-dataset.org/)
+ [ ] **[14]** Jikai Lu, Jianhui Chen, James J. Little, [**Pan-tilt-zoom SLAM for Sports Videos**](https://arxiv.org/pdf/1907.08816.pdf).[C]//British Machine Vision Conference (BMVC) **2019**.
    + <font color = blue>用于体育视频的平移 - 倾斜 - 缩放SLAM</font>
    + 不列颠哥伦比亚大学 &emsp;[代码开源](https://github.com/lulufa390/Pan-tilt-zoom-SLAM)
    
---

#### 3. AR & MR & VR

+ [ ] **[15]** Saran V, Lin J, Zakhor A. [**Augmented Annotations: Indoor Dataset Generation with Augmented Reality**](http://www-video.eecs.berkeley.edu/papers/jameslin/augmented_annotation.pdf)[J]. ISPRS-International Archives of the Photogrammetry, Remote Sensing and Spatial Information Sciences, **2019**, 4213: 873-879.
    + <font color = blue>增强注释：具有增强现实的室内数据集生成</font>
    + 加州大学伯克利分校 &emsp;[项目主页](https://www.6d.ai/)
+ [ ] **[16]** Liao M, Song B, He M, et al. [**SynthText3D: Synthesizing Scene Text Images from 3D Virtual Worlds**](https://arxiv.org/pdf/1907.06007.pdf)[J]. arXiv preprint arXiv:1907.06007, **2019**.
    + <font color = blue>从3D虚拟世界合成场景文本图像</font>
    + 华中科大、北大、Face++ &emsp;[**代码开源**](https://github.com/MhLiao/SynthText3D)
+ [ ] **[17]** [**Shooting Labels by Virtual Reality**](https://static1.squarespace.com/static/5c3f69e1cc8fedbc039ea739/t/5d01638662182d0001b6f7f6/1560372111582/9_CVPR_2019_VR.pdf). **2019**
    + <font color = blue>利用虚拟现实拍摄语义标签</font>
    + 意大利博洛尼亚大学 &emsp;[**代码开源**](https://github.com/pierlui92/Shooting-Labels)

---

#### 4. Learning others
+ [x] **[18]** Ku J, Pon A D, Waslander S L. [**Monocular 3D Object Detection Leveraging Accurate Proposals and Shape Reconstruction**](http://openaccess.thecvf.com/content_CVPR_2019/papers/Ku_Monocular_3D_Object_Detection_Leveraging_Accurate_Proposals_and_Shape_Reconstruction_CVPR_2019_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. **CVPR 2019**: 11867-11876.
    + <font color = blue>**利用精确的提案和形状重建进行单目三维物体检测**</font>
    + 多伦多大学
    + 相关研究：Ku J, Pon A D, Walsh S, et al. [Improving 3D Object Detection for Pedestrians with Virtual Multi-View Synthesis Orientation Estimation](https://arxiv.org/pdf/1907.06777.pdf)[J]. arXiv preprint arXiv:1907.06777, 2019.
+ [x] **[19]** Chiang H, Lin Y, Liu Y, et al. [**A Unified Point-Based Framework for 3D Segmentation**](https://arxiv.org/pdf/1908.00478.pdf)[J]. arXiv preprint arXiv:1908.00478, **2019**.
    + <font color = blue>**一种统一的基于点的三维分割框架**</font>
    + 国立台湾大学、亚马逊 &emsp;[**代码开源**](https://github.com/ken012git/joint_point_based)
+ [ ] **[20]** Zhang Y, Lu Z, Xue J H, et al. [**A New Rotation-Invariant Deep Network for 3D Object Recognition**](https://ieeexplore.ieee.org/abstract/document/8784918)[C]//2019 IEEE International Conference on Multimedia and Expo (ICME). **IEEE**, **2019**: 1606-1611.
    + <font color = blue>一种新的具有旋转不变性的三维物体识别深度网络</font>
    + 清华大学 &emsp; ICME：CCF 计算机图形学与多媒体 B 类会议
+ [x] **[21]** Gao Y, Yuille A L. Estimation of 3D Category-Specific Object Structure: Symmetry, Manhattan and/or Multiple Images[J]. International Journal of Computer Vision, **2019**: 1-26.
    + <font color = blue>**3D 类别特定对象结构的估计：对称性，曼哈顿和或多图像**</font>
    + 中科大 &emsp; 期刊 International Journal of Computer Vision：**中科院一区，JCR Q1，IF 12.389**
+ [ ] **[22]** Palazzi A, Bergamini L, Calderara S, et al. [**Semi-parametric Object Synthesis**](https://arxiv.org/pdf/1907.10634.pdf)[J]. arXiv preprint arXiv:1907.10634, **2019**.
    + <font color = blue>半参数的对象合成</font>
    + 摩德纳大学 &emsp; [代码开源](https://github.com/ndrplz/semiparametric)
+ [ ] **[23]** Christiansen P H, Kragh M F, Brodskiy Y, et al. [**UnsuperPoint: End-to-end Unsupervised Interest Point Detector and Descriptor**](https://arxiv.org/pdf/1907.04011.pdf)[J]. arXiv preprint arXiv:1907.04011, **2019**.
    + <font color = blue>**端到端无监督兴趣点检测器和描述符**</font>
    + 土耳其哈塞特大学 &emsp; **相关代码**：[SuperPointPretrainedNetwork](https://github.com/MagicLeapResearch/SuperPointPretrainedNetwork)，[lf-net-release](https://github.com/vcg-uvic/lf-net-release)
+ [x] **[24]** Chen B X, Tsotsos J K. [**Fast Visual Object Tracking with Rotated Bounding Boxes**](https://arxiv.org/pdf/1907.03892.pdf)[J]. arXiv preprint arXiv:1907.03892, **2019**.
    + <font color = blue>**带旋转边界框的快速视觉目标跟踪**</font>
    + 约克大学、多伦多大学 &emsp; [**代码开源**](https://github.com/baoxinchen/siammask_e)
+ [ ] **[25]** Brazil G, Liu X. [**M3D-RPN: Monocular 3D Region Proposal Network for Object Detection**](https://arxiv.org/pdf/1907.06038.pdf)[J]. arXiv preprint arXiv:1907.06038, **2019**.
    + <font color = blue>用于物体检测的单目 3D 区域提议网络</font>
    + 密歇根州立大学

---

#### 5. Others

+ [ ] **[26]** Zhou Q, Sattler T, Pollefeys M, et al. [**To Learn or Not to Learn: Visual Localization from Essential Matrices**](https://arxiv.org/pdf/1908.01293.pdf)[J]. arXiv preprint arXiv:1908.01293, 2019.
    + <font color = blue>学习或非学习的方法：基础矩阵用于视觉定位</font>
    + 慕尼黑、苏黎世

---

### 2019 年 9 月论文更新（24 篇）

#### 1. Geometric SLAM
        
+ [x] **[1]** Elvira R, Tardós J D, Montiel J M M. [**ORBSLAM-Atlas: a robust and accurate multi-map system**](https://arxiv.org/pdf/1908.11585.pdf)[J]. arXiv preprint arXiv:1908.11585, **2019**.
    + <font color = blue>**ORBSLAM-Atlas：一个鲁棒而准确的多地图系统**</font>
    + 西班牙萨拉戈萨大学，**ORB-SLAM 作者**
+ [ ] **[2]** Yang Y, Dong W, Kaess M. [**Surfel-Based Dense RGB-D Reconstruction With Global And Local Consistency**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8794355)[C]//2019 International Conference on Robotics and Automation (**ICRA**). IEEE, **2019**: 5238-5244.
    + <font color = blue>具有全局和局部一致性的基于面元的 RGB-D 稠密重建</font>
    + CMU 机器人研究所
    + 相关研究：Schöps T, Sattler T, Pollefeys M. [**SurfelMeshing: Online Surfel-Based Mesh Reconstruction**](https://arxiv.gg363.site/pdf/1810.00729)[J]. arXiv preprint arXiv:1810.00729, **2018**.
        + [代码开源](https://github.com/YiChenCityU/surfelmeshing)
+ [x] **[3]** Pire T, Corti J, Grinblat G. [**Online Object Detection and Localization on Stereo Visual SLAM System**](https://link.springer.com/article/10.1007/s10846-019-01074-2)[J]. Journal of Intelligent & Robotic Systems, **2019**: 1-10.
    + <font color = blue>**在线进行三维目标检测的双目视觉 SLAM**</font>
    + 期刊：中科院四区，JCR Q4，IF 2.4
+ [x] **[4]** Ferrer G. [**Eigen-Factors: Plane Estimation for Multi-Frame and Time-Continuous Point Cloud Alignment**](http://sites.skoltech.ru/app/data/uploads/sites/50/2019/07/ferrer2019planes.pdf)[C] **IROS 2019**.
    + <font color = blue>**特征因子：多帧和时间连续点云对齐的平面估计**</font>
    + 俄罗斯斯科尔科沃科技学院，三星 &emsp; [**代码开源**](https://gitlab.com/gferrer/eigen-factors-iros2019) &emsp; [演示视频](https://www.youtube.com/watch?v=_1u_c43DFUE&feature=youtu.be)
+ [ ] **[5]** Zhang Y, Yang J, Zhang H, et al. [**Bundle Adjustment for Monocular Visual Odometry Based on Detected Traffic Sign Features**](https://ieeexplore.ieee.org/abstract/document/8803563)[C]//2019 IEEE International Conference on Image Processing (ICIP). IEEE, **2019**: 4350-4354.
    + <font color = blue>基于交通标志特征检测的单目视觉里程计 BA 优化</font>
    + 北理工、华盛顿大学
+ [ ] **[6]** Zhang X, Wang W, Qi X, et al. [**Point-Plane SLAM Using Supposed Planes for Indoor Environments**](https://www.mdpi.com/1424-8220/19/17/3795/htm)[J]. Sensors, **2019**, 19(17): 3795.
    + <font color = blue>室内环境中使用假设平面的点-平面 SLAM</font>
    + 北京航空航天大学机器人研究所 &emsp; 开源期刊
+ [ ] **[7]** Zheng F, Liu Y H. [**Visual-Odometric Localization and Mapping for Ground Vehicles Using SE (2)-XYZ Constraints**](https://ieeexplore.ieee.org/abstract/document/8793928)[C]//2019 International Conference on Robotics and Automation (**ICRA**). IEEE, **2019**: 3556-3562.
    + <font color = blue>使用 SE(2)-XYZ 约束用于地面车辆定位于建图的视觉里程计</font>
    + 香港中文大学 &emsp;[**代码开源**](https://github.com/izhengfan/se2lam)
+ [x] **[8]** Li H, Xing Y, Zhao J, et al. [**Leveraging Structural Regularity of Atlanta World for Monocular SLAM**](https://ieeexplore.ieee.org/abstract/document/8793716)[C]//2019 International Conference on Robotics and Automation (**ICRA**). IEEE, **2019**: 2412-2418.
    + <font color = blue>**利用亚特兰大世界结构规律的单目 SLAM**</font>
    + 香港中文大学[刘云辉](http://ri.cuhk.edu.hk/yhliu)教授课题组（上面那篇的郑帆博士是他学生），[香港中文大学天石机器人研究所](http://ri.cuhk.edu.hk/)
+ [ ] **[9]** Sun J, Wang Y, Shen Y. [**Fully Scaled Monocular Direct Sparse Odometry with A Distance Constraint**](https://ieeexplore.ieee.org/abstract/document/8813371)[C]//2019 5th International Conference on Control, Automation and Robotics (ICCAR). IEEE, **2019**: 271-275.
    + <font color = blue>具有距离约束的全尺寸单目直接稀疏里程计</font>
    + 北理工
+ [x] **[10]** Dong J, Lv Z. [**miniSAM: A Flexible Factor Graph Non-linear Least Squares Optimization Framework**](https://arxiv.org/pdf/1909.00903.pdf)[J]. arXiv preprint arXiv:1909.00903, **2019**.
    + <font color = blue>**minisam：一种灵活的因子图非线性最小二乘优化框架**</font>
    + Facebook，[**代码开源**](https://github.com/dongjing3309/minisam)，[Google Scholar](https://scholar.google.com/citations?user=99RVk_MAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[11]** Campos C, MM M J, Tardós J D. [**Fast and Robust Initialization for Visual-Inertial SLAM**](https://arxiv.org/pdf/1908.10653.pdf)[C]//2019 International Conference on Robotics and Automation (**ICRA**). IEEE, **2019**: 1288-1294.
    + <font color = blue>视惯 SLAM 快速鲁棒的初始化</font>
    + 西班牙萨拉戈萨大学，ORB-SLAM 课题组
+ [ ] **[12]** He L, Yang M, Li H, et al. [**Graph Matching Pose SLAM based on Road Network Information**](https://ieeexplore.ieee.org/abstract/document/8814093)[C]//2019 IEEE Intelligent Vehicles Symposium (IV). IEEE, **2019**: 1274-1279.
    + <font color = blue>基于路网信息的图匹配位姿 SLAM</font>
    + **上海交通大学**系统控制与信息处理教育部重点实验室
+ [ ] **[13]** Gu T, Yan R. [**An Improved Loop Closure Detection for RatSLAM**](https://ieeexplore.ieee.org/abstract/document/8813378)[C]//2019 5th International Conference on Control, Automation and Robotics (ICCAR). IEEE, **2019**: 884-888.
    + <font color = blue>一种改进的 RatSLAM 闭环检测方法</font>
    + 四川大学

---

#### 2. Semantic/Learning SLAM

+ [x] **[14]** Zhang J, Gui M, Wang Q, et al. [**Hierarchical Topic Model Based Object Association for Semantic SLAM**](https://ieeexplore.ieee.org/abstract/document/8794595)[J]. IEEE transactions on visualization and computer graphics, **2019**.
    + <font color = blue>**基于层次主题模型的语义 SLAM 对象关联** </font>
    + 西班牙萨拉戈萨大学，**ORB-SLAM 作者**
    + 期刊：中科院三区， JCR Q1，IF 3.78
+ [ ] **[15]** Gählert N, Wan J J, Weber M, et al. [**Beyond Bounding Boxes: Using Bounding Shapes for Real-Time 3D Vehicle Detection from Monocular RGB Images**](https://ieeexplore.ieee.org/abstract/document/8814036)[C]//2019 IEEE Intelligent Vehicles Symposium (IV). IEEE, **2019**: 675-682.
    + <font color = blue>超越边界框：使用边界形状从单目 RGB 图像中进行实时 3D 车辆检测</font>
    + 德国耶拿大学
+ [ ] **[16]** Yang N, Wang R, Stuckler J, et al. [**Deep virtual stereo odometry: Leveraging deep depth prediction for monocular direct sparse odometry**](http://openaccess.thecvf.com/content_ECCV_2018/papers/Nan_Yang_Deep_Virtual_Stereo_ECCV_2018_paper.pdf)[C]//Proceedings of the European Conference on Computer Vision (**ECCV**). **2018**: 817-833.
    + <font color = blue>深度虚拟双目里程计：利用单目直接稀疏里程计的深度预测</font>
    + 慕尼黑工业大学；[作者主页](https://vision.in.tum.de/members/yangn)，[项目主页](https://vision.in.tum.de/research/vslam/dvso)
+ [ ] **[17]** Liu H, Ma H, Zhang L. [**Visual Odometry based on Semantic Supervision**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8803013)[C]//2019 IEEE International Conference on Image Processing (**ICIP**). IEEE, **2019**: 2566-2570.
    + <font color = blue>**基于语义监督的视觉里程计** </font>
    + 清华大学；会议 ICIP：CCF 计算机图形学与多媒体 C 类会议
+ [ ] **[18]** Wald J, Avetisyan A, Navab N, et al. [**RIO: 3D Object Instance Re-Localization in Changing Indoor Environments**](https://arxiv.org/abs/1908.06109)[J]. arXiv preprint arXiv:1908.06109, **2019**.
    + <font color = blue>RIO:改变室内环境的 3D 物体实例重定位</font>
    + TUM，Google，[项目主页](https://waldjohannau.github.io/RIO/)，开放数据集

---

#### 3. AR & MR & VR

+ [ ] **[19]** Su Y, Rambach J, Minaskan N, et al. [**Deep Multi-State Object Pose Estimation for Augmented Reality Assembly**](https://www.researchgate.net/profile/Jason_Rambach/publication/335207627_Deep_Multi-State_Object_Pose_Estimation_for_Augmented_Reality_Assembly/links/5d56c09d92851cb74c714724/Deep-Multi-State-Object-Pose-Estimation-for-Augmented-Reality-Assembly.pdf)[C]. IEEE International Symposium on Mixed and Augmented Reality (**ISMAR**) **2019**
    + <font color = blue>增强现实装备的深度多状态目标姿态估计</font>
    + 德国人工智能研究中心
    
---

#### 4. Learning others

+ [ ] **[20]** Huang X, Dai Z, Chen W, et al. [**Improving Keypoint Matching Using a Landmark-Based Image Representation**](https://ieeexplore.ieee.org/abstract/document/8794420)[C]//2019 International Conference on Robotics and Automation (**ICRA**). IEEE, **2019**: 1281-1287.
    + <font color = blue>利用基于地标的图像表示改进关键点匹配</font>
    + 广东工业大学
+ [ ] **[21]** Puscas M M, Xu D, Pilzer A, et al. [**Structured Coupled Generative Adversarial Networks for Unsupervised Monocular Depth Estimation**](https://arxiv.org/pdf/1908.05794.pdf)[J]. arXiv preprint arXiv:1908.05794, **2019**.
    + <font color = blue>无监督单目深度估计的结构耦合生成对抗网络</font>
    + 华为、牛津大学 &emsp;[**代码开源**](https://github.com/mihaipuscas/3dv---coupled-crf-disparity)（还未放出）
    
---

#### 5. Others

+ [x] **[22]** Yang B, Xu X, Li J, et al. [**Landmark Generation in Visual Place Recognition Using Multi-Scale Sliding Window for Robotics**](https://www.mdpi.com/2076-3417/9/15/3146)[J]. Applied Sciences, **2019**, 9(15): 3146.
    + <font color = blue>**基于多尺度滑动窗口的机器人视觉地点识别中的地标生成** </font>
    + 东南大学 &emsp;期刊：开源期刊，中科院三区，JCR Q3
+ [x] **[23]** Hofstetter I, Sprunk M, Schuster F, et al. [**On Ambiguities in Feature-Based Vehicle Localization and their A Priori Detection in Maps**](https://ieeexplore.ieee.org/abstract/document/8813978)[C]//2019 IEEE Intelligent Vehicles Symposium (IV). IEEE, **2019**: 1192-1198.
    + <font color = blue>**基于特征的车辆模糊定位及其在地图中的先验检测** </font>
    + SLAM 中的物体数据关联可参考
+ [ ] **[24]** Kümmerle J, Sons M, Poggenhans F, et al. [**Accurate and Efficient Self-Localization on Roads using Basic Geometric Primitives**](https://ieeexplore.ieee.org/abstract/document/8793497)[C]//2019 International Conference on Robotics and Automation (**ICRA**). IEEE, **2019**: 5965-5971.
    + <font color = blue>基于几何元素在道路中进行准确有效的自定位</font>
    + 德国卡尔斯鲁厄理工学院

---

### 2019 年 10 月论文更新（22 篇）

#### 1. Geometric SLAM

+ [x] **[1]** Sumikura S, Shibuya M, Sakurada K. [**OpenVSLAM: A Versatile Visual SLAM Framework**](https://arxiv.org/pdf/1910.01122.pdf)[J]. arXiv preprint arXiv:1910.01122, **2019**.
    + <font color = blue>**OpenVSLAM: 通用的视觉 SLAM 框架**</font>
    + [代码开源](https://github.com/xdspacelab/openvslam)
    + 日本国家先进工业科学技术研究所，其他工作：Yokozuka M, Oishi S, Simon T, et al. [**VITAMIN-E: VIsual Tracking And Mapping with Extremely Dense Feature Points**](https://arxiv.org/pdf/1904.10324.pdf)[J]. arXiv preprint arXiv:1904.10324, **2019**.
+ [x] **[2]** Chen Y, Huang S, Fitch R, et al. [**On-line 3D active pose-graph SLAM based on key poses using graph topology and sub-maps**](https://ieeexplore.ieee.org/abstract/document/8793632)[C]//2019 International Conference on Robotics and Automation (**ICRA**). IEEE, **2019**: 169-175.
    + <font color = blue>**使用图形拓扑和子图的基于关键姿势的在线 3D 活跃位姿图SLAM**</font>
    + 悉尼科技大学
+ [ ] **[3]** Pfrommer B, Daniilidis K. [**TagSLAM: Robust SLAM with Fiducial Markers**](https://arxiv.org/pdf/1910.00679.pdf)[J]. arXiv preprint arXiv:1910.00679, **2019**.
    + <font color = blue>**TagSLAMM：具有基准标记的鲁棒 SLAM**</font>
    + 宾夕法尼亚大学通用机器人，自动化，感应和感知实验室，[项目主页](https://berndpfrommer.github.io/tagslam_web/)
+ [ ] **[4]** Lin T Y, Clark W, Eustice R M, et al. [**Adaptive Continuous Visual Odometry from RGB-D Images**](https://arxiv.org/pdf/1910.00713.pdf)[J]. arXiv preprint arXiv:1910.00713, **2019**.
    + <font color = blue>RGB-D 图像的自适应连续视觉里程计</font>
    + 密西根大学
+ [ ] **[5]** Y Yang, P Geneva, K Eckenhoff, G Huang. [**Visual-Inertial Odometry with Point and Line Features**](https://www.researchgate.net/profile/Yulin_Yang3/publication/335821879_Visual-Inertial_Odometry_with_Point_and_Line_Features/links/5d7d3ac892851c87c389c719/Visual-Inertial-Odometry-with-Point-and-Line-Features.pdf), **2019**.
    + <font color = blue>点线 VIO</font>
    + 特拉华大学
+ [ ] **[6]** Tarrio J J, Smitt C, Pedre S. [**SE-SLAM: Semi-Dense Structured Edge-Based Monocular SLAM**](https://arxiv.org/pdf/1909.03917.pdf)[J]. arXiv preprint arXiv:1909.03917, **2019**.
    + <font color = blue>SE-SLAM：基于边的单目半稠密 SLAM</font>
    + 阿根廷巴尔塞罗研究所
+ [ ] **[7]** Wu X, Pradalier C. [**Robust Semi-Direct Monocular Visual Odometry Using Edge and Illumination-Robust Cost**](https://arxiv.org/pdf/1909.11362.pdf)[J]. arXiv preprint arXiv:1909.11362, **2019**.
    + <font color = blue>利用边缘和光照鲁棒成本的单目半直接法视觉里程计</font>
    + 佐治亚理工学院
+ [ ] **[8]** Pan Z, Chen H, Li S, et al. [**ClusterMap Building and Relocalization in Urban Environments for Unmanned Vehicles**](https://www.mdpi.com/1424-8220/19/19/4252/htm)[J]. Sensors, **2019**, 19(19): 4252.
    + <font color = blue>无人驾驶车辆在城市环境中的 ClusterMap 构建和重定位</font>
    + 哈工大深圳，港中文，期刊 Sensors：开源期刊，中科院三区 JCR Q2Q3 IF 3.014
+ [ ] **[9]** Zhang M, Zuo X, Chen Y, et al. [**Localization for Ground Robots: On Manifold Representation, Integration, Re-Parameterization, and Optimization**](https://arxiv.org/pdf/1909.03423.pdf)[J]. arXiv preprint arXiv:1909.03423, **2019**.
    + <font color = blue>地面机器人的定位：流形表示，积分，重新参数化和优化</font>
    + 阿里巴巴人工智能实验室
+ [ ] **[10]** Kirsanov P, Gaskarov A, Konokhov F, et al. [**DISCOMAN: Dataset of Indoor SCenes for Odometry, Mapping And Navigation**](https://arxiv.org/pdf/1909.12146.pdf)[J]. arXiv preprint arXiv:1909.12146, **2019**.
    + <font color = blue>DISCOMAN：用于里程计、制图和导航的室内场景数据集</font>
    + 三星 AI 中心，数据集随论文正式发表放出

---

#### 2. Semantic/Learning SLAM

+ [x] **[11]** Pire T, Corti J, Grinblat G. [**Online Object Detection and Localization on Stereo Visual SLAM System**](https://www.researchgate.net/profile/Taihu_Pire/publication/335432416_Online_Object_Detection_and_Localization_on_Stereo_Visual_SLAM_System/links/5d663a14a6fdccf343f93830/Online-Object-Detection-and-Localization-on-Stereo-Visual-SLAM-System.pdf)[J]. Journal of Intelligent & Robotic Systems, **2019**: 1-10.
    + <font color = blue>**在线目标检测和定位的双目视觉 SLAM**</font>
    + 阿根廷国际信息科学中心，[**代码开源**](https://github.com/CIFASIS/object-detection-sptam)
+ [x] **[12]** Rosinol A, Abate M, Chang Y, et al. [**Kimera: an Open-Source Library for Real-Time Metric-Semantic Localization and Mapping**](https://arxiv.org/pdf/1910.02490.pdf)[J]. arXiv preprint arXiv:1910.02490, **2019**.
    + <font color = blue>**Kimera：用于实时度量-语义定位和建图的开源库**</font>
    + MIT，[**代码开源**](https://github.com/MIT-SPARK/Kimera)，[演示视频](https://www.youtube.com/watch?v=3lVD0i-5p10)
+ [ ] **[13]** Feng Q, Meng Y, Shan M, et al. [**Localization and Mapping using Instance-specific Mesh Models**](https://natanaso.github.io/ref/Feng_DeformableMeshModel_IROS19.pdf)[J].**IROS 2019**
    + <font color = blue>使用特定实例网格模型进行定位和建图</font>
    + 加州大学圣地亚哥分校语境机器人研究所，[课题组](https://existentialrobotics.org/pages/publications.html)
+ [ ] **[14]** Liao Z, Shi J, Qi X, et al. [**Coarse-To-Fine Visual Localization Using Semantic Compact Map**](https://arxiv.org/pdf/1910.04936.pdf)[J]. arXiv preprint arXiv:1910.04936, **2019**.
    + <font color = blue>使用语义紧凑图的从粗糙到精细的视觉定位</font>
    + 北航，face++
+ [x] **[15]** Doherty K, Baxter D, Schneeweiss E, et al. [**Probabilistic Data Association via Mixture Models for Robust Semantic SLAM**](https://arxiv.org/pdf/1909.11213.pdf)[J]. arXiv preprint arXiv:1909.11213, **2019**.
    + <font color = blue>**鲁棒的语义 SLAM 中混合模型的概率数据关联**</font>
    + MIT，好像就是之前 [ICRA 2019 多模态概率数据关联](https://marinerobotics.mit.edu/sites/default/files/doherty_icra2019_revised.pdf)
+ [ ] **[16]** Jung E, Yang N, Cremers D. [**Multi-Frame GAN: Image Enhancement for Stereo Visual Odometry in Low Light**](https://arxiv.org/pdf/1910.06632.pdf)[J]. arXiv preprint arXiv:1910.06632, **2019**.
    + <font color = blue>Multi-Frame GAN：弱光照双目视觉里程计的图像增强</font>
    + 慕尼黑工业大学、澳大利亚国立大学，Artisense 自动驾驶公司，LSD、DSO 作者，[Google Scholar](https://scholar.google.com/citations?user=cXQciMEAAAAJ&hl=zh-CN&oi=sra)
+ [x] **[17]** Yu F, Shang J, Hu Y, et al. [**NeuroSLAM: a brain-inspired SLAM system for 3D environments**](https://www.researchgate.net/profile/Fangwen_Yu/publication/336164484_NeuroSLAM_a_brain-inspired_SLAM_system_for_3D_environments/links/5d95f38d458515c1d3908a20/NeuroSLAM-a-brain-inspired-SLAM-system-for-3D-environments.pdf)[J]. Biological Cybernetics, **2019**: 1-31.
    + <font color = blue>**NeuroSLAM：针对 3D 环境的脑启发式 SLAM 系统**</font>
    + 昆士兰科技大学，Rat SLAM 作者，[**代码开源**](https://github.com/cognav/NeuroSLAM)
+ [ ] **[18]** Zeng T, Si B. [**A Brain-Inspired Compact Cognitive Mapping System**](https://arxiv.org/pdf/1910.03913.pdfv)[J]. arXiv preprint arXiv:1910.03913, **2019**.
    + <font color = blue>脑启发的紧凑型认知地图系统</font>
    + 沈自所

---

#### 3. Learning others

+ [x] **[19]** Zhou Y, Qi H, Huang J, et al. [**NeurVPS: Neural Vanishing Point Scanning via Conic Convolution**](https://arxiv.org/pdf/1910.06316.pdf)[J]. arXiv preprint arXiv:1910.06316, **2019**.
    + <font color = blue>**NeurVPS：通过圆锥卷积的神经消失点扫描**</font>
    + 加州伯克利，[代码开源](https://github.com/zhou13/neurvps)
+ [ ] **[20]** Alhashim I, Wonka P. [**High Quality Monocular Depth Estimation via Transfer Learning**]()[J]. arXiv preprint arXiv:1812.11941, **2018**.
    + <font color = blue>通过迁移学习进行高质量单眼深度估计</font>
    + 阿卜杜拉国王科技大学，[代码开源](https://github.com/ialhashim/DenseDepth)

---

#### 4. Others

+ [ ] **[21 ]** Pei L, Liu K, Zou D, et al. [**IVPR: An Instant Visual Place Recognition Approach based on Structural Lines in Manhattan World**](https://ieeexplore.ieee.org/abstract/document/8836504)[J]. IEEE Transactions on Instrumentation and Measurement, **2019**.
    + <font color = blue>IVPR：基于曼哈顿世界中的结构线的即时视觉位置识别方法</font>
    + 上交邹丹平老师，期刊：中科院三区 JCR Q1Q2 IF2.98
+ [ ] **[22]** Sjanic Z. [**Particle Filtering Approach for Data Association**](http://users.isy.liu.se/en/rt/zoran/Publ/fusion2019.pdf)[C]//22nd International Conference on Information Fusion. **2019**.
    + <font color = blue>粒子滤波算法用于数据关联</font>
    + 上交邹丹平老师，期刊：中科院三区 JCR Q1Q2 IF2.98

---
> wuyanminmax@gmail.com    
