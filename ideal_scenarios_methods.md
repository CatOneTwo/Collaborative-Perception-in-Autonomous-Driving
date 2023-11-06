# A summary of state-of-the-art collaborative perception methods for ideal scenarios

<div align="center">
<p align="center">
<a href="#table">Table</a> |
<a href="#references">Refer</a> 
</p>
</div>

## Table
|    Method         |  Venue     |   Modality    |    Scheme    |    Data Fusion    |    Comm Mecha    |    Feat Fusion    |    Loss Func    |    Code                                                            |
|:-----------------:|:----------:|:-------------:|:------------:|:-----------------:|:----------------:|:-----------------:|:---------------:|:------------------------------------------------------------------:|
| Cooper [1]        | ICDCS'19   | LiDAR         | E            | Raw               | -                | -                 | -               | -                                                                  |
| F-Cooper [2]      | SEC'19     | LiDAR         | I            | -                 | -                | Trad              | -               | [Linkn](https://github.com/Aug583/F-COOPER)                         |
| Who2com [3]       | ICRA'20    | Camera        | I            | -                 | Agent            | Trad              | -               | -                                                                  |
| When2com [4]      | CVPR'20    | Camera        | I            | -                 | Agent            | Trad              | -               | [Linkn](https://github.com/GT-RIPL/MultiAgentPerception)            |
| V2VNet [5]        | ECCV'20    | LiDAR         | I            | -                 | -                | Graph             | -               | -                                                                  |
| Coop3D [6]        | TITS'20    | LiDAR         | E, L         | Raw, Out          | -                | -                 | -               | [Linkn](https://github.com/eduardohenriquearnold/coop-3dod-infra)   |
| CoFF [7]          | IoT'21     | LiDAR         | I            | -                 | -                | Trad              | -               | -                                                                  |
| DiscoNet [8]      | NeurIPS'21 | LiDAR         | I            | Raw               | -                | Graph             | -               | [Linkc](https://github.com/ai4ce/DiscoNet)                        |
| MP-Pose [9]       | RAL'22     | Camera        | I            | -                 | -                | Graph             | -               | -                                                                  |
| FPV-RCNN [10]     | RAL'22     | LiDAR         | I            | Out               | Feat             | Trad              | -               | [Linkn](https://github.com/YuanYunshuang/FPV_RCNN)                  |
| AttFusion [11]    | ICRA'22    | LiDAR         | I            | -                 | -                | Atten             | -               | [Linko](https://github.com/DerrickXuNu/OpenCOOD)                 |
| TCLF [12]         | CVPR'22    | LiDAR         | L            | Out               | -                | -                 | -               | [Linkv](https://github.com/AIR-THU/DAIR-V2X)                        |
| COOPERNAUT [13]   | CVPR'22    | LiDAR         | I            | -                 | -                | Atten             | -               | [Linkn](https://github.com/UT-Austin-RPL/Coopernaut)                |
| V2X-ViT [14]      | ECCV'22    | LiDAR         | I            | -                 | -                | Atten             | -               | [Linko](https://github.com/DerrickXuNu/v2x-vit)                     |
| CRCNet [15]       | MM'22      | LiDAR         | I            | -                 | -                | Atten             | Redund          | -                                                                  |
| CoBEVT [16]       | CoRL'22    | Camera        | I            | -                 | -                | Atten             | -               | [Linko](https://github.com/DerrickXuNu/CoBEVT)                      |
| Where2comm [17]   | NeurIPS'22 | LiDAR         | I            | -                 | Agent, Feat      | Atten             | -               | [Linko](https://github.com/MediaBrain-SJTU/Where2comm)              |
| Double-M [18]     | ICRA'23    | LiDAR         | E, I, L      | -                 | -                | -                 | Uncert          | [Linkc](https://github.com/coperception/double-m-quantification)    |
| CoCa3D [19]       | CVPR'23    | Camera        | I            | -                 | Feat             | Trad              | -               | [Linko](https://github.com/MediaBrain-SJTU/CoCa3D)                  |
| HM-ViT [20]       | ICCV'23    | LiDAR, Camera | I            | -                 | -                | Atten             | -               | [Linko](https://github.com/XHwind/HM-ViT)                           |
| CORE [21]         | ICCV'23    | LiDAR         | I            | Raw               | Feat             | Atten             | Recon           | [Linko](https://github.com/zllxot/CORE)                             |
| SCOPE [22]        | ICCV'23    | LiDAR         | I            | -                 | -                | Atten (ST)   | -               | [Linko](https://github.com/starfdu1418/SCOPE)          |
| TransIFF [23]        | ICCV'23    | LiDAR         | I            | -                 | Feat                | Atten    | -               | -       
| UMC [24]        | ICCV'23    | LiDAR         | I            | -                 | Feat                |Graph   | -               | [Linkc](https://github.com/ispc-lab/UMC)                                                         |
| HYDRO-3D [25]        | TIV'23    | LiDAR         | I         | -                 | -                |Atten (ST)             | -              |    - |
| MKD-Cooper [26]        | TIV'23    | LiDAR         | I         | Raw                 | -                |Atten             | -              |    [Linko](https://github.com/EricLee523/MKD-Cooper)|
| V2VFormer++ [27]        | TITS'23    | LiDAR, Camera         | I         | -              | -                |Atten             | -              |    -          |
| How2comm [28]        | NeurIPS'23    | LiDAR          | I         | -              | Feat                |Atten (ST)            | -              |   [Linko](https://github.com/ydk122024/How2comm)|
| What2comm [29]        | MM'23    | LiDAR          | I         | -              | Feat                |Atten (ST)            | -              |    -          |
| BM2CP [30]        | CoRL'23    | LiDAR, Camera          | I         | -              | Feat                |Atten            | -              |  [Linko](https://github.com/byzhaoAI/BM2CP)      |
| VIMI [a1]         | arXiv'23   | Camera        | I            | -                 | -                | Atten             | -               | [Linkv](https://github.com/bosszhe/vimi)                            |
| QUEST [a2]        | arXiv'23    | Camera         | I, L            | -                 | Feat                |Atten   | -               |         -        |
| Select2Col [a3]        | arXiv'23    | LiDAR         | I           | -                 | Agent                |Atten (ST)   | -               | [Linko](https://github.com/huangqzj/select2col)  |
| MOT-CUP [a4]        | arXiv'23    | LiDAR         | E, I, L     | -                 | -                |-             | Uncert             |      [Linkc](https://github.com/susanbao/mot_cup)    |


