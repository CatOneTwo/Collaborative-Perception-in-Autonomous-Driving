# A summary of state-of-the-art collaborative perception methods for real-world issues

<div align="center">
<p align="center">
<a href="#table">Table</a> |
<a href="#references">Refer</a> 
</p>
</div>

## Table
|   Method               |   Venue         | Modality         |       Scheme         |     Loc Error         |   Comm Issue         |     Discrep         |      Security         |    Code                                                                         |
|:----------------------:|:---------------:|:----------------:|:--------------------:|:---------------------:|:--------------------:|:-------------------:|:---------------------:|:-------------------------------------------------------------------------------:|
| RobustV2VNet [1]       | CoRL'20         | LiDAR            | I                    | Loc, Pos              | -                    | -                   | -                     | -                                                                               |
| AOMAC [2]              | ICCV'21         | LiDAR            | I                    | -                     | -                    | -                   | Attack                | -                                                                               |
| P-CNN [3]              | IoT'21          | Camera           | E                    | -                     | -                    | -                   | Privacy               | -                                                                               |
| FPV-RCNN [4]           | RAL'22          | LiDAR            | I                    | Loc, Pos              | -                    | -                   | -                     | [Linkn](https://github.com/YuanYunshuang/FPV_RCNN)    |
| TCLF [5]               | CVPR'22         | LiDAR            | L                    | -                     | Laten                | -                   | -                     | [Linkv](https://github.com/AIR-THU/DAIR-V2X)               |
| V2X-ViT [6]            | ECCV'22         | LiDAR            | I                    | Loc, Pos              | Laten                | -                   | -                     | [Linko](https://github.com/DerrickXuNu/v2x-vit)                                 |
| SyncNet [7]            | ECCV'22         | LiDAR            | I                    | -                     | Laten                | -                   | -                     | [Linkc](https://github.com/MediaBrain-SJTU/SyncNet)     |
| TaskAgnostic [8]       | CoRL'22         | LiDAR            | I                    | -                     | -                    | Task                | -                     | [Linkc](https://github.com/coperception/star)    |
| SecPCV [9]             | TITS'22         | LiDAR            | E                    | -                     | -                    | -                   | Privacy               | -                                                                               |
| ModelAgnostic [10]     | ICRA'23         | LiDAR            | L                    | -                     | -                    | Model               | -                     | [Linko](https://github.com/DerrickXuNu/model_anostic)   |
| MPDA [11]              | ICRA'23         | LiDAR            | I                    | -                     | -                    | Model               | -                     | [Linko](https://github.com/DerrickXuNu/MPDA)            |
| CoAlign [12]           | ICRA'23         | LiDAR            | I, L                 | Loc, Pos              | -                    | -                   | -                     | [Linko](https://github.com/yifanlu0227/CoAlign)                              |
| LCRN [13]              | TIV'23          | LiDAR            | L                    | -                     | Loss                 | -                   | -                     | -                                                                               |
| OptiMatch [14]         | IV'23           | LiDAR            | L                    | Loc, Pos              | -                    | -                   | -                     | -                                                                               |
| P2OD [15]              | IoT'23          | Camera           | E                    | -                     | -                    | -                   | Privacy               | -                                                                               |
| ROBOSAC [16]           | ICCV'23         | LiDAR            | I                    | -                     | -                    | -                   | Attack               | [Linkc](https://github.com/coperception/ROBOSAC)      |
| FFNet [17]             | NeurIPS'23         | LiDAR            | I                    | -                     | Laten                | -                   | -                   | [Linkv](https://github.com/haibao-yu/FFNet-VIC3D)   |
| CoBEVFlow [18]             | NeurIPS'23         | LiDAR            | I                    | -                     | Laten                | -                   | -                   | [Linko](https://github.com/MediaBrain-SJTU/CoBEVFlow)  |
| How2comm [19]             | NeurIPS'23         | LiDAR            | I                    | -                     | Laten                | -                   | -         |     [Linko](https://github.com/ydk122024/How2comm)  |
| FeaCo [20]             | MM'23         | LiDAR            | I                    | Loc, Pos             | -                | -                   | -                   | [Linko](https://github.com/jmgu0212/FeaCo)   |
| ERMVP [21]             | CVPR'24         | LiDAR            | I                    | Loc, Pos             | -                | -                   | -                   | [Linko](https://github.com/Terry9a/ERMVP)            |
| MRCNet [22]             | CVPR'24         | LiDAR            | I                    | Loc, Pos             | -                | -                   | -                   | [Linko](https://github.com/IndigoChildren/collaborative-perception-MRCNet)   |
| RoCo [23]             | MM'24         | LiDAR            | I                    | Loc, Pos             | -                | -                   | -                   | [Linko](https://github.com/HuangZhe885/RoCo)  |
| PnPDA [24]             | ECCV'24         | LiDAR            | I                    | -            | -                | Model                  | -                   | [Linko](https://github.com/luotianyou349/PnPDA)              |
| Hetecooper [25]             | ECCV'24         | LiDAR            | I                    | -            | -                | Model                  | -                   |           |
| NEAT [26]             | ECCV'24         | LiDAR            | I                    | Loc, Pos           | Laten               | -                  | -                   |           |
| V2X-INCOP [27]         | TIV'24        | LiDAR            | I                    | -                     | Inter                | -                   | -                     | -               |
| MADE [28]         | IROS'24        | LiDAR            | I                    | -                     | -                | -                   | Attack                     | -               |
| CP-Guard [29]         | AAAI'25        | LiDAR            | I                    | -                     | -                | -                   | Attack                     | -               |
| PLDA [30]         | AAAI'25        | LiDAR            | I                    | -                     | -                | Model                   | -                     | -               |
| BEVSync [31]         | AAAI'25        | LiDAR            | I                    | -                     | Laten                | -                   | -                     | -               |
| STAMP [32]         | ICLR'25        | LiDAR, Camera          | I                    | -                     | -                | Model, Task             | -                     | [Linko](https://github.com/taco-group/STAMP)      |
| PolyInter [33]         | CVPR'25        | LiDAR          | I                    | -                     | -                | Model             | -                     | - |


