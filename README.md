> **最近更新 2020 年 11 月 9 日：10 月论文更新 +22**

# Visual_SLAM_Related_Research
> @Author：吴艳敏    
@E-mail ：wuyanminmax@gmail.com    
@github ：[yanmin-wu](https://github.com/yanmin-wu) | [wuxiaolang](https://github.com/wuxiaolang)

## 前言
&emsp;&emsp;以下收集的论文、代码等资料主要与本人的学习方向 **视觉 SLAM、增强现实** 相关。    
&emsp;&emsp;目前**重点关注 VO、物体级 SLAM 和语义数据关联**， 对传感器融合、稠密建图也略有关注，所以资料的收集范围也与自己的兴趣比较一致，无法涵盖视觉 SLAM 的所有研究，**请谨慎参考**。主要内容包括：   
`1. 开源代码` ：经典、优秀的**开源工程**    
`2. 优秀作者与实验室` ：在自己感兴趣领域比较**优秀的值得关注的团队或个人**    
`3. SLAM 学习资料` ：**SLAM 相关学习资料**、视频、数据集、公众号和代码注释    
`4. 近期论文` ：自己感兴趣方向的**最新论文**，大概**一个月一更新**（部分论文质量无法保证，主要以对现阶段的工作可能有用为收录原则，请谨慎参考）。部分论文的详/泛读笔记放在我的[博客](https://wym.netlify.com/post/)/[List](https://zhuanlan.zhihu.com/p/138737870)上。    
&emsp;&emsp;**`注：若本仓库内容出现任何错误请批评指出，定及时修改。`**    
&emsp;&emsp;本仓库于 2019 年 3 月（研一下）开始整理（私密）🌚。    
&emsp;&emsp;本仓库于 2020 年 3 月（研二下）公开，正好一周年🌝。    
  > **一些总结性博客或原创性工作：**    
  > **1.** [100 项开源视觉 SLAM 项目够你用了吗？](https://zhuanlan.zhihu.com/p/115599978) 2020 年 3 月 31 日发布于[知乎](https://zhuanlan.zhihu.com/p/115599978)和公众号[3D 视觉工坊] &emsp; &emsp; | [PDF 版本](https://gitee.com/wuxiaolang2008/Notes_of_wu/raw/master/blog/20200330_%E5%BC%80%E6%BA%90SLAM%E4%BB%A3%E7%A0%81%E5%90%88%E9%9B%86_by_%E5%90%B4%E8%89%B3%E6%95%8F.pdf)    
  > **2.** [SLAM 领域国内外优秀实验室汇总](https://zhuanlan.zhihu.com/p/130530891)  &emsp; &emsp; &nbsp; 2020 年 4 月 26 日发布于[知乎](https://zhuanlan.zhihu.com/p/130530891)和公众号[泡泡机器人 SLAM] | [PDF 版本](https://gitee.com/wuxiaolang2008/Notes_of_wu/raw/master/blog/20200418_SLAM%E9%A2%86%E5%9F%9F%E5%9B%BD%E5%86%85%E5%A4%96%E4%BC%98%E7%A7%80%E5%AE%9E%E9%AA%8C%E5%AE%A4%E6%B1%87%E6%80%BB_by_%E5%90%B4%E8%89%B3%E6%95%8F.pdf)    
  > **3.** 单目物体级 SLAM 中的数据关联问题： **EAO-SLAM: Monocular Semi-Dense Object SLAM Based on Ensemble Data Association**, IROS 2020, Wu Y, Zhang Y, Zhu D, Feng Y, S Coleman, D Kerr [[**PDF**](https://arxiv.org/abs/2004.12730)] [[**Code**](https://github.com/yanmin-wu/EAO-SLAM)] [[**YouTube**](https://youtu.be/pvwdQoV1KBI)] [[**Bilibili**](https://www.bilibili.com/video/av94805216)] [[**Project page**](https://yanmin-wu.github.io/project/eaoslam/)]

## 目录
> <small>推荐使用 [GayHub](https://github.com/jawil/GayHub) 插件自动在侧栏展开目录</small>
+ [**1.开源代码**](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#1-%E5%BC%80%E6%BA%90%E4%BB%A3%E7%A0%81)
  + [**1.1 Geometric SLAM**](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#smile-11-geometric-slam)
  + [**1.2 Semantic / Deep SLAM**](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#smile-12-semantic--deep-slam)
  + [**1.3 Multi-Landmarks / Object SLAM**](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#smile-13-multi-landmarks--object-slam)
  + [**1.4 Sensor Fusion**](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#smile-14-sensor-fusion)
  + [**1.5 Dynamic SLAM**](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#smile-15-dynamic-slam)
  + [**1.6 Mapping**](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#smile-16-mapping)
  + [**1.7 Optimization**](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#smile-17-optimization)
+ [**2. 优秀作者与实验室**](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2-%E4%BC%98%E7%A7%80%E4%BD%9C%E8%80%85%E4%B8%8E%E5%AE%9E%E9%AA%8C%E5%AE%A4)
+ [**3. SLAM 学习资料**](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#3-SLAM-%E5%AD%A6%E4%B9%A0%E8%B5%84%E6%96%99)
+ [**4. 近期论文更新**](https://github.com/wuxiaolang/Mark/blob/master/README.md#4-%E8%BF%91%E6%9C%9F%E8%AE%BA%E6%96%87%E6%8C%81%E7%BB%AD%E6%9B%B4%E6%96%B0)
  + [2020 年 10 月论文更新（22 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2020-%E5%B9%B4-10-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B022-%E7%AF%87)
  + [2020 年 09 月论文更新（20 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2020-%E5%B9%B4-9-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B020-%E7%AF%87)
  + [2020 年 08 月论文更新（30 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2020-%E5%B9%B4-8-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B030-%E7%AF%87)
  + [2020 年 07 月论文更新（20 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2020-%E5%B9%B4-7-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B020-%E7%AF%87)
  + [2020 年 06 月论文更新（20 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2020-%E5%B9%B4-6-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B020-%E7%AF%87)
  + [2020 年 05 月论文更新（20 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2020-%E5%B9%B4-5-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B020-%E7%AF%87)
  + [2020 年 04 月论文更新（22 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2020-%E5%B9%B4-4-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B022-%E7%AF%87)
  + [2020 年 03 月论文更新（23 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2020-%E5%B9%B4-3-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B023-%E7%AF%87)
  + [2020 年 02 月论文更新（17 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2020-%E5%B9%B4-2-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B017-%E7%AF%87)
  + [2020 年 01 月论文更新（26 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2020-%E5%B9%B4-1-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B026-%E7%AF%87)
  + -- ↑ 2020年 ↑ === ↓ 2019年 ↓ --
  + [2019 年 12 月论文更新（23 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2019-%E5%B9%B4-12-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B023-%E7%AF%87)
  + [2019 年 11 月论文更新（17 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2019-%E5%B9%B4-11-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B017-%E7%AF%87)
  + [2019 年 10 月论文更新（22 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2019-%E5%B9%B4-10-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B022-%E7%AF%87) 
  + [2019 年 09 月论文更新（24 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2019-%E5%B9%B4-9-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B024-%E7%AF%87)
  + [2019 年 08 月论文更新（26 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2019-%E5%B9%B4-8-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B026-%E7%AF%87)
  + [2019 年 07 月论文更新（36 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2019-%E5%B9%B4-7-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B036-%E7%AF%87)
  + [2019 年 06 月论文更新（21 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2019-%E5%B9%B4-6-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B021-%E7%AF%87)
  + [2019 年 05 月论文更新（51 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2019-%E5%B9%B4-5-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B051-%E7%AF%87)
  + [2019 年 04 月论文更新（17 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2019-%E5%B9%B4-4-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B017-%E7%AF%87)
  + [2019 年 03 月论文更新（13 篇）](https://github.com/wuxiaolang/Visual_SLAM_Related_Research#2019-%E5%B9%B4-3-%E6%9C%88%E8%AE%BA%E6%96%87%E6%9B%B4%E6%96%B013-%E7%AF%87)

---

## 1. 开源代码
> 这一部分整理之后发布在知乎（2020 年 3 月 31 日）：https://zhuanlan.zhihu.com/p/115599978/

### :smile: 1.1 Geometric SLAM

#### 1. PTAM 

+ **论文**：Klein G, Murray D. [**Parallel tracking and mapping for small AR workspaces**](http://www.robots.ox.ac.uk/ActiveVision/Publications/klein_murray_ismar2007/klein_murray_ismar2007.pdf)[C]//Mixed and Augmented Reality, 2007. ISMAR 2007. 6th IEEE and ACM International Symposium on. IEEE, **2007**: 225-234.
+ **代码**：https://github.com/Oxford-PTAM/PTAM-GPL
+ 工程地址：http://www.robots.ox.ac.uk/~gk/PTAM/
+ 作者其他研究：http://www.robots.ox.ac.uk/~gk/publications.html

#### 2. S-PTAM（双目 PTAM）

+ **论文**：Taihú Pire,Thomas Fischer, Gastón Castro, Pablo De Cristóforis, Javier Civera and Julio Jacobo Berlles. [**S-PTAM: Stereo Parallel Tracking and Mapping**](http://webdiis.unizar.es/~jcivera/papers/pire_etal_ras17.pdf). Robotics and Autonomous Systems, **2017**.
+ **代码**：https://github.com/lrse/sptam
+ 作者其他论文：Castro G, Nitsche M A, Pire T, et al. [**Efficient on-board Stereo SLAM through constrained-covisibility strategies**](https://www.researchgate.net/profile/Gaston_Castro/publication/332147108_Efficient_on-board_Stereo_SLAM_through_constrained-covisibility_strategies/links/5cacb327a6fdccfa0e7c3e4b/Efficient-on-board-Stereo-SLAM-through-constrained-covisibility-strategies.pdf)[J]. Robotics and Autonomous Systems, **2019**.

#### 3. MonoSLAM

+ **论文**：Davison A J, Reid I D, Molton N D, et al. [**MonoSLAM: Real-time single camera SLAM**](https://ieeexplore.ieee.org/abstract/document/4160954/)[J]. IEEE transactions on pattern analysis and machine intelligence, **2007**, 29(6): 1052-1067.
+ **代码**：https://github.com/hanmekim/SceneLib2

#### 4. ORB-SLAM2

+ **论文**：Mur-Artal R, Tardós J D. [**Orb-slam2: An open-source slam system for monocular, stereo, and rgb-d cameras**](https://github.com/raulmur/ORB_SLAM2)[J]. IEEE Transactions on Robotics, **2017**, 33(5): 1255-1262.
+ **代码**：https://github.com/raulmur/ORB_SLAM2
+ 作者其他论文：
    + **单目半稠密建图**：Mur-Artal R, Tardós J D. [Probabilistic Semi-Dense Mapping from Highly Accurate Feature-Based Monocular SLAM](https://www.researchgate.net/profile/Raul_Mur-Artal/publication/282807894_Probabilistic_Semi-Dense_Mapping_from_Highly_Accurate_Feature-Based_Monocular_SLAM/links/561cd04308ae6d17308ce267.pdf)[C]//Robotics: Science and Systems. **2015**, 2015.
    + **VIORB**：Mur-Artal R, Tardós J D. [Visual-inertial monocular SLAM with map reuse](https://arxiv.org/pdf/1610.05949.pdf)[J]. IEEE Robotics and Automation Letters, **2017**, 2(2): 796-803.
    + **多地图**：Elvira R, Tardós J D, Montiel J M M. [ORBSLAM-Atlas: a robust and accurate multi-map system](https://arxiv.org/pdf/1908.11585)[J]. arXiv preprint arXiv:1908.11585, **2019**.

> 以下5, 6, 7, 8几项是 TUM 计算机视觉组全家桶，官方主页：https://vision.in.tum.de/research/vslam/dso

#### 5. DSO

+ **论文**：Engel J, Koltun V, Cremers D. [**Direct sparse odometry**](https://ieeexplore.ieee.org/iel7/34/4359286/07898369.pdf)[J]. IEEE transactions on pattern analysis and machine intelligence, **2017**, 40(3): 611-625.
+ **代码**：https://github.com/JakobEngel/dso
+ **双目 DSO**：Wang R, Schworer M, Cremers D. [**Stereo DSO: Large-scale direct sparse visual odometry with stereo cameras**](http://openaccess.thecvf.com/content_ICCV_2017/papers/Wang_Stereo_DSO_Large-Scale_ICCV_2017_paper.pdf)[C]//Proceedings of the IEEE International Conference on Computer Vision. **2017**: 3903-3911.
+ **VI-DSO**：Von Stumberg L, Usenko V, Cremers D. [**Direct sparse visual-inertial odometry using dynamic marginalization**](https://arxiv.org/pdf/1804.05625)[C]//2018 IEEE International Conference on Robotics and Automation (ICRA). IEEE, **2018**: 2510-2517.

#### 6. LDSO

+ 高翔在 DSO 上添加闭环的工作
+ **论文**：Gao X, Wang R, Demmel N, et al. [**LDSO: Direct sparse odometry with loop closure**](https://arxiv.org/pdf/1808.01111)[C]//2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2018**: 2198-2204.
+ **代码**：https://github.com/tum-vision/LDSO

#### 7. LSD-SLAM

+ **论文**：Engel J, Schöps T, Cremers D. [**LSD-SLAM: Large-scale direct monocular SLAM**](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.646.7193&rep=rep1&type=pdf)[C]//European conference on computer vision. Springer, Cham, **2014**: 834-849.
+ **代码**：https://github.com/tum-vision/lsd_slam

#### 8. DVO-SLAM

+ **论文**：Kerl C, Sturm J, Cremers D. [**Dense visual SLAM for RGB-D cameras**]()[C]//2013 IEEE/RSJ International Conference on Intelligent Robots and Systems. IEEE, **2013**: 2100-2106.
+ **代码 1**：https://github.com/tum-vision/dvo_slam
+ **代码 2**：https://github.com/tum-vision/dvo
+ 其他论文：
    + Kerl C, Sturm J, Cremers D. [**Robust odometry estimation for RGB-D cameras**](https://vision.in.tum.de/_media/spezial/bib/kerl13icra.pdf)[C]//2013 IEEE international conference on robotics and automation. IEEE, **2013**: 3748-3754.
    + Steinbrücker F, Sturm J, Cremers D. [**Real-time visual odometry from dense RGB-D images**](https://jsturm.de/publications/data/steinbruecker_sturm_cremers_iccv11.pdf)[C]//2011 IEEE international conference on computer vision workshops (ICCV Workshops). IEEE, **2011**: 719-722.

#### 9. SVO

+ [苏黎世大学机器人与感知课题组](http://rpg.ifi.uzh.ch/publications.html)
+ **论文**：Forster C, Pizzoli M, Scaramuzza D. [**SVO: Fast semi-direct monocular visual odometry**](https://www.zora.uzh.ch/id/eprint/125453/1/ICRA14_Forster.pdf)[C]//2014 IEEE international conference on robotics and automation (ICRA). IEEE, **2014**: 15-22.
+ **代码**：https://github.com/uzh-rpg/rpg_svo
+ Forster C, Zhang Z, Gassner M, et al. [**SVO: Semidirect visual odometry for monocular and multicamera systems**](https://www.zora.uzh.ch/id/eprint/127902/1/TRO16_Forster-SVO.pdf)[J]. IEEE Transactions on Robotics, **2016**, 33(2): 249-265.

#### 10. DSM

+ **论文**：Zubizarreta J, Aguinaga I, Montiel J M M. [**Direct sparse mapping**](https://arxiv.org/pdf/1904.06577)[J]. arXiv preprint arXiv:1904.06577, **2019**.
+ **代码**：https://github.com/jzubizarreta/dsm ；[Video](https://www.youtube.com/watch?v=sj1GIF-7BYo&feature=youtu.be)

#### 11. openvslam

+ 论文：Sumikura S, Shibuya M, Sakurada K. [**OpenVSLAM: A Versatile Visual SLAM Framework**](https://dl.acm.org/ft_gateway.cfm?id=3350539&type=pdf)[C]//Proceedings of the 27th ACM International Conference on Multimedia. **2019**: 2292-2295.
+ 代码：https://github.com/xdspacelab/openvslam ；[文档](https://openvslam.readthedocs.io/en/master/)

#### 12. se2lam（地面车辆位姿估计的视觉里程计）

+ **论文**：Zheng F, Liu Y H. [**Visual-Odometric Localization and Mapping for Ground Vehicles Using SE (2)-XYZ Constraints**](https://ieeexplore.ieee.org/abstract/document/8793928)[C]//2019 International Conference on Robotics and Automation (**ICRA**). IEEE, **2019**: 3556-3562.
+ **代码**：https://github.com/izhengfan/se2lam
+ 作者的另外一项工作
    + 论文：Zheng F, Tang H, Liu Y H. [**Odometry-vision-based ground vehicle motion estimation with se (2)-constrained se (3) poses**](https://ieeexplore.ieee.org/abstract/document/8357438/)[J]. IEEE transactions on cybernetics, **2018**, 49(7): 2652-2663.
    + 代码：https://github.com/izhengfan/se2clam

#### 13. GraphSfM（基于图的并行大规模 SFM）

+ 论文：Chen Y, Shen S, Chen Y, et al. [**Graph-Based Parallel Large Scale Structure from Motion**](https://arxiv.org/pdf/1912.10659.pdf)[J]. arXiv preprint arXiv:1912.10659, **2019**.
+ 代码：https://github.com/AIBluefisher/GraphSfM

#### 14. LCSD_SLAM（松耦合的半直接法单目 SLAM）

+ **论文**：Lee S H, Civera J. [**Loosely-Coupled semi-direct monocular SLAM**](https://arxiv.org/pdf/1807.10073)[J]. IEEE Robotics and Automation Letters, **2018**, 4(2): 399-406.
+ **代码**：https://github.com/sunghoon031/LCSD_SLAM ；[谷歌学术](https://scholar.google.com/citations?user=FeMFP7EAAAAJ&hl=zh-CN&oi=sra) ；[演示视频](https://www.youtube.com/watch?v=j7WnU7ZpZ8c&feature=youtu.be)
+ 作者另外一篇关于**单目尺度**的文章 [代码开源](https://github.com/sunghoon031/stability_scale) ：Lee S H, de Croon G. [**Stability-based scale estimation for monocular SLAM**](https://www.researchgate.net/profile/Seong_Hun_Lee3/publication/322260802_Stability-based_Scale_Estimation_for_Monocular_SLAM/links/5b3def9b0f7e9b0df5f42d67/Stability-based-Scale-Estimation-for-Monocular-SLAM.pdf)[J]. IEEE Robotics and Automation Letters, **2018**, 3(2): 780-787.

#### 15. RESLAM（基于边的 SLAM）

+ **论文**：Schenk F, Fraundorfer F. [**RESLAM: A real-time robust edge-based SLAM system**](https://ieeexplore.ieee.org/abstract/document/8794462/)[C]//2019 International Conference on Robotics and Automation (ICRA). IEEE, **2019**: 154-160.
+ **代码**：https://github.com/fabianschenk/RESLAM ； [项目主页](https://graz.pure.elsevier.com/en/publications/reslam-a-real-time-robust-edge-based-slam-system)

#### 16. scale_optimization（将单目 DSO 拓展到双目）

+ **论文**：Mo J, Sattar J. [**Extending Monocular Visual Odometry to Stereo Camera System by Scale Optimization**](https://arxiv.org/pdf/1905.12723.pdf)[C]. International Conference on Intelligent Robots and Systems (**IROS**), **2019**.
+ **代码**：https://github.com/jiawei-mo/scale_optimization

#### 17. BAD-SLAM（直接法 RGB-D SLAM）

+ **论文**：Schops T, Sattler T, Pollefeys M. [**BAD SLAM: Bundle Adjusted Direct RGB-D SLAM**](http://openaccess.thecvf.com/content_CVPR_2019/papers/Schops_BAD_SLAM_Bundle_Adjusted_Direct_RGB-D_SLAM_CVPR_2019_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. **2019**: 134-144.
+ **代码**：https://github.com/ETH3D/badslam

#### 18. GSLAM（集成 ORB-SLAM2，DSO，SVO 的通用框架）

+ **论文**：Zhao Y, Xu S, Bu S, et al. [**GSLAM: A general SLAM framework and benchmark**](http://openaccess.thecvf.com/content_ICCV_2019/papers/Zhao_GSLAM_A_General_SLAM_Framework_and_Benchmark_ICCV_2019_paper.pdf)[C]//Proceedings of the IEEE International Conference on Computer Vision. **2019**: 1110-1120.
+ **代码**：https://github.com/zdzhaoyong/GSLAM

#### 19. ARM-VO（运行于 ARM 处理器上的单目 VO）

+ **论文**：Nejad Z Z, Ahmadabadian A H. [**ARM-VO: an efficient monocular visual odometry for ground vehicles on ARM CPUs**](https://link.springer.com/article/10.1007/s00138-019-01037-5)[J]. Machine Vision and Applications, **2019**: 1-10.
+ **代码**：https://github.com/zanazakaryaie/ARM-VO

#### 20. cvo-rgbd（直接法 RGB-D VO）

+ **论文**：Ghaffari M, Clark W, Bloch A, et al. [**Continuous Direct Sparse Visual Odometry from RGB-D Images**](https://arxiv.org/pdf/1904.02266.pdf)[J]. arXiv preprint arXiv:1904.02266, **2019**.
+ **代码**：https://github.com/MaaniGhaffari/cvo-rgbd

#### 21. Map2DFusion（单目 SLAM 无人机图像拼接）

+ **论文**：Bu S, Zhao Y, Wan G, et al. [**Map2DFusion: Real-time incremental UAV image mosaicing based on monocular slam**](http://www.adv-ci.com/publications/2016_IROS.pdf)[C]//2016 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2016**: 4564-4571.
+ **代码**：https://github.com/zdzhaoyong/Map2DFusion

#### 22. CCM-SLAM（多机器人协同单目 SLAM）

+ **论文**：Schmuck P, Chli M. [**CCM‐SLAM: Robust and efficient centralized collaborative monocular simultaneous localization and mapping for robotic teams**](https://onlinelibrary.wiley.com/doi/abs/10.1002/rob.21854)[J]. Journal of Field Robotics, **2019**, 36(4): 763-781.
+ **代码**：https://github.com/VIS4ROB-lab/ccm_slam &emsp; [Video](https://www.youtube.com/watch?v=P3b7UiTlmbQ&feature=youtu.be)

#### 23. ORB-SLAM3

+ 论文：Carlos Campos, Richard Elvira, et al.[**ORB-SLAM3: An Accurate Open-Source Library for Visual, Visual-Inertial and Multi-Map SLAM**](https://arxiv.org/abs/2007.11898)[J]. arXiv preprint arXiv:2007.11898, **2020**.
+ 代码：https://github.com/UZ-SLAMLab/ORB_SLAM3 | [Video](https://www.youtube.com/channel/UCXVt-kXG6T95Z4tVaYlU80Q)

### :smile: 1.2 Semantic / Deep SLAM

#### 1. MsakFusion

+ **论文**：Runz M, Buffier M, Agapito L. [**Maskfusion: Real-time recognition, tracking and reconstruction of multiple moving objects**](https://arxiv.org/pdf/1804.09194)[C]//2018 IEEE International Symposium on Mixed and Augmented Reality (ISMAR). IEEE, **2018**: 10-20.
+ **代码**：https://github.com/martinruenz/maskfusion

#### 2. SemanticFusion

+ **论文**：McCormac J, Handa A, Davison A, et al. [**Semanticfusion: Dense 3d semantic mapping with convolutional neural networks**](https://arxiv.org/pdf/1609.05130.pdf)[C]//2017 IEEE International Conference on Robotics and automation (ICRA). IEEE, **2017**: 4628-4635.
+ **代码**：https://github.com/seaun163/semanticfusion

#### 3. semantic_3d_mapping

+ **论文**：Yang S, Huang Y, Scherer S. [**Semantic 3D occupancy mapping through efficient high order CRFs**](https://arxiv.org/pdf/1707.07388.pdf)[C]//2017 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2017**: 590-597.
+ **代码**：https://github.com/shichaoy/semantic_3d_mapping

#### 4. Kimera（实时度量与语义定位建图开源库）

+ 论文：Rosinol A, Abate M, Chang Y, et al. [**Kimera: an Open-Source Library for Real-Time Metric-Semantic Localization and Mapping**](https://arxiv.org/pdf/1910.02490.pdf)[J]. arXiv preprint arXiv:1910.02490, **2019**.
+ 代码：https://github.com/MIT-SPARK/Kimera ；[演示视频](https://www.youtube.com/watch?v=3lVD0i-5p10)

#### 5. NeuroSLAM（脑启发式 SLAM）

+ **论文**：Yu F, Shang J, Hu Y, et al. [**NeuroSLAM: a brain-inspired SLAM system for 3D environments**](https://www.researchgate.net/profile/Fangwen_Yu/publication/336164484_NeuroSLAM_a_brain-inspired_SLAM_system_for_3D_environments/links/5d95f38d458515c1d3908a20/NeuroSLAM-a-brain-inspired-SLAM-system-for-3D-environments.pdf)[J]. Biological Cybernetics, **2019**: 1-31.
+ **代码**：https://github.com/cognav/NeuroSLAM
+ 第四作者就是 Rat SLAM 的作者，文章也比较了十余种脑启发式的 SLAM

#### 6. gradSLAM（自动分区的稠密 SLAM）

+ **论文**：Jatavallabhula K M, Iyer G, Paull L. [**gradSLAM: Dense SLAM meets Automatic Differentiation**](https://arxiv.org/pdf/1910.10672.pdf)[J]. arXiv preprint arXiv:1910.10672, **2019**.
+ **代码**（预计 20 年 4 月放出）：https://github.com/montrealrobotics/gradSLAM ；[项目主页](http://montrealrobotics.ca/gradSLAM/)，[演示视频](https://www.youtube.com/watch?v=2ygtSJTmo08&feature=youtu.be)

#### 7. ORB-SLAM2 + 目标检测/分割的方案语义建图

+ https://github.com/floatlazer/semantic_slam
+ https://github.com/qixuxiang/orb-slam2_with_semantic_labelling
+ https://github.com/Ewenwan/ORB_SLAM2_SSD_Semantic

#### 8. SIVO（语义辅助特征选择）

+ **论文**：Ganti P, Waslander S. [**Network Uncertainty Informed Semantic Feature Selection for Visual SLAM**](https://ieeexplore.ieee.org/abstract/document/8781616)[C]//2019 16th Conference on Computer and Robot Vision (CRV). IEEE, **2019**: 121-128.
+ **代码**：https://github.com/navganti/SIVO

#### 9. FILD（临近图增量式闭环检测）

+ **论文**：Shan An, Guangfu Che, Fangru Zhou, Xianglong Liu, Xin Ma, Yu Chen.[ **Fast and Incremental Loop Closure Detection using Proximity Graphs**](https://arxiv.org/pdf/1911.10752.pdf). pp. 378-385, The 2019 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS **2019**)
+ **代码**：https://github.com/AnshanTJU/FILD

#### 10. object-detection-sptam（目标检测与双目 SLAM）

+ **论文**：Pire T, Corti J, Grinblat G. [**Online Object Detection and Localization on Stereo Visual SLAM System**](https://www.researchgate.net/profile/Taihu_Pire/publication/335432416_Online_Object_Detection_and_Localization_on_Stereo_Visual_SLAM_System/links/5d663a14a6fdccf343f93830/Online-Object-Detection-and-Localization-on-Stereo-Visual-SLAM-System.pdf)[J]. Journal of Intelligent & Robotic Systems, **2019**: 1-10.
+ **代码**：https://github.com/CIFASIS/object-detection-sptam

#### 11. Map Slammer（单目深度估计 + SLAM）

+ **论文**：Torres-Camara J M, Escalona F, Gomez-Donoso F, et al. [**Map Slammer: Densifying Scattered KSLAM 3D Maps with Estimated Depth**](https://link.springer.com/chapter/10.1007/978-3-030-36150-1_46)[C]//Iberian Robotics conference. Springer, Cham, **2019**: 563-574.
+ **代码**：https://github.com/jmtc7/mapSlammer

#### 12. NOLBO（变分模型的概率 SLAM）

+ **论文**：Yu H, Lee B. [**Not Only Look But Observe: Variational Observation Model of Scene-Level 3D Multi-Object Understanding for Probabilistic SLAM**](https://arxiv.org/pdf/1907.09760.pdf)[J]. arXiv preprint arXiv:1907.09760, **2019**.
+ **代码**：https://github.com/bogus2000/NOLBO

#### 13. GCNv2_SLAM （基于图卷积神经网络 SLAM）

+ **论文**：Tang J, Ericson L, Folkesson J, et al. [**GCNv2: Efficient correspondence prediction for real-time SLAM**](https://ieeexplore.ieee.org/abstract/document/8758836/)[J]. IEEE Robotics and Automation Letters, **2019**, 4(4): 3505-3512.
+ **代码**：https://github.com/jiexiong2016/GCNv2_SLAM &emsp; [Video](https://www.youtube.com/watch?v=pz-gdnR9tAM)

#### 14. semantic_suma（激光语义建图）

+ **论文**：Chen X, Milioto A, Palazzolo E, et al. [**SuMa++: Efficient LiDAR-based semantic SLAM**](https://ieeexplore.ieee.org/abstract/document/8967704/)[C]//2019 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2019**: 4530-4537.
+ **代码**：https://github.com/PRBonn/semantic_suma/ ；[Video](https://www.youtube.com/watch?v=uo3ZuLuFAzk&feature=youtu.be)

#### 15. Neural-SLAM（主动神经 SLAM）

+ **论文**：Chaplot D S, Gandhi D, Gupta S, et al. [**Learning to explore using active neural slam**](https://arxiv.org/abs/2004.05155)[C]. ICLR **2020**.
+ **代码**：https://github.com/devendrachaplot/Neural-SLAM

### :smile: 1.3 Multi-Landmarks / Object SLAM

#### 1. PL-SVO（点线 SVO）

+ **论文**：Gomez-Ojeda R, Briales J, Gonzalez-Jimenez J. [**PL-SVO: Semi-direct Monocular Visual Odometry by combining points and line segments**](http://mapir.isa.uma.es/rgomez/publications/iros16plsvo.pdf)[C]//Intelligent Robots and Systems (IROS), 2016 IEEE/RSJ International Conference on. IEEE, **2016**: 4211-4216.
+ **代码**：https://github.com/rubengooj/pl-svo

#### 2. stvo-pl（双目点线 VO）

+ **论文**：Gomez-Ojeda R, Gonzalez-Jimenez J. [**Robust stereo visual odometry through a probabilistic combination of points and line segments**](https://riuma.uma.es/xmlui/bitstream/handle/10630/11515/icra16rgo.pdf?sequence=1&isAllowed=y)[C]//2016 IEEE International Conference on Robotics and Automation (**ICRA**). IEEE, **2016**: 2521-2526.
+ **代码**：https://github.com/rubengooj/stvo-pl

#### 3. PL-SLAM（点线 SLAM）

+ **论文**：Gomez-Ojeda R, Zuñiga-Noël D, Moreno F A, et al. [**PL-SLAM: a Stereo SLAM System through the Combination of Points and Line Segments**](https://arxiv.org/pdf/1705.09479.pdf)[J]. arXiv preprint arXiv:1705.09479, **2017**.
+ **代码**：https://github.com/rubengooj/pl-slam
+ Gomez-Ojeda R, Moreno F A, Zuñiga-Noël D, et al. [**PL-SLAM: a stereo SLAM system through the combination of points and line segments**](https://arxiv.org/pdf/1705.09479)[J]. IEEE Transactions on Robotics, **2019**, 35(3): 734-746.

#### 4. PL-VIO

+ **论文**：He Y, Zhao J, Guo Y, et al. [**PL-VIO: Tightly-coupled monocular visual–inertial odometry using point and line features**](https://www.mdpi.com/1424-8220/18/4/1159)[J]. Sensors, **2018**, 18(4): 1159.
+ **代码**：https://github.com/HeYijia/PL-VIO
+ **VINS + 线段**：https://github.com/Jichao-Peng/VINS-Mono-Optimization

#### 5. lld-slam（用于 SLAM 的可学习型线段描述符）

+ **论文**：Vakhitov A, Lempitsky V. [**Learnable line segment descriptor for visual SLAM**](https://ieeexplore.ieee.org/iel7/6287639/6514899/08651490.pdf)[J]. IEEE Access, **2019**, 7: 39923-39934.
+ **代码**：https://github.com/alexandervakhitov/lld-slam ；[**Video**](https://www.youtube.com/watch?v=ntFFiwXIhoA)

> <small>点线结合的工作还有很多，国内的比如        
> + 上交邹丹平老师的 Zou D, Wu Y, Pei L, et al. [**StructVIO: visual-inertial odometry with structural regularity of man-made environments**](https://arxiv.org/pdf/1810.06796)[J]. IEEE Transactions on Robotics, **2019**, 35(4): 999-1013.         
> + 浙大的 Zuo X, Xie X, Liu Y, et al. [**Robust visual SLAM with point and line features**](https://arxiv.org/pdf/1711.08654)[C]//2017 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, 2017: 1775-1782.</small>

#### 6. PlaneSLAM

+ **论文**：Wietrzykowski J. [**On the representation of planes for efficient graph-based slam with high-level features**](https://yadda.icm.edu.pl/baztech/element/bwmeta1.element.baztech-7ac7a8f3-9caa-4a34-8a27-8f6c5f43408b)[J]. Journal of Automation Mobile Robotics and Intelligent Systems, **2016**, 10.
+ **代码**：https://github.com/LRMPUT/PlaneSLAM
+ 作者另外一项开源代码，没有找到对应的论文：https://github.com/LRMPUT/PUTSLAM

#### 7. Eigen-Factors（特征因子平面对齐）

+ **论文**：Ferrer G. [**Eigen-Factors: Plane Estimation for Multi-Frame and Time-Continuous Point Cloud Alignment**](http://sites.skoltech.ru/app/data/uploads/sites/50/2019/07/ferrer2019planes.pdf)[C]//2019 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2019**: 1278-1284.
+ **代码**：https://gitlab.com/gferrer/eigen-factors-iros2019 ；[演示视频](https://www.youtube.com/watch?v=_1u_c43DFUE&feature=youtu.be)

#### 8. PlaneLoc

+ **论文**：Wietrzykowski J, Skrzypczyński P. [**PlaneLoc: Probabilistic global localization in 3-D using local planar features**]()[J]. Robotics and Autonomous Systems, **2019**, 113: 160-173.
+ **代码**：https://github.com/LRMPUT/PlaneLoc

#### 9. Pop-up SLAM

+ **论文**：Yang S, Song Y, Kaess M, et al. [**Pop-up slam: Semantic monocular plane slam for low-texture environments**](https://arxiv.org/pdf/1703.07334.pdf)[C]//2016 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2016**: 1222-1229.
+ **代码**：https://github.com/shichaoy/pop_up_slam

#### 10. Object SLAM

+ **论文**：Mu B, Liu S Y, Paull L, et al. [**Slam with objects using a nonparametric pose graph**](https://arxiv.org/pdf/1704.05959.pdf)[C]//2016 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2016**: 4602-4609.
+ **代码**：https://github.com/BeipengMu/objectSLAM ；[Video](https://www.youtube.com/watch?v=YANUWdVLJD4&feature=youtu.be)

#### 11. voxblox-plusplus（物体级体素建图）

+ **论文**：Grinvald M, Furrer F, Novkovic T, et al. [**Volumetric instance-aware semantic mapping and 3D object discovery**](https://arxiv.org/pdf/1903.00268.pdf)[J]. IEEE Robotics and Automation Letters, **2019**, 4(3): 3037-3044.
+ **代码**：https://github.com/ethz-asl/voxblox-plusplus

#### 12. Cube SLAM

+ **论文**：Yang S, Scherer S. [**Cubeslam: Monocular 3-d object slam**](https://arxiv.org/pdf/1806.00557)[J]. IEEE Transactions on Robotics, **2019**, 35(4): 925-938.
+ **代码**：https://github.com/shichaoy/cube_slam
+ 对，这就是带我入坑的一项工作，2018 年 11 月份看到这篇论文（当时是预印版）之后开始学习物体级 SLAM，个人对 Cube SLAM 的一些注释和总结：[链接](https://www.wuxiaolang.cn/slam/)。
+ 也有很多有意思的但没开源的物体级 SLAM
    + Ok K, Liu K, Frey K, et al. [**Robust Object-based SLAM for High-speed Autonomous Navigation**](http://groups.csail.mit.edu/rrg/papers/OkLiu19icra.pdf)[C]//2019 International Conference on Robotics and Automation (ICRA). IEEE, **2019**: 669-675.
    + Li J, Meger D, Dudek G. [**Semantic Mapping for View-Invariant Relocalization**](https://www.cim.mcgill.ca/~mrl/pubs/jimmy/li2019icra.pdf)[C]//2019 International Conference on Robotics and Automation (ICRA). IEEE, **2019**: 7108-7115.
    + Nicholson L, Milford M, Sünderhauf N. [**Quadricslam: Dual quadrics from object detections as landmarks in object-oriented slam**](https://arxiv.org/pdf/1804.04011)[J]. IEEE Robotics and Automation Letters, **2018**, 4(1): 1-8.

#### 13. VPS-SLAM（平面语义 SLAM）
+ **论文**：Bavle H, De La Puente P, How J, et al. [**VPS-SLAM: Visual Planar Semantic SLAM for Aerial Robotic Systems**](https://ieeexplore.ieee.org/iel7/6287639/8948470/09045978.pdf)[J]. IEEE Access, **2020**.
+ **代码**：https://bitbucket.org/hridaybavle/semantic_slam/src/master/

#### 14. Structure-SLAM （低纹理环境下点线 SLAM）
+ **论文**：Li Y, Brasch N, Wang Y, et al. [**Structure-SLAM: Low-Drift Monocular SLAM in Indoor Environments**](https://ieeexplore.ieee.org/abstract/document/9165014)[J]. IEEE Robotics and Automation Letters, **2020**, 5(4): 6583-6590.
+ **代码**：https://github.com/yanyan-li/Structure-SLAM-PointLine

### :smile: 1.4 Sensor Fusion

#### 1. msckf_vio

+ **论文**：Sun K, Mohta K, Pfrommer B, et al. [**Robust stereo visual inertial odometry for fast autonomous flight**](https://arxiv.org/pdf/1712.00036)[J]. IEEE Robotics and Automation Letters, **2018**, 3(2): 965-972.
+ **代码**：https://github.com/KumarRobotics/msckf_vio ；[Video](https://www.youtube.com/watch?v=jxfJFgzmNSw&t)

#### 2. rovio

+ **论文**：Bloesch M, Omari S, Hutter M, et al. [**Robust visual inertial odometry using a direct EKF-based approach**](https://www.research-collection.ethz.ch/bitstream/handle/20.500.11850/155340/1/eth-48374-01.pdf)[C]//2015 IEEE/RSJ international conference on intelligent robots and systems (IROS). IEEE, **2015**: 298-304.
+ **代码**：https://github.com/ethz-asl/rovio ；[Video](https://www.youtube.com/watch?v=ZMAISVy-6ao&feature=youtu.be)

#### 3. R-VIO

+ **论文**：Huai Z, Huang G. [**Robocentric visual-inertial odometry**](https://arxiv.org/pdf/1805.04031)[C]//2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2018**: 6319-6326.
+ **代码**：https://github.com/rpng/R-VIO ；[Video](https://www.youtube.com/watch?v=l9IC2ddBEYQ)
+ **VI_ORB_SLAM2**：https://github.com/YoujieXia/VI_ORB_SLAM2

#### 4. okvis

+ **论文**：Leutenegger S, Lynen S, Bosse M, et al. [**Keyframe-based visual–inertial odometry using nonlinear optimization**](https://spiral.imperial.ac.uk/bitstream/10044/1/23413/2/ijrr2014_revision_1.pdf)[J]. The International Journal of Robotics Research, **2015**, 34(3): 314-334.
+ **代码**：https://github.com/ethz-asl/okvis

#### 5. VIORB

+ **论文**：Mur-Artal R, Tardós J D. [Visual-inertial monocular SLAM with map reuse](https://arxiv.org/pdf/1610.05949.pdf)[J]. IEEE Robotics and Automation Letters, **2017**, 2(2): 796-803.
+ **代码**：https://github.com/jingpang/LearnVIORB （VIORB 本身是没有开源的，这是王京大佬复现的一个版本）

#### 6. VINS-mono

+ **论文**：Qin T, Li P, Shen S. [**Vins-mono: A robust and versatile monocular visual-inertial state estimator**](https://arxiv.org/pdf/1708.03852)[J]. IEEE Transactions on Robotics, **2018**, 34(4): 1004-1020.
+ **代码**：https://github.com/HKUST-Aerial-Robotics/VINS-Mono
+ 双目版 **VINS-Fusion**：https://github.com/HKUST-Aerial-Robotics/VINS-Fusion
+ 移动段 **VINS-mobile**：https://github.com/HKUST-Aerial-Robotics/VINS-Mobile

#### 7. VINS-RGBD

+ **论文**：Shan Z, Li R, Schwertfeger S. [**RGBD-Inertial Trajectory Estimation and Mapping for Ground Robots**](https://www.mdpi.com/1424-8220/19/10/2251)[J]. Sensors, **2019**, 19(10): 2251.
+ **代码**：https://github.com/STAR-Center/VINS-RGBD ；[**Video**](https://robotics.shanghaitech.edu.cn/datasets/VINS-RGBD)

#### 8. Open-VINS

+ **论文**：Geneva P, Eckenhoff K, Lee W, et al. [**Openvins: A research platform for visual-inertial estimation**](https://pdfs.semanticscholar.org/cb63/60f21255834297e32826bff6366a769b49e9.pdf)[C]//IROS 2019 Workshop on Visual-Inertial Navigation: Challenges and Applications, Macau, China. **IROS 2019**.
+ **代码**：https://github.com/rpng/open_vins

#### 9. versavis（多功能的视惯传感器系统）

+ 论文：Tschopp F, Riner M, Fehr M, et al. [**VersaVIS—An Open Versatile Multi-Camera Visual-Inertial Sensor Suite**](https://www.mdpi.com/1424-8220/20/5/1439)[J]. Sensors, **2020**, 20(5): 1439.
+ 代码：https://github.com/ethz-asl/versavis

#### 10. CPI（视惯融合的封闭式预积分）

+ **论文**：Eckenhoff K, Geneva P, Huang G. [**Closed-form preintegration methods for graph-based visual–inertial navigation**](http://sage.cnpereading.com/paragraph/article/10.1177/0278364919835021)[J]. The International Journal of Robotics Research, 2018.
+ **代码**：https://github.com/rpng/cpi ；[**Video**](https://www.youtube.com/watch?v=yIgQX2SH_pI)

#### 11. TUM Basalt

+ **论文**：Usenko V, Demmel N, Schubert D, et al. [Visual-inertial mapping with non-linear factor recovery](https://link.zhihu.com/?target=https%3A//arxiv.org/pdf/1904.06504.pdf)[J]. IEEE Robotics and Automation Letters, **2019**.
+ **代码**：[https://github.com/VladyslavUsenko/basalt-mirror](https://link.zhihu.com/?target=https%3A//github.com/VladyslavUsenko/basalt-mirror) ；[Video](https://link.zhihu.com/?target=https%3A//www.youtube.com/watch%3Fv%3Dr3CJ2JP75Tc)；[Project Page](https://link.zhihu.com/?target=https%3A//vision.in.tum.de/research/vslam/basalt)

#### 12. Limo（激光单目视觉里程计）

+ **论文**：Graeter J, Wilczynski A, Lauer M. [**Limo: Lidar-monocular visual odometry**](https://arxiv.org/pdf/1807.07524)[C]//2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2018**: 7872-7879.
+ **代码**：https://github.com/johannes-graeter/limo ； [**Video**](https://www.youtube.com/watch?v=wRemjJBjp64&feature=youtu.be)

#### 13. LARVIO（多状态约束卡尔曼滤波的单目 VIO）

+ **论文**：Qiu X, Zhang H, Fu W, et al. [Monocular Visual-Inertial Odometry with an Unbiased Linear System Model and Robust Feature Tracking Front-End](https://www.mdpi.com/1424-8220/19/8/1941)[J]. Sensors, **2019**, 19(8): 1941.
+ **代码**：https://github.com/PetWorm/LARVIO
+ 北航邱笑晨博士的一项工作

#### 14. vig-init（垂直边缘加速视惯初始化）

+ **论文**：Li J, Bao H, Zhang G. [**Rapid and Robust Monocular Visual-Inertial Initialization with Gravity Estimation via Vertical Edges**](http://www.cad.zju.edu.cn/home/gfzhang/projects/iros2019-vi-initialization.pdf)[C]//2019 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2019**: 6230-6236.
+ **代码**：https://github.com/zju3dv/vig-init
+ 浙大章国峰老师组的一项工作

#### 15. vilib（VIO 前端库）

+ **论文**：Nagy B, Foehn P, Scaramuzza D. [**Faster than FAST: GPU-Accelerated Frontend for High-Speed VIO**](https://arxiv.org/pdf/2003.13493)[J]. arXiv preprint arXiv:2003.13493, **2020**.
+ **代码**：https://github.com/uzh-rpg/vilib

#### 16. Kimera-VIO

+ **论文**：A. Rosinol, M. Abate, Y. Chang, L. Carlone, [**Kimera: an Open-Source Library for Real-Time Metric-Semantic Localization and Mapping**](https://arxiv.org/abs/1910.02490). IEEE Intl. Conf. on Robotics and Automation (ICRA), 2020.
+ **代码**：https://github.com/MIT-SPARK/Kimera-VIO

#### 17. maplab（视惯建图框架）
+ **论文**：Schneider T, Dymczyk M, Fehr M, et al. [**maplab: An open framework for research in visual-inertial mapping and localization**](https://arxiv.org/pdf/1711.10250)[J]. IEEE Robotics and Automation Letters, **2018**, 3(3): 1418-1425. 
+ **代码**：https://github.com/ethz-asl/maplab
+ 多会话建图，地图合并，视觉惯性批处理优化和闭环

### :smile: 1.5 Dynamic SLAM

#### 1. DynamicSemanticMapping（动态语义建图）

+ **论文**：Kochanov D, Ošep A, Stückler J, et al. [**Scene flow propagation for semantic mapping and object discovery in dynamic street scenes**](http://web-info8.informatik.rwth-aachen.de/media/papers/paper_compressed.pdf)[C]//Intelligent Robots and Systems (IROS), 2016 IEEE/RSJ International Conference on. IEEE, **2016**: 1785-1792.
+ **代码**：https://github.com/ganlumomo/DynamicSemanticMapping ；[wiki](https://github.com/ganlumomo/DynamicSemanticMapping/wiki)

#### 2. DS-SLAM（动态语义 SLAM）

+ **论文**：Yu C, Liu Z, Liu X J, et al. [**DS-SLAM: A semantic visual SLAM towards dynamic environments**](https://arxiv.org/pdf/1809.08379)[C]//2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2018**: 1168-1174.
+ **代码**：https://github.com/ivipsourcecode/DS-SLAM

#### 3. Co-Fusion（实时分割与跟踪多物体）

+ **论文**：Rünz M, Agapito L. [**Co-fusion: Real-time segmentation, tracking and fusion of multiple objects**](https://ieeexplore.ieee.org/abstract/document/7989518)[C]//2017 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2017: 4471-4478.
+ **代码**：https://github.com/martinruenz/co-fusion ； [Video](http://visual.cs.ucl.ac.uk/pubs/cofusion/index.html)

#### 4. DynamicFusion

+ **论文**：Newcombe R A, Fox D, Seitz S M. [**Dynamicfusion: Reconstruction and tracking of non-rigid scenes in real-time**](https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Newcombe_DynamicFusion_Reconstruction_and_2015_CVPR_paper.pdf)[C]//Proceedings of the IEEE conference on computer vision and pattern recognition. **2015**: 343-352.
+ **代码**：https://github.com/mihaibujanca/dynamicfusion

#### 5. ReFusion（动态场景利用残差三维重建）

+ **论文**：Palazzolo E, Behley J, Lottes P, et al. [**ReFusion: 3D Reconstruction in Dynamic Environments for RGB-D Cameras Exploiting Residuals**](https://arxiv.org/pdf/1905.02082.pdf)[J]. arXiv preprint arXiv:1905.02082, **2019**.
+ **代码**：https://github.com/PRBonn/refusion ；[**Video**](https://www.youtube.com/watch?v=1P9ZfIS5-p4&feature=youtu.be)

#### 6. DynSLAM（室外大规模稠密重建）

+ **论文**：Bârsan I A, Liu P, Pollefeys M, et al. [**Robust dense mapping for large-scale dynamic environments**](https://arxiv.org/pdf/1905.02781.pdf?utm_term)[C]//2018 IEEE International Conference on Robotics and Automation (ICRA). IEEE, **2018**: 7510-7517.
+ **代码**：https://github.com/AndreiBarsan/DynSLAM
+ **作者博士学位论文**：Barsan I A. [**Simultaneous localization and mapping in dynamic scenes**](https://www.research-collection.ethz.ch/bitstream/handle/20.500.11850/202829/1/Barsan_Ioan.pdf)[D]. ETH Zurich, Department of Computer Science, **2017**.

#### 7. VDO-SLAM（动态物体感知的 SLAM）

+ **论文**：Zhang J, Henein M, Mahony R, et al. [**VDO-SLAM: A Visual Dynamic Object-aware SLAM System**](https://arxiv.org/abs/2005.11052)[J]. arXiv preprint arXiv:2005.11052, **2020**.（IJRR Under Review）
  + 相关论文
    + IROS 2020 [Robust Ego and Object 6-DoF Motion Estimation and Tracking](https://arxiv.org/abs/2007.13993)
    + ICRA 2020 [Dynamic SLAM: The Need For Speed](https://arxiv.org/abs/2002.08584)
+ **代码**：https://github.com/halajun/VDO_SLAM | [video](https://drive.google.com/file/d/1PbL4KiJ3sUhxyJSQPZmRP6mgi9dIC0iu/view)

### :smile: 1.6 Mapping

#### 1. InfiniTAM（跨平台 CPU 实时重建）

+ 论文：Prisacariu V A, Kähler O, Golodetz S, et al. [**Infinitam v3: A framework for large-scale 3d reconstruction with loop closure**](https://arxiv.org/pdf/1708.00783)[J]. arXiv preprint arXiv:1708.00783, **2017**.
+ 代码：https://github.com/victorprad/InfiniTAM ；[project page](http://www.robots.ox.ac.uk/~victor/infinitam/)

#### 2. BundleFusion

+ **论文**：Dai A, Nießner M, Zollhöfer M, et al. [**Bundlefusion: Real-time globally consistent 3d reconstruction using on-the-fly surface reintegration**](https://arxiv.org/pdf/1604.01093.pdf)[J]. ACM Transactions on Graphics (TOG), **2017**, 36(4): 76a.
+ **代码**：https://github.com/niessner/BundleFusion ；[工程地址](http://graphics.stanford.edu/projects/bundlefusion/)
  
#### 3. KinectFusion

+ **论文**：Newcombe R A, Izadi S, Hilliges O, et al. [**KinectFusion: Real-time dense surface mapping and tracking**](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/kinectfusion-uist-comp.pdf)[C]//2011 10th IEEE International Symposium on Mixed and Augmented Reality. IEEE, **2011**: 127-136.
+ **代码**：https://github.com/chrdiller/KinectFusionApp

#### 4. ElasticFusion

+ **论文**：Whelan T, Salas-Moreno R F, Glocker B, et al. [**ElasticFusion: Real-time dense SLAM and light source estimation**](https://spiral.imperial.ac.uk/bitstream/10044/1/39502/4/Whelan16ijrr.pdf)[J]. The International Journal of Robotics Research, **2016**, 35(14): 1697-1716.
+ **代码**：https://github.com/mp3guy/ElasticFusion

#### 5. Kintinuous

+ ElasticFusion 同一个团队的工作，帝国理工 Stefan Leutenegger [谷歌学术](https://scholar.google.com/citations?user=SmGQ48gAAAAJ&hl=zh-CN&oi=sra)
+ **论文**：Whelan T, Kaess M, Johannsson H, et al. [**Real-time large-scale dense RGB-D SLAM with volumetric fusion**](https://dspace.mit.edu/bitstream/handle/1721.1/97583/Leonard_Real-time.pdf%3Bjsessionid%3D8C351776D7D5E5C614AF641625837212?sequence%3D1)[J]. The International Journal of Robotics Research, **2015**, 34(4-5): 598-626.
+ **代码**：https://github.com/mp3guy/Kintinuous

#### 6. ElasticReconstruction

+ **论文**：Choi S, Zhou Q Y, Koltun V. [**Robust reconstruction of indoor scenes**](https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Choi_Robust_Reconstruction_of_2015_CVPR_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. **2015**: 5556-5565.
+ **代码**：https://github.com/qianyizh/ElasticReconstruction ；[作者主页](http://qianyi.info/publication.html)

#### 7. FlashFusion

+ **论文**：Han L, Fang L. [**FlashFusion: Real-time Globally Consistent Dense 3D Reconstruction using CPU Computing**](http://www.roboticsproceedings.org/rss14/p06.pdf)[C]. RSS, 2018.
+ **代码**（一直没放出来）：https://github.com/lhanaf/FlashFusion ； [Project Page](http://www.luvision.net/FlashFusion/?tdsourcetag=s_pctim_aiomsg)

#### 8. RTAB-Map（激光视觉稠密重建）

+ **论文**：Labbé M, Michaud F. [**RTAB‐Map as an open‐source lidar and visual simultaneous localization and mapping library for large‐scale and long‐term online operation**](https://pdfs.semanticscholar.org/3957/7f85f3b1a16f496a2160d1a71894d12c1acc.pdf)[J]. Journal of Field Robotics, **2019**, 36(2): 416-446.
+ **代码**：https://github.com/introlab/rtabmap ；[Video](https://www.youtube.com/user/matlabbe) ；[project page](http://introlab.github.io/rtabmap/)

#### 9. RobustPCLReconstruction（户外稠密重建）

+ **论文**：Lan Z, Yew Z J, Lee G H. [**Robust Point Cloud Based Reconstruction of Large-Scale Outdoor Scenes**](http://openaccess.thecvf.com/content_CVPR_2019/papers/Lan_Robust_Point_Cloud_Based_Reconstruction_of_Large-Scale_Outdoor_Scenes_CVPR_2019_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. **2019**: 9690-9698.
+ **代码**：https://github.com/ziquan111/RobustPCLReconstruction ；[Video](https://www.youtube.com/watch?v=ZZQT_REkItU)

#### 10. plane-opt-rgbd（室内平面重建）

+ **论文**：Wang C, Guo X. [**Efficient Plane-Based Optimization of Geometry and Texture for Indoor RGB-D Reconstruction**](http://openaccess.thecvf.com/content_CVPRW_2019/papers/SUMO/Wang_Efficient_Plane-Based_Optimization_of_Geometry_and_Texture_for_Indoor_RGB-D_CVPRW_2019_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition Workshops. **2019**: 49-53.
+ **代码**：https://github.com/chaowang15/plane-opt-rgbd

#### 11. DenseSurfelMapping（稠密表面重建）

+ **论文**：Wang K, Gao F, Shen S. [**Real-time scalable dense surfel mapping**](https://arxiv.org/pdf/1909.04250.pdf)[C]//2019 International Conference on Robotics and Automation (ICRA). IEEE, **2019**: 6919-6925.
+ **代码**：https://github.com/HKUST-Aerial-Robotics/DenseSurfelMapping

#### 12. surfelmeshing（网格重建）

+ **论文**：Schöps T, Sattler T, Pollefeys M. [**Surfelmeshing: Online surfel-based mesh reconstruction**](https://arxiv.org/pdf/1810.00729.pdf)[J]. IEEE Transactions on Pattern Analysis and Machine Intelligence, **2019**.
+ **代码**：https://github.com/puzzlepaint/surfelmeshing

#### 13. DPPTAM（单目稠密重建）

+ **论文**：Concha Belenguer A, Civera Sancho J. [**DPPTAM: Dense piecewise planar tracking and mapping from a monocular sequence**](https://zaguan.unizar.es/record/36752/files/texto_completo.pdf)[C]//Proc. IEEE/RSJ Int. Conf. Intell. Rob. Syst. **2015** (ART-2015-92153).
+ **代码**：https://github.com/alejocb/dpptam
+ **相关研究**：基于超像素的单目 SLAM：[**Using Superpixels in Monocular SLAM**](http://webdiis.unizar.es/~jcivera/papers/concha_civera_icra14.pdf) ICRA 2014 ；[谷歌学术](https://scholar.google.com/citations?user=GIaG3CsAAAAJ&hl=zh-CN&oi=sra)

#### 14. VI-MEAN（单目视惯稠密重建）

+ **论文**：Yang Z, Gao F, Shen S. [**Real-time monocular dense mapping on aerial robots using visual-inertial fusion**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7989529)[C]//2017 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2017: 4552-4559.
+ **代码**：https://github.com/dvorak0/VI-MEAN ；[Video](https://www.youtube.com/watch?v=M4BMks6bQbc)

#### 15. REMODE（单目概率稠密重建）

+ **论文**：Pizzoli M, Forster C, Scaramuzza D. [**REMODE: Probabilistic, monocular dense reconstruction in real time**](https://files.ifi.uzh.ch/rpg/website/rpg.ifi.uzh.ch/html/docs/ICRA14_Pizzoli.pdf)[C]//2014 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2014: 2609-2616.
+ **原始开源代码**：https://github.com/uzh-rpg/rpg_open_remode
+ **与 ORB-SLAM2 结合版本**：https://github.com/ayushgaud/ORB_SLAM2  https://github.com/ayushgaud/ORB_SLAM2

#### 16. DeepFactors（实时的概率单目稠密 SLAM）

+ 帝国理工学院戴森机器人实验室
+ **论文**：Czarnowski J, Laidlow T, Clark R, et al. [**DeepFactors: Real-Time Probabilistic Dense Monocular SLAM**](https://arxiv.org/pdf/2001.05049.pdf)[J]. arXiv preprint arXiv:2001.05049, **2020**.
+ **代码**：https://github.com/jczarnowski/DeepFactors （还未放出）
+ 其他论文：Bloesch M, Czarnowski J, Clark R, et al. [**CodeSLAM—learning a compact, optimisable representation for dense visual SLAM**](http://openaccess.thecvf.com/content_cvpr_2018/papers/Bloesch_CodeSLAM_--_Learning_CVPR_2018_paper.pdf)[C]//Proceedings of the IEEE conference on computer vision and pattern recognition. **2018**: 2560-2568.

#### 17. probabilistic_mapping（单目概率稠密重建）

+ 港科沈邵劼老师团队
+ **论文**：Ling Y, Wang K, Shen S. [**Probabilistic dense reconstruction from a moving camera**](https://arxiv.org/pdf/1903.10673.pdf)[C]//2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2018**: 6364-6371.
+ **代码**：https://github.com/ygling2008/probabilistic_mapping
+ 另外一篇稠密重建文章的代码一直没放出来 [Github](https://github.com/ygling2008/dense_mapping) ：Ling Y, Shen S. [**Real‐time dense mapping for online processing and navigation**](https://onlinelibrary.wiley.com/doi/abs/10.1002/rob.21868)[J]. Journal of Field Robotics, **2019**, 36(5): 1004-1036.

#### 18. ORB-SLAM2 单目半稠密建图

+ **论文**：Mur-Artal R, Tardós J D. [Probabilistic Semi-Dense Mapping from Highly Accurate Feature-Based Monocular SLAM](https://www.researchgate.net/profile/Raul_Mur-Artal/publication/282807894_Probabilistic_Semi-Dense_Mapping_from_Highly_Accurate_Feature-Based_Monocular_SLAM/links/561cd04308ae6d17308ce267.pdf)[C]//Robotics: Science and Systems. **2015**, 2015.
+ **代码**（本身没有开源，贺博复现的一个版本）：https://github.com/HeYijia/ORB_SLAM2
+ 加上线段之后的半稠密建图
    + **论文**：He S, Qin X, Zhang Z, et al. [**Incremental 3d line segment extraction from semi-dense slam**](https://arxiv.org/pdf/1708.03275)[C]//2018 24th International Conference on Pattern Recognition (ICPR). IEEE, **2018**: 1658-1663.
    + **代码**：https://github.com/shidahe/semidense-lines
    + 作者在此基础上用于指导远程抓取操作的一项工作：https://github.com/atlas-jj/ORB-SLAM-free-space-carving

#### 19. Voxgraph（SDF 体素建图）

+ **论文**：Reijgwart V, Millane A, Oleynikova H, et al. [**Voxgraph: Globally Consistent, Volumetric Mapping Using Signed Distance Function Submaps**](https://www.research-collection.ethz.ch/bitstream/handle/20.500.11850/385682/1/Voxgraph-ETHpreprintversion.pdf)[J]. IEEE Robotics and Automation Letters, **2019**, 5(1): 227-234.
+ **代码**：https://github.com/ethz-asl/voxgraph

#### 20. SegMap（三维分割建图）
+ **论文**：Dubé R, Cramariuc A, Dugas D, et al. [**SegMap: 3d segment mapping using data-driven descriptors**](https://arxiv.org/pdf/1804.09557)[J]. arXiv preprint arXiv:1804.09557, **2018**.
+ **代码**：https://github.com/ethz-asl/segmap

### :smile: 1.7 Optimization

#### 1. 后端优化库

+ **GTSAM**：https://github.com/borglab/gtsam ；[官网](https://gtsam.org/)
+ **g2o**：https://github.com/RainerKuemmerle/g2o
+ **ceres**：http://ceres-solver.org/

#### 2. ICE-BA

+ **论文**：Liu H, Chen M, Zhang G, et al. [**Ice-ba: Incremental, consistent and efficient bundle adjustment for visual-inertial slam**](http://openaccess.thecvf.com/content_cvpr_2018/papers/Liu_ICE-BA_Incremental_Consistent_CVPR_2018_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. **2018**: 1974-1982.
+ **代码**：https://github.com/baidu/ICE-BA

#### 3. minisam（因子图最小二乘优化框架）

+ **论文**：Dong J, Lv Z. [**miniSAM: A Flexible Factor Graph Non-linear Least Squares Optimization Framework**](https://arxiv.org/pdf/1909.00903.pdf)[J]. arXiv preprint arXiv:1909.00903, **2019**.
+ **代码**：https://github.com/dongjing3309/minisam ； [文档](https://minisam.readthedocs.io/)

#### 4. SA-SHAGO（几何基元图优化）

+ **论文**：Aloise I, Della Corte B, Nardi F, et al. [**Systematic Handling of Heterogeneous Geometric Primitives in Graph-SLAM Optimization**](http://rss2019.informatik.uni-freiburg.de/papers/0285_FI.pdf)[J]. IEEE Robotics and Automation Letters, **2019**, 4(3): 2738-2745.
+ **代码**：https://srrg.gitlab.io/sashago-website/index.html#

#### 5. MH-iSAM2（SLAM 优化器）

+ **论文**：Hsiao M, Kaess M. [**MH-iSAM2: Multi-hypothesis iSAM using Bayes Tree and Hypo-tree**](http://www.cs.cmu.edu/~kaess/pub/Hsiao19icra.pdf)[C]//2019 International Conference on Robotics and Automation (ICRA). IEEE, **2019**: 1274-1280.
+ **代码**：https://bitbucket.org/rpl_cmu/mh-isam2_lib/src/master/

#### 6. MOLA（用于定位和建图的模块化优化框架）

+ **论文**：Blanco-Claraco J L. [**A Modular Optimization Framework for Localization and Mapping**](http://roboticsproceedings.org/rss15/p43.pdf)[J]. Proc. of Robotics: Science and Systems (RSS), FreiburgimBreisgau, Germany, **2019**, 2.
+ **代码**：https://github.com/MOLAorg/mola ；[**Video**](https://www.youtube.com/watch?v=Bb92aMBJR44) ；[使用文档](https://docs.mola-slam.org/latest/)

---
## 2. 优秀作者与实验室
> 这一部分整理之后发布在知乎（2020 年 4 月 19 日）：https://zhuanlan.zhihu.com/p/130530891

#### 1. 美国卡耐基梅陇大学机器人研究所

+ **研究方向**：机器人感知、结构，服务型、运输、制造业、现场机器
+ **研究所主页**：https://www.ri.cmu.edu/
+ 下属 **Field Robotic Center** 主页：https://frc.ri.cmu.edu/
+ **发表论文**：https://www.ri.cmu.edu/pubs/
+ 👦 **Michael Kaess**：[个人主页](https://www.ri.cmu.edu/ri-faculty/michael-kaess/) ，[谷歌学术](https://scholar.google.com/citations?user=27eupmsAAAAJ&hl=zh-CN&oi=ao)
+ 👦 **Sebastian Scherer**：[个人主页](https://www.ri.cmu.edu/ri-faculty/sebastian-scherer/) ，[谷歌学术](https://scholar.google.com/citations?hl=zh-CN&user=gxoPfIYAAAAJ)
+ 📜 Kaess M, Ranganathan A, Dellaert F. [**iSAM: Incremental smoothing and mapping**](https://smartech.gatech.edu/bitstream/handle/1853/26572/kaess_michael_200812_phd.pdf?sequence=1&isAllowed=y)[J]. IEEE Transactions on Robotics, **2008**, 24(6): 1365-1378.
+ 📜 Hsiao M, Westman E, Zhang G, et al. [**Keyframe-based dense planar SLAM**](http://www.cs.cmu.edu/~kaess/pub/Hsiao17icra.pdf)[C]//2017 IEEE International Conference on Robotics and Automation (ICRA). IEEE, **2017**: 5110-5117.
+ 📜 Kaess M. [**Simultaneous localization and mapping with infinite planes**](https://www.cs.cmu.edu/~kaess/pub/Kaess15icra.pdf)[C]//2015 IEEE International Conference on Robotics and Automation (ICRA). IEEE, **2015**: 4605-4611.

#### 2. 美国加州大学圣地亚哥分校语境机器人研究所

+ **研究方向**：多模态环境理解，语义导航，自主信息获取
+ **实验室主页**：https://existentialrobotics.org/index.html
+ **发表论文汇总**：https://existentialrobotics.org/pages/publications.html
+ 👦 **Nikolay Atanasov**：[个人主页](https://natanaso.github.io/)&emsp;[谷歌学术](https://scholar.google.com/citations?user=RTkSatQAAAAJ&hl=zh-CN&oi=sra)
    + 机器人状态估计与感知课程 ppt：https://natanaso.github.io/ece276a2019/schedule.html
+ 📜 **语义 SLAM 经典论文**：Bowman S L, Atanasov N, Daniilidis K, et al. [**Probabilistic data association for semantic slam**](http://erl.ucsd.edu/ref/Bowman_SemanticSLAM_ICRA17.pdf)[C]//2017 IEEE international conference on robotics and automation (ICRA). IEEE, **2017**: 1722-1729.
+ 📜 **实例网格模型定位与建图**：Feng Q, Meng Y, Shan M, et al. [**Localization and Mapping using Instance-specific Mesh Models**](http://erl.ucsd.edu/ref/Feng_DeformableMeshModel_IROS19.pdf)[C]//2019 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2019**: 4985-4991.
+ 📜 **基于事件相机的 VIO**：Zihao Zhu A, Atanasov N, Daniilidis K. [**Event-based visual inertial odometry**](http://openaccess.thecvf.com/content_cvpr_2017/papers/Zhu_Event-Based_Visual_Inertial_CVPR_2017_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. **2017**: 5391-5399.

#### 3. 美国特拉华大学机器人感知与导航组

+ **研究方向**：SLAM、VINS、语义定位与建图等
+ **实验室主页**：https://sites.udel.edu/robot/
+ **发表论文汇总**：https://sites.udel.edu/robot/publications/
+ **Github 地址**：https://github.com/rpng?page=2
+ 📜 Geneva P, Eckenhoff K, Lee W, et al. [**Openvins: A research platform for visual-inertial estimation**](https://pdfs.semanticscholar.org/cb63/60f21255834297e32826bff6366a769b49e9.pdf)[C]//IROS 2019 Workshop on Visual-Inertial Navigation: Challenges and Applications, Macau, China. **IROS 2019**.（**代码**：https://github.com/rpng/open_vins ）
+ 📜 Huai Z, Huang G. [**Robocentric visual-inertial odometry**](https://arxiv.org/pdf/1805.04031)[C]//2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2018**: 6319-6326.（**代码**：https://github.com/rpng/R-VIO ）
+ 📜 Zuo X, Geneva P, Yang Y, et al. [**Visual-Inertial Localization With Prior LiDAR Map Constraints**](https://link.zhihu.com/?target=https%3A//arxiv.org/pdf/1911.05787)[J]. IEEE Robotics and Automation Letters, **2019**, 4(4): 3394-3401.
+ 📜 Zuo X, Ye W, Yang Y, et al. [**Multimodal localization: Stereo over LiDAR map**](https://link.zhihu.com/?target=https%3A//onlinelibrary.wiley.com/doi/abs/10.1002/rob.21936)[J]. Journal of Field Robotics, **2020** （ 左星星博士[谷歌学术](https://link.zhihu.com/?target=https%3A//scholar.google.com/citations%3Fuser%3DCePv8agAAAAJ%26hl%3Dzh-CN%26oi%3Dao)）
+ 👦 [黄国权教授主页](http://udel.edu/~ghuang/index.html)

#### 4. 美国麻省理工学院航空航天实验室

+ **研究方向**：位姿估计与导航，路径规划，控制与决策，机器学习与强化学习
+ **实验室主页**：http://acl.mit.edu/
+ **发表论文**：http://acl.mit.edu/publications （实验室的**学位论文**也可以在这里找到）
+ 👦 **Jonathan P. How** 教授：[个人主页](http://www.mit.edu/people/jhow/) &emsp;[谷歌学术](https://scholar.google.com/citations?user=gX7rSCcAAAAJ&hl=en)
+ 👦 **Kasra Khosoussi**（SLAM 图优化）：[谷歌学术](https://scholar.google.com/citations?user=SRCCuo0AAAAJ&hl=zh-CN&oi=sra)
+ 📜 **物体级 SLAM**：Mu B, Liu S Y, Paull L, et al. [**Slam with objects using a nonparametric pose graph**](https://arxiv.org/pdf/1704.05959.pdf?source=post_page---------------------------)[C]//2016 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2016**: 4602-4609.（**代码**：https://github.com/BeipengMu/objectSLAM）
+ 📜 **物体级 SLAM 导航**：Ok K, Liu K, Frey K, et al. [**Robust Object-based SLAM for High-speed Autonomous Navigation**](http://groups.csail.mit.edu/rrg/papers/OkLiu19icra.pdf)[C]//2019 International Conference on Robotics and Automation (ICRA). IEEE, **2019**: 669-675.
+ 📜 **SLAM 的图优化**：Khosoussi, K., Giamou, M., Sukhatme, G., Huang, S., Dissanayake, G., and How, J. P., [**Reliable Graphs for SLAM**](https://journals.sagepub.com/doi/full/10.1177/0278364918823086) [C]//International Journal of Robotics Research (IJRR), 2019.

#### 5. 美国麻省理工学院 SPARK 实验室

+ **研究方向**：移动机器人环境感知
+ **实验室主页**：http://web.mit.edu/sparklab/
+ 👦 **Luca Carlone** 教授：[个人主页](https://lucacarlone.mit.edu/) &emsp;[谷歌学术](https://scholar.google.com/citations?user=U4kKRdMAAAAJ&hl=zh-CN&oi=sra)
+ 📜 **SLAM 经典综述**：Cadena C, Carlone L, Carrillo H, et al. [**Past, present, and future of simultaneous localization and mapping: Toward the robust-perception age**](https://arxiv.org/pdf/1606.05830)[J]. IEEE Transactions on robotics, **2016**, 32(6): 1309-1332.
+ 📜 **VIO 流形预积分**：Forster C, Carlone L, Dellaert F, et al. [**On-Manifold Preintegration for Real-Time Visual--Inertial Odometry**](https://arxiv.org/pdf/1512.02363)[J]. IEEE Transactions on Robotics, **2016**, 33(1): 1-21.
+ 📜 **开源语义 SLAM**：Rosinol A, Abate M, Chang Y, et al. [**Kimera: an Open-Source Library for Real-Time Metric-Semantic Localization and Mapping**](https://arxiv.org/pdf/1910.02490)[J]. arXiv preprint arXiv:1910.02490, **2019**.（代码：https://github.com/MIT-SPARK/Kimera ）

#### 6. 美国麻省理工学院海洋机器人组

+ **研究方向**：水下或陆地移动机器人导航与建图
+ **实验室主页**：https://marinerobotics.mit.edu/ （隶属于 MIT [计算机科学与人工智能实验室](https://www.csail.mit.edu/)）
+ 👦 **John Leonard 教授**：[谷歌学术](https://scholar.google.com/citations?user=WPe7vWwAAAAJ&hl=zh-CN&authuser=1&oi=ao)
+ **发表论文汇总**：https://marinerobotics.mit.edu/biblio
+ 📜 **面向物体的 SLAM**：Finman R, Paull L, Leonard J J. [**Toward object-based place recognition in dense rgb-d maps**](http://marinerobotics.mit.edu/sites/default/files/icra2015.pdf)[C]//ICRA Workshop Visual Place Recognition in Changing Environments, Seattle, WA. **2015**.
+ 📜 **拓展 KinectFusion**：Whelan T, Kaess M, Fallon M, et al. [**Kintinuous: Spatially extended kinectfusion**]()[J]. **2012**.
+ 📜 **语义 SLAM 概率数据关联**：Doherty K, Fourie D, Leonard J. [**Multimodal semantic slam with probabilistic data association**](https://marinerobotics.mit.edu/sites/default/files/doherty_icra2019_revised.pdf)[C]//2019 international conference on robotics and automation (ICRA). IEEE, **2019**: 2419-2425.

#### 7. 美国明尼苏达大学多元自主机器人系统实验室

+ **研究方向**：视觉、激光、惯性导航系统，移动设备大规模三维建模与定位
+ **实验室主页**：http://mars.cs.umn.edu/index.php
+ **发表论文汇总**：http://mars.cs.umn.edu/publications.php
+ 👦 **Stergios I. Roumeliotis**：[个人主页](https://www-users.cs.umn.edu/~stergios/) ，[谷歌学术](https://scholar.google.com/citations?user=c5HeXxsAAAAJ&hl=zh-CN&oi=ao)
+ 📜 **移动设备 VIO**：Wu K, Ahmed A, Georgiou G A, et al. [**A Square Root Inverse Filter for Efficient Vision-aided Inertial Navigation on Mobile Devices**](http://roboticsproceedings.org/rss11/p08.pdf)[C]//Robotics: Science and Systems. **2015**, 2.（**项目主页**：http://mars.cs.umn.edu/research/sriswf.php ）
+ 📜 **移动设备大规模三维半稠密建图**：Guo C X, Sartipi K, DuToit R C, et al. [**Resource-aware large-scale cooperative three-dimensional mapping using multiple mobile devices**](https://pdfs.semanticscholar.org/e0fd/6d963307a0d5d6dfb6f05ad21845dd4f40c8.pdf)[J]. IEEE Transactions on Robotics, **2018**, 34(5): 1349-1369. （**项目主页**：http://mars.cs.umn.edu/research/semi_dense_mapping.php ）
+ 📜 **VIO 相关研究**：http://mars.cs.umn.edu/research/vins_overview.php

#### 8. 美国宾夕法尼亚大学 Vijay Kumar 实验室

+ **研究方向**：自主微型无人机
+ **实验室主页**：https://www.kumarrobotics.org/
+ **发表论文**：https://www.kumarrobotics.org/publications/
+ **研究成果视频**：https://www.youtube.com/user/KumarLabPenn/videos
+ 📜 **无人机半稠密 VIO**：Liu W, Loianno G, Mohta K, et al. [**Semi-Dense Visual-Inertial Odometry and Mapping for Quadrotors with SWAP Constraints**](https://www.cis.upenn.edu/~kostas/mypub.dir/wenxin18icra.pdf)[C]//2018 IEEE International Conference on Robotics and Automation (ICRA). IEEE, **2018**: 1-6.
+ 📜 **语义数据关联**：Liu X, Chen S W, Liu C, et al. [**Monocular Camera Based Fruit Counting and Mapping with Semantic Data Association**](https://arxiv.org/pdf/1811.01417)[J]. IEEE Robotics and Automation Letters, **2019**, 4(3): 2296-2303.

#### 9. Srikumar Ramalingam（美国犹他大学计算机学院）

+ **研究方向**：三维重构、语义分割、视觉 SLAM、图像定位、深度神经网络
+ 👦 **Srikumar Ramalingam**：[个人主页](https://www.cs.utah.edu/~srikumar/) &emsp; [谷歌学术](https://scholar.google.com/citations?user=6m1ptOgAAAAJ&hl=en/)
+ 📜 **点面 SLAM**：Taguchi Y, Jian Y D, Ramalingam S, et al. [**Point-plane SLAM for hand-held 3D sensors**](https://merl.com/publications/docs/TR2013-031.pdf)[C]//2013 IEEE international conference on robotics and automation. IEEE, **2013**: 5182-5189.
+ 📜 **点线定位**：Ramalingam S, Bouaziz S, Sturm P. [**Pose estimation using both points and lines for geo-localization**](https://hal.inria.fr/inria-00590279/document)[C]//2011 IEEE International Conference on Robotics and Automation. IEEE, **2011**: 4716-4723.（[视频](https://www.youtube.com/watch?v=wc7hK0zEkCw&feature=emb_logo)）
+ 📜 **2D 3D 定位**：Ataer-Cansizoglu E, Taguchi Y, Ramalingam S. [**Pinpoint SLAM: A hybrid of 2D and 3D simultaneous localization and mapping for RGB-D sensors**](http://yuichitaguchi.com/pub/16ICRA_PinpointSLAM.pdf)[C]//2016 IEEE international conference on robotics and automation (ICRA). IEEE, **2016**: 1300-1307.（[视频](https://www.youtube.com/watch?v=iZ1psxcMvrQ&feature=emb_logo)）

#### 10. Frank Dellaert（美国佐治亚理工学院机器人与智能机器研究中心）

+ **研究方向**：SLAM，图像时空重构
+ 👦 [个人主页](https://www.cc.gatech.edu/~dellaert/FrankDellaert/Frank_Dellaert/Frank_Dellaert.html)，[谷歌学术](https://scholar.google.com/citations?user=ZxXBaswAAAAJ&hl=en)
+ 📜 **因子图**：Dellaert F. [**Factor graphs and GTSAM: A hands-on introduction**](https://smartech.gatech.edu/handle/1853/45226)[R]. Georgia Institute of Technology, **2012**. （GTSAM 代码：http://borg.cc.gatech.edu/ ）
+ 📜 **多机器人分布式 SLAM**：Cunningham A, Wurm K M, Burgard W, et al. [**Fully distributed scalable smoothing and mapping with robust multi-robot data association**](https://smartech.gatech.edu/bitstream/handle/1853/44686/Cunningham12icra.pdf?sequence=1&isAllowed=y)[C]//2012 IEEE International Conference on Robotics and Automation. IEEE, **2012**: 1093-1100.
+ 📜 Choudhary S, Trevor A J B, Christensen H I, et al. [**SLAM with object discovery, modeling and mapping**](https://smartech.gatech.edu/bitstream/handle/1853/53723/Choudhary14iros.pdf)[C]//2014 IEEE/RSJ International Conference on Intelligent Robots and Systems. IEEE, **2014**: 1018-1025.

#### 11. 赵轶璞（美国佐治亚理工学院智能视觉与自动化实验室）

+ **研究方向**：视觉 SLAM、三维重建、多目标跟踪
+ 👦 [个人主页](https://sites.google.com/site/zhaoyipu/home?authuser=0) &emsp; [谷歌学术](https://scholar.google.com/citations?user=HiM_WcYAAAAJ&hl=zh-CN&authuser=1&oi=ao)
+ 📜 Zhao Y, Smith J S, Karumanchi S H, et al. [**Closed-Loop Benchmarking of Stereo Visual-Inertial SLAM Systems: Understanding the Impact of Drift and Latency on Tracking Accuracy**](https://arxiv.org/pdf/2003.01317)[J]. arXiv preprint arXiv:2003.01317, **2020**.
+ 📜 Zhao Y, Vela P A. [**Good feature selection for least squares pose optimization in VO/VSLAM**](https://arxiv.org/pdf/1905.07807)[C]//2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2018**: 1183-1189.（**代码**：https://github.com/ivalab/FullResults_GoodFeature ）
+ 📜 Zhao Y, Vela P A. [**Good line cutting: Towards accurate pose tracking of line-assisted VO/VSLAM**](http://openaccess.thecvf.com/content_ECCV_2018/papers/Yipu_Zhao_Good_Line_Cutting_ECCV_2018_paper.pdf)[C]//Proceedings of the European Conference on Computer Vision (ECCV). **2018**: 516-531. （**代码**：https://github.com/ivalab/GF_PL_SLAM ）

#### 12. 加拿大蒙特利尔大学 机器人与嵌入式 AI 实验室

+ **研究方向**：SLAM，不确定性建模
+ **实验室主页**：http://montrealrobotics.ca/
+ 👦 **Liam Paull** 教授：[个人主页](https://liampaull.ca/index.html)&emsp;[谷歌学术](https://scholar.google.com/citations?user=H9xADK0AAAAJ&hl=zh-CN&oi=ao)
+ 📜 Mu B, Liu S Y, Paull L, et al. [**Slam with objects using a nonparametric pose graph**](https://arxiv.org/pdf/1704.05959.pdf?source=post_page---------------------------)[C]//2016 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2016**: 4602-4609.（**代码**：https://github.com/BeipengMu/objectSLAM）
+ 📜 Murthy Jatavallabhula K, Iyer G, Paull L. [**gradSLAM: Dense SLAM meets Automatic Differentiation**](http://adsabs.harvard.edu/abs/2019arXiv191010672M)[J]. arXiv preprint arXiv:1910.10672, **2019**.（**代码**：https://github.com/montrealrobotics/gradSLAM ）

#### 13. 加拿大舍布鲁克大学智能、交互、综合、跨学科机器人实验室

+ **研究方向**：移动机器人软硬件设计
+ **实验室主页**：https://introlab.3it.usherbrooke.ca/
+ 📜 **激光视觉稠密重建**：Labbé M, Michaud F. [**RTAB‐Map as an open‐source lidar and visual simultaneous localization and mapping library for large‐scale and long‐term online operation**](https://pdfs.semanticscholar.org/3957/7f85f3b1a16f496a2160d1a71894d12c1acc.pdf)[J]. Journal of Field Robotics, **2019**, 36(2): 416-446.
    + 代码：https://github.com/introlab/rtabmap
    + 项目主页：http://introlab.github.io/rtabmap/
    
#### 14. 瑞士苏黎世大学机器人与感知课题组

+ **研究方向**：移动机器人、无人机环境感知与导航，**VISLAM**，**事件相机**
+ **实验室主页**：http://rpg.ifi.uzh.ch/index.html
+ **发表论文汇总**：http://rpg.ifi.uzh.ch/publications.html
+ **Github 代码公开地址**：https://github.com/uzh-rpg
+ 📜 Forster C, Pizzoli M, Scaramuzza D. [**SVO: Fast semi-direct monocular visual odometry**](https://www.zora.uzh.ch/id/eprint/125453/1/ICRA14_Forster.pdf)[C]//2014 IEEE international conference on robotics and automation (ICRA). IEEE, **2014**: 15-22.
+ 📜 VO/VIO 轨迹评估工具 **rpg_trajectory_evaluation**：https://github.com/uzh-rpg/rpg_trajectory_evaluation
+ 📜 事件相机项目主页：http://rpg.ifi.uzh.ch/research_dvs.html
+ 👦 **人物**：[Davide Scaramuzza](http://rpg.ifi.uzh.ch/people_scaramuzza.html) &emsp;[张子潮](https://www.ifi.uzh.ch/en/rpg/people/zichao.html)

#### 15. 瑞士苏黎世联邦理工计算机视觉与几何实验室

+ **研究方向**：定位、三维重建、语义分割、机器人视觉
+ **实验室主页**：http://www.cvg.ethz.ch/index.php
+ **发表论文**：http://www.cvg.ethz.ch/publications/
+ 📜 **视觉语义里程计**：Lianos K N, Schonberger J L, Pollefeys M, et al. [**Vso: Visual semantic odometry**](http://openaccess.thecvf.com/content_ECCV_2018/papers/Konstantinos-Nektarios_Lianos_VSO_Visual_Semantic_ECCV_2018_paper.pdf)[C]//Proceedings of the European conference on computer vision (ECCV). **2018**: 234-250.
+ 📜 **视觉语义定位**：CVPR 2018 [**Semantic visual localization**](http://openaccess.thecvf.com/content_cvpr_2018/papers/Schonberger_Semantic_Visual_Localization_CVPR_2018_paper.pdf)
    + **作者博士学位论文**：2018 [**Robust Methods for Accurate and Efficient 3D Modeling from Unstructured Imagery**](https://www.research-collection.ethz.ch/handle/20.500.11850/295763)
+ 📜 **大规模户外建图**：Bârsan I A, Liu P, Pollefeys M, et al. [**Robust dense mapping for large-scale dynamic environments**](https://arxiv.org/pdf/1905.02781.pdf?utm_term)[C]//2018 IEEE International Conference on Robotics and Automation (ICRA). IEEE, **2018**: 7510-7517.
    + **代码**：https://github.com/AndreiBarsan/DynSLAM 
    + **作者博士学位论文**：Barsan I A. [**Simultaneous localization and mapping in dynamic scenes**](https://www.research-collection.ethz.ch/bitstream/handle/20.500.11850/202829/1/Barsan_Ioan.pdf)[D]. ETH Zurich, Department of Computer Science, **2017**.
+ 👦 **Marc Pollefeys**：[个人主页](http://people.inf.ethz.ch/pomarc/index.html)，[谷歌学术](https://scholar.google.com/citations?user=YYH0BjEAAAAJ&hl=zh-CN&oi=ao)
+ 👦 **Johannes L. Schönberger**：[个人主页](https://demuc.de/)，[谷歌学术](https://scholar.google.com/citations?user=MlcMCd0AAAAJ)

#### 16. 英国帝国理工学院戴森机器人实验室

+ **研究方向**：机器人视觉场景与物体理解、机器人操纵
+ **实验室主页**：https://www.imperial.ac.uk/dyson-robotics-lab/
+ **发表论文**：https://www.imperial.ac.uk/dyson-robotics-lab/publications/
+ **代表性工作**：**MonoSLAM、CodeSLAM、ElasticFusion、KinectFusion**
    + 📜 **ElasticFusion**：Whelan T, Leutenegger S, Salas-Moreno R, et al. [**ElasticFusion: Dense SLAM without a pose graph**](https://spiral.imperial.ac.uk/bitstream/10044/1/23438/2/whelan2015rss.pdf)[C]. Robotics: Science and Systems, **2015**.（**代码**：https://github.com/mp3guy/ElasticFusion ）
    + 📜 **Semanticfusion**：McCormac J, Handa A, Davison A, et al. [**Semanticfusion: Dense 3d semantic mapping with convolutional neural networks**](https://arxiv.org/pdf/1609.05130)[C]//2017 IEEE International Conference on Robotics and automation (ICRA). IEEE, **2017**: 4628-4635.（**代码**：https://github.com/seaun163/semanticfusion ）
    + 📜 **Code-SLAM**：Bloesch M, Czarnowski J, Clark R, et al. [**CodeSLAM—learning a compact, optimisable representation for dense visual SLAM**](http://openaccess.thecvf.com/content_cvpr_2018/papers/Bloesch_CodeSLAM_--_Learning_CVPR_2018_paper.pdf)[C]//Proceedings of the IEEE conference on computer vision and pattern recognition. **2018**: 2560-2568.
+ 👦 **Andrew Davison**：[谷歌学术](https://scholar.google.com/citations?user=A0ae1agAAAAJ&hl=zh-CN&oi=ao)

#### 17. 英国牛津大学信息工程学

+ **研究方向**：SLAM、目标跟踪、运动结构、场景增强、移动机器人运动规划、导航与建图等等等
+ **实验室主页**：http://www.robots.ox.ac.uk/
    + 主动视觉实验室：http://www.robots.ox.ac.uk/ActiveVision/
    + 牛津机器人学院：https://ori.ox.ac.uk/
+ **发表论文汇总**：
    + 主动视觉实验室：http://www.robots.ox.ac.uk/ActiveVision/Publications/index.html
    + 机器人学院：https://ori.ox.ac.uk/publications/papers/
+ **代表性工作**：
    + 📜 Klein G, Murray D. [**PTAM: Parallel tracking and mapping for small AR workspaces**](https://dl.acm.org/ft_gateway.cfm?id=1514363&type=pdf)[C]//2007 6th IEEE and ACM international symposium on mixed and augmented reality. IEEE, **2007**: 225-234.
    + 📜 RobotCar 数据集：https://robotcar-dataset.robots.ox.ac.uk/
+ 👦 **人物**（谷歌学术）：[David Murray](https://scholar.google.com.hk/citations?hl=zh-CN&user=O5QreiwAAAAJ) &emsp; [Maurice Fallon](https://ori.ox.ac.uk/ori-people/maurice-fallon/)
+ 部分博士学位论文可以在这里搜到：https://ora.ox.ac.uk/

#### 18. 德国慕尼黑工业大学计算机视觉组

+ **研究方向**：三维重建、机器人视觉、深度学习、**视觉 SLAM** 等
+ **实验室主页**：https://vision.in.tum.de/research/vslam
+ **发表论文汇总**：https://vision.in.tum.de/publications
+ **代表作**：DSO、LDSO、LSD_SLAM、DVO_SLAM
    + 📜 **DSO**：Engel J, Koltun V, Cremers D. [**Direct sparse odometry**](https://ieeexplore.ieee.org/iel7/34/4359286/07898369.pdf)[J]. IEEE transactions on pattern analysis and machine intelligence, **2017**, 40(3): 611-625.（**代码**：https://github.com/JakobEngel/dso ）
    + 📜 **LSD-SLAM**： Engel J, Schöps T, Cremers D. [LSD-SLAM: Large-scale direct monocular SLAM](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.646.7193&rep=rep1&type=pdf)[C]//European conference on computer vision. Springer, Cham, **2014**: 834-849.（**代码**：https://github.com/tum-vision/lsd_slam ）2. 
+ **Github 地址**：https://github.com/tum-vision
+ 👦 **Daniel Cremers** 教授：[个人主页](https://vision.in.tum.de/members/cremers) [谷歌学术](https://scholar.google.com/citations?user=cXQciMEAAAAJ)
+ 👦 **Jakob Engel**（LSD-SLAM，DSO 作者）：[个人主页](https://jakobengel.github.io/) &emsp;[谷歌学术](https://scholar.google.de/citations?user=ndOMZXMAAAAJ)

#### 19. 德国马克斯普朗克智能系统研究所嵌入式视觉组

+ **研究方向**：智能体自主环境理解、导航与物体操纵
+ **实验室主页**：https://ev.is.tuebingen.mpg.de/
+ 👦 负责人 **Jörg Stückler**（前 TUM 教授）：[个人主页](https://ev.is.tuebingen.mpg.de/person/jstueckler) &emsp; [谷歌学术](https://scholar.google.de/citations?user=xrOzfucAAAAJ&hl=de)
+ 📜 **发表论文汇总**：https://ev.is.tuebingen.mpg.de/publications
+ Kasyanov A, Engelmann F, Stückler J, et al. [**Keyframe-based visual-inertial online SLAM with relocalization**](https://arxiv.org/pdf/1702.02175)[C]//2017 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2017**: 6662-6669.
+ 📜 Strecke M, Stuckler J. [**EM-Fusion: Dynamic Object-Level SLAM with Probabilistic Data Association**](http://openaccess.thecvf.com/content_ICCV_2019/papers/Strecke_EM-Fusion_Dynamic_Object-Level_SLAM_With_Probabilistic_Data_Association_ICCV_2019_paper.pdf)[C]//Proceedings of the IEEE International Conference on Computer Vision. **2019**: 5865-5874.
+ 📜 Usenko, V., Demmel, N., Schubert, D., Stückler, J., Cremers, D. [**Visual-Inertial Mapping with Non-Linear Factor Recovery**](https://arxiv.org/pdf/1904.06504) IEEE Robotics and Automation Letters (RA-L), 5, **2020**

#### 20. 德国弗莱堡大学智能自主系统实验室

+ **研究方向**：多机器人导航与协作，环境建模与状态估计
+ **实验室主页**：http://ais.informatik.uni-freiburg.de/index_en.php
+ **发表论文汇总**：http://ais.informatik.uni-freiburg.de/publications/index_en.php （学位论文也可以在这里找到）
+ 👦 **Wolfram Burgard**：[谷歌学术](https://scholar.google.com/citations?user=zj6FavAAAAAJ&hl=zh-CN&oi=ao)
+ **开放数据集**：http://aisdatasets.informatik.uni-freiburg.de/
+ 📜 **RGB-D SLAM**：Endres F, Hess J, Sturm J, et al. [**3-D mapping with an RGB-D camera**](http://perpustakaan.unitomo.ac.id/repository/3-D%20Mapping%20With%20an%20RGB-D%20Camera06594910.pdf)[J]. IEEE transactions on robotics, **2013**, 30(1): 177-187.（**代码**：https://github.com/felixendres/rgbdslam_v2 ）
+ 📜 **跨季节的 SLAM**：Naseer T, Ruhnke M, Stachniss C, et al. [**Robust visual SLAM across seasons**](http://ais.informatik.uni-freiburg.de/publications/papers/naseer15iros.pdf)[C]//2015 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2015**: 2529-2535.
+ 📜 **博士学位论文**：[Robust Graph-Based Localization and Mapping](http://ais.informatik.uni-freiburg.de/publications/papers/agarwal15phd.pdf) 2015
+ 📜 **博士学位论文**：[Discovering and Leveraging Deep Multimodal Structure for Reliable Robot Perception and Localization](http://ais.informatik.uni-freiburg.de/publications/papers/valada19phd.pdf) 2019
+ 📜 **博士学位论文**：[Robot Localization and Mapping in Dynamic Environments](https://freidok.uni-freiburg.de/fedora/objects/freidok:149938/datastreams/FILE1/content) 2019

#### 21. 西班牙萨拉戈萨大学机器人、感知与实时组 SLAM 实验室

+ **研究方向**：视觉 SLAM、物体 SLAM、非刚性 SLAM、机器人、增强现实
+ **实验室主页**：http://robots.unizar.es/slamlab/
+ **发表论文**：http://robots.unizar.es/slamlab/?extra=3 （论文好像没更新，可以访问下面实验室大佬的谷歌学术查看最新论文）
+ 👦 **J. M. M. Montiel**：[谷歌学术](https://scholar.google.com/citations?user=D99JRxwAAAAJ&hl=zh-CN&oi=sra)
+ 📜 Mur-Artal R, Tardós J D. [**Orb-slam2: An open-source slam system for monocular, stereo, and rgb-d cameras**](https://github.com/raulmur/ORB_SLAM2)[J]. IEEE Transactions on Robotics, **2017**, 33(5): 1255-1262.
+ Gálvez-López D, Salas M, Tardós J D, et al. [**Real-time monocular object slam**](https://arxiv.org/pdf/1504.02398.pdf)[J]. Robotics and Autonomous Systems, **2016**, 75: 435-449.
+ 📜 Strasdat H, Montiel J M M, Davison A J. [**Real-time monocular SLAM: Why filter?**](http://www.hauke.strasdat.net/files/strasdat2010icra.pdf)[C]//2010 IEEE International Conference on Robotics and Automation. IEEE, **2010**: 2657-2664.
+ 📜 Zubizarreta J, Aguinaga I, Montiel J M M. [**Direct sparse mapping**](https://arxiv.org/pdf/1904.06577)[J]. arXiv preprint arXiv:1904.06577, **2019**.
    + Elvira R, Tardós J D, Montiel J M M. [**ORBSLAM-Atlas: a robust and accurate multi-map system**](https://arxiv.org/pdf/1908.11585)[J]. arXiv preprint arXiv:1908.11585, **2019**.
    
#### 22. 西班牙马拉加大学机器感知与智能机器人课题组

+ **研究方向**：自主机器人、人工嗅觉、计算机视觉
+ **实验室主页**：http://mapir.uma.es/mapirwebsite/index.php/topics-2.html
+ **发表论文汇总**：http://mapir.isa.uma.es/mapirwebsite/index.php/publications-menu-home.html
+ 📜 Gomez-Ojeda R, Moreno F A, Zuñiga-Noël D, et al. [**PL-SLAM: a stereo SLAM system through the combination of points and line segments**](https://arxiv.org/pdf/1705.09479)[J]. IEEE Transactions on Robotics, **2019**, 35(3): 734-746.（代码：https://github.com/rubengooj/pl-slam ）
+ 👦 [**Francisco-Angel Moreno**](http://mapir.isa.uma.es/mapirwebsite/index.php/people/199-francisco-moreno-due%C3%B1as)
+ 👦 [**Ruben Gomez-Ojeda**](https://scholar.google.com/citations?user=7jne0V4AAAAJ&hl=zh-CN&oi=sra) 点线 SLAM
    + 📜 Gomez-Ojeda R, Briales J, Gonzalez-Jimenez J. [**PL-SVO: Semi-direct Monocular Visual Odometry by combining points and line segments**](http://mapir.isa.uma.es/rgomez/publications/iros16plsvo.pdf)[C]//Intelligent Robots and Systems (IROS), 2016 IEEE/RSJ International Conference on. IEEE, **2016**: 4211-4216.（**代码**：https://github.com/rubengooj/pl-svo ）
    + 📜 Gomez-Ojeda R, Gonzalez-Jimenez J. [**Robust stereo visual odometry through a probabilistic combination of points and line segments**](https://riuma.uma.es/xmlui/bitstream/handle/10630/11515/icra16rgo.pdf?sequence=1&isAllowed=y)[C]//2016 IEEE International Conference on Robotics and Automation (**ICRA**). IEEE, **2016**: 2521-2526.（**代码**：https://github.com/rubengooj/stvo-pl ）
    + 📜 Gomez-Ojeda R, Zuñiga-Noël D, Moreno F A, et al. [**PL-SLAM: a Stereo SLAM System through the Combination of Points and Line Segments**](https://arxiv.org/pdf/1705.09479.pdf)[J]. arXiv preprint arXiv:1705.09479, **2017**.（**代码**：https://github.com/rubengooj/pl-slam ）

#### 23. Alejo Concha（Oculus VR，西班牙萨拉戈萨大学）

+ **研究方向**：SLAM，单目稠密重建，传感器融合
+ 👦 **个人主页**：https://sites.google.com/view/alejoconcha/ &emsp; [**谷歌学术**](https://scholar.google.com/citations?user=GIaG3CsAAAAJ&hl=zh-CN&oi=sra)
+ Github：https://github.com/alejocb
+ 📜 **IROS 2015** 单目平面重建：[**DPPTAM: Dense piecewise planar tracking and mapping from a monocular sequence**](https://zaguan.unizar.es/record/36752/files/texto_completo.pdf) （代码：https://github.com/alejocb/dpptam ）
+ 📜 **IROS 2017** 开源 RGB-D SLAM：[**RGBDTAM: A Cost-Effective and Accurate RGB-D Tracking and Mapping System**](http://webdiis.unizar.es/~jcivera/papers/concha_etal_icra16.pdf)（代码：https://github.com/alejocb/rgbdtam ）
+ 📜 **ICRA 2016**：[**Visual-inertial direct SLAM**](http://webdiis.unizar.es/~jcivera/papers/concha_etal_icra16.pdf)
+ 📜 **ICRA 2014**：[**Using Superpixels in Monocular SLAM**](https://www.researchgate.net/profile/Alejo_Concha/publication/281559193_Using_superpixels_in_monocular_SLAM/links/55edffcb08aedecb68fc6ac2/Using-superpixels-in-monocular-SLAM.pdf)
+ **RSS 2014**：[**Manhattan and Piecewise-Planar Constraints for Dense Monocular Mapping**](http://roboticsproceedings.org/rss10/p16.pdf)

#### 24. 奥地利格拉茨技术大学计算机图形学与视觉研究所

+ **研究方向**：AR/VR，机器人视觉，机器学习，目标识别与三维重建
+ **实验室主页**：https://www.tugraz.at/institutes/icg/home/
+ 👦 **Friedrich Fraundorfer** 教授：[团队主页](https://www.tugraz.at/institutes/icg/research/team-fraundorfer/) &emsp;[谷歌学术](https://scholar.google.com/citations?user=M0boL5kAAAAJ&hl=zh-CN&oi=sra)
    + 📜 [**Visual Odometry: Part I The First 30 Years and Fundamentals**](http://www.eng.auburn.edu/~troppel/courses/7970%202015A%20AdvMobRob%20sp15/literature/vis%20odom%20tutor%20part1%20.pdf)
    + 📜 [**Visual Odometry: Part II: Matching, Robustness, Optimization, and Applications**](https://www.zora.uzh.ch/id/eprint/71030/1/Fraundorfer_Scaramuzza_Visual_odometry.pdf)
    + 📜 Schenk F, Fraundorfer F. [**RESLAM: A real-time robust edge-based SLAM system**](https://ieeexplore.ieee.org/abstract/document/8794462/)[C]//2019 International Conference on Robotics and Automation (ICRA). IEEE, **2019**: 154-160.（**代码**：https://github.com/fabianschenk/RESLAM ）
+ 👦 **Dieter Schmalstieg** 教授：[团队主页](https://www.tugraz.at/institutes/icg/research/team-schmalstieg/) &emsp;[谷歌学术](https://scholar.google.com/citations?user=xXu8K6IAAAAJ&hl=zh-CN&oi=ao)
    + 📜 教科书：[Augmented Reality: Principles and Practice](augmentedrealitybook.org)
    + 📜 Arth C, Pirchheim C, Ventura J, et al. [**Instant outdoor localization and slam initialization from 2.5 d maps**](https://ieeexplore.ieee.org/abstract/document/7164332/)[J]. IEEE transactions on visualization and computer graphics, **2015**, 21(11): 1309-1318.
    + 📜 Hachiuma R, Pirchheim C, Schmalstieg D, et al. [**DetectFusion: Detecting and Segmenting Both Known and Unknown Dynamic Objects in Real-time SLAM**](https://arxiv.org/pdf/1907.09127)[J]. arXiv preprint arXiv:1907.09127, **2019**.
    
#### 25. 波兰波兹南工业大学移动机器人实验室

+ **研究方向**：SLAM，机器人运动规划，控制
+ **实验室主页**：http://lrm.put.poznan.pl/
+ **Github 主页**：https://github.com/LRMPUT
+ 📜 Wietrzykowski J. [**On the representation of planes for efficient graph-based slam with high-level features**](https://yadda.icm.edu.pl/baztech/element/bwmeta1.element.baztech-7ac7a8f3-9caa-4a34-8a27-8f6c5f43408b)[J]. Journal of Automation Mobile Robotics and Intelligent Systems, **2016**, 10.（**代码**：https://github.com/LRMPUT/PlaneSLAM ）
+ 📜 Wietrzykowski J, Skrzypczyński P. [**PlaneLoc: Probabilistic global localization in 3-D using local planar features**](https://www.sciencedirect.com/science/article/pii/S0921889018303701)[J]. Robotics and Autonomous Systems, **2019**.（**代码**：https://github.com/LRMPUT/PlaneLoc ）
+ 📜 **PUTSLAM**：http://lrm.put.poznan.pl/putslam/

#### 26. Alexander Vakhitov（三星莫斯科 AI 中心）

+ **研究方向**：SLAM，几何视觉
+ 👦 **个人主页**：https://alexandervakhitov.github.io/ ，[谷歌学术](https://scholar.google.ru/citations?user=g_2iut0AAAAJ&hl=ru%22)
+ 📜 **点线 SLAM**：ICRA 2017 [**PL-SLAM: Real-time monocular visual SLAM with points and lines**](https://upcommons.upc.edu/bitstream/handle/2117/110259/1836-PL-SLAM--Real-Time-Monocular-Visual-SLAM-with-Points-and-Lines.pdf)
+ 📜 **点线定位**：Pumarola A, Vakhitov A, Agudo A, et al. [**Relative localization for aerial manipulation with PL-SLAM**](https://upcommons.upc.edu/bitstream/handle/2117/182388/2205-Relative-localization-for-aerial-manipulation-with-PL-SLAM.pdf)[M]//Aerial Robotic Manipulation. Springer, Cham, **2019**: 239-248.
+ 📜 **学习型线段**：IEEE Access 2019 [**Learnable line segment descriptor for visual SLAM**](https://ieeexplore.ieee.org/iel7/6287639/6514899/08651490.pdf)（**代码**：https://github.com/alexandervakhitov/lld-slam ）

#### 27. 澳大利亚昆士兰科技大学机器人技术中心

+ **研究方向**：脑启发式机器人，采矿机器人，机器人视觉
+ **实验室主页**：https://www.qut.edu.au/research/centre-for-robotics
+ **开源代码**：https://research.qut.edu.au/qcr/open-source-code/
+ 👦 **Niko Sünderhauf**：[个人主页](https://nikosuenderhauf.github.io/) ，[谷歌学术](https://scholar.google.com/citations?user=WnKjfFEAAAAJ&hl=zh-CN&oi=ao)
    + 📜 RA-L 2018 **二次曲面 SLAM**：[**QuadricSLAM: Dual quadrics from object detections as landmarks in object-oriented SLAM**](https://ieeexplore.ieee.org/abstract/document/8440105/)
    + 📜 Nicholson L, Milford M, Sunderhauf N. [**QuadricSLAM: Dual quadrics as SLAM landmarks**](http://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w9/Nicholson_QuadricSLAM_Dual_Quadrics_CVPR_2018_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition Workshops. **2018**: 313-314.
    + 📜 **Semantic SLAM 项目主页**：http://www.semanticslam.ai/
    + 📜 **IROS 2017**：[**Meaningful maps with object-oriented semantic mapping**](https://arxiv.org/pdf/1609.07849)
+ 👦 **Michael Milford**：谷歌学术 https://scholar.google.com/citations?user=TDSmCKgAAAAJ&hl=zh-CN&oi=ao
    + 📜 **ICRA 2012**：[**SeqSLAM: Visual route-based navigation for sunny summer days and stormy winter nights**](http://www.cim.mcgill.ca/~dudek/417/Resources/seqslam-milford.pdf) （代码：https://michaelmilford.com/seqslam/）
    + 📜 Ball D, Heath S, Wiles J, et al. [**OpenRatSLAM: an open source brain-based SLAM system**](https://static.springer.com/sgw/documents/1388513/application/pdf/10-3.pdf)[J]. Autonomous Robots, **2013**, 34(3): 149-176.（代码：https://openslam-org.github.io/openratslam.html ）
    + 📜 Yu F, Shang J, Hu Y, et al. [**NeuroSLAM: a brain-inspired SLAM system for 3D environments**](https://link.springer.com/article/10.1007/s00422-019-00806-9)[J]. Biological Cybernetics, **2019**, 113(5-6): 515-545. （**代码**：https://github.com/cognav/NeuroSLAM ）

#### 28. 澳大利亚机器人视觉中心

+ **研究方向**：机器人感知、理解与学习 （集合了昆士兰科技大学，澳大利亚国立大学，阿德莱德大学，昆士兰大学等学校机器人领域的研究者）
+ **实验室主页**：https://www.roboticvision.org/
+ **人物**：https://www.roboticvision.org/rv_person_category/researchers/
+ **发表论文汇总**：https://www.roboticvision.org/publications/scientific-publications/
+ 👦 **Yasir Latif**：[个人主页](http://ylatif.github.io/)，[谷歌学术](https://scholar.google.com/citations?user=pGsO6EkAAAAJ&hl=zh-CN)
    + 📜 Latif Y, Cadena C, Neira J. [**Robust loop closing over time for pose graph SLAM**](http://webdiis.unizar.es/~ylatif/papers/IJRR.pdf)[J]. The International Journal of Robotics Research, **2013**, 32(14): 1611-1626.
    + 📜 Latif Y, Cadena C, Neira J. [**Robust loop closing over time**](https://pdfs.semanticscholar.org/62fb/619f7fc036c4dfb4c55a7c53907a112fe001.pdf)[C]//Proc. Robotics: Science Systems. **2013**: 233-240.（代码：https://github.com/ylatif/rrr ）
+ 👦 **Ian D Reid**：谷歌学术：https://scholar.google.com/citations?user=ATkNLcQAAAAJ&hl=zh-CN&oi=sra
    + 📜 **ICRA 2019**：[**Real-time monocular object-model aware sparse SLAM**](https://arxiv.org/pdf/1809.09149)
    + 📜 Reid I. [**Towards semantic visual SLAM**](https://ieeexplore.ieee.org/abstract/document/7064267/)[C]//2014 13th International Conference on Control Automation Robotics & Vision (ICARCV). IEEE, **2014**: 1-1.
    
#### 29. 日本国立先进工业科学技术研究所

+ **人工智能研究中心**：https://www.airc.aist.go.jp/en/intro/
+ 👦 **Ken Sakurada**：[个人主页](https://kensakurada.github.io/)，[谷歌学术](https://scholar.google.com/citations?user=Q4JO-ncAAAAJ&hl=zh-CN&oi=sra)
    + 📜 Sumikura S, Shibuya M, Sakurada K. [**OpenVSLAM: A Versatile Visual SLAM Framework**](https://dl.acm.org/doi/pdf/10.1145/3343031.3350539)[C]//Proceedings of the 27th ACM International Conference on Multimedia. **2019**: 2292-2295.（**代码**：https://github.com/xdspacelab/openvslam ）
+ 👦 **Shuji Oishi**：[谷歌学术](https://scholar.google.com/citations?user=wlPYSDgAAAAJ&hl=zh-CN&oi=sra)
    + 📜 极稠密特征点建图：Yokozuka M, Oishi S, Thompson S, et al. [**VITAMIN-E: visual tracking and MappINg with extremely dense feature points**](http://openaccess.thecvf.com/content_CVPR_2019/papers/Yokozuka_VITAMIN-E_VIsual_Tracking_and_MappINg_With_Extremely_Dense_Feature_Points_CVPR_2019_paper.pdf)[C]//Proceedings of the IEEE conference on computer vision and pattern recognition. **2019**: 9641-9650.
    + 📜 Oishi S, Inoue Y, Miura J, et al. [**SeqSLAM++: View-based robot localization and navigation**](https://staff.aist.go.jp/shuji.oishi/assets/papers/published/SeqSLAM++_RAS2019.pdf)[J]. Robotics and Autonomous Systems, **2019**, 112: 13-21.
    
#### 30. Pyojin Kim（韩国首尔大学自主机器人实验室）

+ **研究方向**：视觉里程计，定位，AR/VR
+ 👦 [个人主页](http://pyojinkim.com/)，[谷歌学术](https://scholar.google.com/citations?user=NHpe_8IAAAAJ&hl=en)
+ 📜 **平面 SLAM**：ECCV 2018：[**Linear RGB-D SLAM for planar environments**](http://openaccess.thecvf.com/content_ECCV_2018/papers/Pyojin_Kim_Linear_RGB-D_SLAM_ECCV_2018_paper.pdf)
+ 📜 **光照变化下的鲁棒 SLAM**：ICRA 2017：[**Robust visual localization in changing lighting conditions**](https://www.nasa.gov/sites/default/files/atoms/files/kim2017robust.pdf)
+ 📜 **线面 SLAM**：CVPR 2018：[**Indoor RGB-D Compass from a Single Line and Plane**](http://openaccess.thecvf.com/content_cvpr_2018/papers/Kim_Indoor_RGB-D_Compass_CVPR_2018_paper.pdf)
+ 📜 **博士学位论文**：[**Low-Drift Visual Odometry for Indoor Robotics**](http://pyojinkim.com/download/papers/2019_pjinkim_PhDthesis_low.pdf)

#### 31. 香港科技大学空中机器人实验室

+ **研究方向**：空中机器人在复杂环境下的自主运行，包括状态估计、建图、运动规划、多机器人协同以及低成本传感器和计算组件的实验平台开发。
+ **实验室主页**：http://uav.ust.hk/
+ **发表论文**：http://uav.ust.hk/publications/ 
+ 👦 沈邵劼教授[**谷歌学术**](https://scholar.google.com/citations?user=u8Q0_xsAAAAJ&hl=zh-CN)
+ **代码公开地址**：https://github.com/HKUST-Aerial-Robotics
+ 📜 Qin T, Li P, Shen S. [**Vins-mono: A robust and versatile monocular visual-inertial state estimator**](https://arxiv.org/pdf/1708.03852.pdf)[J]. IEEE Transactions on Robotics, **2018**, 34(4): 1004-1020.（**代码**：https://github.com/HKUST-Aerial-Robotics/VINS-Mono ）
+ 📜 Wang K, Gao F, Shen S. [**Real-time scalable dense surfel mapping**](https://arxiv.org/pdf/1909.04250)[C]//2019 International Conference on Robotics and Automation (ICRA). IEEE, **2019**: 6919-6925.（**代码**：https://github.com/HKUST-Aerial-Robotics/DenseSurfelMapping ）

#### 32. 香港科技大学机器人与多感知实验室 RAM-LAB

+ **研究方向**：无人车；无人船；室内定位；机器学习。
+ **实验室主页**：https://www.ram-lab.com/
+ **发表论文**：https://www.ram-lab.com/publication/ 
+ 👦 刘明教授[**谷歌学术**](https://scholar.google.com/citations?user=CdV5LfQAAAAJ&hl=zh-CN&oi=sra)
+ 📜 Ye H, Chen Y, Liu M. [**Tightly coupled 3d lidar inertial odometry and mapping**](https://arxiv.org/pdf/1904.06993.pdf)[C]//2019 International Conference on Robotics and Automation (ICRA). IEEE, **2019**: 3144-3150.（**代码**：https://github.com/hyye/lio-mapping ）
+ 📜 Zhang J, Tai L, Boedecker J, et al. [**Neural slam: Learning to explore with external memory**]()[J]. arXiv preprint arXiv:1706.09520, **2017**.

#### 33. 香港中文大学天石机器人实验室

+ **研究方向**：工业、物流、手术机器人，三维影像，机器学习
+ **实验室主页**：http://ri.cuhk.edu.hk/
+ 👦 **刘云辉教授**：http://ri.cuhk.edu.hk/yhliu
+ 👦 **李浩昂**：[个人主页](https://sites.google.com/view/haoangli/homepage)，[谷歌学术](https://scholar.google.com/citations?user=KnnPc0YAAAAJ&hl=zh-CN&oi=sra)
    + 📜 Li H, Yao J, Bazin J C, et al. [**A monocular SLAM system leveraging structural regularity in Manhattan world**](http://cvrs.whu.edu.cn/projects/Struct-PL-SLAM/source/file/Struct_PL_SLAM.pdf)[C]//2018 IEEE International Conference on Robotics and Automation (ICRA). IEEE, **2018**: 2518-2525.
    + 📜 Li H, Yao J, Lu X, et al. [**Combining points and lines for camera pose estimation and optimization in monocular visual odometry**](https://ieeexplore.ieee.org/abstract/document/8202304/)[C]//2017 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2017**: 1289-1296.
    + 📜 消失点检测：Lu X, Yaoy J, Li H, et al. [**2-Line Exhaustive Searching for Real-Time Vanishing Point Estimation in Manhattan World**](https://www.computer.org/csdl/proceedings/wacv/2017/4822/00/07926628.pdf)[C]//Applications of Computer Vision (WACV), 2017 IEEE Winter Conference on. IEEE, **2017**: 345-353.（代码：https://github.com/xiaohulugo/VanishingPointDetection ）
+ 👦 **郑帆**：[个人主页](https://fzheng.me/cnabout/)，[谷歌学术](https://scholar.google.com/citations?user=PZOTyfIAAAAJ&hl=zh-CN&oi=sra)
    + 📜 Zheng F, Tang H, Liu Y H. [**Odometry-vision-based ground vehicle motion estimation with se (2)-constrained se (3) poses**](https://ieeexplore.ieee.org/abstract/document/8357438/)[J]. IEEE transactions on cybernetics, **2018**, 49(7): 2652-2663.（代码：https://github.com/izhengfan/se2clam ）
    + 📜 Zheng F, Liu Y H. [**Visual-Odometric Localization and Mapping for Ground Vehicles Using SE (2)-XYZ Constraints**](https://ieeexplore.ieee.org/abstract/document/8793928/)[C]//2019 International Conference on Robotics and Automation (ICRA). IEEE, **2019**: 3556-3562.（代码：https://github.com/izhengfan/se2lam ）

#### 34. 浙江大学 CAD&CG 国家重点实验室

+ **研究方向**：SFM/SLAM，三维重建，增强现实
+ **实验室主页**：http://www.zjucvg.net/
+ **Github 代码地址**：https://github.com/zju3dv
+ 👦 **章国峰教授**：[个人主页](http://www.cad.zju.edu.cn/home/gfzhang/)，[谷歌学术](https://scholar.google.com/citations?user=F0xfpXAAAAAJ&hl=zh-CN&oi=sra)
+ 📜 **ICE-BA**：Liu H, Chen M, Zhang G, et al. [**Ice-ba: Incremental, consistent and efficient bundle adjustment for visual-inertial slam**](http://openaccess.thecvf.com/content_cvpr_2018/papers/Liu_ICE-BA_Incremental_Consistent_CVPR_2018_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. **2018**: 1974-1982.（代码：https://github.com/zju3dv/EIBA ）
+ 📜 **RK-SLAM**：Liu H, Zhang G, Bao H. [**Robust keyframe-based monocular SLAM for augmented reality**](https://ieeexplore.ieee.org/abstract/document/7781760/)[C]//2016 IEEE International Symposium on Mixed and Augmented Reality (ISMAR). IEEE, **2016**: 1-10.（项目主页：http://www.zjucvg.net/rkslam/rkslam.html ）
+ 📜 **RD-SLAM**：Tan W, Liu H, Dong Z, et al. [**Robust monocular SLAM in dynamic environments**](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.431.8137&rep=rep1&type=pdf)[C]//2013 IEEE International Symposium on Mixed and Augmented Reality (ISMAR). IEEE, **2013**: 209-218.

#### 35. 邹丹平（上海交通大学）

+ **研究方向**：视觉 SLAM，SFM，多源导航，微型无人机
+ 👦 **个人主页**：http://drone.sjtu.edu.cn/dpzou/index.php ， [谷歌学术](https://scholar.google.com/citations?user=y6FsLDQAAAAJ&hl=en&oi=ao)
+ 📜 **Co-SLAM**：Zou D, Tan P. [**Coslam: Collaborative visual slam in dynamic environments**](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.463.8135&rep=rep1&type=pdf)[J]. IEEE transactions on pattern analysis and machine intelligence, **2012**, 35(2): 354-366.（**代码**：https://github.com/danping/CoSLAM ）
+ 📜 **StructSLAM**：Zhou H, Zou D, Pei L, et al. [**StructSLAM: Visual SLAM with building structure lines**]()[J]. IEEE Transactions on Vehicular Technology, **2015**, 64(4): 1364-1375.（**项目主页**：http://drone.sjtu.edu.cn/dpzou/project/structslam.php ）
+ 📜 **StructVIO**：Zou D, Wu Y, Pei L, et al. [**StructVIO: visual-inertial odometry with structural regularity of man-made environments**](https://arxiv.org/pdf/1810.06796)[J]. IEEE Transactions on Robotics, **2019**, 35(4): 999-1013.

#### 36. 布树辉教授（西北工业大学智能系统实验室）

+ **研究方向**：语义定位与建图、SLAM、在线学习与增量学习
+ 👦 **个人主页**：http://www.adv-ci.com/blog/ &emsp; [谷歌学术](https://scholar.google.com/citations?user=spwZ6b4AAAAJ&hl=zh-CN&oi=ao)
+ **布老师的课件**：http://www.adv-ci.com/blog/course/
+ 实验室 2018 年暑期培训资料：https://github.com/zdzhaoyong/SummerCamp2018
+ 📜 **开源的通用 SLAM 框架**：Zhao Y, Xu S, Bu S, et al. [**GSLAM: A general SLAM framework and benchmark**](http://openaccess.thecvf.com/content_ICCV_2019/papers/Zhao_GSLAM_A_General_SLAM_Framework_and_Benchmark_ICCV_2019_paper.pdf)[C]//Proceedings of the IEEE International Conference on Computer Vision. **2019**: 1110-1120.（**代码**：https://github.com/zdzhaoyong/GSLAM ）
+ 📜 Bu S, Zhao Y, Wan G, et al. [**Map2DFusion: Real-time incremental UAV image mosaicing based on monocular slam**](http://www.adv-ci.com/publications/2016_IROS.pdf)[C]//2016 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2016**: 4564-4571.（**代码**：https://github.com/zdzhaoyong/Map2DFusion ）
+ 📜 Wang W, Zhao Y, Han P, et al. [**TerrainFusion: Real-time Digital Surface Model Reconstruction based on Monocular SLAM**](https://ieeexplore.ieee.org/abstract/document/8967663/)[C]//2019 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2019**: 7895-7902.

#### +1 Cyrill Stachniss（德国波恩大学摄影测量与机器人实验室）

+ **研究方向**：概率机器人、SLAM、自主导航、视觉激光感知、场景分析与分配、无人飞行器
+ **实验室主页**：https://www.ipb.uni-bonn.de/
+ 👦 **个人主页**：https://www.ipb.uni-bonn.de/people/cyrill-stachniss/ [谷歌学术](https://scholar.google.com/citations?user=8vib2lAAAAAJ&hl=zh-CN&authuser=1&oi=ao)
+ 发表论文：https://www.ipb.uni-bonn.de/publications/
+ 开源代码：https://github.com/PRBonn
+ 📜 IROS 2019 激光语义 SLAM：Chen X, Milioto A, Palazzolo E, et al. [**SuMa++: Efficient LiDAR-based semantic SLAM**](https://ieeexplore.ieee.org/abstract/document/8967704/)[C]//2019 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2019**: 4530-4537.（代码：https://github.com/PRBonn/semantic_suma/ ）
+ Cyrill Stachniss 教授 SLAM 公开课：[youtube](https://www.youtube.com/watch?v=4QG0y0pIOBE&list=PLgnQpQtFTOGQh_J16IMwDlji18SWQ2PZ6) ； [bilibili](https://space.bilibili.com/16886998/channel/detail?cid=118821)
+ 波恩大学另外一个**智能自主系统实验室**：http://www.ais.uni-bonn.de/research.html

#### +1 上海科技大学

+ **Mobile Perception Lab**：http://mpl.sist.shanghaitech.edu.cn/
+ 👦 Laurent Kneip：[个人主页](https://www.laurentkneip.com/)；[谷歌学术](https://scholar.google.com.au/citations?user=lTmh1e0AAAAJ&hl=en)
+ 📜 Zhou Y, Li H, Kneip L. [**Canny-vo: Visual odometry with rgb-d cameras based on geometric 3-d–2-d edge alignment**](https://ieeexplore.ieee.org/abstract/document/8510917/)[J]. IEEE Transactions on Robotics, **2018**, 35(1): 184-199.
+ **自主移动机器人实验室**：https://robotics.shanghaitech.edu.cn/zh
+ 👦 Sören Schwertfeger：[个人主页](https://robotics.shanghaitech.edu.cn/zh/people/soeren)；[谷歌学术](https://scholar.google.com.au/citations?user=Y2olJ9kAAAAJ&hl=en&oi=ao)
+ 📜 Shan Z, Li R, Schwertfeger S. [**RGBD-Inertial Trajectory Estimation and Mapping for Ground Robots**](https://link.zhihu.com/?target=https%3A//www.mdpi.com/1424-8220/19/10/2251)[J]. Sensors, **2019**, 19(10): 2251.（代码：https://github.com/STAR-Center/VINS-RGBD ）

#### +1 美国密歇根大学机器人研究所

+ **学院官网**：https://robotics.umich.edu/
+ **研究方向**：https://robotics.umich.edu/research/focus-areas/
+ **感知机器人实验室（PeRL）**
    + 实验室主页：http://robots.engin.umich.edu/About/
    + 👦 **Ryan M. Eustice** [谷歌学术](https://scholar.google.com/citations?user=WroYmiAAAAAJ&hl=en&oi=ao)
    + 📜 激光雷达数据集 Pandey G, McBride J R, Eustice R M. [**Ford campus vision and lidar data set**](https://journals.sagepub.com/doi/abs/10.1177/0278364911400640)[J]. The International Journal of Robotics Research, **2011**, 30(13): 1543-1552. | [数据集](http://robots.engin.umich.edu/SoftwareData/Ford)
+ **APRIL robotics lab**
    + 实验室主页：https://april.eecs.umich.edu/
    + 👦 **Edwin Olson** [个人主页](https://april.eecs.umich.edu/people/ebolson/) | [谷歌学术](https://scholar.google.com/citations?user=GwtVjKYAAAAJ&hl=en&oi=ao)
    + 📜 Olson E. [**AprilTag: A robust and flexible visual fiducial system**](https://april.eecs.umich.edu/pdfs/olson2010tags.pdf)[C]//2011 IEEE International Conference on Robotics and Automation. IEEE, **2011**: 3400-3407. | [**代码**](https://github.com/AprilRobotics/apriltag)
    + 📜 Wang X, Marcotte R, Ferrer G, et al. [**ApriISAM: Real-time smoothing and mapping**](https://april.eecs.umich.edu/papers/details.php?name=wang2018aprilsam)[C]//2018 IEEE International Conference on Robotics and Automation (ICRA). IEEE, **2018**: 2486-2493. | [**代码**](https://github.com/xipengwang/AprilSAM)
    
#### +1 瑞士苏黎世联邦理工自主系统实验室

+ **研究方向**：复杂多样环境中自主运行的机器人和智能系统
+ **实验室主页**：https://asl.ethz.ch/
+ 发表论文：https://asl.ethz.ch/publications-and-sources/publications.html
+ [youtube](https://www.youtube.com/channel/UCgqwlRBPdDL2k4OWvH6Oppg) | [Github](https://github.com/ethz-asl)
+ 👦 **Cesar Cadena** [个人主页](http://n.ethz.ch/~cesarc/)
+ 📜 Schneider T, Dymczyk M, Fehr M, et al. [**maplab: An open framework for research in visual-inertial mapping and localization**](https://arxiv.org/pdf/1711.10250)[J]. IEEE Robotics and Automation Letters, **2018**, 3(3): 1418-1425. | [**代码**](https://github.com/ethz-asl/maplab)
+ 📜 Dubé R, Cramariuc A, Dugas D, et al. [**SegMap: 3d segment mapping using data-driven descriptors**](https://arxiv.org/pdf/1804.09557)[J]. arXiv preprint arXiv:1804.09557, **2018**. | [**代码**](https://github.com/ethz-asl/segmap)
+ 📜 Millane A, Taylor Z, Oleynikova H, et al. [**C-blox: A scalable and consistent tsdf-based dense mapping approach**](https://arxiv.org/pdf/1710.07242)[C]//2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, 2018: 995-1002. | [**代码**](https://github.com/ethz-asl/cblox)

#### +1 美国麻省理工学院 Robust Robotics Group

+ **研究方向**：MAV 导航与控制；人机交互的自然语言理解；自主海洋机器人的语义理解
+ **实验室主页**：http://groups.csail.mit.edu/rrg/index.php
+ 👦 Nicholas Roy：[Google Scholar](https://scholar.google.com/citations?user=aM3i_9oAAAAJ&hl=zh-CN&oi=ao)
+ 📜 Greene W N, Ok K, Lommel P, et al. [**Multi-level mapping: Real-time dense monocular SLAM**](https://ieeexplore.ieee.org/abstract/document/7487213/)[C]//2016 IEEE International Conference on Robotics and Automation (**ICRA**). IEEE, **2016**: 833-840. [video](https://www.youtube.com/watch?v=qk2ViPVxmq0&feature=youtu.be)
+ 📜 ICRA 2020 [Metrically-Scaled Monocular SLAM using Learned Scale Factors." International Conference on Robotics and Automation](http://groups.csail.mit.edu/rrg/papers/greene_icra20.pdf) | [video](https://www.youtube.com/watch?v=qk2ViPVxmq0&feature=youtu.be)       
+ 📜 ICRA 2019 [Robust Object-based SLAM for High-speed Autonomous Navigation](http://groups.csail.mit.edu/rrg/papers/OkLiu19icra.pdf)

#### +1 瑞士苏黎世联邦理工 Vision for Robotics Lab

+ **研究方向**：机器人视觉，无人机，自主导航，多机器人协同
+ **实验室主页**：https://v4rl.ethz.ch/the-group.html
+ 👦 **Margarita Chli**：[个人主页](http://www.margaritachli.com/)  | [Google Scholar](https://scholar.google.com/citations?user=C0UhwEIAAAAJ&hl=zh-CN&oi=ao)
+ 📜 Schmuck P, Chli M. [**CCM‐SLAM: Robust and efficient centralized collaborative monocular simultaneous localization and mapping for robotic teams**](https://onlinelibrary.wiley.com/doi/full/10.1002/rob.21854)[J]. Journal of Field Robotics, **2019**, 36(4): 763-781. [**code**](https://github.com/VIS4ROB-lab/ccm_slam) | [video](https://www.youtube.com/watch?v=P3b7UiTlmbQ&feature=youtu.be)       
+ 📜 Bartolomei L, Karrer M, Chli M. [**Multi-robot Coordination with Agent-Server Architecture for Autonomous Navigation in Partially Unknown Environments**](https://www.research-collection.ethz.ch/handle/20.500.11850/441280)[C]//IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS 2020)(virtual). **2020**. [**code**](https://github.com/VIS4ROB-lab/multi_robot_coordination) | [video](https://www.youtube.com/watch?v=ATQiTsbaSOw)       
+ 📜 Schmuck P, Chli M. [**Multi-uav collaborative monocular slam**](https://ieeexplore.ieee.org/abstract/document/7989445/)[C]//2017 IEEE International Conference on Robotics and Automation (ICRA). IEEE, **2017**: 3863-3870.

---

## 3. SLAM 学习资料
> 这一部分的内容不太完整，陆续丰富，欢迎补充

### 3.1 国内资料

+ **1)** SLAMcn：http://www.slamcn.org/index.php/
+ **2)** SLAM 最新研究更新 Recent_SLAM_Research ：https://github.com/YiChenCityU/Recent_SLAM_Research
+ **3)** **西北工大智能系统实验室 SLAM 培训**：https://github.com/zdzhaoyong/SummerCamp2018
  + 布树辉老师课件：http://www.adv-ci.com/blog/course/
+ **4)** IROS 2019 **视觉惯导导航**的挑战与应用研讨会：http://udel.edu/~ghuang/iros19-vins-workshop/index.html
+ **5)** 泡泡机器人 **VIO** 相关资料：https://github.com/PaoPaoRobot/Awesome-VIO
+ **6)** 崔华坤：主流 **VIO 论文推导及代码解析**：https://github.com/StevenCui/VIO-Doc
+ **7)** 李言：[SLAM 中的几何与学习方法](https://github.com/yanyan-li/SLAM-BOOK)
+ **8)** 黄山老师状态估计视频：[bilibili](https://www.bilibili.com/video/av66258275)
+ **9)** 谭平老师-SLAM 6小时课程：[bilibili](https://www.bilibili.com/video/BV1v4411p735)
+ **10)** 2020 年 SLAM 技术及应用暑期学校：[视频-bilibili](https://www.bilibili.com/video/BV1Hf4y1X7P5/) | [课件](http://www.cad.zju.edu.cn/home/gfzhang/download/2020-SLAM-Summer-School-slides.zip)

### 3.2 国外资料

+ **1)** **事件相机**相关研究与发展：https://github.com/uzh-rpg/event-based_vision_resources
+ **2)** 加州大学圣地亚哥分校**语境机器人研究所** Nikolay Atanasov 教授**机器人状态估计与感知课程** ppt：https://natanaso.github.io/ece276a2019/schedule.html
+ **3)** 波恩大学 **Mobile Sensing and Robotics Course** 公开课 ：[youtube](https://www.youtube.com/playlist?list=PLgnQpQtFTOGQJXx-x0t23RmRbjp_yMb4v) ，[bilibili](https://space.bilibili.com/16886998/channel/detail?cid=118821)

### 3.3 公众号

+ **泡泡机器人 SLAM**：paopaorobot_slam

### 3.4 代码注释

> 今天（2020.04.25）刚想到的一个点，就算前面整理了大量的开源工作，但是看原版的代码还是会有很大的困难，**感谢国内 SLAM 爱好者的将自己的代码注释分享出来，促进交流，共同进步**。这一小节的内容陆续发掘，期待大家的推荐代码注释（可以在 issue 中留言）。

### 3.5 数据集

+ [泡泡机器人 - SLAM 数据集合集](https://mp.weixin.qq.com/s/zRjwus68Kf4unIqPIubraw)
+ [计算机视觉life - SLAM、重建、语义相关数据集大全](https://zhuanlan.zhihu.com/p/68294012)
+ [水下 SLAM 相关研究 - 代码、数据集](http://note.youdao.com/s/GjCXvWFR)        

---

## 4. 近期论文（持续更新）

### 2020 年 10 月论文更新（22 篇）
 
> **本期更新于 2020 年 11 月 09 日       
共 22 篇论文，其中 7 项（待）开源工作       
9,10,11：SLAM 中动态物体跟踪，动态物体级 SLAM 今年很火        
3,7,8,14,18：线段相关**

#### 1. Geometric SLAM

+ [ ] **[1]** Bhutta M, Kuse M, Fan R, et al. [**Loop-box: Multi-Agent Direct SLAM Triggered by Single Loop Closure for Large-Scale Mapping**](https://arxiv.org/abs/2009.13851)[J]. arXiv preprint arXiv:2009.13851, **2020**. IEEE Transactions on Cybernetics, 2020
    + <font color = blue>用于大规模建图的由单闭环触发的多智能体直接 SLAM</font>
    + 香港科技大学；[项目主页](https://usmanmaqbool.github.io/loop-box)；[video](https://www.youtube.com/watch?v=AatjVz5ysV8)
    + 期刊：中科院一区，JCR Q1，IF 11.079
+ [ ] **[2]** Zhou B, He Y, Qian K, et al. [**S4-SLAM: A real-time 3D LIDAR SLAM system for ground/watersurface multi-scene outdoor applications**](https://link.springer.com/article/10.1007/s10514-020-09948-3)[J]. Autonomous Robots, **2020**: 1-22.
    + <font color = blue>S4-SLAM：用于地面/水面多场景户外应用的实时 3D LIDAR SLAM 系统</font>
    + 东南大学；期刊：中科院三区，JCR Q1，IF 3.6
+ [x] **[3]** Li Y, Yunus R, Brasch N, et al. [**RGB-D SLAM with Structural Regularities**](https://arxiv.org/abs/2010.07997)[J]. arXiv preprint arXiv:2010.07997, **2020**.
    + <font color = blue>**具有结构规律的 RGB-D SLAM**</font>
    + TUM
+ [ ] **[4]** Rodríguez J J G, Lamarca J, Morlana J, et al. [**SD-DefSLAM: Semi-Direct Monocular SLAM for Deformable and Intracorporeal Scenes**](https://arxiv.org/abs/2010.09409)[J]. arXiv preprint arXiv:2010.09409, **2020**.
    + <font color = blue>SD-DefSLAM：适用于可变形和体内场景的半直接法单目 SLAM</font>
    + 萨拉戈萨大学；ICRA 2021 投稿论文；[Video](https://www.youtube.com/watch?v=gkcC0IR3X6A&feature=youtu.be)
+ [x] **[5]** Millane A, Oleynikova H, Lanegger C, et al. [**Freetures: Localization in Signed Distance Function Maps**](https://arxiv.org/abs/2010.09378)[J]. arXiv preprint arXiv:2010.09378, **2020**.
    + <font color = blue>**Freetures：在 SDF 地图中进行定位**</font>
    + ETH；[代码开源](https://github.com/alexmillane/freetures)（待开源）；[Video](https://www.youtube.com/watch?v=O7ztVZDtDb0&feature=youtu.be)
+ [ ] **[6]** Long R, Rauch C, Zhang T, et al. [**RigidFusion: Robot Localisation and Mapping in Environments with Large Dynamic Rigid Objects**](https://arxiv.org/abs/2010.10841)[J]. arXiv preprint arXiv:2010.10841, **2020**.
    + <font color = blue>RigidFusion: 在具有动态刚体物体的大型场景中进行机器人定位与建图</font>
    + 爱丁堡大学机器人中心
+ [x] **[7]** Garcia-Fidalgo E, Ortiz A, Islands B. [**LiPo-LCD: Combining Lines and Points for Appearance-based Loop Closure Detection**](https://arxiv.org/abs/2009.09897)[J]. arXiv e-prints, **2020**: arXiv: 2009.09897.
    + <font color = blue>**LiPo-LCD：点线几何的基于外观的闭环检测**</font>
    + 巴利阿里群岛大学
+ [ ] **[8]** Han J, Dong R, Kan J. [**A novel loop closure detection method with the combination of points and lines based on information entropy**](https://onlinelibrary.wiley.com/doi/full/10.1002/rob.21992)[J]. Journal of Field Robotics. **2020**
    + <font color = blue>一种新的基于信息熵的点线闭环检测方法</font>
    + 北京林业大学；期刊：中科院二区，JCR Q1，IF 3.58

---

#### 2. Semantic/Deep SLAM

+ [x] **[9]** Bescos B, Campos C, Tardós J D, et al. [**DynaSLAM II: Tightly-Coupled Multi-Object Tracking and SLAM**](https://arxiv.org/abs/2010.07820)[J]. arXiv preprint arXiv:2010.07820, **2020**.
    + <font color = blue>**DynaSLAM II: 多目标跟踪与 SLAM 紧耦合**</font>
    + 萨拉戈萨大学；一作是 DynaSLAM 的作者，二作是 ORB-SLAM3 的作者
+ [x] **[10]** Bescos B, Cadena C, Neira J. [**Empty Cities: a Dynamic-Object-Invariant Space for Visual SLAM**](https://arxiv.org/abs/2010.07646)[J]. arXiv preprint arXiv:2010.07646, **2020**.
    + <font color = blue>**视觉 SLAM 动态的物体不变空间**</font>
    + 萨拉戈萨大学、ETH；[代码开源](https://github.com/bertabescos/EmptyCities_SLAM)
    + [个人主页](https://bertabescos.github.io/)，相关论文：
        + ICRA 2018 Empty Cities: Image Inpainting for a Dynamic-Object-Invariant Space
+ [x] **[11]** Ballester I, Fontan A, Civera J, et al. [**DOT: Dynamic Object Tracking for Visual SLAM**](https://arxiv.org/abs/2010.00052)[J]. arXiv preprint arXiv:2010.00052, **2020**.
    + <font color = blue>**视觉 SLAM 的动态物体跟踪**</font>
    + 萨拉戈萨大学
+ [ ] **[12]** Wu S C, Tateno K, Navab N, et al. [**SCFusion: Real-time Incremental Scene Reconstruction with Semantic Completion**](https://arxiv.org/abs/2010.13662)[J]. arXiv preprint arXiv:2010.13662, **2020**.
    + <font color = blue>SCFusion：具有完整语义的实时增量场景重建</font>
    + TUM
+ [ ] **[13]** Mallick A, Stückler J, Lensch H. [**Learning to Adapt Multi-View Stereo by Self-Supervision**](https://arxiv.org/abs/2009.13278)[J]. arXiv preprint arXiv:2009.13278, **2020**.
    + <font color = blue>**通过自监督学习的自适应多视图立体匹配**</font>
    + 图宾根大学，马普所 Jörg Stückler，**BMVC 2020**
    + 基于 ECCV 2018 [MVSNet: Depth Inference for Unstructured Multi-view Stereo](https://arxiv.org/abs/1804.02505)，[代码](https://github.com/xy-guo/MVSNet_pytorch)

---

#### 3. Sensor Fusion

+ [x] **[14]** Li X, Li Y, Ornek E P, et al. [**Co-Planar Parametrization for Stereo-SLAM and Visual-Inertial Odometry**](https://ieeexplore.ieee.org/abstract/document/9207814)[J]. IEEE Robotics and Automation Letters, **2020**.
    + <font color = blue>**双目 SLAM 和 VIO 的共面参数化**</font>
    + 北京大学，[代码开源](https://github.com/LiXin97/Co-Planar-Parametrization)（暂未放出）
+ [ ] **[15]** Liu Z, Zhang F. [**BALM: Bundle Adjustment for Lidar Mapping**](https://arxiv.org/abs/2010.08215)[J]. arXiv preprint arXiv:2010.08215, **2020**.
    + <font color = blue>BALM：激光雷达建图中的 BA 优化</font>
    + 香港大学，[代码开源](https://github.com/hku-mars/BALM)
+ [x] **[16]** Nguyen T M, Yuan S, Cao M, et al. [**VIRAL-Fusion: A Visual-Inertial-Ranging-Lidar Sensor Fusion Approach**](https://arxiv.org/abs/2010.12274)[J]. arXiv preprint arXiv:2010.12274, **2020**.
    + <font color = blue>**VIRAL-Fusion: 视觉-惯性-测距-激光雷达传感器融合方法**</font>
    + 南洋理工
+ [ ] **[17]** Liu J, Gao W, Hu Z. [**Optimization-Based Visual-Inertial SLAM Tightly Coupled with Raw GNSS Measurements**](https://arxiv.org/abs/2010.11675)[J]. arXiv preprint arXiv:2010.11675, **2020**.
    + <font color = blue>基于优化的视觉惯性 SLAM 与原始 GNSS 测量紧耦合</font>
    + 中科院自动化所；ICRA 2021 投稿论文

---

#### 4. Others

+ [ ] **[18]** Taubner F, Tschopp F, Novkovic T, et al. [**LCD--Line Clustering and Description for Place Recognition**](https://arxiv.org/abs/2010.10867)[J]. arXiv preprint arXiv:2010.10867, 2020. (**3DV 2020**)
    + <font color = blue>LCD: 用于位置识别的线段聚类和描述</font>
    + ETH；[代码开源](https://github.com/ethz-asl/lcd)
+ [x] **[19]** Triebel R. [**3D Scene Reconstruction from a Single Viewport**](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123670052.pdf). ECCV 2020
    + <font color = blue>**单视角进行三维场景重建**</font>
    + TUM；[代码开源](https://github.com/DLR-RM/SingleViewReconstruction)
+ [ ] **[20]** Hidalgo-Carrió J, Gehrig D, Scaramuzza D. [**Learning Monocular Dense Depth from Events**](https://arxiv.org/pdf/2010.08350.pdf)[J]. arXiv preprint arXiv:2010.08350, 2020.(**3DV 2020**)
    + <font color = blue>从事件中学习单目稠密深度</font>
    + 苏黎世大学；[代码开源](https://github.com/uzh-rpg/rpg_e2depth)；[项目主页](http://rpg.ifi.uzh.ch/E2DEPTH.html)
+ [x] **[21]** Yang B. [**Learning to reconstruct and segment 3D objects**](https://arxiv.org/abs/2010.09582)[J]. arXiv preprint arXiv:2010.09582, **2020**.
    + <font color = blue>**学习重建和分割 3D 物体**</font>
    + 牛津大学 [BoYang](https://yang7879.github.io/) 博士学位论文
+ [ ] **[22]** von Stumberg L, Wenzel P, Yang N, et al. [**LM-Reloc: Levenberg-Marquardt Based Direct Visual Relocalization**](**粗体文本**)[J]. arXiv preprint arXiv:2010.06323, **2020**.
    + <font color = blue>LM-Reloc：基于Levenberg-Marquardt 的直接视觉重定位</font>
    + TUM
    + 相关论文：von Stumberg L, Wenzel P, Khan Q, et al. [**Gn-net: The gauss-newton loss for multi-weather relocalization**](https://arxiv.org/abs/1904.11932)[J]. IEEE Robotics and Automation Letters, 2020, 5(2): 890-897.

---

### 2020 年 9 月论文更新（20 篇）
 
> **本期更新于 2020 年 9 月 28 日       
共 20 篇论文，其中 6 项（待）开源工作       
4-5：机器人自主探索        
8-11：多路标 SLAM        
13: Jan Czarnowski 博士学位论文        
17-20：增强现实相关的几项很好玩的工作**

#### 1. Geometric SLAM

+ [ ] **[1]** FZhao Y, Smith J S, Vela P A. [**Good graph to optimize: Cost-effective, budget-aware bundle adjustment in visual SLAM**](https://arxiv.org/abs/2008.10123)[J]. arXiv preprint arXiv:2008.10123, **2020**.
    + <font color = blue>Good Graph to Optimize: 视觉 SLAM 中具有成本效益、可感知预算的 BA</font>
    + 佐治亚理工学院 [Yipu Zhao](https://sites.google.com/site/zhaoyipu/)
    + 作者有很多 Good 系列的文章
        + IROS 2018 **Good feature selection for least squares pose optimization in VO/VSLAM**
        + ECCV 2018 **Good line cutting: Towards accurate pose tracking of line-assisted VO/VSLAM**
        + T-RO 2020 **Good Feature Matching: Towards Accurate, Robust VO/VSLAM with Low Latency**
+ [ ] **[2]** Fu Q, Yu H, Wang X, et al. [**FastORB-SLAM: a Fast ORB-SLAM Method with Coarse-to-Fine Descriptor Independent Keypoint Matching**](https://arxiv.org/pdf/2008.09870.pdf)[J]. arXiv preprint arXiv:2008.09870, **2020**.
    + <font color = blue>FastORB-SLAM: 一种 Coarse-to-Fine 描述符独立关键点匹配的快速 ORB-SLAM 方法</font>
    + 湖南大学
+ [x] **[3]** Wenzel P, Wang R, Yang N, et al. [**4Seasons: A Cross-Season Dataset for Multi-Weather SLAM in Autonomous Driving**](https://arxiv.org/abs/2009.06364)[J]. arXiv preprint arXiv:2009.06364, **2020**.
    + <font color = blue>**4Seasons：自动驾驶中多天气SLAM的跨季节数据集**</font>
    + 慕尼黑工业大学 [Nan Yang](https://vision.in.tum.de/members/yangn)
    + 数据集网页：http://www.4seasons-dataset.com/
+ [x] **[4]** Duong T, Yip M, Atanasov N. [**Autonomous Navigation in Unknown Environments with Sparse Bayesian Kernel-based Occupancy Mapping**](https://arxiv.org/abs/2009.07207)[J]. arXiv preprint arXiv:2009.07207, **2020**.
    + <font color = blue>**基于稀疏贝叶斯核占有地图的未知环境自主导航**</font>
    + UCSD [Nikolay A. Atanasov](https://natanaso.github.io/)
    + [项目主页](https://thaipduong.github.io/sbkm/) | [**代码开源**](https://github.com/thaipduong/sbkm)
+ [ ] **[5]** Bartolomei L, Karrer M, Chli M. [**Multi-robot Coordination with Agent-Server Architecture for Autonomous Navigation in Partially Unknown Environments**](https://www.research-collection.ethz.ch/bitstream/handle/20.500.11850/441280/IROS_2020_Multi_Robot_compressed_v4.pdf?sequence=1)[C]//IEEE/RSJ International Conference on Intelligent Robots and Systems (**IROS** 2020)(virtual). **2020**.
    + <font color = blue>在部分未知环境中实现自主导航的多机器人协同代理服务器架构</font>
    + ETH | [代码开源](https://github.com/VIS4ROB-lab/voxblox_multi_agent) | [video](https://www.youtube.com/watch?v=BlFbiuV-d10&feature=youtu.be)
+ [ ] **[6]** Kern A, Bobbe M, Khedar Y, et al. [**OpenREALM: Real-time Mapping for Unmanned Aerial Vehicles**](https://arxiv.org/abs/2009.10492)[J]. arXiv preprint arXiv:2009.10492, **2020**.
    + <font color = blue>OpenREALM：无人机实时建图框架</font>
    + [代码开源](https://github.com/laxnpander/OpenREALM) | [video](https://www.youtube.com/watch?v=9MvPTHP0r0c)
+ [ ] **[7]** Du Z J, Huang S S, Mu T J, et al. [**Accurate RGB-D SLAM in Dynamic Environment using Observationally Consistent Conditional Random Fields**](https://cg.cs.tsinghua.edu.cn/people/~shisheng/Papers/OC-CRF/paper6.pdf). 2020
    + <font color = blue>动态环境中使用观察一致 CRF 的精确 RGB-D SLAM</font>
    + 清华大学
+ [ ] **[8]** Holynski A, Geraghty D, Frahm J M, et al. [**Reducing Drift in Structure from Motion using Extended Features**](https://arxiv.org/abs/2008.12295)[J]. arXiv preprint arXiv:2008.12295, **2020**.
    + <font color = blue>使用拓展特征减小 SFM 中的漂移</font>
    + 华盛顿大学，Facebook
+ [ ] **[9]** Fu Q, Wang J, Yu H, et al. [**PL-VINS: Real-Time Monocular Visual-Inertial SLAM with Point and Line**](https://arxiv.org/abs/2009.07462)[J]. arXiv preprint arXiv:2009.07462, **2020**.
    + <font color = blue>PL-VINS: 实时点线单目视觉惯性 SLAM</font>
    + 湖南大学 | [代码开源](https://github.com/cnqiangfu/PL-VINS)
+ [ ] **[10]** Company-Corcoles J P, Garcia-Fidalgo E, Ortiz A. [**LiPo-LCD: Combining Lines and Points for Appearance-based Loop Closure Detection**](https://arxiv.org/abs/2009.09897)[J]. arXiv preprint arXiv:2009.09897, 2020.(**BMVC 2020**)
    + <font color = blue>几何点线的基于外观的闭环检测</font>
    + 巴利阿里群岛大学
+ [x] **[11]** Wang Q, Yan Z, Wang J, et al. [**Line Flow based SLAM**]()[J]. arXiv preprint arXiv:2009.09972, **2020**.
    + <font color = blue>**基于 SLAM 的线流**</font>
    + 北大
+ [ ] **[12]** Badias A, Alfaro I, Gonzalez D, et al. [**MORPH-DSLAM: Model Order Reduction for PHysics-based Deformable SLAM**](https://arxiv.org/abs/2009.00576)[J]. arXiv preprint arXiv:2009.00576, **2020**.
    + <font color = blue>基于物理可变形 SLAM 降低模型阶数</font>
    + 萨拉戈萨大学

---

#### 2. Semantic/Deep SLAM

+ [x] **[13]** Czarnowski J. [**Learned representations for real-time monocular SLAM**](https://spiral.imperial.ac.uk/handle/10044/1/82178)[J]. 2020.
    + <font color = blue>**实时单目 SLAM 的学习表示**</font>
    + 帝国理工学院 [Jan Czarnowski](https://scholar.google.com/citations?user=t-eq4skAAAAJ&hl=zh-CN&oi=sra) 博士学位论文 | 导师 Andrew Davison
    + 代表作
        + CVPR 2018 [CodeSLAM—learning a compact, optimisable representation for dense visual SLAM](https://openaccess.thecvf.com/content_cvpr_2018/papers/Bloesch_CodeSLAM_--_Learning_CVPR_2018_paper.pdf)
        + RAL 2020 [Deepfactors: Real-time probabilistic dense monocular slam](https://arxiv.org/pdf/2001.05049.pdf)
        + icra 2018 [DeepFusion: real-time dense 3D reconstruction for monocular SLAM using single-view depth and gradient predictions](https://www.imperial.ac.uk/media/imperial-college/research-centres-and-groups/dyson-robotics-lab/tlaidlow_etal_icra2019.pdf)
+ [ ] **[14]** Li J, Pei L, Zou D, et al. [**Attention-SLAM: A Visual Monocular SLAM Learning from Human Gaze**](https://arxiv.org/abs/2009.06886)[J]. arXiv preprint arXiv:2009.06886, **2020**.
    + <font color = blue>Attention-SLAM：从人类视线中学习的单目视觉 SLAM</font>
    + 上海交通大学
+ [ ] **[15]** Cremona J, Uzal L, Pire T. [**WGANVO: Monocular Visual Odometry based on Generative Adversarial Networks**](https://arxiv.org/abs/2007.13704)[J]. arXiv preprint arXiv:2007.13704, **2020**.
    + <font color = blue>WGANVO: 基于生成对抗网络的单目视觉里程计</font>
    + 阿根廷 CIFASIS | [代码开源](https://github.com/CIFASIS/wganvo) | [video](https://www.youtube.com/watch?v=zg5BlvUQhWE)
+ [x] **[16]** Labbé Y, Carpentier J, Aubry M, et al. [**CosyPose: Consistent multi-view multi-object 6D pose estimation**](https://arxiv.org/abs/2008.08465)[J]. arXiv preprint arXiv:2008.08465, **2020**.（ECCV 2020）
    + <font color = blue>**CosyPose：一致的多视图多物体 6D 位姿估计**</font>
    + Object SLAM @ 物体位姿估计

---

#### 3. AR/VR/MR

+ [x] **[17]** Yang X, Zhou L, Jiang H, et al. [**Mobile3DRecon: Real-time Monocular 3D Reconstruction on a Mobile Phone**](https://ieeexplore.ieee.org/document/9201064/authors#authors)[J]. IEEE Annals of the History of Computing, **2020** (01): 1-1.
    + <font color = blue>**Mobile3DRecon手机上的实时单目重建**</font>
    + 商汤、浙大
+ [ ] **[18]** Ungureanu D, Bogo F, Galliani S, et al. HoloLens 2 Research Mode as a Tool for Computer Vision Research[J]. arXiv preprint arXiv:2008.11239, 2020.
    + <font color = blue>HoloLens 2 研究模式作为计算机视觉研究的工具</font>
    + 三星 AI 中心，微软
+ [ ] **[19]** Mori S, Erat O, Broll W, et al. [**InpaintFusion: Incremental RGB-D Inpainting for 3D Scenes**](https://ieeexplore.ieee.org/abstract/document/9184389)[J]. IEEE Transactions on Visualization and Computer Graphics, **2020**, 26(10): 2994-3007.
    + <font color = blue>InpaintFusion：3D场景的增量RGB-D修复</font>
    + 格拉茨工业大学 期刊：中科院二区,JCR Q1, IF 4.558
+ [ ] **[20]** [**AAR: Augmenting a Wearable Augmented Reality Display with an Actuated Head-Mounted Projector**](https://jjhartmann.github.io/AugmentedAugmentedReality/assets/Hartmann_AugmentedAugmentedReality_UIST2020_LowRes.pdf). 2020
    + <font color = blue>使用可驱动的头戴式投影仪增强可穿戴的增强现实显示</font>
    + 滑铁卢大学
    + 在 AR 眼镜上再装个投影仪。。。。会玩

---

### 2020 年 8 月论文更新（30 篇）

> **本期更新于 2020 年 8 月 27 日       
共 30 篇论文，其中 11 项（待）开源工作       
这个月公开的论文比较多，且有意思、高质量的工作也不少，多来自于 IROS、RAL(大部分也同步发表于 IROS)，比如融合视觉、惯导、LiDAR 的 LIC-Fusion 2.0 和 融合物体语义的视惯里程计 OrcVIO，其他：         
4-6、15：多机/多地图        
8-13：结构化/室内 SLAM**

#### 1. Geometric SLAM

+ [ ] **[1]** Geppert M, Larsson V, Speciale P, et al. [**Privacy Preserving Structure-from-Motion**](https://cvg.ethz.ch/research/privacy-preserving-sfm/paper/Geppert2020ECCV.pdf)[J]. **2020**.
    + <font color = blue>具有隐私保护的 SFM</font>
    + 苏黎世联邦理工
    + 相关论文：
        + CVPR 2019 [Privacy Preserving Image-Based Localization](http://openaccess.thecvf.com/content_CVPR_2019/papers/Speciale_Privacy_Preserving_Image-Based_Localization_CVPR_2019_paper.pdf)
        + ECCV 2020 [Privacy Preserving Visual SLAM](https://arxiv.org/abs/2007.10361)
+ [x] **[2]** Zhang Z, Scaramuzza D. [**Fisher Information Field: an Efficient and Differentiable Map for Perception-aware Planning**](https://arxiv.org/abs/2008.03324)[J]. arXiv preprint arXiv:2008.03324, **2020**.
    + <font color = blue>Fisher 信息场：一种用于感知规划的高效且可微分的地图</font>
    + 苏黎世大学[张子潮](http://www.ifi.uzh.ch/en/rpg/people/zichao.html) | [代码开源](https://github.com/uzh-rpg/rpg_information_field)
    + 相关工作：ICRA 2019 [Beyond Point Clouds: Fisher Information Field for Active Visual Localization](http://rpg.ifi.uzh.ch/docs/ICRA19_Zhang.pdf)
+ [ ] **[3]** Zhou Y, Gallego G, Shen S. [**Event-based Stereo Visual Odometry**](https://arxiv.org/abs/2007.15548)[J]. arXiv preprint arXiv:2007.15548, **2020**.
    + <font color = blue>基于事件相机的双目视觉里程计</font>
    + 港科沈邵劼组 | [代码开源](https://github.com/HKUST-Aerial-Robotics/ESVO)（暂未公开）| [video](https://www.youtube.com/watch?v=3CPPs1gz04k&feature=youtu.be)
+ [ ] **[4]** Yue Y, Zhao C, Wu Z, et al. [**Collaborative Semantic Understanding and Mapping Framework for Autonomous Systems**](https://www.researchgate.net/profile/Yufeng_Yue/publication/343519028_Collaborative_Semantic_Understanding_and_Mapping_Framework_for_Autonomous_Systems/links/5f329ae4458515b72915ab09/Collaborative-Semantic-Understanding-and-Mapping-Framework-for-Autonomous-Systems.pdf)[J]. IEEE/ASME Transactions on Mechatronics, **2020**.
    + <font color = blue>自治系统协作式语义理解和建图框架</font>
    + 南洋理工大学 | 期刊：中科院二区，JCR Q1，IF 5.6
+ [ ] **[5]** Do H, Hong S, Kim J. [**Robust Loop Closure Method for Multi-Robot Map Fusion by Integration of Consistency and Data Similarity**](https://ieeexplore.ieee.org/abstract/document/9145697)[J]. IEEE Robotics and Automation Letters, **2020**, 5(4): 5701-5708.
    + <font color = blue>融合一致性和数据相似性的多机器人地图融合的闭环方法</font>
    + 韩国启明大学 | [Google Scholar](https://scholar.google.com/citations?user=rGX5_gEAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[6]** Zhan Z, Jian W, Li Y, et al. [**A SLAM Map Restoration Algorithm Based on Submaps and an Undirected Connected Graph**](https://arxiv.org/abs/2007.14592)[J]. arXiv preprint arXiv:2007.14592, **2020**.
    + <font color = blue>基于子图和无向连通图的 SLAM 地图恢复算法</font>
    + 武汉大学
+ [ ] **[7]** Chen H, Zhang G, Ye Y. [**Semantic Loop Closure Detection with Instance-Level Inconsistency Removal in Dynamic Industrial Scenes**](https://ieeexplore.ieee.org/abstract/document/9145862)[J]. IEEE Transactions on Industrial Informatics, **2020**.
    + <font color = blue>动态工业场景中具有实例级不一致消除功能的语义闭环检测</font>
    + 厦门大学 | 期刊：中科院一区，JCR Q1，IF 9.1 
+ [ ] **[8]** Li Y, Brasch N, Wang Y, et al. [**Structure-SLAM: Low-Drift Monocular SLAM in Indoor Environments**](https://ieeexplore.ieee.org/abstract/document/9165014)[J]. IEEE Robotics and Automation Letters, **2020**, 5(4): 6583-6590.
    + <font color = blue>Structure-SLAM：室内环境中的低漂移单目 SLAM</font>
    + TUM | [代码开源](https://github.com/yanyan-li/Structure-SLAM-PointLine)
+ [ ] **[9]** Liu J, Meng Z. [**Visual SLAM with Drift-Free Rotation Estimation in Manhattan World**](https://ieeexplore.ieee.org/abstract/document/9161354/)[J]. IEEE Robotics and Automation Letters, **2020**.
    + <font color = blue>亚特兰大世界的全局最优和有效消失点估计</font>
    + 港中文刘云辉教授组 [Haoang Li](https://scholar.google.com/citations?user=KnnPc0YAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[10]** Hou J, Yu L, Fei S. [**A highly robust automatic 3D reconstruction system based on integrated optimization by point line features**](https://www.sciencedirect.com/science/article/pii/S0952197620302256)[J]. Engineering Applications of Artificial Intelligence, **2020**, 95: 103879.
    + <font color = blue>基于点线联合优化的自动三维重建</font>
    + 苏州大学、东南大学 | 期刊：中科院二区，JCR Q1，IF 4.2
+ [ ] **[11]** Li H, Kim P, Zhao J, et al. [**Globally Optimal and Efficient Vanishing Point Estimation in Atlanta World**](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123670154.pdf)[J]. **2020**.
    + <font color = blue>曼哈顿世界中无漂移旋转估计的视觉 SLAM</font>
    + 港中文，西蒙弗雷泽大学
+ [ ] **[12]** Wang X, Christie M, Marchand E. [**Relative Pose Estimation and Planar Reconstruction via Superpixel-Driven Multiple Homographies**](https://hal.inria.fr/hal-02915045/document)[C]//IEEE/RSJ Int. Conf. on Intelligent Robots and Systems, **IROS'20**. 2020.
    + <font color = blue>通过超像素驱动的多个单应性的相对姿势估计和平面重建</font>
    + 雷恩大学
+ [ ] **[13]** Zuñiga-Noël D, Jaenal A, Gomez-Ojeda R, et al. [**The UMA-VI dataset: Visual–inertial odometry in low-textured and dynamic illumination environments**](https://journals.sagepub.com/doi/abs/10.1177/0278364920938439)[J]. The International Journal of Robotics Research, **2020**: 0278364920938439.
    + <font color = blue>UMA-VI 数据集：在低纹理和动态照明环境中的视觉惯性里程计</font>
    + 马拉加大学 | PL-SLAM 的[作者](http://mapir.uma.es/mapirwebsite/index.php/people/270) | 期刊：中科院二区，JCR Q1，IF 4.0 | [数据集地址](http://mapir.isa.uma.es/mapirwebsite/index.php/mapir-downloads/291-uma-visual-inertial-dataset.html)

---

#### 2. Sensor Fusion

+ [x] **[14]** Zuo X, Yang Y, Geneva P, et al. [**LIC-Fusion 2.0: LiDAR-Inertial-Camera Odometry with Sliding-Window Plane-Feature Tracking**](https://arxiv.org/abs/2008.07196)[J]. arXiv preprint arXiv:2008.07196, **2020**.
    + <font color = blue>**LIC-Fusion 2.0：滑动窗口平面特征跟踪的 LiDAR-惯性-视觉里程计**</font>
    + 浙大、ETH [Google Scholar](https://scholar.google.com/citations?user=CePv8agAAAAJ&hl=zh-CN&oi=sra)
    + 相关论文：[LIC-Fusion: LiDAR-Inertial-Camera Odometry](https://arxiv.org/abs/1909.04102)
+ [ ] **[15]** Alliez P, Bonardi F, Bouchafa S, et al. [**Real-Time Multi-SLAM System for Agent Localization and 3D Mapping in Dynamic Scenarios**](https://hal.inria.fr/hal-02913098/)[C]//International Confererence on Intelligent Robots and Systems (IROS 2020). **2020**.
    + <font color = blue>实时 Multi-SLAM 系统，用于动态场景中智能体定位和 3D 建图</font>
    + 法国国家信息与自动化研究所
+ [ ] **[16]** Shao X, Zhang L, Zhang T, et al. [**A Tightly-coupled Semantic SLAM System with Visual, Inertial and Surround-view Sensors for Autonomous Indoor Parking**](https://sse.tongji.edu.cn/linzhang/files/VISSLAM.pdf)[J].**2020**.
    + <font color = blue>具有视觉、惯性和全景传感器的紧密耦合语义 SLAM 系统，用于自主室内停车</font>
    + 同济大学
+ [x] **[17]** Shan M, Feng Q, Atanasov N. [**OrcVIO: Object residual constrained Visual-Inertial Odometry**](https://arxiv.org/abs/2007.15107)[J]. arXiv preprint arXiv:2007.15107, 2020.(**IROS 2020**)
    + <font color = blue>**物体残差约束的 VIO**</font>
    + 加州大学圣地亚哥分校 | [Nikolay A. Atanasov](https://scholar.google.com/citations?user=RTkSatQAAAAJ&hl=zh-CN&oi=sra) | [Mo Shan](http://me-llamo-sean.cf/)
+ [ ] **[18]** Seok H, Lim J. [**ROVINS: Robust Omnidirectional Visual Inertial Navigation System**](https://ieeexplore.ieee.org/abstract/document/9144432/)[J]. IEEE Robotics and Automation Letters, **2020**.
    + <font color = blue>鲁棒的全方位视觉惯性导航系统</font>
    + 韩国汉阳大学
+ [ ] **[19]** Liu W, Caruso D, Ilg E, et al. [**TLIO: Tight Learned Inertial Odometry**](https://ieeexplore.ieee.org/abstract/document/9134860)[J]. IEEE Robotics and Automation Letters, **2020**, 5(4): 5653-5660.
    + <font color = blue>基于学习的紧耦合的惯性里程计</font>
    + 宾夕法尼亚大学 | [代码开源](https://github.com/CathIAS/TLIO) | [项目主页](https://cathias.github.io/TLIO/)
+ [ ] **[20]** Sartipi K, Do T, Ke T, et al. [**Deep Depth Estimation from Visual-Inertial SLAM**](https://arxiv.org/abs/2008.00092)[J]. arXiv preprint arXiv:2008.00092, **2020**.
    + <font color = blue>视觉惯性 SLAM 深度估计</font>
    + 明尼苏达大学 | [代码开源](https://github.com/MARSLab-UMN/vi_depth_completion)

---

#### 3. Semantic/Deep SLAM

+ [x] **[21]** Gomez C, Hernandez A C, Derner E, et al. [**Object-Based Pose Graph for Dynamic Indoor Environments**](https://ieeexplore.ieee.org/abstract/document/9134440)[J]. IEEE Robotics and Automation Letters, **2020**, 5(4): 5401-5408.
    + <font color = blue>**动态室内环境中基于物体的位姿图**</font>
    + 马德里卡洛斯三世大学 | [Google Scholar](https://scholar.google.com/citations?user=2HNQTKwAAAAJ&hl=zh-CN&oi=sra)（有很多基于物体的机器人导航的工作）
+ [ ] **[22]** Wang H, Wang C, Xie L. [**Online Visual Place Recognition via Saliency Re-identification**](https://arxiv.org/abs/2007.14549)[J]. arXiv preprint arXiv:2007.14549, 2020.（**IROS 2020**）
    + <font color = blue>通过显著性重识别进行视觉场景重识别</font>
    + CMU | [代码开源](https://github.com/wh200720041/SRLCD)
+ [ ] **[23]** Jau Y Y, Zhu R, Su H, et al. [**Deep Keypoint-Based Camera Pose Estimation with Geometric Constraints**](https://arxiv.org/abs/2007.15122)[J]. arXiv preprint arXiv:2007.15122, 2020.（**IROS 2020**）
    + <font color = blue>具有几何约束的基于深度关键点的相机姿势估计</font>
    + 加州大学圣地亚哥分校 | [代码开源](https://github.com/eric-yyjau/pytorch-deepFEPE)
+ [ ] **[24]** Gong X, Liu Y, Wu Q, et al. [**An Accurate, Robust Visual Odometry and Detail-preserving Reconstruction System**](http://www.3dgp.net/paper/2020/An%20Accurate,%20Robust%20Visual%20Odometry%20and%20Detail-preserving%20Reconstruction%20System.pdf)[J]. **2020**.
    + <font color = blue>准确、鲁棒的视觉里程计和保留细节的重建系统</font>
    + 南京航空航天大学 | [代码开源](https://github.com/NUAA-XiaoxiG/EDI-VO)（暂未公开）
+ [ ] **[25]** Wei P, Hua G, Huang W, et al. [**Unsupervised Monocular Visual-inertial Odometry Network**](https://www.ijcai.org/Proceedings/2020/0325.pdf)[J].IJCAI 2020
    + <font color = blue>无监督单目视惯里程计网络</font>
    + 北大 | [代码开源](https://github.com/Ironbrotherstyle/UnVIO) （暂未公开）     
+ [ ] **[26]** Li D, Shi X, Long Q, et al. [**DXSLAM: A Robust and Efficient Visual SLAM System with Deep Features**](https://arxiv.org/abs/2008.05416)[J]. arXiv preprint arXiv:2008.05416, 2020.（**IROS 2020**）
    + <font color = blue>基于深度信息的鲁棒高效视觉 SLAM 系统</font>
    + 清华大学 | [代码开源](https://github.com/ivipsourcecode/dxslam)

---

#### 4. AR/VR/MR

+ [x] **[27]** Tahara T, Seno T, Narita G, et al. [**Retargetable AR: Context-aware Augmented Reality in Indoor Scenes based on 3D Scene Graph**](https://arxiv.org/abs/2008.07817)[J]. arXiv preprint arXiv:2008.07817, **2020**.
    + <font color = blue>**可重定位的 AR：基于室内 3D 场景图中的情景感知增强现实**</font>
    + 索尼
+ [ ] **[28]** Li X, Tian Y, Zhang F, et al. [**Object Detection in the Context of Mobile Augmented Reality**](https://arxiv.org/abs/2008.06655)[J]. arXiv preprint arXiv:2008.06655, 2020.（**ISMAR 2020**）
    + <font color = blue>移动增强现实环境下的目标检测</font>
    + oppo
+ [x] **[29]** Liu C, Shen S. [**An Augmented Reality Interaction Interface for Autonomous Drone**](https://arxiv.org/abs/2008.02234)[J]. arXiv preprint arXiv:2008.02234, 2020.（**IROS 2020**）
    + <font color = blue>**自主无人机增强现实交互界面**</font>
    + 港科沈邵劼组
+ [ ] **[30]** Du R, Turner E L, Dzitsiuk M, et al. [DepthLab: Real-time 3D Interaction with Depth Maps for Mobile Augmented Reality](https://research.google/pubs/pub49275/)[J]. 2020.
    + <font color = blue>使用深度地图实时 3D 交互的移动增强现实</font>
    + Google

---

### 2020 年 7 月论文更新（20 篇）

> **本期更新于 2020 年 7 月 27 日       
共 20 篇论文，其中 8 项（待）开源工作       
本月月初 ECCV，IROS 放榜，不少新论文出现        
2 隐私保护的视觉 SLAM，11 秦通大佬的 AVP-SLAM       
月底 ORB-SLAM3 又制造了大新闻，谷歌学术都没来得及收录，国内公众号都出解析了**

#### 1. Geometric SLAM

+ [x] **[1]** Carlos Campos, Richard Elvira, et al.[**ORB-SLAM3: An Accurate Open-Source Library for Visual, Visual-Inertial and Multi-Map SLAM**](https://arxiv.org/abs/2007.11898)[J]. arXiv preprint arXiv:2007.11898, **2020**.
    + <font color = blue>**ORB-SLAM3: 集视觉、视惯、多地图 SLAM 于一体**</font>
    + 西班牙萨拉戈萨大学 | [**代码开源**](https://github.com/UZ-SLAMLab/ORB_SLAM3) | [Video](https://www.youtube.com/channel/UCXVt-kXG6T95Z4tVaYlU80Q)
+ [x] **[2]** Shibuya M, Sumikura S, Sakurada K. [**Privacy Preserving Visual SLAM**](https://arxiv.org/abs/2007.10361)[J]. arXiv preprint arXiv:2007.10361, 2020.(**ECCV 2020**)
    + <font color = blue>**保护隐私的视觉 SLAM**</font>
    + 日本国立先进工业科学技术研究院；东京工业大学
    + 作者 Shinya Sumikura [谷歌学术](https://scholar.google.com/citations?user=BNC4JasAAAAJ&hl=zh-CN&oi=sra)，**OpenVSLAM** 的作者 | [项目主页](https://xdspacelab.github.io/lcvslam/) | [Video](https://www.youtube.com/watch?v=gEtUqnHx83w&feature=youtu.be)
    + 相关论文：CVPR 2019 [**Privacy preserving image-based localization**](http://openaccess.thecvf.com/content_CVPR_2019/html/Speciale_Privacy_Preserving_Image-Based_Localization_CVPR_2019_paper.html)
+ [x] **[3]** Tompkins A, Senanayake R, Ramos F. [**Online Domain Adaptation for Occupancy Mapping**](https://arxiv.org/abs/2007.00164)[J]. arXiv preprint arXiv:2007.00164, 2020.（**RSS 2020**）
    + <font color = blue>**在线区域调整以进行占有地图构建**</font>
    + 悉尼大学 | [**代码开源**](https://github.com/MushroomHunting/RSS2020-online-domain-adaptation-pot) | [Video](https://www.youtube.com/watch?v=qLv0mM9Le8E&feature=youtu.be)
+ [x] **[4]** Li Y, Zhang T, Nakamura Y, et al. [**SplitFusion: Simultaneous Tracking and Mapping for Non-Rigid Scenes**](https://arxiv.org/abs/2007.02108)[J]. arXiv preprint arXiv:2007.02108, 2020.(**IROS 2020**)
    + <font color = blue>**SplitFusion：非刚性场景的 SLAM**</font>
    + 东京大学
+ [ ] **[5]** WeiChen Dai, Yu Zhang, Ping Li, and Zheng Fang, Sebastian Scherer. [**RGB-D SLAM in Dynamic Environments Using Points Correlations**](https://arxiv.org/abs/1811.03217). IEEE Transactions on Pattern Analysis and Machine Intelligence (**TPAMI**), **2020**.
    + <font color = blue>**动态环境中使用点关联的 RGB-D SLAM**</font>
    + 浙江大学；期刊：PAMI 中科院一区，JCR Q1，IF 17.86
+ [x] **[6]** Huang H, Ye H, Sun Y, et al. [**GMMLoc: Structure Consistent Visual Localization with Gaussian Mixture Models**](https://ieeexplore.ieee.org/abstract/document/9126150)[J]. IEEE Robotics and Automation Letters, **2020**.
    + <font color = blue>**高斯混合模型的结构一致视觉定位**</font>
    + 香港科技大学 | [代码开源](https://github.com/HyHuang1995/gmmloc)

---

#### 2. Sensor Fusion

+ [ ] **[7]** Zuo X, Ye W, Yang Y, et al. [**Multimodal localization: Stereo over LiDAR map**](https://onlinelibrary.wiley.com/doi/full/10.1002/rob.21936)[J]. Journal of Field Robotics, **2020**.
    + <font color = blue>多模式定位：在 LiDAR 先验地图中使用双目相机定位</font>
    + 浙江大学、特拉华大学 | 作者[谷歌学术](https://scholar.google.com/citations?user=CePv8agAAAAJ&hl=zh-CN&oi=sra) | 期刊：中科院二区，JCR Q2，IF 4.19
+ [ ] **[8]** Shan T, Englot B, Meyers D, et al. [**LIO-SAM: Tightly-coupled Lidar Inertial Odometry via Smoothing and Mapping**](https://arxiv.org/abs/2007.00258)[J]. arXiv preprint arXiv:2007.00258, 2020.（**IROS 2020**）
    + <font color = blue>平滑紧耦合的激光雷达里程计和建图</font>
    + MIT | [**代码开源**](https://github.com/TixiaoShan/LIO-SAM) | [Video](https://www.youtube.com/watch?v=A0H8CoORZJU&feature=youtu.be)
+ [ ] **[9]** Rozenberszki D, Majdik A. [**LOL: Lidar-Only Odometry and Localization in 3D Point Cloud Maps**](https://arxiv.org/abs/2007.01595)[J]. arXiv preprint arXiv:2007.01595, 2020.（**ICRA 2020**）
    + <font color = blue>3D 点云地图中仅激光雷达的里程计和定位</font>
    + 匈牙利科学院机器感知实验室 | [**代码开源**](https://github.com/RozDavid/LOL) | [Video](https://www.youtube.com/watch?v=ektGb5SQGRM&feature=youtu.be)
+ [ ] **[10]** You R, Hou H. [**Real-Time Pose Estimation by Fusing Visual and Inertial Sensors for Autonomous Driving**]()[J]. **2020**.
    + <font color = blue>通过融合视觉和惯性传感器进行自动驾驶的实时位姿估计</font>
    + 瑞典查尔默斯理工大学 硕士学位论文 | [代码开源](https://github.com/chalmersfsd/cfsd-perception-slam)

---

#### 3. Semantic/Deep SLAM

+ [x] **[11]** Qin T, Chen T, Chen Y, et al. [**AVP-SLAM: Semantic Visual Mapping and Localization for Autonomous Vehicles in the Parking Lot**](https://arxiv.org/abs/2007.01813)[J]. arXiv preprint arXiv:2007.01813, **2020**.(**IROS 2020**)
    + <font color = blue>**AVP-SLAM：停车场中自动驾驶车辆的语义 SLAM**</font>
    + 华为秦通 | [知乎文章](https://zhuanlan.zhihu.com/p/157340737)
+ [x] **[12]** Gomez C, Silva A C H, Derner E, et al. [**Object-Based Pose Graph for Dynamic Indoor Environments**](https://ieeexplore.ieee.org/abstract/document/9134440)[J]. IEEE Robotics and Automation Letters, **2020**.
    + <font color = blue>**动态室内环境中基于物体的位姿图**</font>
    + 西班牙马德里卡洛斯三世大学
+ [ ] **[13]** Costante G, Mancini M. [**Uncertainty Estimation for Data-Driven Visual Odometry**](https://ieeexplore.ieee.org/abstract/document/9126117/)[J]. IEEE Transactions on Robotics, **2020**.
    + <font color = blue>数据驱动的视觉测程的不确定度估计</font>
    + 意大利佩鲁贾大学 | [**代码开源**](https://github.com/isarlab-department-engineering/UA-VO)（还未放出） | 期刊：中科院二区，JCR Q1，IF 7.0
+ [ ] **[14]** Min Z, Yang Y, Dunn E. [**VOLDOR: Visual Odometry From Log-Logistic Dense Optical Flow Residuals**](http://openaccess.thecvf.com/content_CVPR_2020/html/Min_VOLDOR_Visual_Odometry_From_Log-Logistic_Dense_Optical_Flow_Residuals_CVPR_2020_paper.html)[C]//Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. **CVPR 2020**: 4898-4909.
    + <font color = blue>对数逻辑密集光流残差的视觉里程计</font>
    + 史蒂文斯技术学院 | [**代码开源**](https://github.com/htkseason/VOLDOR)（还未放出）
+ [ ] **[15]** Zou Y, Ji P, Tran Q H, et al. [**Learning Monocular Visual Odometry via Self-Supervised Long-Term Modeling**](https://arxiv.org/abs/2007.10983)[J]. arXiv preprint arXiv:2007.10983, 2020.（**ECCV 2020**）
    + <font color = blue>自监督长期建模学习单目视觉里程计</font>
    + 弗吉尼亚理工大学 | [项目主页](https://yuliang.vision/LTMVO/) | 代码 Coming soon
+ [ ] **[16]** Wei P, Hua G, Huang W, et al. Unsupervised Monocular Visual-inertial Odometry Network[J].2020
    + <font color = blue>无监督单目视惯里程计</font>
    + 北京大学 | [**代码开源**](https://github.com/Ironbrotherstyle/UnVIO)（还未放出）

---

#### 4. AR/VR/MR

+ [ ] **[17]** Chen Y, Zhang B, Zhou J, et al. [**Real-time 3D unstructured environment reconstruction utilizing VR and Kinect-based immersive teleoperation for agricultural field robots**](https://www.sciencedirect.com/science/article/pii/S0168169920311479)[J]. Computers and Electronics in Agriculture, **2020**, 175: 105579.
    + <font color = blue>利用 VR 和基于 Kinect 的沉浸式远程操作技术对农业机器人进行实时 3D 非结构化环境重构</font>
    + 南京农业大学 | 期刊：中科院二区，JCR Q1，IF 4.0
+ [ ] **[18]** Choi J, Son M G, Lee Y Y, et al. [**Position-based augmented reality platform for aiding construction and inspection of offshore plants**](https://link.springer.com/article/10.1007/s00371-020-01902-9)[J]. The Visual Computer, **2020**: 1-11.
    + <font color = blue>基于位置的增强现实平台，用于辅助海上工厂的建设和检查</font>
    + 韩国光州科学技术院 | 期刊：中科院四区，JCR Q3

---

#### 5. Others

+ [ ] **[19]** Brazil G, Pons-Moll G, Liu X, et al. [**Kinematic 3D Object Detection in Monocular Video**](https://arxiv.org/abs/2007.09548)[J]. arXiv preprint arXiv:2007.09548, 2020.(**ECCV 2020**)
    + <font color = blue>**单目视频中运动 3D 目标检测**</font>
    + 密歇根州立大学 | [实验室主页](http://cvlab.cse.msu.edu/) | [项目主页](http://cvlab.cse.msu.edu/project-kinematic.html)（论文中说会开源）
+ [x] **[20]** Yu Z, Jin L, Gao S. [**P2Net: Patch-match and Plane-regularization for Unsupervised Indoor Depth Estimation**](https://arxiv.org/abs/2007.07696)[J]. arXiv preprint arXiv:2007.07696, 2020.（**ECCV 2020**）
    + <font color = blue>**无监督室内深度估计的块匹配和平面正则化**</font>
    + 上海科技大学 | [**代码开源**](https://github.com/svip-lab/Indoor-SfMLearner)

---

### 2020 年 6 月论文更新（20 篇）

> **本期更新于 2020 年 6 月 27 日       
共 20 篇论文，其中 3 项开源工作       
4,5,6,12,13 线、边、平面、物体多路标 SLAM       
2,3 多机器人 SLAM       
7,16 拓扑相关       
11：深度学习用于定位和建图的调研**

#### 1. Geometric SLAM

+ [ ] **[1]** Zhang T, Zhang H, Li Y, et al. [**FlowFusion: Dynamic Dense RGB-D SLAM Based on Optical Flow**](https://arxiv.org/abs/2003.05102)[C]. **ICRA 2020**.
    + <font color = blue>FlowFusion：基于光流的动态稠密 RGB-D SLAM</font>
    + 东京大学；[作者谷歌学术](https://scholar.google.com/citations?user=pKo_rrMAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[2]** Lajoie P Y, Ramtoula B, Chang Y, et al. [**DOOR-SLAM: Distributed, online, and outlier resilient SLAM for robotic teams**](https://ieeexplore.ieee.org/abstract/document/8962967/)[J]. IEEE Robotics and Automation Letters, **2020**, 5(2): 1656-1663.
    + <font color = blue>**适用于多机器人的分布式，在线和异常灵活的 SLAM**</font>
    + 加拿大蒙特利尔理工学院；[**代码开源**](https://github.com/MISTLab/DOOR-SLAM)
+ [ ] **[3]** Chakraborty K, Deegan M, Kulkarni P, et al. [**JORB-SLAM: A Jointly optimized Multi-Robot Visual SLAM**](https://um-mobrob-t12-w19.github.io/docs/report.pdf)[J].
    + <font color = blue>多机器人 SLAM 联合优化</font>
    + 密歇根大学机器人研究所
+ [x] **[4]** Zhang H, Ye C. [**Plane-Aided Visual-Inertial Odometry for 6-DOF Pose Estimation of a Robotic Navigation Aid**](https://ieeexplore.ieee.org/abstract/document/9091872/)[J]. IEEE Access, **2020**, 8: 90042-90051.
    + <font color = blue>用于机器人导航 6 自由度位姿估计的平面辅助 VIO</font>
    + 弗吉尼亚联邦大学；开源期刊；[谷歌学术](https://scholar.google.com/citations?user=u7uY5DMAAAAJ&hl=zh-CN&oi=sra)
+ [x] **[5]** Ali A J B, Hashemifar Z S, Dantu K. [**Edge-SLAM: edge-assisted visual simultaneous localization and mapping**](https://dl.acm.org/doi/pdf/10.1145/3386901.3389033)[C]//Proceedings of the 18th International Conference on Mobile Systems, Applications, and Services. **2020**: 325-337.
    + <font color = blue>**Edge-SLAM: 边辅助的视觉 SLAM**</font>
    + 布法罗大学
+ [ ] **[6]** Mateus A, Ramalingam S, Miraldo P. [**Minimal Solvers for 3D Scan Alignment With Pairs of Intersecting Lines**](http://openaccess.thecvf.com/content_CVPR_2020/papers/Mateus_Minimal_Solvers_for_3D_Scan_Alignment_With_Pairs_of_Intersecting_CVPR_2020_paper.pdf)[C]//Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. **2020**: 7234-7244.
    + <font color = blue>成对的相交线 3D 扫描对齐的最少求解器</font>
    + 葡萄牙里斯本大学，谷歌
+ [ ] **[7]** Xue W, Ying R, Gong Z, et al. [**SLAM Based Topological Mapping and Navigation**](https://ieeexplore.ieee.org/abstract/document/9110190/)[C]//2020 IEEE/ION Position, Location and Navigation Symposium (PLANS). IEEE, **2020**: 1336-1341.
    + <font color = blue>基于 SLAM 的拓扑建图与导航</font>
    + 上交
    
---

#### 2. Sensor Fusion

+ [ ] **[8]** Lee W, Eckenhoff K, Geneva P, et al. [**Intermittent GPS-aided VIO: Online Initialization and Calibration**](https://www.researchgate.net/profile/Patrick_Geneva/publication/341713067_Intermittent_GPS-aided_VIO_Online_Initialization_and_Calibration/links/5ed0063b299bf1c67d26cf5d/Intermittent-GPS-aided-VIO-Online-Initialization-and-Calibration.pdf)[J].**2020**
    + <font color = blue>间歇性 GPS 辅助 VIO：在线初始化和校准</font>
    + 特拉华大学，黄国权教授
+ [ ] **[9]** Alliez P, Bonardi F, Bouchafa S, et al. [**Indoor Localization and Mapping: Towards Tracking Resilience Through a Multi-SLAM Approach**](https://hal.inria.fr/hal-02611679/document)[C]//28th Mediterranean Conference on Control and Automation (MED 2020). **2020**.
    + <font color = blue>室内定位和制图：通过多传感器 SLAM 方法实现弹性跟踪</font>
+ [ ] **[10]** Nam D V, Gon-Woo K. [**Robust Stereo Visual Inertial Navigation System Based on Multi-Stage Outlier Removal in Dynamic Environments**](https://www.mdpi.com/1424-8220/20/10/2922)[J]. Sensors, **2020**, 20(10): 2922.
    + <font color = blue>动态环境中基于多阶段离群值剔除的鲁棒双目视觉惯性导航系统</font>
    + 韩国忠北国立大学，开源期刊，[作者主页](https://sites.google.com/view/dinhnam/)

---

#### 3. Semantic/Deep SLAM

+ [x] **[11]** Chen C, Wang B, Lu C X, et al. [**A Survey on Deep Learning for Localization and Mapping: Towards the Age of Spatial Machine Intelligence**](https://arxiv.org/abs/2006.12567)[J]. arXiv preprint arXiv:2006.12567, **2020**.
    + <font color = blue>**深度学习用于定位和建图的调研：走向空间机器智能时代**</font>
    + 牛津大学；所有涉及到的**论文的列表**：[Github](https://github.com/changhao-chen/deep-learning-localization-mapping)
+ [x] **[12]** Li J, Koreitem K, Meger D, et al. [**View-Invariant Loop Closure with Oriented Semantic Landmarks**](http://www.cim.mcgill.ca/~jimmyli/pubs/li2020icra.pdf)[C]. ICRA 2020.
    + <font color = blue>**面向语义路标的视图不变闭环**</font>
    + 麦吉尔大学；[谷歌学术](https://scholar.google.com/citations?user=DVuM2KsAAAAJ&hl=zh-CN&oi=sra)
+ [x] **[13]** Bavle H, De La Puente P, How J, et al. [**VPS-SLAM: Visual Planar Semantic SLAM for Aerial Robotic Systems**](https://ieeexplore.ieee.org/iel7/6287639/8948470/09045978.pdf)[J]. IEEE Access, **2020**.
    + <font color = blue>**VPS-SLAM：航空机器人的视觉平面语义 SLAM**</font>
    + 马德里理工大学自动化与机器人研究中心，MIT 航空航天控制实验室
    + [代码开源](https://bitbucket.org/hridaybavle/semantic_slam/src/master/)
+ [ ] **[14]** Shi T, Cui H, Song Z, et al. [**Dense Semantic 3D Map Based Long-Term Visual Localization with Hybrid Features**](https://arxiv.org/abs/2005.10766)[J]. arXiv preprint arXiv:2005.10766, **2020**.
    + <font color = blue>使用混合特征的基于密集 3D 语义地图的长距离视觉定位</font>
    + 中科院自动化所
+ [ ] **[15]** [**Metrically-Scaled Monocular SLAM using Learned Scale Factors**](https://wngreene.github.io/data/papers/greene_icra20.pdf) [C]. **ICRA 2020** Best Paper Award in Robot Vision
    + <font color = blue>通过学习尺度因子的单目度量 SLAM</font>
    + MIT；[作者主页](https://wngreene.github.io/)
+ [ ] **[16]** Chaplot D S, Salakhutdinov R, Gupta A, et al. [**Neural Topological SLAM for Visual Navigation**](http://openaccess.thecvf.com/content_CVPR_2020/papers/Chaplot_Neural_Topological_SLAM_for_Visual_Navigation_CVPR_2020_paper.pdf)[C]//Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. **CVPR 2020**: 12875-12884.
    + <font color = blue>用于视觉导航的神经拓扑SLAM</font>
    + CMU；[项目主页](https://www.cs.cmu.edu/~dchaplot/projects/neural-topological-slam.html)
+ [ ] **[17]** Min Z, Yang Y, Dunn E. [**VOLDOR: Visual Odometry From Log-Logistic Dense Optical Flow Residuals**](http://openaccess.thecvf.com/content_CVPR_2020/papers/Min_VOLDOR_Visual_Odometry_From_Log-Logistic_Dense_Optical_Flow_Residuals_CVPR_2020_paper.pdf)[C]//Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition. **CVPR 2020**: 4898-4909.
    + <font color = blue>基于对数逻辑稠密光流残差的视觉里程计</font>
    + 史蒂文斯理工学院；[代码开源](https://github.com/htkseason/VOLDOR)（还未放出）
+ [ ] **[18]** Loo S Y, Mashohor S, Tang S H, et al. [**DeepRelativeFusion: Dense Monocular SLAM using Single-Image Relative Depth Prediction**](https://arxiv.org/abs/2006.04047)[J]. arXiv preprint arXiv:2006.04047, **2020**.
    + <font color = blue>使用单视图深度预测的单目稠密 SLAM</font>
    + 哥伦比亚大学
    
---

#### 4. AR/VR/MR

+ [x] **[19]** Choudhary S, Sekhar N, Mahendran S, et al. [**Multi-user, Scalable 3D Object Detection in AR Cloud**](http://itzsid.github.io/scalable_or/CV4ARVR_Paper.pdf)[C]. CVPR Workshop on Computer Vision for Augmented and Virtual Reality, Seattle, WA, 2020.
    + <font color = blue>**AR 云进行多用户可扩展的 3D 目标检测**</font>
    + Magic Leap ；[项目主页](http://itzsid.github.io/scalable_or/index.html)
+ [ ] **[20]** Tang F, Wu Y, Hou X, et al. [**3D Mapping and 6D Pose Computation for Real Time Augmented Reality on Cylindrical Objects**](https://ieeexplore.ieee.org/abstract/document/8887213/)[J]. IEEE Transactions on Circuits and Systems for Video Technology, **2019**.
    + <font color = blue>圆柱物体上实时增强现实的 3D 建图和 6D 位姿计算</font>
    + 中科院自动化所

---

### 2020 年 5 月论文更新（20 篇）

> **本期更新于 2020 年 5 月 23 日       
共 20 篇论文，其中 5 项开源工作       
最近不知道是不是受疫情影响，论文好像有点少了        
Voxgraph：苏黎世理工开源的实时体素建图        
Neural-SLAM：CMU 开源的主动神经网络**

#### 1. Geometric SLAM

+ [x] **[1]** Wang W, Zhu D, Wang X, et al. [**TartanAir: A Dataset to Push the Limits of Visual SLAM**](https://arxiv.org/pdf/2003.14338)[J]. arXiv preprint arXiv:2003.14338, **2020**.
    + <font color = blue>**TartanAir：突破视觉 SLAM 极限的数据集**</font>
    + CMU，港中文；数据集公开：http://theairlab.org/tartanair-dataset/
    + 朱德龙师兄参与的一项工作，上个月推荐过了，这个月刚完善网站再推荐一遍，并在 CVPR 2020 组织了 [workshop](https://sites.google.com/view/vislocslamcvpr2020/slam-challenge)
+ [x] **[2]** Reijgwart V, Millane A, Oleynikova H, et al. [**Voxgraph: Globally Consistent, Volumetric Mapping Using Signed Distance Function Submaps**](https://www.research-collection.ethz.ch/bitstream/handle/20.500.11850/385682/1/Voxgraph-ETHpreprintversion.pdf)[J]. IEEE Robotics and Automation Letters, **2019**, 5(1): 227-234.
    + <font color = blue>**使用 SDF 子图的全局一致体素建图**</font>
    + 苏黎世联邦理工；[**代码开源**](https://github.com/ethz-asl/voxgraph)
+ [x] **[3]** Fontán A, Civera J, Triebel R. [**Information-Driven Direct RGB-D Odometry**](https://vision.in.tum.de/_media/spezial/bib/fontan20information.pdf)[J].2020.
    + <font color = blue>信息驱动的直接法 RGB-D SLAM</font>
    + 萨拉戈萨大学， TUM
+ [x] **[4]** Murai R, Saeedi S, Kelly P H J. [**BIT-VO: Visual Odometry at 300 FPS using Binary Features from the Focal Plane**](https://arxiv.org/abs/2004.11186)[J]. arXiv preprint arXiv:2004.11186, **2020**.
    + <font color = blue>**BIT-VO：使用焦平面的二进制特征以 300 FPS 运行的视觉里程计**</font>
    + 帝国理工 [项目主页、演示视频](https://rmurai0610.github.io/BIT-VO/)
+ [x] **[5]** Du S, Guo H, Chen Y, et al. [**GPO: Global Plane Optimization for Fast and Accurate Monocular SLAM Initialization**](https://arxiv.org/abs/2004.12051)[J]. ICRA **2020**.
    + <font color = blue>准确快速单目 SLAM 初始化的全局平面优化</font>
    + 中科院自动化所，字节跳动
+ [ ] **[6]** Li F, Fu C, Gostar A K, et al. [**Advanced Mapping Using Planar Features Segmented from 3D Point Clouds**](https://ieeexplore.ieee.org/abstract/document/9074570/)[C]//2019 International Conference on Control, Automation and Information Sciences (ICCAIS). IEEE, **2019**: 1-6.
    + <font color = blue>利用 3D 点云分割的平面进行建图</font>
    + 重庆大学
+ [ ] **[7]** Zou Y, Chen L, Jiang J. [**Lightweight Indoor Modeling Based on Vertical Planes and Lines**](https://ieeexplore.ieee.org/abstract/document/9078949/)[C]//2020 11th International Conference on Information and Communication Systems (ICICS). IEEE, **2020**: 136-142.
    + <font color = blue>基于垂直平面和线段的室内轻量化建图</font>
    + 国防科大；ICICS：CCF C 类会议
+ [ ] **[8]** Nobis F, Papanikolaou O, Betz J, et al. [**Persistent Map Saving for Visual Localization for Autonomous Vehicles: An ORB-SLAM Extension**](https://arxiv.org/abs/2005.07429)[J]. arXiv preprint arXiv:2005.07429, **2020**.
    + <font color = blue>ORB-SLAM2 的拓展应用：永久保存车辆视觉定位的地图</font>
    + TUM 汽车技术研究所；[**代码开源**](https://github.com/TUMFTM/orbslam-map-saving-extension)
    
---

#### 2. Sensor Fusion

+ [x] **[9]** Li X, He Y, Lin J, et al. [**Leveraging Planar Regularities for Point Line Visual-Inertial Odometry**](https://arxiv.org/abs/2004.11969)[J]. arXiv preprint arXiv:2004.11969, **2020**.
    + <font color = blue>利用平面规律的点线 VIO</font>
    + 北京大学；IROS 2020 投稿论文
+ [ ] **[10]** Liu J, Gao W, Hu Z. [**Bidirectional Trajectory Computation for Odometer-Aided Visual-Inertial SLAM**](https://arxiv.org/abs/2002.00195)[J]. arXiv preprint arXiv:2002.00195, **2020**.
    + <font color = blue>里程计辅助视惯 SLAM 的双向轨迹计算</font>
    + 中科院自动化所；**解决 SLAM 在转弯之后容易退化的问题**
+ [ ] **[11]** Liu R, Marakkalage S H, Padmal M, et al. [**Collaborative SLAM based on Wifi Fingerprint Similarity and Motion Information**](https://ieeexplore.ieee.org/abstract/document/8920098/)[J]. IEEE Internet of Things Journal, **2019**.
    + <font color = blue>基于 Wifi 指纹相似度和运动信息的协作式 SLAM</font>
    + 新加坡科技设计大学；期刊：中科院一区，JCR Q1，IF 11.2
+ [ ] **[12]** Jung J H, Heo S, Park C G. [**Observability Analysis of IMU Intrinsic Parameters in Stereo Visual-Inertial Odometry**](https://ieeexplore.ieee.org/abstract/document/9056527/)[J]. IEEE Transactions on Instrumentation and Measurement, **2020**.
    + <font color = blue>立体视觉惯性里程计中IMU内部参数的可观察性分析</font>
    + 韩国首尔大学；期刊：中科院三区，JCR Q2，IF 3.0

---

#### 3. Semantic/Deep SLAM

+ [x] **[13]** Wu Y, Zhang Y, Zhu D, et al. [**EAO-SLAM: Monocular Semi-Dense Object SLAM Based on Ensemble Data Association**](https://arxiv.org/abs/2004.12730)[J]. arXiv preprint arXiv:2004.12730, **2020**.
    + <font color = blue>**基于集合数据关联的单目半稠密物体级 SLAM**</font>
    + 东北大学，港中文；IROS 2020 投稿论文
    + 厚着脸皮推荐一下自己的工作，欢迎批评指正
    + [**代码开源**]()（还未公开）；演示视频：[**YouTube**](https://youtu.be/pvwdQoV1KBI) | [**bilibili**](https://www.bilibili.com/video/av94805216)
+ [ ] **[14]** Vasilopoulos V, Pavlakos G, Schmeckpeper K, et al. [**Reactive Navigation in Partially Familiar Planar Environments Using Semantic Perceptual Feedback**](https://arxiv.org/abs/2002.08946)[J]. arXiv preprint arXiv:2002.08946, **2020**.
    + <font color = blue>使用语义感知反馈的部分熟悉平面环境中的反应性导航</font>
    + 宾夕法尼亚大学
+ [x] **[15]** Chaplot D S, Gandhi D, Gupta S, et al. [**Learning to explore using active neural slam**](https://arxiv.org/abs/2004.05155)[C]. ICLR **2020**.
    + <font color = blue>**使用主动神经 SLAM 进行学习探索**</font>
    + CMU；[**代码开源**](https://github.com/devendrachaplot/Neural-SLAM)；[项目主页](https://www.cs.cmu.edu/~dchaplot/projects/neural-slam.html)
+ [ ] **[16]** Li S, Wang X, Cao Y, et al. [**Self-Supervised Deep Visual Odometry with Online Adaptation**]()[C]. CVPR. 2020.
    + <font color = blue>在线自适应的自监督视觉里程计</font>
    + 北京大学
+ [x] **[17]** Li W, Gu J, Chen B, et al. [**Incremental Instance-Oriented 3D Semantic Mapping via RGB-D Cameras for Unknown Indoor Scene**](https://www.hindawi.com/journals/ddns/2020/2528954/)[J]. Discrete Dynamics in Nature and Society, 2020, **2020**.
    + <font color = blue>RGB-D 相机室内增量式三维实例语义建图</font>
    + 河北工业大学；期刊：中科院三区，JCR Q3Q4 开源期刊
+ [x] **[18]** Tiwari L, Ji P, Tran Q H, et al. [**Pseudo RGB-D for Self-Improving Monocular SLAM and Depth Prediction**](https://arxiv.org/abs/2004.10681)[J]. arXiv preprint arXiv:2004.10681, **2020**.
    + <font color = blue>伪 RGB-D 用于改善单目 SLAM 和深度预测</font>（单目 SLAM + 单目深度估计）
    + 印度德里 Indraprastha 信息技术学院(IIIT-Delhi)

---

#### 4. Others

+ [ ] **[19]** Wald J, Dhamo H, Navab N, et al. [**Learning 3D Semantic Scene Graphs from 3D Indoor Reconstructions**](https://arxiv.org/pdf/2004.03967.pdf)[C]. CVPR **2020**.
    + <font color = blue>从三维室内重建中学习 3D 语义场景图</font>
    + TUM；[项目主页](https://3dssg.github.io/)；[Video](https://www.youtube.com/watch?v=8D3HjYf6cYw)
+ [ ] **[20]** Sommer C, Sun Y, Bylow E, et al. [**PrimiTect: Fast Continuous Hough Voting for Primitive Detection**](https://arxiv.org/abs/2005.07457)[C]. ICRA **2020**.
    + <font color = blue>用于基元检验的快速连续霍夫投票</font>
    + TUM

---

### 2020 年 4 月论文更新（22 篇）
> **本期更新于 2020 年 4 月 25 日       
共 22 篇论文，其中 7 项开源工作， 1 项公开数据集；     
2、8、12 跟线段有关       
9、10 VIO 相关        
TartanAir 突破视觉 SLAM 极限的数据集，投稿于 IROS 2020        
VPS-SLAM 平面语义 SLAM 比较有意思，代码开源**

#### 1. Geometric SLAM

+ [x] **[1]** Wang W, Zhu D, Wang X, et al. [**TartanAir: A Dataset to Push the Limits of Visual SLAM**](https://arxiv.org/pdf/2003.14338)[J]. arXiv preprint arXiv:2003.14338, **2020**.
    + <font color = blue>**TartanAir：突破视觉 SLAM 极限的数据集**</font>
    + CMU，港中文；数据集公开：http://theairlab.org/tartanair-dataset/
    + **朱德龙师兄的工作，置顶推荐一下**
+ [x] **[2]** Gomez-Ojeda R. [**Robust Visual SLAM in Challenging Environments with Low-texture and Dynamic Illumination**](https://riuma.uma.es/xmlui/handle/10630/19479)[J]. **2020**.
    + <font color = blue>**低纹理和动态光照挑战环境下的鲁棒视觉 SLAM**</font>
    + 西班牙马拉加大学，**点线 SLAM 作者的博士学位论文**
+ [ ] **[3]** Yang S, Li B, Cao Y P, et al. [**Noise-resilient reconstruction of panoramas and 3D scenes using robot-mounted unsynchronized commodity RGB-D cameras**](http://orca.cf.ac.uk/130657/1/DepthPano-TOG2020.pdf)[J]. ACM Transactions on Graphics, **2020**.
    + <font color = blue>使用安装在机器人上的非商用 RGB-D 相机对全景图和三维场景进行抗噪声重建</font>
    + 清华大学胡事民教授，期刊：中科院二区，JCR Q1，IF 7.176
+ [x] **[4]** Huang J, Yang S, Mu T J, et al. [**ClusterVO: Clustering Moving Instances and Estimating Visual Odometry for Self and Surroundings**](https://arxiv.org/pdf/2003.12980)[J]. arXiv preprint arXiv:2003.12980, **2020**.
    + <font color = blue>**ClusterVO：对移动实例进行聚类并估算自身和周围环境的视觉里程计**</font>
    + 清华大学胡事民教授；[演示视频](https://www.youtube.com/watch?v=paK-WCQpX-Y&feature=youtu.be)
    + Huang J, Yang S, Zhao Z, et al. [**ClusterSLAM: A SLAM Backend for Simultaneous Rigid Body Clustering and Motion Estimation**](http://openaccess.thecvf.com/content_ICCV_2019/papers/Huang_ClusterSLAM_A_SLAM_Backend_for_Simultaneous_Rigid_Body_Clustering_and_ICCV_2019_paper.pdf)[C]//Proceedings of the IEEE International Conference on Computer Vision. **2019**: 5875-5884.
+ [ ] **[5]** Quenzel J, Rosu R A, Läbe T, et al. [**Beyond Photometric Consistency: Gradient-based Dissimilarity for Improving Visual Odometry and Stereo Matching**](https://arxiv.org/pdf/2004.04090)[C]. International Conference on Robotics and Automation (ICRA), **2020**.
    + <font color = blue>超越光度一致性：用于改善视觉里程计和立体匹配的基于梯度的差异</font>
    + [波恩大学智能自主实验室](http://www.ais.uni-bonn.de/research.html)
+ [ ] **[6]** Yang Y, Tang D, Wang D, et al. [**Multi-camera visual SLAM for off-road navigation**](https://www.sciencedirect.com/science/article/pii/S0921889019308711)[J]. Robotics and Autonomous Systems, **2020**: 103505.
    + <font color = blue>用于越野导航的多相机 SLAM</font>
    + 北理工自动化学院
+ [ ] **[7]** Cheng W. [**Methods for large-scale image-based localization using structure-from-motion point clouds**](https://dr.ntu.edu.sg/bitstream/10356/137803/2/wentao_cheng_PhD_thesis.pdf)[J]. **2020**.
    + <font color = blue>利用 SFM 点云在大规模环境下的基于图像的定位</font>
    + 南洋理工大学博士学位论文；[相关代码](https://github.com/wentaocheng-cv/cpf_localization)
+ [ ] **[8]** Sun T, Song D, Yeung D Y, et al. [**Semi-semantic Line-Cluster Assisted Monocular SLAM for Indoor Environments**](https://arxiv.org/pdf/1811.01592)[C]//International Conference on Computer Vision Systems. Springer, Cham, **2019**: 63-74.
    + <font color = blue>室内环境中半语义线段簇辅助单目 SLAM</font>
    + 香港科技大学机器人与多感知实验室 RAM-LAB

---

#### 2. Sensor Fusion

+ [x] **[9]** Nagy B, Foehn P, Scaramuzza D. [**Faster than FAST: GPU-Accelerated Frontend for High-Speed VIO**](https://arxiv.org/pdf/2003.13493)[J]. arXiv preprint arXiv:2003.13493, **2020**.
    + <font color = blue>**用于高速 VIO 的前端 GPU 加速**</font>
    + 苏黎世大学、苏黎世联邦理工；[**代码开源**](https://github.com/uzh-rpg/vilib)
+ [x] **[10]** Li J, Yang B, Huang K, et al. [**Robust and Efficient Visual-Inertial Odometry with Multi-plane Priors**](http://www.cad.zju.edu.cn/home/gfzhang/projects/prcv2019-planeVIO.pdf)[C]//Chinese Conference on Pattern Recognition and Computer Vision (PRCV). Springer, Cham, **2019**: 283-295.
    + <font color = blue>具有多平面先验的稳健高效的视觉惯性里程计</font>
    + 浙大 CAD&CG 实验室，章国峰；[章老师主页](http://www.cad.zju.edu.cn/home/gfzhang/)上是显示**将会开源**
+ [ ] **[11]** Debeunne C, Vivet D. [**A Review of Visual-LiDAR Fusion based Simultaneous Localization and Mapping**](https://www.mdpi.com/1424-8220/20/7/2068)[J]. Sensors, **2020**, 20(7): 2068.
    + <font color = blue>视觉-激光 SLAM 综述</font>
    + 图卢兹大学；开源期刊，中科院三区，JCR Q2Q3
+ [ ] **[12]** Yu H, Zhen W, Yang W, et al. [**Monocular Camera Localization in Prior LiDAR Maps with 2D-3D Line Correspondences**](https://arxiv.org/pdf/2004.00740)[J]. arXiv preprint arXiv:2004.00740, **2020**.
    + <font color = blue>在先验雷达地图中通过 2D-3D 线段关联实现单目视觉定位</font>
    + CMU，武汉大学；[**代码开源**](https://github.com/levenberg/2D-3D-pose-tracking)

---

#### 3. Semantic/Deep SLAM

+ [x] **[13]** Bavle H, De La Puente P, How J, et al. [**VPS-SLAM: Visual Planar Semantic SLAM for Aerial Robotic Systems**](https://ieeexplore.ieee.org/iel7/6287639/8948470/09045978.pdf)[J]. IEEE Access, **2020**.
    + <font color = blue>**VPS-SLAM：航空机器人的视觉平面语义 SLAM**</font>
    + 马德里理工大学自动化与机器人研究中心，MIT 航空航天控制实验室
    + [代码开源](https://bitbucket.org/hridaybavle/semantic_slam/src/master/)，[视频](https://vimeo.com/368217703)
+ [x] **[14]** Liao Z, Wang W, Qi X, et al. [**Object-oriented SLAM using Quadrics and Symmetry Properties for Indoor Environments**](https://arxiv.org/ftp/arxiv/papers/2004/2004.05303.pdf)[J]. arXiv preprint arXiv:2004.05303, **2020**.
    + <font color = blue>**室内环境中使用二次曲面和对偶属性的面向物体的 SLAM**</font>
    + 北航；[代码开源](https://github.com/XunshanMan/Object-oriented-SLAM)，[视频](https://www.youtube.com/watch?v=u9zRBp4TPIs)
+ [x] **[15]** Ma Q M, Jiang G, Lai D Z. [**Robust Line Segments Matching via Graph Convolution Networks**](https://arxiv.org/pdf/2004.04993.pdf)[J]. arXiv preprint arXiv:2004.04993, **2020**.
    + <font color = blue>**图卷积神经网络线段匹配**</font>
    + 西安电子科大；[代码开源](https://github.com/mameng1/GraphLineMatching)
+ [ ] **[16]** Li R, Wang S, Gu D. [**DeepSLAM: A Robust Monocular SLAM System with Unsupervised Deep Learning**](https://ieeexplore.ieee.org/abstract/document/9047170/)[J]. IEEE Transactions on Industrial Electronics, **2020**.
    + <font color = blue>DeepSLAM：无监督深度学习的单目 SLAM</font>
    + 中国国家国防科技创新研究院，期刊：中科院一区，JCR Q1，IF 8.4
    + ICRA 2018 无监督单目 VO：[Undeepvo: Monocular visual odometry through unsupervised deep learning](https://arxiv.org/pdf/1709.06841)
    + Cognitive Computation 2018 SLAM 从几何到深度学习：挑战与机遇：[Ongoing evolution of visual SLAM from geometry to deep learning: challenges and opportunities](https://www.researchgate.net/profile/Ruihao_Li4/publication/327531951_Ongoing_Evolution_of_Visual_SLAM_from_Geometry_to_Deep_Learning_Challenges_and_Opportunities/links/5c8650db92851c1d5e156d7f/Ongoing-Evolution-of-Visual-SLAM-from-Geometry-to-Deep-Learning-Challenges-and-Opportunities.pdf)

---

#### 4. AR/VR/MR

+ [ ] **[17]** Baker L, Ventura J, Zollmann S, et al. [**SPLAT: Spherical Localization and Tracking in Large Spaces**](http://www.jventura.net/sites/default/files/lbaker_vr20b.pdf)[J].**2020**.
    + <font color = blue>SPLAT：大场景中球形定位与跟踪</font>
    + 新西兰奥塔哥大学
+ [ ] **[18]** Valentini I, Ballestin G, Bassano C, et al. [**Improving Obstacle Awareness to Enhance Interaction in Virtual Reality**](https://conferences.computer.org/vr-tvcg/2020/pdfs/VR2020-2f8MzUJjtCXG6Ue9RYFSN2/560800a044/560800a044.pdf)[C]. IEEE Conference on Virtual Reality and 3D User Interfaces (VR). **2020**.
    + <font color = blue>增强障碍意识以提升虚拟现实中的互动</font>
    + 意大利热那亚大学；[video](https://www.youtube.com/watch?v=dPJ9rSK_p3I&feature=youtu.be)
+ [ ] **[19]** Stylianidis E, Valari E, Pagani A, et al. [**Augmented Reality Geovisualisation for Underground Utilities**](https://link.springer.com/content/pdf/10.1007/s41064-020-00108-x.pdf)[J]. **2020**.
    + <font color = blue>增强现实地理可视化</font>
    + 希腊亚里士多德大学

---

#### 5. Others

+ [ ] **[20]** Sengupta S, Jayaram V, Curless B, et al. [**Background Matting: The World is Your Green Screen**](https://arxiv.org/pdf/2004.00626.pdf)[J]. arXiv preprint arXiv:2004.00626, **2020**.
    + <font color = blue>背景抠图</font>
    + 华盛顿大学；[**代码开源**](https://github.com/senguptaumd/Background-Matting)
+ [ ] **[21]** Wang L, Wei H. [**Avoiding non-Manhattan obstacles based on projection of spatial corners in indoor environment**](https://ieeexplore.ieee.org/abstract/document/9049452/)[J]. IEEE/CAA Journal of Automatica Sinica, **2020**.
    + <font color = blue>室内环境中基于空间角投影避免非曼哈顿障碍物</font>
    + 北大、上海理工、复旦；期刊：自动化学报英文版
+ [ ] **[22]** Spencer J, Bowden R, Hadfield S. [**Same Features, Different Day: Weakly Supervised Feature Learning for Seasonal Invariance**](https://arxiv.org/pdf/2003.13431)[J]. arXiv preprint arXiv:2003.13431, **2020**.
    + <font color = blue>不同时间的相同特征：季节性不变的弱监督特征学习</font>
    + 英国萨里大学；[**代码开源**](https://github.com/jspenmar/DejaVu_Features)（还未放出）

--- 

### 2020 年 3 月论文更新（23 篇）
> **本期 23 篇论文，其中 7 项开源工作；     
1、2 多相机 SLAM 系统       
9、10 VIO        
21、22 3D 目标检测        
12-19 八篇跟 semantic/deep learning 有关，趋势？        
注：没有特意整理 CVPR，ICRA 新的论文，大部分都半年前就有预印版了，在这个仓库里基本上也早收录了        
2020 年 3 月 29 日更新**
        
#### 1. Geometric SLAM

+ [ ] **[1]** Kuo J, Muglikar M, Zhang Z, et al. [**Redesigning SLAM for Arbitrary Multi-Camera Systems**](https://arxiv.org/pdf/2003.02014.pdf)[C]. ICRA **2020**.
    + <font color = blue>任意多相机 SLAM 系统</font>
    + 苏黎世大学、苏黎世联邦理工 [机器人与感知课题组](http://rpg.ifi.uzh.ch/research_vo.html)；[演示视频](https://www.youtube.com/watch?v=JGL4H93BiNw&feature=youtu.be)
+ [ ] **[2]** Won C, Seok H, Cui Z, et al. [**OmniSLAM: Omnidirectional Localization and Dense Mapping for Wide-baseline Multi-camera Systems**](https://arxiv.org/pdf/2003.08056.pdf)[J]. arXiv preprint arXiv:2003.08056, **2020**.
    + <font color = blue>**OmniSLAM：宽基线和多相机的全向定位和建图**</font>
    + 韩国汉阳大学计算机科学系
+ [ ] **[3]** Colosi M, Aloise I, Guadagnino T, et al. [**Plug-and-Play SLAM: A Unified SLAM Architecture for Modularity and Ease of Use**](https://arxiv.org/pdf/2003.00754.pdf)[J]. arXiv preprint arXiv:2003.00754, **2020**.
    + <font color = blue>**即插即用型 SLAM：模块化且易用的 SLAM 统一框架**</font>
    + 意大利罗马萨皮恩扎大学；[**代码开源**](https://github.com/srrg-sapienza/srrg2_slam_interfaces)
    + 作者之前一篇类似的文章，教你怎么模块化一个 SLAM 系统：
        + Schlegel D, Colosi M, Grisetti G. [**Proslam: Graph SLAM from a programmer's perspective**](https://arxiv.org/pdf/1709.04377.pdf)[C]//2018 IEEE International Conference on Robotics and Automation (**ICRA**). IEEE, **2018**: 1-9.
        + [代码开源](https://gitlab.com/srrg-software/srrg_proslam)
+ [ ] **[4]** Wu X, Vela P, Pradalier C. [**Robust Monocular Edge Visual Odometry through Coarse-to-Fine Data Association**](https://www.researchgate.net/profile/Xiaolong_Wu5/publication/336056167_Robust_Monocular_Edge_Visual_Odometry_through_Coarse-to-Fine_Data_Association/links/5e700cc4458515eb5aba76fd/Robust-Monocular-Edge-Visual-Odometry-through-Coarse-to-Fine-Data-Association.pdf)[J].**2020**.
    + <font color = blue>通过从粗到细的数据关联实现鲁棒的单目基于边的视觉里程计</font>
    + 佐治亚理工学院
+ [ ] **[5]** Rosinol A, Gupta A, Abate M, et al. [**3D Dynamic Scene Graphs: Actionable Spatial Perception with Places, Objects, and Humans**]()[J]. arXiv preprint arXiv:2002.06289, **2020**.
    + <font color = blue>3D 动态场景图：具有位置，物体和人的可操作空间感知</font>
    + MIT；[Kimera](https://github.com/MIT-SPARK/Kimera-Semantics) 的作者；[演示视频](https://www.youtube.com/watch?v=SWbofjhyPzI&feature=youtu.be)；[Google Scholar](https://scholar.google.com/citations?user=aFGYNYgAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[6]** Zeng T, Li X, Si B. [**StereoNeuroBayesSLAM: A Neurobiologically Inspired Stereo Visual SLAM System Based on Direct Sparse Method**]()[J]. arXiv preprint arXiv:2003.03091, **2020**.
    + <font color = blue>类脑双目直接稀疏 SLAM</font>
    + 沈自所斯老师
+ [x] **[7]** Oleynikova H, Taylor Z, Siegwart R, et al. [**Sparse 3d topological graphs for micro-aerial vehicle planning**](https://arxiv.org/pdf/1803.04345.pdf)[C]//2018 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, **2018**: 1-9.
    + <font color = blue>**微型飞行器路径规划的稀疏 3D 拓扑图**</font>
    + 苏黎世联邦理工；[作者主页](http://helenol.github.io/)；路径规划与建图部分[代码开源](https://github.com/ethz-asl/voxblox)，相关论文：
        + Oleynikova H, Taylor Z, Fehr M, et al. [**Voxblox: Incremental 3d euclidean signed distance fields for on-board mav planning**](https://arxiv.org/pdf/1611.03631)[C]//2017 Ieee/rsj International Conference on Intelligent Robots and Systems (iros). IEEE, **2017**: 1366-1373.
+ [ ] **[8]** Ye H, Huang H, Liu M. [**Monocular Direct Sparse Localization in a Prior 3D Surfel Map**](https://arxiv.org/pdf/2002.09923.pdf)[J]. arXiv preprint arXiv:2002.09923, **2020**.
    + <font color = blue>在 Surfel 地图中的单目稀疏直接法定位</font>
    + [港科大 RAM 实验室](https://ram-lab.com/)
    + Tips：构造稀疏点的全局平面信息
    
---

#### 2. 传感器融合

+ [ ] **[9]** Zhao Y, Smith J S, Karumanchi S H, et al. [**Closed-Loop Benchmarking of Stereo Visual-Inertial SLAM Systems: Understanding the Impact of Drift and Latency on Tracking Accuracy**](https://arxiv.org/pdf/2003.01317.pdf)[C].  **ICRA 2020**.
    + <font color = blue>双目视觉里程计闭环检测基准系统：关于测试漂移和延迟对跟踪准确性的影响</font>
    + 佐治亚理工学院 IVALab [ROBO SLAM](https://ivalab.github.io/RoboSLAM/public/research/)；[**代码开源**](https://github.com/ivalab/meta_ClosedLoopBench)；[作者主页](https://sites.google.com/site/zhaoyipu/)
+ [ ] **[10]** Giubilato R, Chiodini S, Pertile M, et al. [**MiniVO: Minimalistic Range Enhanced Monocular System for Scale Correct Pose Estimation**]()[J]. **2020**.
    + <font color = blue>用于正确尺度位姿估计的最小范围增强单目视觉里程计</font>
    + 意大利帕多瓦大学
    + Tips：1D LiDAR 矫正单目尺度
+ [ ] **[11]** Huang W, Liu H, Wan W. [**An Online Initialization and Self-Calibration Method for Stereo Visual-Inertial Odometry**](https://www.researchgate.net/profile/Weibo_Huang2/publication/339394318_An_Online_Initialization_and_Self-Calibration_Method_for_Stereo_Visual-Inertial_Odometry/links/5e58b0b2299bf1bdb840bd59/An-Online-Initialization-and-Self-Calibration-Method-for-Stereo-Visual-Inertial-Odometry.pdf)[J]. IEEE Transactions on Robotics, **2020**.
    + <font color = blue>一种双目视惯里程计的在线初始化和自标定方法</font>
    + 北京大学；[Google Scholar](https://scholar.google.com/citations?user=d72ju6AAAAAJ&hl=zh-CN&authuser=1&oi=sra)；作者另外一篇文章：
        + Huang W, Liu H. [**Online initialization and automatic camera-IMU extrinsic calibration for monocular visual-inertial SLAM**](http://robotics.pkusz.edu.cn/static/papers/ICRA2018-huangweibo.pdf)[C]//2018 IEEE International Conference on Robotics and Automation (**ICRA**). IEEE, **2018**: 5182-5189.

---

#### 3. Semantic/Deep SLAM

+ [ ] **[12]** Landgraf Z, Falck F, Bloesch M, et al. [**Comparing View-Based and Map-Based Semantic Labelling in Real-Time SLAM**](https://arxiv.org/pdf/2002.10342.pdf)[J]. arXiv preprint arXiv:2002.10342, **2020**.
    + <font color = blue>在实时 SLAM 中比较基于视图和基于地图的语义标签</font>
    + 帝国理工学院计算机系戴森机器人实验室
+ [ ] **[13]** Singh G, Wu M, Lam S K. [**Fusing Semantics and Motion State Detection for Robust Visual SLAM**](http://openaccess.thecvf.com/content_WACV_2020/papers/Singh_Fusing_Semantics_and_Motion_State_Detection_for_Robust_Visual_SLAM_WACV_2020_paper.pdf)[C]//The IEEE Winter Conference on Applications of Computer Vision. **2020**: 2764-2773.
    + <font color = blue>融合语义和运动状态检测以实现鲁棒的视觉 SLAM</font>
    + 南洋理工大学
+ [ ] **[14]** Gupta A, Iyer G, Kodgule S. [**DeepEvent-VO: Fusing Intensity Images and Event Streams for End-to-End Visual Odometry**](https://epiception.github.io/assets/Projects/deep_event_vo.pdf)[J].
    + <font color = blue>DeepEvent-VO：融合强度图像和事件流的端到端视觉测距</font>
    + CMU；[**代码开源**](https://github.com/SuhitK/DeepEvent-VO)
+ [ ] **[15]** Wagstaff B, Peretroukhin V, Kelly J. [**Self-Supervised Deep Pose Corrections for Robust Visual Odometry**](https://arxiv.org/pdf/2002.12339.pdf)[J]. arXiv preprint arXiv:2002.12339, **2020**.
    + <font color = blue>鲁棒视觉里程计的自监督深度位姿矫正</font>
    + 多伦多大学 STARS 实验室；[**代码开源**](https://github.com/utiasSTARS/ss-dpc-net)
+ [ ] **[16]** Ye X, Ji X, Sun B, et al. [**DRM-SLAM: Towards dense reconstruction of monocular SLAM with scene depth fusion**](https://www.sciencedirect.com/science/article/abs/pii/S0925231220302344)[J]. Neurocomputing, 2020.
    + <font color = blue>DRM-SLAM：通过场景深度融合实现单目 SLAM 的稠密重建</font>
    + 大连理工大学；期刊：中科院二区，JCR Q1，IF 3.824
+ [ ] **[17]** Yang N, von Stumberg L, Wang R, et al. [**D3VO: Deep Depth, Deep Pose and Deep Uncertainty for Monocular Visual Odometry**](https://arxiv.org/pdf/2003.01060.pdf)[C]. CVPR **2020**.
    + <font color = blue>D3VO：单目视觉里程计中针对深度、位姿和不确定性的深度网络</font>
    + TUM 计算机视觉组；[个人主页](https://vision.in.tum.de/members/wangr)
+ [ ] **[18]** Chen C, Rosa S, Miao Y, et al. [**Selective sensor fusion for neural visual-inertial odometry**](http://openaccess.thecvf.com/content_CVPR_2019/papers/Chen_Selective_Sensor_Fusion_for_Neural_Visual-Inertial_Odometry_CVPR_2019_paper.pdf)[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. **2019**: 10542-10551.
    + <font color = blue>神经视觉 VIO 的选择性传感器融合</font>
    + 牛津大学计算机科学系；[Google Scholar](https://scholar.google.com/citations?user=OqlY-98AAAAJ&hl=zh-CN&authuser=1&oi=sra)
+ [ ] **[19]** Towards the Probabilistic [**Fusion of Learned Priors into Standard Pipelines for 3D Reconstruction**](https://www.doc.ic.ac.uk/~sleutene/publications/Laidlow_ICRA2020_CameraReady.pdf)[C]. ICRA **2020**.
    + <font color = blue>将学习的先验信息融合到标准的三维重建中</font>
    + [帝国理工学院戴森机器人实验室](https://www.imperial.ac.uk/dyson-robotics-lab/publications/)

---

#### 4. AR/VR/MR

+ [ ] **[20]** Wu L, Wan W, Yu X, et al. [**A novel augmented reality framework based on monocular semi‐dense simultaneous localization and mapping**](https://onlinelibrary.wiley.com/doi/pdf/10.1002/cav.1922?casa_token=1GWiXGz2GzIAAAAA:1vDJn5Dx97ruaTSTthXoUpfBDRPe4rjvRl5UsTbRSbgvzU3YrXin54Al_jQWLdhwDm-TCm7HF-92cA)[J]. Computer Animation and Virtual Worlds, **2020**: e1922.
    + <font color = blue>**基于单目半稠密 SLAM 的新型 AR 框架**</font>
    + 上海大学；期刊：中科院四区，JCR Q4，IF 0.794
    
---

#### 5. Others

+ [x] **[21]** Shi W. [**Point-GNN: Graph Neural Network for 3D Object Detection in a Point Cloud**]()[C]. **CVPR 2020**.
    + <font color = blue>**Point-GNN: 图神经网络用于点云中的 3D 目标对象检测**</font>
    + CMU； [**代码开源**](https://github.com/WeijingShi/Point-GNN)；[谷歌学术](https://scholar.google.com/citations?user=K7AoP_wAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[22]** Chen Y, Tai L, Sun K, et al. [**MonoPair: Monocular 3D Object Detection Using Pairwise Spatial Relationships**](https://arxiv.org/pdf/2003.00504.pdf)[C]. **CVPR 2020**.
    + <font color = blue>MonoPair: 使用成对空间关系的单目 3D 对象检测</font>
    + 阿里巴巴
+ [ ] **[23]** Chen X, Song J, Hilliges O. [**Monocular neural image based rendering with continuous view control**](http://openaccess.thecvf.com/content_ICCV_2019/papers/Chen_Monocular_Neural_Image_Based_Rendering_With_Continuous_View_Control_ICCV_2019_paper.pdf)[C]//Proceedings of the IEEE International Conference on Computer Vision. **2019**: 4090-4100.
    + <font color = blue>基于连续视图控制的单目神经图像绘制</font>
    + [苏黎世联邦理工 AIT 实验室](https://ait.ethz.ch/)
    + 类似于百度自动驾驶仿真 AADS 采用的新视图合成？

---

### 2020 年 2 月论文更新（17 篇）
> **这个月赶论文，看的论文比较少，本期 17 篇，其中 3 项开源工作；     
1、2、3、4 建图相关        
7、8、9 动态相关        
10、11 视惯融合        
13、14、15 AR相关        
2020 年 2 月 25 日更新**
        
#### 1. Geometric SLAM

+ [x] **[1]** Muglikar M, Zhang Z, Scaramuzza D. [**Voxel map for visual slam**](https://arxiv.org/pdf/2003.02247.pdf)[C]. ICRA **2020**.
    + <font color = blue>**使用体素图的视觉 SLAM**</font>
    + 苏黎世大学，张子潮
+ [ ] **[2]** Ye X, Ji X, Sun B, et al. [**DRM-SLAM: Towards Dense Reconstruction of Monocular SLAM with Scene Depth Fusion**](https://www.sciencedirect.com/science/article/pii/S0925231220302344)[J]. Neurocomputing, **2020**.
    + <font color = blue>通过场景深度融合实现单目 SLAM 的稠密重建</font>
    + 大连理工大学，期刊：中科院二区， IF 4.0
+ [x] **[3]** Nardi F, Grisetti G, Nardi D. [**High-Level Environment Representations for Mobile Robots**](https://iris.uniroma1.it/retrieve/handle/11573/1222797/982918/Tesi_dottorato_Nardi.pdf). **2019**.
    + <font color = blue>**移动机器人高级别的环境表示**</font>
    + 罗马大学博士学位论文
+ [ ] **[4]** Puligilla S S, Tourani S, Vaidya T, et al. [**Topological Mapping for Manhattan-like Repetitive Environments**](https://arxiv.org/pdf/2002.06575.pdf)[J]. arXiv preprint arXiv:2002.06575, **2020**.
    + <font color = blue>类曼哈顿重复环境中的拓扑建图</font>
    + 印度海得拉巴国际信息技术研究所；[代码开源](https://github.com/Shubodh/ICRA2020)；[演示视频](https://www.youtube.com/watch?v=swYcwrjprh0)
+ [ ] **[5]** Li X, Ling H. [**Hybrid Camera Pose Estimation with Online Partitioning for SLAM**](https://www3.cs.stonybrook.edu/~hling/publication/slam-icra20.pdf)[J]. IEEE Robotics and Automation Letters, **2020**, 5(2): 1453-1460.
    + <font color = blue>在线分割 SLAM 中的混合相机位姿估计</font>
    + 天普大学，林海滨教授
+ [ ] **[6]** Karimian A, Yang Z, Tron R. [**Statistical Outlier Identification in Multi-robot Visual SLAM using Expectation Maximization**](https://arxiv.org/pdf/2002.02638.pdf)[J]. arXiv preprint arXiv:2002.02638, **2020**.
    + <font color = blue>使用最大期望识别多机器人 VSLAM 中的异常值</font>
    + 波士顿大学
+ [x] **[7]** Henein M, Zhang J, Mahony R, et al. [**Dynamic SLAM: The Need For Speed**](https://arxiv.org/pdf/2002.08584.pdf)[J]. arXiv preprint arXiv:2002.08584, **2020**.
    + <font color = blue>**满足速度估计需求的动态 SLAM**</font>
    + 澳大利亚国立大学，作者主要研究动态 SLAM [**Google Scholar**](https://scholar.google.com/citations?user=PUBFzCAAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[8]** Nair G B, Daga S, Sajnani R, et al. [**Multi-object Monocular SLAM for Dynamic Environments**](https://arxiv.org/pdf/2002.03528.pdf)[J]. arXiv preprint arXiv:2002.03528, **2020**.
    + <font color = blue>用于动态环境的多目标单目 SLAM</font>
    + 印度海得拉巴理工学院
+ [ ] **[9]** Cheng J, Zhang H, Meng M Q H. [**Improving Visual Localization Accuracy in Dynamic Environments Based on Dynamic Region Removal**](https://ieeexplore.ieee.org/abstract/document/8972551/)[J]. IEEE Transactions on Automation Science and Engineering, **2020**.
    + <font color = blue>通过动态区域剔除来提升动态环境中视觉定位的准确性</font>
    + 港中文；中科院二区 JCR Q1

---

#### 2. 传感器融合

+ [ ] **[10]** Patel N, Khorrami F, Krishnamurthy P, et al. [**Tightly Coupled Semantic RGB-D Inertial Odometry for Accurate Long-Term Localization and Mapping**](https://ieeexplore.ieee.org/abstract/document/8981658/)[C]//2019 19th International Conference on Advanced Robotics (**ICAR**). IEEE, **2019**: 523-528.
    + <font color = blue>用于精确、长期定位和建图的紧耦合语义 RGB-D 惯性里程计</font>
    + 纽约大学
+ [ ] **[11]** Chiodini S, Giubilato R, Pertile M, et al. [**Retrieving Scale on Monocular Visual Odometry Using Low Resolution Range Sensors**](https://ieeexplore.ieee.org/abstract/document/8950136/)[J]. IEEE Transactions on Instrumentation and Measurement, **2020**.
    + <font color = blue>使用低分辨率距离传感器恢复单目视觉里程计的尺度</font>
    + 意大利帕多瓦大学，期刊：中科院三区 JCR Q1Q2

---

#### 3. Semantic/Deep SLAM

+ [ ] **[12]** Jin S, Chen L, Sun R, et al. [**A novel vSLAM framework with unsupervised semantic segmentation based on adversarial transfer learning**](https://www.sciencedirect.com/science/article/pii/S1568494620300934)[J]. Applied Soft Computing, **2020**: 106153.
    + <font color = blue>基于对抗迁移学习的无监督语义分割的新型 vSLAM 框架</font>
    + 苏州大学，期刊：中科院二区 JCR Q1

---

#### 4. AR/VR/MR

+ [x] **[13]** Liu R, Zhang J, Chen S, et al. [**Towards SLAM-based outdoor localization using poor GPS and 2.5 D building models**]()[C]//2019 IEEE International Symposium on Mixed and Augmented Reality (ISMAR). IEEE, **2019**: 1-7.
    + <font color = blue>**使用粗糙的 GPS 和 2.5 D 建筑模型实现基于 SLAM 的户外定位**</font>
    + 浙江工业大学； [代码开源](https://github.com/luyujiangmiao/Buiding-GPS-SLAM)
+ [x] **[14]** Miyamoto K, Shiraga T, Okato Y. [**User-Selected Object Data Augmentation for 6DOF CNN Localization**](https://pdfs.semanticscholar.org/1ddc/9ba1668db506717fbe180ae63152917d174f.pdf)[J].
    + <font color = blue>**6 自由度 CNN 定位的用户选择目标数据增强**</font>
+ [x] **[15]** Gui Z W. [**Register Based on Large Scene for Augmented Reality System**](https://jit.ndhu.edu.tw/article/view/2226)[J]. Journal of Internet Technology, **2020**, 21(1): 99-111.
    + <font color = blue>基于大场景的增强现实三维注册</font>
    + 北理工，期刊：中科院四区， IF 0.7

---

#### 5. Others

+ [x] **[16]** Gao G, Lauri M, Wang Y, et al. [**6D Object Pose Regression via Supervised Learning on Point Clouds**](https://arxiv.org/pdf/2001.08942.pdf)[C]. ICRA 2020.
    + <font color = blue>**通过点云上的监督学习进行 6D 物体位姿回归**</font>
    + 德国汉堡大学、清华大学； [代码开源](https://github.com/GeeeG/CloudPose)； [演示视频](https://www.youtube.com/watch?v=OhNMngzxFDQ)
+ [x] **[17]** Habib R, Saii M. [**Object Pose Estimation in Monocular Image Using Modified FDCM**](https://journals.agh.edu.pl/csci/article/view/3426)[J]. Computer Science, **2020**, 21(1).
    + <font color = blue>使用改进的 FDCM 估计单目图像中的物体位置</font>
    + 类似于旋转物体检验？
    
---

### 2020 年 1 月论文更新（26 篇）
> **本期 26 篇论文，其中 7 项开源工作，1 项开放数据集；     
5、6、10 关于线段的 SLAM        
7 基于事件相机的 SLAM 综述        
8、9、10 视惯融合        
16、17 AR+SLAM        
2020 年 1 月 28 日更新**

#### 1. Geometric SLAM

+ [ ] **[1]** RÜCKERT, Darius; INNMANN, Matthias; STAMMINGER, Marc. [**FragmentFusion: A Light-Weight SLAM Pipeline for Dense Reconstruction**](https://ieeexplore.ieee.org/abstract/document/8951922/). In: 2019 IEEE International Symposium on Mixed and Augmented Reality Adjunct (ISMAR-Adjunct). IEEE, **2019**. p. 342-347.
    + <font color = blue>FragmentFusion：一种轻量级的用于稠密重建的方案</font>
    + 德国埃朗根-纽伦堡大学
+ [x] **[2]** Chen Y, Shen S, Chen Y, et al. [**Graph-Based Parallel Large Scale Structure from Motion**](https://arxiv.org/pdf/1912.10659.pdf)[J]. arXiv preprint arXiv:1912.10659, **2019**.
    + <font color = blue>基于图的并行大尺度的 SFM</font>
    + 中科院自动化所，[**代码开源**](https://github.com/AIBluefisher/GraphSfM)
+ [x] **[3]** Sommer C, Sun Y, Guibas L, et al. [**From Planes to Corners: Multi-Purpose Primitive Detection in Unorganized 3D Point Clouds**](https://arxiv.org/pdf/2001.07360.pdf)[J]. arXiv preprint arXiv:2001.07360, **2020**.
    + <font color = blue>**从平面到角点：无组织的点云中的多用途基本体检测**</font>
    + 慕尼黑工业大学，[代码开源](https://github.com/c-sommer/orthogonal-planes)
+ [x] **[4]** Zhao Y, Vela P A. [**Good feature matching: Towards accurate, robust VO/VSLAM with low latency**](https://arxiv.xilesou.top/pdf/2001.00714.pdf)[J]. IEEE Transactions on Robotics, **2019**, 7: 181800-181811.
    + <font color = blue>良好的特征匹配：面向低延迟、准确且鲁棒的 VO / VSLAM</font>
    + 佐治亚理工学院，[作者主页](https://sites.google.com/site/zhaoyipu/home?authuser=0)，[**代码开源**](https://github.com/ivalab/FullResults_GoodFeature)，期刊中科院二区  JCR Q1
+ [ ] **[5]** Luo X, Tan Z, Ding Y. [**Accurate Line Reconstruction for Point and Line-Based Stereo Visual Odometry**](https://ieeexplore.ieee.org/abstract/document/8936964/)[J]. IEEE Access, **2019**, 7: 185108-185120.
    + <font color = blue>基于双目点线视觉里程计的精确线段重构</font>
    + 浙江大学超大规模集成电路设计研究院，IEEE Access 开源期刊
+ [ ] **[6]** Ma J, Wang X, He Y, et al. [**Line-Based Stereo SLAM by Junction Matching and Vanishing Point Alignment**](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8935194)[J]. IEEE Access, **2019**, 7: 181800-181811.
    + <font color = blue>通过节点匹配与消失点对齐的基于线的双目 SLAM</font>
    + 武汉大学、中科院自动化所，IEEE Access 开源期刊
+ [ ] **[7]** 马艳阳, 叶梓豪, 刘坤华, 等. [**基于事件相机的定位与建图算法: 综述**](http://www.aas.net.cn/cn/article/doi/10.16383/j.aas.c190550)[J]. 自动化学报, **2020**, 46: 1-11.
    + 中山大学

#### 2. 传感器融合

+ [x] **[8]** WEN, Shuhuan, et al. [**Joint optimization based on direct sparse stereo visual-inertial odometry**](https://link.springer.com/article/10.1007/s10514-019-09897-6). Autonomous Robots, **2020**, 1-19.
    + <font color = blue>基于直接稀疏双目视觉惯导里程计的联合优化</font>
+ [x] **[9]** Chen C, Zhu H, Wang L, et al. [**A Stereo Visual-Inertial SLAM Approach for Indoor Mobile Robots in Unknown Environments Without Occlusions**](https://ieeexplore.ieee.org/abstract/document/8937551/)[J]. IEEE Access, **2019**, 7: 185408-185421.
    + <font color = blue>无遮挡未知环境中室内移动机器人的双目视觉惯性 SLAM 方法</font>
    + 中国矿业大学，[**代码开源**](https://github.com/cumtxz/STCM-SLAM)（还未放出），IEEE Access 开源期刊
+ [x] **[10]** Yan D, Wu C, Wang W, et al. [**Invariant Cubature Kalman Filter for Monocular Visual Inertial Odometry with Line Features**](https://arxiv.org/ftp/arxiv/papers/1912/1912.11749.pdf)[J]. arXiv preprint arXiv:1912.11749, **2019**.
    + <font color = blue>单目线特征视觉惯性里程法的不变容积卡尔曼滤波</font>
    + 石家庄铁道大学、北京交通大学

#### 3. Semantic/Deep SLAM

+ [ ] **[11]** XU, Jingao, et al. [**Edge Assisted Mobile Semantic Visual SLAM**](http://tns.thss.tsinghua.edu.cn/~jingao/papers/infocom20_edgeSLAM.pdf).
    + <font color = blue>边缘辅助移动语义视觉SLAM</font>
    + 清华、大工、微软
+ [ ] **[12]** ZHAO, Zirui, et al. [**Visual Semantic SLAM with Landmarks for Large-Scale Outdoor Environment**](https://arxiv.org/pdf/2001.01028.pdf). arXiv preprint arXiv:2001.01028, **2020**.
    + <font color = blue>用于大规模室外环境的具有路标的视觉语义 SLAM</font>
    + 西安交大、北京交大
+ [x] **[13]** WANG, Li, et al. [**Object-Aware Hybrid Map for Indoor Robot Visual Semantic Navigation**](https://ieeexplore.ieee.org/abstract/document/8961495/). In: 2019 IEEE International Conference on Robotics and Biomimetics (**ROBIO**). IEEE, **2019**. p. 1166-1172.
    + <font color = blue>**用于室内机器人视觉语义导航的对象感知混合地图**</font>
    + 燕山大学、加拿大阿尔伯塔大学、伦敦大学；Autonomous Robots 期刊中科院三区，JCR Q1， IF 2.244
+ [ ] **[14]** Czarnowski, J., Laidlow, T., Clark, R., & Davison, A. J. (**2020**). [**DeepFactors: Real-Time Probabilistic Dense Monocular SLAM**](https://arxiv.org/pdf/2001.05049.pdf). IEEE Robotics and Automation Letters, 5(2), 721–728. doi:10.1109/lra.2020.2965415
    + <font color = blue>DeepFactors：实时的概率单目稠密 SLAM</font>
    + 帝国理工学院戴森机器人实验室，[代码开源](https://github.com/jczarnowski/DeepFactors)
+ [ ] **[15]** TRIPATHI, Nivedita; SISTU, Ganesh; YOGAMANI, Senthil. [**Trained Trajectory based Automated Parking System using Visual SLAM**](https://arxiv.org/pdf/2001.02161.pdf). arXiv preprint arXiv:2001.02161, **2020**.
    + <font color = blue>使用视觉 SLAM 基于轨迹训练的自动停车系统</font>
    + 爱尔兰法雷奥视觉系统公司

#### 4. AR/VR/MR

+ [ ] **[16]** WANG, Cheng, et al. [**NEAR: The NetEase AR Oriented Visual Inertial Dataset**](https://ieeexplore.ieee.org/abstract/document/8951909). In: 2019 IEEE International Symposium on Mixed and Augmented Reality Adjunct (ISMAR-Adjunct). IEEE, **2019**. p. 366-371.
    + <font color = blue>**面向视觉惯导数据集的网易 AR**</font>
    + 网易，[**数据集地址**](https://github.com/EZXR-Research/NEAR-VI-Dataset)
+ [ ] **[17]** HUANG, Ningsheng; CHEN, Jing; MIAO, Yuandong. [**Optimization for RGB-D SLAM Based on Plane Geometrical Constraint**](https://ieeexplore.ieee.org/abstract/document/8952003/). In: 2019 IEEE International Symposium on Mixed and Augmented Reality Adjunct (ISMAR-Adjunct). IEEE, **2019**. p. 326-331.
    + <font color = blue>**基于平面几何约束优化的 RGB-D SLAM**</font>
    + 北理工
+ [ ] **[18]** WU, Yi-Chin; CHAN, Liwei; LIN, Wen-Chieh. [**Tangible and Visible 3D Object Reconstruction in Augmented Reality**](https://ieeexplore.ieee.org/abstract/document/8943645/). In: 2019 IEEE International Symposium on Mixed and Augmented Reality (ISMAR). IEEE, **2019**. p. 26-36.
    + <font color = blue>增强现实中有形且可见的三维物体重建</font>
    + 台湾国立交通大学计算机科学系
+ [ ] **[19]** FEIGL, Tobias, et al. [**Localization Limitations of ARCore, ARKit, and Hololens in Dynamic Large-Scale Industry Environments**](https://www2.cs.fau.de/publication/download/GRAPP2020.pdf).
    + <font color = blue>大型工业动态环境中 ARCore，ARKit 和 Hololens 的定位局限性</font>
    + 德国弗里德里希-亚历山大大学
+ [ ] **[20]** Yang X, Yang J, He H, et al. [**A Hybrid 3D Registration Method of Augmented Reality for Intelligent Manufacturing**](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8933068)[J]. IEEE Access, **2019**, 7: 181867-181883.
    + <font color = blue>用于智能制造的增强现实混合三维注册方法</font>
    + 广东工业大学，开源期刊
    
#### 5. Others

+ [x] **[21]** Speciale P. [**Novel Geometric Constraints for 3D Computer Vision Applications**](https://www.research-collection.ethz.ch/handle/20.500.11850/380042)[D]. ETH Zurich, **2019**.
    + <font color = blue>**适用于 3D 计算机视觉应用的新型几何约束**</font>
    + 苏黎世联邦理工博士学位论文、微软，[Google Scholar](https://scholar.google.com/citations?user=-LEhIh0AAAAJ&hl=zh-CN&oi=sra)
+ [x] **[22]** Patil V, Van Gansbeke W, Dai D, et al. [**Don't Forget The Past: Recurrent Depth Estimation from Monocular Video**](https://arxiv.org/pdf/2001.02613.pdf)[J]. arXiv preprint arXiv:2001.02613, **2020**.
    + <font color = blue>不要忘记过去的信息:从单目视频中的重复深度估计</font>
    + 苏黎世联邦理工，[**代码开源**](https://github.com/wvangansbeke/Recurrent-Depth-Estimation/branches)（还未放出）
+ [x] **[23]** CHIU, Hsu-kuang, et al. [**Probabilistic 3D Multi-Object Tracking for Autonomous Driving**](https://arxiv.org/pdf/2001.05673.pdf). arXiv preprint arXiv:2001.05673, **2020**.
    + <font color = blue>用于自动驾驶的概率 3D 多目标跟踪</font>
    + 斯坦福大学、丰田研究所，[**代码开源**](https://github.com/eddyhkchiu/mahalanobis_3d_multi_object_tracking)
+ [x] **[24]** ZHOU, Boyu, et al. [**Robust Real-time UAV Replanning Using Guided Gradient-based Optimization and Topological Paths**](https://arxiv.org/pdf/1912.12644.pdf). arXiv preprint arXiv:1912.12644, **2019**.
    + <font color = blue>使用基于梯度优化和拓扑路径引导进行鲁棒且实时的无人机重规划</font>
    + 港科大，代码开源：[Fast-Planner](https://github.com/HKUST-Aerial-Robotics/Fast-Planner), [
TopoTraj](https://github.com/HKUST-Aerial-Robotics/TopoTraj)
+ [x] **[25]** [**Object-based localization**](https://patents.google.com/patent/US20190392212A1/en)，**2019**.
    + <font color = blue>专利：基于物体的定位</font>
+ [x] **[26]** [**Device pose estimation using 3d line clouds**](https://patents.google.com/patent/US20200005486A1/en)，**2019**.
    + <font color = blue>专利：使用 3D 线云的设备位姿估计</font>

---

### 2019 年 12 月论文更新（23 篇）
> **本期 23 篇论文，其中 5 项开源工作；     
比较有意思的有 TextSLAM、VersaVIS 和单目 3D 目标检测。**

#### 1. Geometric SLAM

+ [x] **[1]** Tanke J, Kwon O H, Stotko P, et al. [**Bonn Activity Maps: Dataset Description**](https://arxiv.org/pdf/1912.06354.pdf)[J]. arXiv preprint arXiv:1912.06354, **2019**.
    + <font color = blue>**包含人体跟踪、姿态和环境语义三维重建的数据集**</font>
    + 波恩大学，[项目、数据集主页](https://github.com/bonn-activity-maps/bonn_activity_maps)
+ [x] **[2]** An S, Che G, Zhou F, et al. [**Fast and Incremental Loop Closure Detection Using Proximity Graphs**](https://arxiv.org/pdf/1911.10752.pdf)[J]. arXiv preprint arXiv:1911.10752, **2019**.
    + <font color = blue>**使用邻近图的快速增量式闭环检测**</font>
    + 京东、北航，[代码开源](https://github.com/AnshanTJU/FILD)
+ [x] **[3]** Li B, Zou D, Sartori D, et al. [**TextSLAM: Visual SLAM with Planar Text Features**](https://arxiv.org/pdf/1912.05002.pdf)[J]. arXiv preprint arXiv:1912.05002, 2019.
    + <font color = blue>**TextSLAM：基于平面文本的视觉 SLAM**</font>
    + 上交邹丹平老师
+ [x] **[4]** [Bundle Adjustment Revisited](https://arxiv.org/pdf/1912.03858.pdf)
    + <font color = blue>**再谈 BA**</font>
    + 北京大学
+ [ ] **[5]** Lange M, Raisch C, Schilling A. [LVO: Line only stereo Visual Odometry](https://ieeexplore.ieee.org/abstract/document/8911808)[C]//2019 International Conference on Indoor Positioning and Indoor Navigation (IPIN). IEEE, 1-8.
    + <font color = blue>双目线 VO</font>
    + 图宾根大学
    + 相关论文：Vakhitov A, Lempitsky V. [**Learnable Line Segment Descriptor for Visual SLAM**](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8651490)[J]. IEEE Access, 2019, 7: 39923-39934. [代码开源](https://github.com/alexandervakhitov/lld-slam)
+ [ ] **[6]** Liu W, Mo Y, Jiao J. [**An efficient edge-feature constraint visual SLAM**](https://dl.acm.org/citation.cfm?id=3371455)[C]//Proceedings of the International Conference on Artificial Intelligence, Information Processing and Cloud Computing. ACM, **2019**: 13.
    + <font color = blue>一种高效的基于边缘特征约束的视觉 SLAM</font>
    + 北邮
+ [ ] **[7]** Pan L, Wang P, Cao J, et al. [**Dense RGB-D SLAM with Planes Detection and Mapping**](https://ieeexplore.ieee.org/abstract/document/8927657)[C]//IECON 2019-45th Annual Conference of the IEEE Industrial Electronics Society. IEEE, **2019**, 1: 5192-5197.
    + <font color = blue>使用平面检测与建图的稠密 RGB-D SLAM</font>
    + 新加坡国立大学
+ [ ] **[8]** Ji S, Qin Z, Shan J, et al. [**Panoramic SLAM from a multiple fisheye camera rig**](https://www.sciencedirect.com/science/article/pii/S0924271619302758)[J]. ISPRS Journal of Photogrammetry and Remote Sensing, **2020**, 159: 169-183.
    + <font color = blue>多鱼眼相机的全景 SLAM</font>
    + 武汉大学
+ [ ] **[9]** Lecrosnier L, Boutteau R, Vasseur P, et al. [**Vision based vehicle relocalization in 3D line-feature map using Perspective-n-Line with a known vertical direction**]()[C]//2019 IEEE Intelligent Transportation Systems Conference (ITSC). IEEE, **2019**: 1263-1269.
    + <font color = blue>使用具有已知垂直方向的透视线在 3D 线特征图中进行基于视觉的车辆重定位</font>
    + 诺曼底大学
+ [x] **[10]** de Souza Muñoz M E, Menezes M C, de Freitas E P, et al. [**A Parallel RatSlam C++ Library Implementation**](https://link.springer.com/chapter/10.1007/978-3-030-36636-0_13)[C]//Latin American Workshop on Computational Neuroscience. Springer, Cham, **2019**: 173-183.
    + <font color = blue>并行 Rat SLAM C++ 库的实现</font>
    
---

#### 2. 传感器融合

+ [x] **[11]** Tschopp F, Riner M, Fehr M, et al. [**VersaVIS: An Open Versatile Multi-Camera Visual-Inertial Sensor Suite**](https://arxiv.org/pdf/1912.02469.pdf)[J]. arXiv preprint arXiv:1912.02469, **2019**.
    + <font color = blue>**VersaVIS：开源多功能多相机的视觉惯性传感器套件**</font>
    + 苏黎世联邦理工学院，[**代码开源**](https://github.com/ethz-asl/versavis)
+ [x] **[12]** Geneva P, Eckenhoff K, Lee W, et al. [**Openvins: A research platform for visual-inertial estimation**](https://pdfs.semanticscholar.org/cb63/60f21255834297e32826bff6366a769b49e9.pdf)[C]//IROS 2019 Workshop on Visual-Inertial Navigation: Challenges and Applications, Macau, China. **IROS 2019**.
    + <font color = blue>**Openvins：用于视觉惯性估计的研究平台**</font>
    + 特拉华大学，[**代码开源**](https://github.com/rpng/open_vins)
+ [ ] **[13]** Barrau A, Bonnabel S. [**A Mathematical Framework for IMU Error Propagation with Applications to Preintegration**](https://hal-mines-paristech.archives-ouvertes.fr/hal-02394774/document)[J]. **2019**.
    + <font color = blue>IMU错误传播的数学框架及其在预积分中的应用</font>
    + PSL Research University
+ [ ] **[14]** Ke T, Wu K J, Roumeliotis S I. RISE-SLAM: A Resource-aware Inverse Schmidt Estimator for SLAM[C]. **IROS 2019**.
    + <font color = blue>用于 SLAM 的资源感知的逆施密特估计器</font>
    
---

#### 3. Semantic/Deep SLAM

+ [x] **[15]** Dong Y, Wang S, Yue J, et al. [**A Novel Texture-Less Object Oriented Visual SLAM System**](https://ieeexplore.ieee.org/abstract/document/8901152)[J]. IEEE Transactions on Intelligent Transportation Systems, **2019**.
    + <font color = blue>**一种新型的面向低纹理物体的视觉 SLAM 系统**</font>
    + 同济大学，期刊 中科院二区，JCR Q1，IF 6
+ [x] **[16]** Peng J, Shi X, Wu J, et al. [**An Object-Oriented Semantic SLAM System towards Dynamic Environments for Mobile Manipulation**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8868371)[C]//2019 IEEE/ASME International Conference on Advanced Intelligent Mechatronics (**AIM**). IEEE, **2019**: 199-204.
    + <font color = blue>**用于动态环境中移动机器人抓取的面向物体的语义 SLAM**</font>
    + 上海交大机械学院，AIM：CCF 人工智能 C 类会议
+ [ ] **[17]** Kim U H, Kim S H, Kim J H. [**SimVODIS: Simultaneous Visual Odometry, Object Detection, and Instance Segmentation**](https://arxiv.org/pdf/1911.05939.pdf)[J]. arXiv preprint arXiv:1911.05939, **2019**.
    + <font color = blue>SimVODIS：同时进行视觉里程计、目标检测和语义分割</font>
    + 韩国高等科学技术院
+ [ ] **[18]** Howard Mahe, Denis Marraud, Andrew I. Comport. [**Real-time RGB-D semantic keyframe SLAM based on image segmentation learning from industrial CAD models**](https://hal.archives-ouvertes.fr/hal-02391499/file/ICAR19_0187_FI.pdf). International Conference on Advanced Robotics, Dec 2019, Belo Horizonte, Brazil. ffhal-02391499
    + <font color = blue>基于工业 CAD 模型图像分割学习的实时 RGB-D 语义关键帧 SLAM</font>
    + 相关工作：**基于稠密类级别分割的仅使用语义的视觉里程表** Mahé H, Marraud D, Comport A I. [**Semantic-only Visual Odometry based on dense class-level segmentation**](https://hal.archives-ouvertes.fr/hal-01874544/document)[C]//2018 24th International Conference on Pattern Recognition (ICPR). IEEE, **2018**: 1989-1995.

---

#### 4. AR/VR/MR

+ [x] **[19]** Chandu S, Bhavan Jasani G J, Manglik A. [**Deleting 3D Objects in Augmented Reality using RGBD-SLAM**](https://bhavanj.github.io/files/SLAM_Final_Report.pdf)[J].**2019**
    + <font color = blue>使用 RGBD-SLAM 在增强现实中删除 3D 对象</font>
    + 亚马逊
+ [x] **[20]** Sartipi K, DuToit R C, Cobar C B, et al. [**Decentralized visual-inertial localization and mapping on mobile devices for augmented reality**](http://mars.cs.umn.edu/tr/decentralizedvi19.pdf)[R]. Google, Tech. Rep., Aug. **2019**.[Online]. Available: http://mars. cs. umn. edu/tr/decentralizedvi19. pdf.
    + <font color = blue>用于移动设备增强现实的分布式视觉惯导定位与建图</font>
    + 明尼苏达大学

---

#### 5. Others

+ [x] **[21]** Yan Z, Zha H. [**Flow-based SLAM: From geometry computation to learning**](https://www.sciencedirect.com/science/article/pii/S2096579619300622)[J]. Virtual Reality & Intelligent Hardware, **2019**, 1(5): 435-460.
    + <font color = blue>**基于流的 SLAM：从几何计算到学习的方法**</font>
    + 北京大学，[Google Scholar](https://scholar.google.com/citations?user=Rawfmp4AAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[22]** Li J, Liu Y, Yuan X, et al. [**Depth Based Semantic Scene Completion With Position Importance Aware Loss**](https://ieeexplore.ieee.org/abstract/document/8902045)[J]. IEEE Robotics and Automation Letters, **2019**, 5(1): 219-226.
    + <font color = blue>具有位置重要性感知损失的基于深度的语义场景理解</font>
    + 南京大学，[**代码开源**](https://github.com/UniLauX/PALNet)，[演示视频](https://www.youtube.com/watch?v=j-LAMcMh0yg&feature=youtu.be)
+ [x] **[23]** Simonelli A, Bulò S R R, Porzi L, et al. [**Disentangling Monocular 3D Object Detection**](https://arxiv.org/pdf/1905.12365.pdf)[J]. arXiv preprint arXiv:1905.12365, **2019**.
    + <font color = blue>**揭秘单目 3D 目标检测**</font>
    + 意大利特伦托大学，作者其他论文
        + 使用虚拟相机进行单阶段单目 3D 目标检测：Simonelli A, Bulò S R, Porzi L, et al. [**Single-Stage Monocular 3D Object Detection with Virtual Cameras**](https://arxiv.org/pdf/1912.08035.pdf)[J]. arXiv preprint arXiv:1912.08035, **2019**.

---

### 2019 年 11 月论文更新（17 篇）

#### 1. Geometric SLAM

+ [x] **[1]** Jatavallabhula K M, Iyer G, Paull L. [**gradSLAM: Dense SLAM meets Automatic Differentiation**](https://arxiv.org/pdf/1910.10672.pdf)[J]. arXiv preprint arXiv:1910.10672, **2019**.
    + <font color = blue>**自动区分的稠密 SLAM**</font>
    + [项目主页](http://montrealrobotics.ca/gradSLAM/)，[演示视频](https://www.youtube.com/watch?v=2ygtSJTmo08&feature=youtu.be)，[**代码开源**](https://github.com/montrealrobotics/gradSLAM)（还未放出）
    + 加拿大蒙特卡尔大学（[实验室主页](http://montrealrobotics.ca/)），CMU
+ [x] **[2]** Lee S J, Hwang S S. [**Elaborate Monocular Point and Line SLAM With Robust Initialization**](http://openaccess.thecvf.com/content_ICCV_2019/papers/Lee_Elaborate_Monocular_Point_and_Line_SLAM_With_Robust_Initialization_ICCV_2019_paper.pdf)[C]//**ICCV 2019**: 1121-1129.
    + <font color = blue>**具有鲁棒初始化的单目点线 SLAM**</font>
    + 韩国韩东国际大学
+ [ ] **[3]** Wen F, Ying R, Gong Z, et al. [**Efficient Algorithms for Maximum Consensus Robust Fitting**](https://ieeexplore.ieee.org/abstract/document/8870243)[J]. IEEE Transactions on Robotics, **2019**.
    + <font color = blue>最大一致性稳健拟合的有效算法</font>
    + 期刊 中科院二区，JCRQ1，IF 1.038，[代码开源](https://github.com/FWen/emc)
    + 上海交通大学电子工程系/脑启发式应用技术中心
+ [ ] **[4]** Civera J, Lee S H. [**RGB-D Odometry and SLAM**](https://link.springer.com/chapter/10.1007/978-3-030-28603-3_6#citeas)[M]//RGB-D Image Analysis and Processing. Springer, Cham, **2019**: 117-144.
    + <font color = blue>RGB-D SLAM 与里程计</font>
    + 专著
+ [ ] **[5]** Wang H, Li J, Ran M, et al. [**Fast Loop Closure Detection via Binary Content**](https://ieeexplore.ieee.org/abstract/document/8899937)[C]//2019 IEEE 15th International Conference on Control and Automation (**ICCA**). IEEE, **2019**: 1563-1568.
    + <font color = blue>通过二进制内容进行快速闭环检测</font>
    + 南洋理工大学，ICCV 会议 
+ [ ] **[6]** Liu W, Wu S, Wu Z, et al. [**Incremental Pose Map Optimization for Monocular Vision SLAM Based on Similarity Transformation**](https://www.mdpi.com/1424-8220/19/22/4945/htm)[J]. Sensors, **2019**, 19(22): 4945.
    + <font color = blue>基于相似度变换的单目 SLAM 增量式位姿图优化</font>
    + 北航，开源期刊
+ [ ] **[7]** Wang S, Yue J, Dong Y, et al. [**A synthetic dataset for Visual SLAM evaluation**](https://www.sciencedirect.com/science/article/pii/S0921889019301009#appSB)[J]. Robotics and Autonomous Systems, **2019**: 103336.
    + <font color = blue>用于视觉 SLAM 评估的合成数据集</font>
    + 同济大学，期刊中科院三区， JCR Q2， IF 2.809
+ [ ] **[8]** Han B, Li X, Yu Q, et al. [**A Novel Visual Odometry Aided by Vanishing Points in the Manhattan World**](https://www.researchgate.net/profile/Huimin_Lu/publication/336605825_A_Novel_Visual_Odometry_Aided_by_Vanishing_Points_in_the_Manhattan_World/links/5da85553a6fdccdad54c40ae/A-Novel-Visual-Odometry-Aided-by-Vanishing-Points-in-the-Manhattan-World.pdf)[J].
    + <font color = blue>曼哈顿世界消失点辅助的新型视觉里程计</font>
    + 国防科大，作者 [Google Scholar](https://scholar.google.com/citations?user=cp-6u7wAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[9]** Yuan Z, Zhu D, Chi C, et al. [**Visual-Inertial State Estimation with Pre-integration Correction for Robust Mobile Augmented Reality**](http://delivery.acm.org/10.1145/3360000/3351079/p1410-yuan.pdf?ip=219.216.73.1&id=3351079&acc=ACTIVE%20SERVICE&key=BF85BBA5741FDC6E%2E4183B12E3311CD37%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&__acm__=1574657773_86a30bc436c42e34852cca493a18c66c)[C]//Proceedings of the 27th ACM International Conference on Multimedia. ACM, **2019**: 1410-1418.
    + <font color = blue>用于鲁棒的移动增强现实中基于预积分校正的视觉惯性状态估计</font>
    + 华中科大，会议 ACM MM：CCF A 类会议
+ [ ] **[10]** Zhong D, Han L, Fang L. [**iDFusion: Globally Consistent Dense 3D Reconstruction from RGB-D and Inertial Measurements**](https://dl.acm.org/citation.cfm?id=3351085)[C]//Proceedings of the 27th ACM International Conference on Multimedia. ACM, **2019**: 962-970.
    + <font color = blue>iDFusion：RGB-D 和惯导的全局一致性稠密三维建图</font>
    + 清华大学、港科，会议 ACM MM：CCF A 类会议，[Google Scholar](https://scholar.google.com/citations?user=fI5pZ_cAAAAJ&hl=zh-CN&oi=sra)
+ [ ] **[11]** Duhautbout T, Moras J, Marzat J. [**Distributed 3D TSDF Manifold Mapping for Multi-Robot Systems**](https://ieeexplore.ieee.org/abstract/document/8870930)[C]//2019 European Conference on Mobile Robots (**ECMR**). IEEE, **2019**: 1-8.
    + <font color = blue>多机器人系统的分布式三维 TSDF 流形建图</font>
    + TSDF 开源库：https://github.com/personalrobotics/OpenChisel

---

#### 2. Semantic/Deep SLAM

+ [x] **[12]** Schorghuber M, Steininger D, Cabon Y, et al. [**SLAMANTIC-Leveraging Semantics to Improve VSLAM in Dynamic Environments**](http://openaccess.thecvf.com/content_ICCVW_2019/papers/DL4VSLAM/Schorghuber_SLAMANTIC_-_Leveraging_Semantics_to_Improve_VSLAM_in_Dynamic_Environments_ICCVW_2019_paper.pdf)[C]//**ICCV Workshops**. **2019**: 0-0.
    + <font color = blue>**SLAMANTIC：在动态环境中利用语义来改善VSLAM**</font>
    + 奥地利理工学院, [**代码开源**](https://github.com/mthz/slamantic)
+ [ ] **[13]** Lee C Y, Lee H, Hwang I, et al. [**Spatial Perception by Object-Aware Visual Scene Representation**](http://openaccess.thecvf.com/content_ICCVW_2019/papers/DL4VSLAM/Lee_Spatial_Perception_by_Object-Aware_Visual_Scene_Representation_ICCVW_2019_paper.pdf)[C]//**ICCV Workshops 2019**: 0-0.
    + <font color = blue>由物体视觉场景表示的空间感知</font>
    + 首尔大学
+ [ ] **[14]** Peng J, Shi X, Wu J, et al. [**An Object-Oriented Semantic SLAM System towards Dynamic Environments for Mobile Manipulation**](https://ieeexplore.ieee.org/abstract/document/8868371)[C]//2019 IEEE/ASME International Conference on Advanced Intelligent Mechatronics (**AIM**). IEEE, **2019**: 199-204.
    + <font color = blue>用于动态环境移动操作的物体级语义 SLAM 系统</font>
    + 上海交大，AIM：CCF 人工智能 C 类会议
+ [ ] **[15]** Cui L, Ma C. [**SOF-SLAM: A semantic visual SLAM for Dynamic Environments**](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8894002)[J]. IEEE Access, **2019**.
    + <font color = blue>一种用于动态环境的语义视觉里程计</font>
    + 北航，IEEE Access 开源期刊
+ [ ] **[16]** Zheng L, Tao W. [**Semantic Object and Plane SLAM for RGB-D Cameras**](https://link.springer.com/chapter/10.1007/978-3-030-31726-3_12)[C]//Chinese Conference on Pattern Recognition and Computer Vision (**PRCV**). Springer, Cham, **2019**: 137-148.
    + <font color = blue>RGB-D 物体语义与平面级 SLAM</font>
    + 平面分割采用 [PEAC](https://github.com/symao/PEAC)，PRCV 第二届今年在西安举办的那个
    + 华中科大
+ [ ] **[17]** Kim U H, Kim S H, Kim J H. [**SimVODIS: Simultaneous Visual Odometry, Object Detection, and Instance Segmentation**](https://arxiv.org/abs/1911.05939)[J]. arXiv preprint arXiv:1911.05939, **2019**.
    + <font color = blue>SimVODIS：同时进行视觉里程计、目标检测和实例分割</font>

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

#### 2. Semantic/Deep SLAM

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
    + 上交[裴凌老师](https://scholar.google.com/citations?user=Vm7d2EkAAAAJ&hl=zh-CN&oi=sra)，期刊：中科院三区 JCR Q1Q2 IF2.98
+ [ ] **[22]** Sjanic Z. [**Particle Filtering Approach for Data Association**](http://users.isy.liu.se/en/rt/zoran/Publ/fusion2019.pdf)[C]//22nd International Conference on Information Fusion. **2019**.
    + <font color = blue>粒子滤波算法用于数据关联</font>

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

#### 2. Semantic/Deep SLAM

+ [x] **[14]** Zhang J, Gui M, Wang Q, et al. [**Hierarchical Topic Model Based Object Association for Semantic SLAM**](https://ieeexplore.ieee.org/abstract/document/8794595)[J]. IEEE transactions on visualization and computer graphics, **2019**.
    + <font color = blue>**基于层次主题模型的语义 SLAM 对象关联** </font>
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

#### 2. Semantic/Deep SLAM

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
    + [明尼苏达大学交互式机器人和视觉实验室](http://irvlab.cs.umn.edu/publication)
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

#### 2. Semantic/Deep SLAM

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

#### 2. Semantic/Deep SLAM

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
    + 新加坡国立  &emsp; [代码开源](https://github.com/ziquan111/RobustPCLReconstruction)（还未放出）
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
#### 3. Semantic/Deep SLAM
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
+ [x] **[7]** Zhou D, Dai Y, Li H. [**Ground Plane based Absolute Scale Estimation for Monocular Visual Odometry**](https://ieeexplore.ieee.org/abstract/document/8708682/)[J]. arXiv preprint arXiv:1903.00912, **2019**.
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
> wuyanminmax@gmail.com    