Note:
- Schemes include early (E), intermediate (I) and late (L) collaboration.
- **Data Fusion**: data fusion includes raw data fusion (**Raw**) and output fusion (**Out**).
- **Comm Mecha**: communication mechanism includes agent selection (**Agent**) and feature selection (**Feat**).
- **Feat Fusion**: feature fusion can be divided into traditional (**Trad**), graph-based (**Graph**) and attention-based (**Atten**) feature fusion. （ST: spatio-temporal）
- **Loss Func**: loss function can be used for uncertainty estimation (**Uncert**), redundancy minimization (**Redund**) and Reconstruction (**Recon**), etc.
- **Code Framework**: o ([OpenCOOD](https://github.com/DerrickXuNu/OpenCOOD)), v ([VIC3D](https://github.com/AIR-THU/DAIR-V2X)), c ([CoPerception](https://github.com/coperception/coperception)), n (Non-mainstream framework)

Back to [Contents](README.md) 🔙 

## References
### Published
1. Cooper: Cooperative perception for connected autonomous vehicles based on 3d point clouds (ICDCS'19) [[`pdf`](https://arxiv.org/abs/1905.05265)] 
2. F-Cooper: Feature based cooperative perception for autonomous vehicle edge computing system using 3D point clouds (SEC'19) [[`pdf`](https://arxiv.org/abs/1909.06459)] 
3. Who2com: Collaborative perception via learnable handshake communication (ICRA'20) [[`pdf`](https://arxiv.org/abs/2003.09575)]
4. When2com: Multi-agent perception via communication graph grouping (CVPR'20) [[`pdf`](https://arxiv.org/abs/2006.00176)]
5. V2VNet: Vehicle-to-Vehicle Communication for Joint Perception and Prediction (ECCV'20) [[`pdf`](https://arxiv.org/abs/2008.07519)]
6. Cooperative perception for 3D object detection in driving scenarios using infrastructure sensors (TITS'20) [[`pdf`](https://arxiv.org/abs/1912.12147)]
7. CoFF: Cooperative spatial feature fusion for 3-d object detection on autonomous vehicles (IoT'21) [[`pdf`](https://arxiv.org/abs/2009.11975)]
8. Learning distilled collaboration graph for multi-agent perception (NeurIPS'21) [[`pdf`](https://arxiv.org/abs/2111.00643)] [[`code`](https://github.com/ai4ce/DiscoNet)]
9. Multi-Robot Collaborative Perception with Graph Neural Networks (RAL'22) [[`pdf`](https://arxiv.org/abs/2201.01760)]
10. Keypoints-Based Deep Feature Fusion for Cooperative Vehicle Detection of Autonomous Driving (RAL'22) [[`pdf`](https://arxiv.org/abs/2109.11615)] [[`code`](https://github.com/YuanYunshuang/FPV_RCNN)]
11. OPV2V: An open benchmark dataset and fusion pipeline for perception with vehicle-to-vehicle communication (ICRA'22) [[`pdf`](https://arxiv.org/abs/2109.07644)] [[`code`](https://github.com/DerrickXuNu/OpenCOOD)]
12. DAIR-V2X: A Large-Scale Dataset for Vehicle-Infrastructure Cooperative 3D Object Detection (CVPR'22) [[`pdf`](https://arxiv.org/abs/2204.05575)] [[`code`](https://github.com/AIR-THU/DAIR-V2X)]
13. COOPERNAUT: End-to-End Driving with Cooperative Perception for Networked Vehicles (CVPR'22) [[`pdf`](https://arxiv.org/abs/2205.02222)] [[`code`](https://github.com/UT-Austin-RPL/Coopernaut)]
14. V2X-ViT: Vehicle-to-everything cooperative perception with vision transformer (ECCV'22) [[`pdf`](https://arxiv.org/abs/2203.10638)] [[`code`]()]
15. Complementarity-Enhanced and Redundancy-Minimized Collaboration Network for Multi-agent Perception (MM'22) [[`pdf`](https://dl.acm.org/doi/abs/10.1145/3503161.3548197)]
16. CoBEVT: Cooperative Bird's Eye View Semantic Segmentation with Sparse Transformers (CoRL'22) [[`pdf`](https://arxiv.org/abs/2207.02202)] [[`code`](https://github.com/DerrickXuNu/v2x-vit)]
17. Where2comm: Communication-Efficient Collaborative Perception via Spatial Confidence Maps (NeurIPS'22) [[`pdf`](https://arxiv.org/abs/2209.12836)] [[`code`](https://github.com/MediaBrain-SJTU/Where2comm)]
18. Uncertainty Quantification of Collaborative Detection for Self-Driving (ICRA'23) [[`pdf`](https://arxiv.org/abs/2209.08162)] [[`code`](https://github.com/coperception/double-m-quantification)]
19. Collaboration Helps Camera Overtake LiDAR in 3D Detection (CVPR'23) [[`pdf`](https://arxiv.org/abs/2303.13560)] [[`code`](https://github.com/MediaBrain-SJTU/CoCa3D)]
20. HM-ViT: Hetero-modal Vehicle-to-Vehicle Cooperative perception with vision transformer (ICCV'23) [[`pdf`](https://arxiv.org/abs/2304.10628)]
21. CORE: Cooperative Reconstruction for Multi-Agent Perception (ICCV'23) [[`pdf`](https://arxiv.org/abs/2307.11514)] [[`code`](https://github.com/zllxot/CORE)]
22. Spatio-Temporal Domain Awareness for Multi-Agent Collaborative Perception (ICCV'23) [[`pdf`](https://arxiv.org/abs/2307.13929)] [[`code`](https://github.com/starfdu1418/SCOPE)]
23. TransIFF: An Instance-Level Feature Fusion Framework for Vehicle-Infrastructure Cooperative 3D Detection with Transformers (ICCV'23) [[`pdf`](https://openaccess.thecvf.com/content/ICCV2023/papers/Chen_TransIFF_An_Instance-Level_Feature_Fusion_Framework_for_Vehicle-Infrastructure_Cooperative_3D_ICCV_2023_paper.pdf)]
24. UMC: A Unified Bandwidth-efficient and Multi-resolution based Collaborative Perception Framework (ICCV'23) [[`pdf`](https://arxiv.org/abs/2303.12400)] [[`code`](https://github.com/ispc-lab/UMC)]
25. HYDRO-3D: Hybrid Object Detection and Tracking for Cooperative Perception Using 3D LiDAR (TIV'23) [[`pdf`](https://ieeexplore.ieee.org/abstract/document/10148929)]
26. MKD-Cooper: Cooperative 3D Object Detection for Autonomous Driving via Multi-teacher Knowledge Distillation (TIV'23) [[`pdf`](https://ieeexplore.ieee.org/abstract/document/10236578)] [[`code`](https://github.com/EricLee523/MKD-Cooper)]
27. V2VFormer ++ : Multi-Modal Vehicle-to-Vehicle Cooperative Perception via Global-Local Transformer (TITS'23) [[`pdf`](https://ieeexplore.ieee.org/document/10265751/)]
28. How2comm: Communication-Efficient and Collaboration-Pragmatic Multi-Agent Perception (NeurIPS'23) [[`pdf`](https://openreview.net/forum?id=Dbaxm9ujq6)] [[`code`](https://github.com/ydk122024/How2comm)]
29. What2comm: Towards Communication-efficient Collaborative Perception via Feature Decoupling (MM'23) [[`pdf`](https://dl.acm.org/doi/10.1145/3581783.3611699)]
30. BM2CP: Efficient Collaborative Perception with LiDAR-Camera Modalities (CoRL'23) [[`pdf`](https://openreview.net/forum?id=uJqxFjF1xWp)] [[`code`](https://github.com/byzhaoAI/BM2CP)]

### ArXiv
1. VIMI: Vehicle-Infrastructure Multi-view Intermediate Fusion for Camera-based 3D Object Detection (arXiv'23) [[`pdf`](https://arxiv.org/abs/2303.10975)] [[`code`](https://github.com/bosszhe/vimi)]
2. QUEST: Query Stream for Vehicle-Infrastructure Cooperative Perception (arXiv'23) [[`pdf`](https://arxiv.org/abs/2308.01804)] 
3. Select2Col: Leveraging Spatial-Temporal Importance of Semantic Information for Efficient Collaborative Perception (arXiv'23) [[`pdf`](https://arxiv.org/abs/2307.16517)] [[`code`](https://github.com/huangqzj/select2col)]
4. Collaborative Multi-Object Tracking with Conformal Uncertainty Propagation (arXiv'23) [[`pdf`](https://arxiv.org/abs/2303.14346)] [[`code`](https://github.com/susanbao/mot_cup)]


  
