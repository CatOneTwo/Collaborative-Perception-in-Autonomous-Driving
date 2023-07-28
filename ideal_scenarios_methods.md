# A summary of state-of-the-art collaborative perception methods for ideal scenarios

|    Method         |  Venue     |   Modality    |    Scheme    |    Data Fusion    |    Comm Mecha    |    Feat Fusion    |    Loss Func    |    Code                                                            |
|:-----------------:|:----------:|:-------------:|:------------:|:-----------------:|:----------------:|:-----------------:|:---------------:|:------------------------------------------------------------------:|
| Cooper [1]        | ICDCS'19   | LiDAR         | E            | Raw               | -                | -                 | -               | -                                                                  |
| F-Cooper [2]      | SEC'19     | LiDAR         | I            | -                 | -                | Trad              | -               | [Link](https://github.com/Aug583/F-COOPER)                         |
| Who2com [3]       | ICRA'20    | Camera        | I            | -                 | Agent            | Trad              | -               | -                                                                  |
| When2com [4]      | CVPR'20    | Camera        | I            | -                 | Agent            | Trad              | -               | [Link](https://github.com/GT-RIPL/MultiAgentPerception)            |
| V2VNet [5]        | ECCV'20    | LiDAR         | I            | -                 | -                | Graph             | -               | -                                                                  |
| Coop3D [6]        | TITS'20    | LiDAR         | E, L         | Raw, Out          | -                | -                 | -               | [Link](https://github.com/eduardohenriquearnold/coop-3dod-infra)   |
| CoFF [7]          | IoT'21     | LiDAR         | I            | -                 | -                | Trad              | -               | -                                                                  |
| DiscoNet [8]      | NeurIPS'21 | LiDAR         | I            | Raw               | -                | Graph             | -               | [Link](https://github.com/ai4ce/DiscoNet)                          |
| MP-Pose [9]       | RAL'22     | Camera        | I            | -                 | -                | Graph             | -               | -                                                                  |
| FPV-RCNN [10]     | RAL'22     | LiDAR         | I            | Out               | Feat             | Trad              | -               | [Link](https://github.com/YuanYunshuang/FPV_RCNN)                  |
| AttFusion [11]    | ICRA'22    | LiDAR         | I            | -                 | -                | Atten             | -               | [Link](https://github.com/DerrickXuNu/OpenCOOD)                    |
| TCLF [12]         | CVPR'22    | LiDAR         | L            | Out               | -                | -                 | -               | [Link](https://github.com/AIR-THU/DAIR-V2X)                        |
| COOPERNAUT [13]   | CVPR'22    | LiDAR         | I            | -                 | -                | Atten             | -               | [Link](https://github.com/UT-Austin-RPL/Coopernaut)                |
| V2X-ViT [14]      | ECCV'22    | LiDAR         | I            | -                 | -                | Atten             | -               | [Link](https://github.com/DerrickXuNu/v2x-vit)                     |
| CRCNet [15]       | MM'22      | LiDAR         | I            | -                 | -                | Atten             | Redund          | -                                                                  |
| CoBEVT [16]       | CoRL'22    | Camera        | I            | -                 | -                | Atten             | -               | [Link](https://github.com/DerrickXuNu/CoBEVT)                      |
| Where2comm [17]   | NeurIPS'22 | LiDAR         | I            | -                 | Agent, Feat      | Atten             | -               | [Link](https://github.com/MediaBrain-SJTU/Where2comm)              |
| Double-M [18]     | ICRA'23    | LiDAR         | E, I, L      | -                 | -                | -                 | Uncert          | [Link](https://github.com/coperception/double-m-quantification)    |
| CoCa3D [19]       | CVPR'23    | Camera        | I            | -                 | Feat             | Trad              | -               | [Link](https://github.com/MediaBrain-SJTU/CoCa3D)                  |
| VIMI [20]         | arXiv'23   | Camera        | I            | -                 | -                | Atten             | -               | -                                                                  |
| HM-ViT [21]       | ICCV'23    | LiDAR, Camera | I            | -                 | -                | Atten             | -               | -                                                                  |
| CORE [22]         | ICCV'23    | LiDAR         | I            | Raw               | Feat             | Atten             | Recon           | [Link](https://github.com/zllxot/CORE)                             |

