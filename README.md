# Mark
## 前言
以下收集的论文、代码等资料主要与本人的学习方向**视觉 SLAM、增强现实** 相关。    
目前（2019年3月）**重点关注前端，语义、传感器融合、稠密建图也略有关注**，所以资料的收集范围也与自己的兴趣比较一致，无法涵盖视觉 SLAM 的所有研究，请谨慎参考。   
`1. 论文` ：**代码开源**的相关论文    
`2. 算法、知识点与代码` ：一些零散的知识点和算法    
`3. 工具` ：论文或实验用到的一些工具    
`4. 优秀作者与团队` ：在自己感兴趣领域比较**优秀的值得关注的团队或个人**    
`5. 资料` ：可供参考的资料或备忘    
`6. 论文` ：自己感兴趣方向的**最新论文**，大概半个月一更新    
能力有限，欢迎大家补充。
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
  
---

## 5. 资料
+ SLAM 最新研究更新 Recent_SLAM_Research ：https://github.com/YiChenCityU/Recent_SLAM_Research
+ 西北工大智能系统实验室 SLAM 培训：https://github.com/zdzhaoyong/SummerCamp2018

---

## 6. 近期论文（持续更新）
### 2019.03.14 更新（13 篇）
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
### 2019.04.01 更新（17 篇）
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
> wuyanminmax@gmail.com    
