# A summary of large-scale collaborative perception datasets

**Usage of Common Datasets** (from papers with code):
- [V2X-SIM](https://paperswithcode.com/dataset/v2x-sim) | [OPV2V](https://paperswithcode.com/dataset/opv2v) | [V2XSet](https://paperswithcode.com/dataset/v2xset) | [DAIR-V2X](https://paperswithcode.com/dataset/dair-v2x) | [V2V4Real](https://paperswithcode.com/dataset/v2v4real) | [DAIR-V2X-Seq](https://paperswithcode.com/dataset/dair-v2x-seq)


| **Dataset**      | **Venue** | **Source** | **Frame** | **V2V**  | **V2I** | **I2I**  | **Agents** | **Camera** | **LiDAR** | **Depth** | **OD**    | **SS**    | **OT**    | **MP**    | **Website**                                          |
|:----------------:|:---------:|:----------:|:---------:|:--------:|:--------:|:----------:|:----------:|:----------:|:---------:|:---------:|:---------:|:---------:|:---------:|:---------:|:----------------------------------------------------:|
| V2V-Sim [1]      | ECCV'20   | Simu       | 51K       | &#10004; | -        |  -   |  1-7        | -          | &#10004;  | -         | &#10004;  | -         | -         |  &#10004; | -                                                    |
| V2X-Sim [2]      | RAL'21    | Simu       | 10k       | &#10004; | &#10004; |  -   |1-5        | &#10004;   | &#10004;  | &#10004;  | &#10004;  |  &#10004; |  &#10004; | -         | [Link](https://ai4ce.github.io/V2X-Sim)              |
| OPV2V [3]        | ICRA'22   | Simu       | 11K       | &#10004; | -        |  -        |1-7        | &#10004;   | &#10004;  | -         | &#10004;  |  &#10004; | -         | -         | [Link](https://mobility-lab.seas.ucla.edu/opv2v)     |
| DAIR-V2X-C [4]   | CVPR'22   | Real       | 39k       | -        | &#10004; |  -    |2          | &#10004;   | &#10004;  | -         |  &#10004; | -         | -         | -         | [Link](https://thudair.baai.ac.cn/coop-dtest)        |
| V2XSet [5]       | ECCV'22   | Simu       | 11K       | &#10004; | &#10004; |  -    |2-5        | &#10004;   | &#10004;  | -         |  &#10004; | -         | -         | -         | [Link](https://github.com/DerrickXuNu/v2x-vit)       |
| DOLPHINS [6]     | ACCV'22   | Simu       | 42k       | &#10004; | &#10004; |  -    |3          | &#10004;   | &#10004;  | -         |  &#10004; | -         | -         | -         | [Link](https://dolphins-dataset.net)                 |
| V2V4Real [7]     | CVPR'23   | Real       | 20K       | &#10004; | -        |  -    |2          | &#10004;   | &#10004;  | -         |  &#10004; | -         |  &#10004; | -         | [Link](https://mobility-lab.seas.ucla.edu/v2v4real/) |
| V2X-Seq [8]      | CVPR'23   | Real       | 15k       | -        | &#10004; |  -    |2          | &#10004;   | &#10004;  | -         |  &#10004; | -         |  &#10004; |  &#10004; | [Link](https://thudair.baai.ac.cn/coop-forecast)     |
| DeepAccident [9] | AAAI'24  | Simu       | 57K       | &#10004; | &#10004; |  -    |1-5        | &#10004;   | &#10004;  | -         |  &#10004; |  &#10004; |  &#10004; |  &#10004; | [Link](https://deepaccident.github.io/index.html)    |
| HoloVIC [10] | CVPR'24  | Real       | 100K       | -             | &#10004; |  -    |2        | &#10004;   | &#10004;  | -         |  &#10004; |  -       |  &#10004; |  - | [Link](https://holovic.net/)    |
| TUMTraf-V2X [11] | CVPR'24  | Real       | 2K       | -             | &#10004; |  -    |2        | &#10004;   | &#10004;  | -         |  &#10004; |  -       |  &#10004; |  - | [Link](https://tum-traffic-dataset.github.io/tumtraf-v2x/)    |
| R-Cooper [12] | CVPR'24  | Real       | 30K       | -             | - |  &#10004;    | 2        | &#10004;   | &#10004;  | -         |  &#10004; |  -       |  &#10004; |  - | [Link](https://tum-traffic-dataset.github.io/tumtraf-v2x/)    |
| MARS [13] | CVPR'24  | Real       | 1.5k     | &#10004;           | - |  -    |2-3        | &#10004;   | &#10004;  | -         |  -|  -       |-|  - | [Link](https://ai4ce.github.io/MARS/)    |
| V2X-Real [14] | ECCV'24  | Real       | 33k     | &#10004;           | &#10004;  |  &#10004;   |2-4        | &#10004;   | &#10004;  | -    |  &#10004; |  -       |-|  - | [Link](https://github.com/ucla-mobility/V2X-Real)    |
| V2XPnP [15] | ICCV'25  | Real       | 44k     | &#10004;           | &#10004;  |  &#10004;   |2-4        | &#10004;   | &#10004;  | -    |  &#10004; |  -       |&#10004;|  &#10004; | [Link](https://mobility-lab.seas.ucla.edu/v2xpnp/)    |


Notes:
- Source: simulator (Simu) and real-world (Real).
- Frame refers to the annotated LiDAR-based cooperative perception frame number.
- Supported common perception tasks: 3D object detection (OD), BEV semantic segmentation (SS), 3D object tracking (OT), motion prediction (MP).


Back to [Contents](README.md) 🔙 

References:
1. [V2VNet: Vehicle-to-Vehicle Communication for Joint Perception and Prediction](https://arxiv.org/abs/2008.07519) (ECCV'20)
2. [V2X-Sim: Multi-Agent Collaborative Perception Dataset and Benchmark for Autonomous Driving](https://arxiv.org/abs/2202.08449) (RAL'21)
3. [OPV2V: An open benchmark dataset and fusion pipeline for perception with vehicle-to-vehicle communication](https://arxiv.org/abs/2109.07644) (ICRA'22)
4. [DAIR-V2X: A Large-Scale Dataset for Vehicle-Infrastructure Cooperative 3D Object Detection](https://arxiv.org/abs/2204.05575) (CVPR'22)
5. [V2X-ViT: Vehicle-to-everything cooperative perception with vision transformer](https://arxiv.org/abs/2203.10638) (ECCV'22)
6. [DOLPHINS: Dataset for Collaborative Perception enabled Harmonious and Interconnected Self-driving](https://arxiv.org/abs/2207.07609) (ACCV'22)
7. [V2V4Real: A Real-world Large-scale Dataset for Vehicle-to-Vehicle Cooperative Perception](https://arxiv.org/abs/2303.07601) (CVPR'23)
8. [V2X-Seq: A large-scale sequential dataset for vehicle-infrastructure cooperative perception and forecasting](https://arxiv.org/abs/2305.05938) (CVPR'23)
9. [DeepAccident: A Motion and Accident Prediction Benchmark for V2X Autonomous Driving](https://arxiv.org/abs/2304.01168) (AAAI'24)
10. [HoloVIC: Large-scale Dataset and Benchmark for Multi-Sensor Holographic Intersection and Vehicle-Infrastructure Cooperative](https://arxiv.org/abs/2403.02640) (CVPR'24)
11. [TUMTraf V2X Cooperative Perception Dataset](https://arxiv.org/abs/2403.01316) (CVPR'24)
12. [RCooper: A Real-world Large-scale Dataset for Roadside Cooperative Perception](https://arxiv.org/abs/2403.10145) (CVPR'24)
13. [Multiagent Multitraversal Multimodal Self-Driving: Open MARS Dataset](https://openaccess.thecvf.com/content/CVPR2024/papers/Li_Multiagent_Multitraversal_Multimodal_Self-Driving_Open_MARS_Dataset_CVPR_2024_paper.pdf) (CVPR'24)
14. [V2X-Real: a Largs-Scale Dataset for Vehicle-to-Everything Cooperative Perception](https://arxiv.org/abs/2403.16034) (ECCV'24)
15. [V2XPnP: Vehicle-to-Everything Spatio-Temporal Fusion for Multi-Agent Perception and Prediction](https://arxiv.org/abs/2412.01812) (ICCV'25)
   