Notes:
- Schemes include early (E), intermediate (I) and late (L) collaboration.
- **Loc Error** includes localization (**Loc**) and pose (**Pos**) errors.
- **Comm Issue** includes latency (**Laten**), interruption (**Inter**) and loss (**Loss**).
- **Discrep** includes model (**Model**) and task (**Task**) discrepancies.
- **Security** includes attack defense (**Attack**) and privacy protection (**Privacy**).
- **Code Framework**: o ([OpenCOOD](https://github.com/DerrickXuNu/OpenCOOD)), v ([VIC3D](https://github.com/AIR-THU/DAIR-V2X)), c ([CoPerception](https://github.com/coperception/coperception)), n (Non-mainstream framework)

Back to [Contents](README.md) 🔙 

## References
### Published
1. Learning to Communicate and Correct Pose Errors (CoRL'20) [[`pdf`](https://arxiv.org/abs/2011.05289)] 
2. Adversarial attacks on multi-agent communication (ICCV'21) [[`pdf`](https://arxiv.org/abs/2101.06560)]
3. Toward lightweight, privacy-preserving cooperative object classification for connected autonomous vehicles (IoT'21) [[`pdf`](https://ieeexplore.ieee.org/document/9468670)]
4. Keypoints-Based Deep Feature Fusion for Cooperative Vehicle Detection of Autonomous Driving (RAL'22) [[`pdf`](https://arxiv.org/abs/2109.11615)] [[`code`](https://github.com/YuanYunshuang/FPV_RCNN)]
5. DAIR-V2X: A Large-Scale Dataset for Vehicle-Infrastructure Cooperative 3D Object Detection (CVPR'22) [[`pdf`](https://arxiv.org/abs/2204.05575)] [[`code`](https://github.com/AIR-THU/DAIR-V2X)]
6. V2X-ViT: Vehicle-to-everything cooperative perception with vision transformer (ECCV'22) [[`pdf`](https://arxiv.org/abs/2203.10638)] [[`code`](https://github.com/DerrickXuNu/v2x-vit)]
7. Latency-Aware Collaborative Perception (ECCV'22) [[`pdf`](https://arxiv.org/abs/2207.08560)] [[`code`](https://github.com/MediaBrain-SJTU/SyncNet)]
8. Multi-robot scene completion: Towards task-agnostic collaborative perception (CoRL'22) [[`pdf`](https://openreview.net/forum?id=hW0tcXOJas2)] [[`code`](https://github.com/coperception/star)]
9. Edge-Cooperative Privacy-Preserving Object Detection Over Random Point Cloud Shares for Connected Autonomous Vehicles (TITS'22) [[`pdf`](https://ieeexplore.ieee.org/document/9928424)]
10. Model-Agnostic Multi-Agent Perception Framework (ICRA'23) [[`pdf`](https://arxiv.org/abs/2203.13168)] [[`code`](https://github.com/DerrickXuNu/model_anostic)]
11. Bridging the Domain Gap for Multi-Agent Perception (ICRA'23) [[`pdf`](https://arxiv.org/abs/2210.08451)] [[`code`](https://github.com/DerrickXuNu/MPDA)]
12. Robust Collaborative 3D Object Detection in Presence of Pose Errors (ICRA'23) [[`pdf`](https://arxiv.org/abs/2211.07214)] [[`code`](https://github.com/yifanlu0227/CoAlign)]
13. Learning for Vehicle-to-Vehicle Cooperative Perception under Lossy Communication (TIV'23) [[`pdf`](https://arxiv.org/abs/2212.08273)]
14. A Cooperative Perception System Robust to Localization Errors (IV'23) [[`pdf`](https://arxiv.org/abs/2210.06289)]
15. Achieving Lightweight and Privacy-Preserving Object Detection for Connected Autonomous Vehicles (IoT'23) [[`pdf`](https://ieeexplore.ieee.org/document/9913215)]
16. Among Us: Adversarially Robust Collaborative Perception by Consensus (ICCV'23) [[`pdf`](https://arxiv.org/abs/2303.09495)] [[`code`](https://github.com/coperception/ROBOSAC)]
17. Flow-Based Feature Fusion for Vehicle-Infrastructure Cooperative 3D Object Detection (NeurIPS'23) [[`pdf`](https://openreview.net/forum?id=gsglrhvQxX)] [[`code`](https://github.com/haibao-yu/FFNet-VIC3D)]
18. Robust Asynchronous Collaborative 3D Detection via Bird’s Eye View Flow (NeurIPS'23) [[`pdf`](https://arxiv.org/abs/2309.16940)] [[`code`](https://github.com/MediaBrain-SJTU/CoBEVFlow)]
19. How2comm: Communication-Efficient and Collaboration-Pragmatic Multi-Agent Perception (NeurIPS'23) [[`pdf`](https://openreview.net/forum?id=Dbaxm9ujq6)] [[`code`](https://github.com/ydk122024/How2comm)]
20. FeaCo: Reaching Robust Feature-Level Consensus in Noisy Pose Conditions (MM'23) [[`pdf`](https://dl.acm.org/doi/abs/10.1145/3581783.3611880)]
21. ERMVP: Communication-Efﬁcient and Collaboration-Robust Multi-Vehicle Perception in Challenging Environments (CVPR'24) [[`pdf`](https://openaccess.thecvf.com/content/CVPR2024/papers/Zhang_ERMVP_Communication-Efficient_and_Collaboration-Robust_Multi-Vehicle_Perception_in_Challenging_Environments_CVPR_2024_paper.pdf)]
22. Multi-agent Collaborative Perception via Motion-aware Robust Communication Network (CVPR'24) [[`pdf`](https://openaccess.thecvf.com/content/CVPR2024/papers/Hong_Multi-agent_Collaborative_Perception_via_Motion-aware_Robust_Communication_Network_CVPR_2024_paper.pdf)]
23. RoCo: Robust Cooperative Perception By Iterative Object Matching and Pose Adjustment (MM'24) [[`pdf`](https://openreview.net/forum?id=TFFnsgu2Pr)]
24. Plug and Play: A Representation Enhanced Domain Adapter for Collaborative Perception (ECCV'24) [[`pdf`](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/10564.pdf)] [[`code`](https://github.com/luotianyou349/PnPDA)]
25. Hetecooper: Feature Collaboration Graph for Heterogeneous Collaborative Perception (ECCV'24) [[`pdf`](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/07071.pdf)]
26. Align before Collaborate: Mitigating Feature Misalignment for Robust Multi-Agent Perception (ECCV'24) [[`pdf`](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/00560.pdf)]
27. Interruption-Aware Cooperative Perception for V2X Communication-Aided Autonomous Driving (TIV'24) [[`pdf`](https://arxiv.org/abs/2304.11821)]
28. Malicious Agent Detection for Robust Multi-Agent Collaborative Perception (IROS'24) [[`pdf`](https://arxiv.org/abs/2304.11821)]
29. CP-Guard: Malicious Agent Detection and Defense in Collaborative Bird’s Eye View Perception (AAAI'25) [[`pdf`](https://arxiv.org/abs/2412.12000)]
30. Privacy-Preserving V2X Collaborative Perception Integrating Unknown Collaborators (AAAI'25)
31. BEVSync: Asynchronous Data Alignment for Camera-based Vehicle-Infrastructure Cooperative Perception Under Uncertain Delays (AAAI'25)
32. STAMP: Scalable Task And Model-agnostic Collaborative Perception (ICLR'25) [[`pdf`](https://arxiv.org/abs/2501.18616)] [[`code`](https://github.com/taco-group/STAMP)]
33. One is Plenty: A Polymorphic Feature Interpreter for Immutable Heterogeneous Collaborative Perception (CVPR'25) [[`pdf`](https://arxiv.org/abs/2411.16799)] 

