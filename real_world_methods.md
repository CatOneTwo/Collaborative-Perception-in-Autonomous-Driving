# A summary of state-of-the-art collaborative perception methods for real-world issues
|   Method               |   Venue         | Modality         |       Scheme         |     Loc Error         |   Comm Issue         |     Discrep         |      Security         |    Code                                                                         |
|:----------------------:|:---------------:|:----------------:|:--------------------:|:---------------------:|:--------------------:|:-------------------:|:---------------------:|:-------------------------------------------------------------------------------:|
| RobustV2VNet [1]       | CoRL'20         | LiDAR            | I                    | Loc, Pos              | -                    | -                   | -                     | -                                                                               |
| AOMAC [2]              | ICCV'21         | LiDAR            | I                    | -                     | -                    | -                   | Attack                | -                                                                               |
| P-CNN [3]              | IoT'21          | Camera           | E                    | -                     | -                    | -                   | Privacy               | -                                                                               |
| FPV-RCNN [4]           | RAL'22          | LiDAR            | I                    | Loc, Pos              | -                    | -                   | -                     | [Link](https://github.com/YuanYunshuang/FPV_RCNN)                              |
| TCLF [5]               | CVPR'22         | LiDAR            | L                    | -                     | Laten                | -                   | -                     | [Link](https://github.com/AIR-THU/DAIR-V2X)                                     |
| V2X-ViT [6]            | ECCV'22         | LiDAR            | I                    | Loc, Pos              | Laten                | -                   | -                     | [Link](https://github.com/DerrickXuNu/v2x-vit)                                  |
| SyncNet [7]            | ECCV'22         | LiDAR            | I                    | -                     | Laten                | -                   | -                     | [Link](https://github.com/MediaBrain-SJTU/SyncNet)                              |
| TaskAgnostic [8]       | CoRL'23         | LiDAR            | I                    | -                     | -                    | Task                | -                     | [Link](https://github.com/coperception/star)                                    |
| SecPCV [9]             | TITS'22         | LiDAR            | E                    | -                     | -                    | -                   | Privacy               | -                                                                               |
| ModelAgnostic [10]     | ICRA'23         | LiDAR            | L                    | -                     | -                    | Model               | -                     | [Link](https://github.com/DerrickXuNu/model_anostic)                            |
| MPDA [11]              | ICRA'23         | LiDAR            | I                    | -                     | -                    | Model               | -                     | [Link](https://github.com/DerrickXuNu/MPDA)                                     |
| CoAlign [12]           | ICRA'23         | LiDAR            | I, L                 | Loc, Pos              | -                    | -                   | -                     | [Link](https://github.com/yifanlu0227/CoAlign)                                  |
| LCRN [13]              | TIV'23          | LiDAR            | L                    | -                     | Loss                 | -                   | -                     | -                                                                               |
| OptiMatch [14]         | IV'23           | LiDAR            | L                    | Loc, Pos              | -                    | -                   | -                     | -                                                                               |
| P2OD [15]              | IoT'23          | Camera           | E                    | -                     | -                    | -                   | Privacy               | -                                                                               |
| V2X-INCOP [16]         | arXiv'23        | LiDAR            | I                    | -                     | Inter                | -                   | -                     | -                                                                               |
| ROBOSAC [17]           | ICCV'23         | LiDAR            | I                    | -                     | -                    | -                   | Attack               | [Link](https://github.com/coperception/ROBOSAC)                                  |

Notes:
- Schemes include early (E), intermediate (I) and late (L) collaboration.
- **Loc Error** includes localization (**Loc**) and pose (**Pos**) errors.
- **Comm Issue** includes latency (**Laten**), interruption (**Inter**) and loss (**Loss**).
- **Discrep** includes model (**Model**) and task (**Task**) discrepancies.
- **Security** includes attack defense (**Attack**) and privacy protection (**Privacy**).

▶️ Go back to [Main Page](README.md)

## References:
1. [Learning to Communicate and Correct Pose Errors](https://arxiv.org/abs/2011.05289)
2. [Adversarial attacks on multi-agent communication](https://arxiv.org/abs/2101.06560)
3. [Toward lightweight, privacy-preserving cooperative object classification for connected autonomous vehicles](https://ieeexplore.ieee.org/document/9468670)
4. [Keypoints-Based Deep Feature Fusion for Cooperative Vehicle Detection of Autonomous Driving](https://arxiv.org/abs/2109.11615)
5. [DAIR-V2X: A Large-Scale Dataset for Vehicle-Infrastructure Cooperative 3D Object Detection](https://arxiv.org/abs/2204.05575)
6. [V2X-ViT: Vehicle-to-everything cooperative perception with vision transformer](https://arxiv.org/abs/2203.10638)
7. [Latency-Aware Collaborative Perception](https://arxiv.org/abs/2207.08560)
8. [Multi-robot scene completion: Towards task-agnostic collaborative perception](https://openreview.net/forum?id=hW0tcXOJas2)
9. [Edge-Cooperative Privacy-Preserving Object Detection Over Random Point Cloud Shares for Connected Autonomous Vehicles](https://ieeexplore.ieee.org/document/9928424)
10. [Model-Agnostic Multi-Agent Perception Framework](https://arxiv.org/abs/2203.13168)
11. [Bridging the Domain Gap for Multi-Agent Perception](https://arxiv.org/abs/2210.08451)
12. [Robust Collaborative 3D Object Detection in Presence of Pose Errors](https://arxiv.org/abs/2211.07214)
13. [Learning for Vehicle-to-Vehicle Cooperative Perception under Lossy Communication](https://arxiv.org/abs/2212.08273)
14. [A Cooperative Perception System Robust to Localization Errors](https://arxiv.org/abs/2210.06289)
15. [Achieving Lightweight and Privacy-Preserving Object Detection for Connected Autonomous Vehicles](https://ieeexplore.ieee.org/document/9913215)
16. [Interruption-Aware Cooperative Perception for V2X Communication-Aided Autonomous Driving](https://arxiv.org/abs/2304.11821)
17. [Among Us: Adversarially Robust Collaborative Perception by Consensus](https://arxiv.org/abs/2303.09495)