Note:
- Schemes include early (E), intermediate (I) and late (L) collaboration.
- **Data Fusion**: data fusion includes raw data fusion (**Raw**) and output fusion (**Out**).
- **Comm Mecha**: communication mechanism includes agent selection (**Agent**) and feature selection (**Feat**).
- **Feat Fusion**: feature fusion can be divided into traditional (**Trad**), graph-based (**Graph**) and attention-based (**Atten**) feature fusion.
- **Loss Func**: loss function can be used for uncertainty estimation (**Uncert**), redundancy minimization (**Redund**) and Reconstruction (**Recon**), etc.

▶️ Go back to [Main Page](README.md)

References:
1. [Cooper: Cooperative perception for connected autonomous vehicles based on 3d point clouds](https://arxiv.org/abs/1905.05265)
2. [F-Cooper: Feature based cooperative perception for autonomous vehicle edge computing system using 3D point clouds](https://arxiv.org/abs/1909.06459)
3. [Who2com: Collaborative perception via learnable handshake communication](https://arxiv.org/abs/2003.09575)
4. [When2com: Multi-agent perception via communication graph grouping](https://arxiv.org/abs/2006.00176)
5. [V2VNet: Vehicle-to-Vehicle Communication for Joint Perception and Prediction](https://arxiv.org/abs/2008.07519)
6. [Cooperative perception for 3D object detection in driving scenarios using infrastructure sensors](https://arxiv.org/abs/1912.12147)
7. [CoFF: Cooperative spatial feature fusion for 3-d object detection on autonomous vehicles](https://arxiv.org/abs/2009.11975)
8. [Learning distilled collaboration graph for multi-agent perception](https://arxiv.org/abs/2111.00643)
9. [Multi-Robot Collaborative Perception with Graph Neural Networks](https://arxiv.org/abs/2201.01760)
10. [Keypoints-Based Deep Feature Fusion for Cooperative Vehicle Detection of Autonomous Driving](https://arxiv.org/abs/2109.11615)
11. [OPV2V: An open benchmark dataset and fusion pipeline for perception with vehicle-to-vehicle communication](https://arxiv.org/abs/2109.07644)
12. [DAIR-V2X: A Large-Scale Dataset for Vehicle-Infrastructure Cooperative 3D Object Detection](https://arxiv.org/abs/2204.05575)
13. [COOPERNAUT: End-to-End Driving with Cooperative Perception for Networked Vehicles](https://arxiv.org/abs/2205.02222)
14. [V2X-ViT: Vehicle-to-everything cooperative perception with vision transformer](https://arxiv.org/abs/2203.10638)
15. [Complementarity-Enhanced and Redundancy-Minimized Collaboration Network for Multi-agent Perception](https://dl.acm.org/doi/abs/10.1145/3503161.3548197)
16. [CoBEVT: Cooperative Bird's Eye View Semantic Segmentation with Sparse Transformers](https://arxiv.org/abs/2207.02202)
17. [Where2comm: Communication-Efficient Collaborative Perception via Spatial Confidence Maps](https://arxiv.org/abs/2209.12836)
18. [Uncertainty Quantification of Collaborative Detection for Self-Driving](https://arxiv.org/abs/2209.08162)
19. [Collaboration Helps Camera Overtake LiDAR in 3D Detection](https://arxiv.org/abs/2303.13560)
20. [VIMI: Vehicle-Infrastructure Multi-view Intermediate Fusion for Camera-based 3D Object Detection](https://arxiv.org/abs/2303.10975)
21. [HM-ViT: Hetero-modal Vehicle-to-Vehicle Cooperative perception with vision transformer](https://arxiv.org/abs/2304.10628)
22. [CORE: Cooperative Reconstruction for Multi-Agent Perception](https://arxiv.org/abs/2307.11514)


  
