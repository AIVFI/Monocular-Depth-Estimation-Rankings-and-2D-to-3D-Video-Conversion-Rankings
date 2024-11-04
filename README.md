# <p align=center>Monocular Depth Estimation Rankings<br />and 2D to 3D Video Conversion Rankings</p>

## <p align=center>List of Rankings</p>

### Monocular Depth Estimation Rankings
#### I. New layout
1. [**ScanNet++ (98 video clips with 32 frames each): TAE**](#scannet-98-video-clips-with-32-frames-each-tae)
1. [**NYU-Depth V2: OPW<=0.37**](#nyu-depth-v2-opw037)
1. [**NYU-Depth V2: AbsRel<=0.045 [test: new layout]**](#nyu-depth-v2-absrel0045-test-new-layout)
#### II. Old layout [currently no longer up to date]
1. [**NYU-Depth V2 (640×480): AbsRel<=0.058 [currently no longer up to date]**](#nyu-depth-v2-640480-absrel0058-currently-no-longer-up-to-date)
1. [**DA-2K (mostly 1500×2000): Acc (%)>=86**](#da-2k-mostly-15002000-acc-86)
1. [**UnrealStereo4K (3840×2160): AbsRel<=0.04**](#unrealstereo4k-38402160-absrel004)
1. [**Middlebury2021 (1920×1080): SqRel<=0.5**](#middlebury2021-19201080-sqrel05)

### 2D to 3D Video Conversion Rankings
#### I. Light Field Video Reconstruction from Monocular Video Rankings
1. **Hybrid with 7×7 synthetic light field views✖️: LPIPS😍** (no data) 
1. [**Hybrid with 7×7 synthetic light field views✖️: PSNR😞>=32dB**](#hybrid-with-77-synthetic-light-field-views%EF%B8%8F-psnr32db)
### Appendices
- **Appendix 1: Rules for qualifying models for the rankings** (to do)
- **Appendix 2: Metrics selection for the rankings** (to do)
- [**Appendix 3: List of all research papers from the above rankings**](#appendix-3-list-of-all-research-papers-from-the-above-rankings)

--------------------

## ScanNet++ (98 video clips with 32 frames each): TAE
| RK | Model <br />*Links:*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;Repository&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;TAE&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2410.10815)<br />DAV |
|:---:|:---:|:---:|
| 1 | **Depth Any Video**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2410.10815) [![GitHub Stars](https://img.shields.io/github/stars/Nightmare-n/DepthAnyVideo?logo=GitHub&label=Stars)](https://github.com/Nightmare-n/DepthAnyVideo) | **2.1** {MF} |
| 2 | **DepthCrafter**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2409.02095) [![GitHub Stars](https://img.shields.io/github/stars/Tencent/DepthCrafter?logo=GitHub&label=Stars)](https://github.com/Tencent/DepthCrafter) | **2.2** {MF} |
| 3 | **ChronoDepth**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2406.01493) [![GitHub Stars](https://img.shields.io/github/stars/jhaoshao/ChronoDepth)](https://github.com/jhaoshao/ChronoDepth) | **2.3** {MF} |
| 4 | **NVDS**<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_Neural_Video_Depth_Stabilizer_ICCV_2023_paper.html) [![GitHub Stars](https://img.shields.io/github/stars/RaymondWang987/NVDS?logo=GitHub&label=Stars)](https://github.com/RaymondWang987/NVDS) | **3.7** {4} |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## NYU-Depth V2: OPW<=0.37
| RK | Model <br />*Links:*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;Repository&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;OPW&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2403.12953)<br />FD | &nbsp;&nbsp;&nbsp;OPW&nbsp;↓&nbsp;&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10707178)<br />NVDS<sup>+</sup> | &nbsp;&nbsp;OPW&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_Neural_Video_Depth_Stabilizer_ICCV_2023_paper.html)<br />NVDS |
|:---:|:---:|:---:|:---:|:---:|
| 1 | **FutureDepth**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2403.12953) | **0.303** {4} | - | - |
| 2 | **NVDS<sup>+</sup>**<br />[![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10707178) [![GitHub Stars](https://img.shields.io/github/stars/RaymondWang987/NVDS?logo=GitHub&label=Stars)](https://github.com/RaymondWang987/NVDS) | - | **0.339** {4} | - |
| 3 | **NVDS**<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_Neural_Video_Depth_Stabilizer_ICCV_2023_paper.html) [![GitHub Stars](https://img.shields.io/github/stars/RaymondWang987/NVDS?logo=GitHub&label=Stars)](https://github.com/RaymondWang987/NVDS) | **0.364** {4} | - | **0.364** {4} |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## NYU-Depth V2: AbsRel<=0.045 [test: new layout]
| RK | Model <br />*Links:*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;Repository&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2407.17952)<br />BD | &nbsp;&nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10638254)<br />M3D v2 | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Depth_Anything_Unleashing_the_Power_of_Large-Scale_Unlabeled_Data_CVPR_2024_paper.html)<br />DA | &nbsp;&nbsp;&nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![NeurIPS](https://img.shields.io/badge/2024-NeurIPS-68448a)](https://arxiv.org/abs/2406.09414)<br />DA V2 | - | - | - | - |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1-2 | **BetterDepth**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2407.17952) | **0.042** {1} | - | - | - | - | - | - | - |
| 1-2 | **Metric3D v2 ViT-Large**<br />[![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10638254) [![GitHub Stars](https://img.shields.io/github/stars/YvanYin/Metric3D?logo=GitHub&label=Stars)](https://github.com/YvanYin/Metric3D) | - | **0.042** {1} | - | - | - | - | - | - |
| 3 | **Depth Anything Large**<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Depth_Anything_Unleashing_the_Power_of_Large-Scale_Unlabeled_Data_CVPR_2024_paper.html) [![GitHub Stars](https://img.shields.io/github/stars/LiheYoung/Depth-Anything?logo=GitHub&label=Stars)](https://github.com/LiheYoung/Depth-Anything) | **0.043** {1} | **0.043** {1} | **0.043** {1} | **0.043** {1} | - | - | - | - |
| 4 | **Depth Anything V2 Large**<br />[![NeurIPS](https://img.shields.io/badge/2024-NeurIPS-68448a)](https://arxiv.org/abs/2406.09414) [![GitHub Stars](https://img.shields.io/github/stars/DepthAnything/Depth-Anything-V2?logo=GitHub&label=Stars)](https://github.com/DepthAnything/Depth-Anything-V2) | - | - | - | **0.045** {1} | - | - | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## NYU-Depth V2 (640×480): AbsRel<=0.058 [currently no longer up to date]
| RK | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | Vapour-<br />Synth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1-2 | BetterDepth<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2407.17952)<br />*Backbone:*<br />Depth Anything & Marigold | **0.042** {1}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2407.17952) | Hypersim & Virtual KITTI | - | - | - |
| 1-2 | Metric3D v2 CSTM_label<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Yin_Metric3D_Towards_Zero-shot_Metric_3D_Prediction_from_A_Single_Image_ICCV_2023_paper.html)<br />*ENH:*<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2404.15506)<br />*Backbone:*<br />DINOv2 with registers (ViT-L/14) | **0.042** {1}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2404.15506) | DDAD & Lyft & Driving Stereo & DIML & Arogoverse2 & Cityscapes & DSEC & Mapillary PSD & Pandaset & UASOL & Virtual KITTI & Waymo & Matterport3d & Taskonomy & Replica & ScanNet & HM3d & Hypersim | [![GitHub Stars](https://img.shields.io/github/stars/YvanYin/Metric3D?logo=GitHub&label=Stars)](https://github.com/YvanYin/Metric3D) | - | - |
| 3 | Depth Anything Large<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Depth_Anything_Unleashing_the_Power_of_Large-Scale_Unlabeled_Data_CVPR_2024_paper.html)<br />*Backbone:*<br />DINOv2 (ViT-L/14) | **0.043** {1}<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Depth_Anything_Unleashing_the_Power_of_Large-Scale_Unlabeled_Data_CVPR_2024_paper.html) | *Pretraining*: BlendedMVS & DIML & HR-WSI & IRS & MegaDepth & TartanAir<br />*Training*: BDD100K & Google Landmarks & ImageNet-21K & LSUN & Objects365 & Open Images V7 & Places365 & SA-1B | [![GitHub Stars](https://img.shields.io/github/stars/LiheYoung/Depth-Anything?logo=GitHub&label=Stars)](https://github.com/LiheYoung/Depth-Anything) | - | - |
| 4 | MiDaS v3.1 BEiT<sub>L-512</sub><br />[![TPAMI](https://img.shields.io/badge/2022-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/9178977)<br />*ENH:*<br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2307.14460)<br />*Backbone:*<br />BEiT<sub>512</sub>-L (ViT-L/16) | **0.048** {1}<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Depth_Anything_Unleashing_the_Power_of_Large-Scale_Unlabeled_Data_CVPR_2024_paper.html) | *Pretraining*: ReDWeb & HR-WSI & BlendedMVS & NYU-Depth V2 & KITTI<br />*Training*: ReDWeb & DIML & 3D Movies & MegaDepth & WSVD & TartanAir & HR-WSI & ApolloScape & BlendedMVS & IRS & NYU-Depth V2 & KITTI | [![GitHub Stars](https://img.shields.io/github/stars/isl-org/MiDaS?logo=GitHub&label=Stars)](https://github.com/isl-org/MiDaS) | - | [![PyTorch](https://img.shields.io/badge/PyTorch-ee4c2c?logo=PyTorch&logoColor=white)](https://github.com/HolyWu/vs-midas)<br />[![GitHub Stars](https://img.shields.io/github/stars/HolyWu/vs-midas?logo=GitHub&label=Stars)](https://github.com/HolyWu/vs-midas) |
| 5 | GeoWizard<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2403.12013)<br />*Backbone:*<br />Stable Diffusion v2 | **0.052** {1}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2403.12013) | Hypersim & Replica & 3D Ken Burns & Objaverse & proprietary | [![GitHub Stars](https://img.shields.io/github/stars/fuxiao0719/GeoWizard?logo=GitHub&label=Stars)](https://github.com/fuxiao0719/GeoWizard) | - | - |
| 6 | Marigold<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Ke_Repurposing_Diffusion-Based_Image_Generators_for_Monocular_Depth_Estimation_CVPR_2024_paper.html)<br />*Backbone:*<br />Stable Diffusion v2 | **0.055** {1}<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Ke_Repurposing_Diffusion-Based_Image_Generators_for_Monocular_Depth_Estimation_CVPR_2024_paper.html) | Hypersim & Virtual KITTI | [![GitHub Stars](https://img.shields.io/github/stars/prs-eth/Marigold?logo=GitHub&label=Stars)](https://github.com/prs-eth/Marigold) | - | - |
| 7 | GenPercept<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2403.06090)<br />*Backbone:*<br />Stable Diffusion v2.1 | **0.056** {1}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2403.06090) | Hypersim & Virtual KITTI | [![GitHub Stars](https://img.shields.io/github/stars/aim-uofa/GenPercept?logo=GitHub&label=Stars)](https://github.com/aim-uofa/GenPercept) | - | - |
| 8 | NeWCRFs + LightedDepth<br />[![CVPR](https://img.shields.io/badge/2022-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2022/html/Yuan_Neural_Window_Fully-Connected_CRFs_for_Monocular_Depth_Estimation_CVPR_2022_paper.html)<br />*ENH:*<br />[![CVPR](https://img.shields.io/badge/2023-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2023/html/Zhu_LightedDepth_Video_Depth_Estimation_in_Light_of_Limited_Inference_View_CVPR_2023_paper.html) | **0.057** {2}<br />[![CVPR](https://img.shields.io/badge/2023-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2023/html/Zhu_LightedDepth_Video_Depth_Estimation_in_Light_of_Limited_Inference_View_CVPR_2023_paper.html) | *ENH:*<br />NYU-Depth V2 | [![GitHub Stars](https://img.shields.io/github/stars/aliyun/NeWCRFs?logo=GitHub&label=Stars)](https://github.com/aliyun/NeWCRFs)<br />*ENH:*<br />[![GitHub Stars](https://img.shields.io/github/stars/ShngJZ/LightedDepth?logo=GitHub&label=Stars)](https://github.com/ShngJZ/LightedDepth) | - | - |
| 9 | UniDepth-V<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Piccinelli_UniDepth_Universal_Monocular_Metric_Depth_Estimation_CVPR_2024_paper.html)<br />*Backbone:*<br />DINOv2 (ViT-L/14) | **0.0578** {1}<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Piccinelli_UniDepth_Universal_Monocular_Metric_Depth_Estimation_CVPR_2024_paper.html) | A2D2 & Argoverse2 & BDD100k & CityScapes & DrivingStereo & Mapillary PSD & ScanNet & Taskonomy & Waymo | [![GitHub Stars](https://img.shields.io/github/stars/lpiccinelli-eth/UniDepth?logo=GitHub&label=Stars)](https://github.com/lpiccinelli-eth/UniDepth) | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## DA-2K (mostly 1500×2000): Acc (%)>=86
| RK | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;Acc&nbsp;(%)&nbsp;↑&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | Vapour-<br />Synth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | Depth Anything V2 Giant<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Depth_Anything_Unleashing_the_Power_of_Large-Scale_Unlabeled_Data_CVPR_2024_paper.html)<br />*ENH:*<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2406.09414)<br />*Backbone:*<br />DINOv2 (ViT-G/14) | **97.4** {1}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2406.09414) | *Pretraining*: BlendedMVS & Hypersim & IRS & TartanAir & VKITTI 2<br />*Training*: BDD100K & Google Landmarks & ImageNet-21K & LSUN & Objects365 & Open Images V7 & Places365 & SA-1B | [![GitHub Stars](https://img.shields.io/github/stars/LiheYoung/Depth-Anything?logo=GitHub&label=Stars)](https://github.com/LiheYoung/Depth-Anything)<br />*ENH:*<br />[![GitHub Stars](https://img.shields.io/github/stars/DepthAnything/Depth-Anything-V2?logo=GitHub&label=Stars)](https://github.com/DepthAnything/Depth-Anything-V2) | - | - |
| 2 | GeoWizard<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2403.12013)<br />*Backbone:*<br />Stable Diffusion v2 | **88.1** {1}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2406.09414) | Hypersim & Replica & 3D Ken Burns & Objaverse & proprietary | [![GitHub Stars](https://img.shields.io/github/stars/fuxiao0719/GeoWizard?logo=GitHub&label=Stars)](https://github.com/fuxiao0719/GeoWizard) | - | - |
| 3 | Marigold<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Ke_Repurposing_Diffusion-Based_Image_Generators_for_Monocular_Depth_Estimation_CVPR_2024_paper.html)<br />*Backbone:*<br />Stable Diffusion v2 | **86.8** {1}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2406.09414) | Hypersim & Virtual KITTI | [![GitHub Stars](https://img.shields.io/github/stars/prs-eth/Marigold?logo=GitHub&label=Stars)](https://github.com/prs-eth/Marigold) | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## UnrealStereo4K (3840×2160): AbsRel<=0.04
| RK | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | Vapour-<br />Synth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | ZoeDepth +PF<sub>R=128</sub><br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2302.12288)<br />*ENH:*<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Li_PatchFusion_An_End-to-End_Tile-Based_Framework_for_High-Resolution_Monocular_Metric_Depth_CVPR_2024_paper.html) | **0.0388** {1}<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Li_PatchFusion_An_End-to-End_Tile-Based_Framework_for_High-Resolution_Monocular_Metric_Depth_CVPR_2024_paper.html) | *ENH:*<br />UnrealStereo4K | [![GitHub Stars](https://img.shields.io/github/stars/isl-org/ZoeDepth?logo=GitHub&label=Stars)](https://github.com/isl-org/ZoeDepth)<br />*ENH:*<br />[![GitHub Stars](https://img.shields.io/github/stars/zhyever/PatchFusion?logo=GitHub&label=Stars)](https://github.com/zhyever/PatchFusion) | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## Middlebury2021 (1920×1080): SqRel<=0.5
| RK | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;SqRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | VapourSynth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | LeReS-GBDMF<br />[![CVPR](https://img.shields.io/badge/2021-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2021/html/Yin_Learning_To_Recover_3D_Scene_Shape_From_a_Single_Image_CVPR_2021_paper.html)<br />*ENH:*<br />[![AAAI](https://img.shields.io/badge/2023-AAAI-fddfa0)](https://ojs.aaai.org/index.php/AAAI/article/view/25123) | **0.444** {1}<br />[![AAAI](https://img.shields.io/badge/2023-AAAI-fddfa0)](https://ojs.aaai.org/index.php/AAAI/article/view/25123) | *ENH:*<br />HR-WSI | [![GitHub Stars](https://img.shields.io/github/stars/aim-uofa/AdelaiDepth?logo=GitHub&label=Stars)](https://github.com/aim-uofa/AdelaiDepth)<br />*ENH:*<br />[![GitHub Stars](https://img.shields.io/github/stars/YuiNsky/Gradient-based-depth-map-fusion?logo=GitHub&label=Stars)](https://github.com/YuiNsky/Gradient-based-depth-map-fusion) | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)



## Hybrid with 7×7 synthetic light field views✖️: PSNR😞>=32dB
| RK | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;PSNR&nbsp;↑&nbsp;&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | VapourSynth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | LFVRT<br />[![ECCV](https://img.shields.io/badge/2022-ECCV-67cd84)](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/4122_ECCV_2022_paper.php)<br />*MDE:* DPT<br />[![ICCV](https://img.shields.io/badge/2021-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2021/html/Ranftl_Vision_Transformers_for_Dense_Prediction_ICCV_2021_paper.html)<br />*Backbone:*<br />ViT | **32.66** {3+1D}<br />[![ECCV](https://img.shields.io/badge/2022-ECCV-67cd84)](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/4122_ECCV_2022_paper.php) | GoPro & TAMULF | [![GitHub Stars](https://img.shields.io/github/stars/ShrisudhanG/Synthesizing-Light-Field-Video-from-Monocular-Video?logo=GitHub&label=Stars)](https://github.com/ShrisudhanG/Synthesizing-Light-Field-Video-from-Monocular-Video)<br />*MDE:*<br />[![GitHub Stars](https://img.shields.io/github/stars/isl-org/DPT?logo=GitHub&label=Stars)](https://github.com/isl-org/DPT) | - | - |

📝 **Note:** The above ranking includes only one model, as the other methods are image-based and don't have any temporal information making them unsuitable for light field video reconstruction from monocular video.

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## Appendix 3: List of all research papers from the above rankings

| Method | Paper | &nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;&nbsp; |
|:---:|:---:|:---:|
| BetterDepth | BetterDepth: Plug-and-Play Diffusion Refiner for Zero-Shot Monocular Depth Estimation | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2407.17952) |
| ChronoDepth | Learning Temporally Consistent Video Depth from Video Diffusion Priors | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2406.01493) |
| Depth Any Video | Depth Any Video with Scalable Synthetic Data | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2410.10815) |
| Depth Anything | Depth Anything: Unleashing the Power of Large-Scale Unlabeled Data | [![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Depth_Anything_Unleashing_the_Power_of_Large-Scale_Unlabeled_Data_CVPR_2024_paper.html) |
| Depth Anything V2 | Depth Anything V2 | [![NeurIPS](https://img.shields.io/badge/2024-NeurIPS-68448a)](https://arxiv.org/abs/2406.09414) |
| DepthCrafter | DepthCrafter: Generating Consistent Long Depth Sequences for Open-world Videos | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2409.02095) |
| DPT | Vision Transformers for Dense Prediction | [![ICCV](https://img.shields.io/badge/2021-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2021/html/Ranftl_Vision_Transformers_for_Dense_Prediction_ICCV_2021_paper.html) |
| FutureDepth | FutureDepth: Learning to Predict the Future Improves Video Depth Estimation | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2403.12953) |
| GBDMF | Multi-Resolution Monocular Depth Map Fusion by Self-Supervised Gradient-Based Composition | [![AAAI](https://img.shields.io/badge/2023-AAAI-fddfa0)](https://ojs.aaai.org/index.php/AAAI/article/view/25123) |
| GenPercept | Diffusion Models Trained with Large Data Are Transferable Visual Models | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2403.06090) |
| GeoWizard | GeoWizard: Unleashing the Diffusion Priors for 3D Geometry Estimation from a Single Image | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2403.12013) |
| LeReS | Learning to Recover 3D Scene Shape from a Single Image | [![CVPR](https://img.shields.io/badge/2021-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2021/html/Yin_Learning_To_Recover_3D_Scene_Shape_From_a_Single_Image_CVPR_2021_paper.html) |
| LightedDepth | LightedDepth: Video Depth Estimation in light of Limited Inference View Angles | [![CVPR](https://img.shields.io/badge/2023-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2023/html/Zhu_LightedDepth_Video_Depth_Estimation_in_Light_of_Limited_Inference_View_CVPR_2023_paper.html) |
| LFVRT | Synthesizing Light Field Video from Monocular Video | [![ECCV](https://img.shields.io/badge/2022-ECCV-67cd84)](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/4122_ECCV_2022_paper.php) |
| Marigold | Repurposing Diffusion-Based Image Generators for Monocular Depth Estimation | [![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Ke_Repurposing_Diffusion-Based_Image_Generators_for_Monocular_Depth_Estimation_CVPR_2024_paper.html) |
| Metric3D | Metric3D: Towards Zero-shot Metric 3D Prediction from A Single Image | [![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Yin_Metric3D_Towards_Zero-shot_Metric_3D_Prediction_from_A_Single_Image_ICCV_2023_paper.html) |
| Metric3D v2 | Metric3D v2: A Versatile Monocular Geometric Foundation Model for Zero-shot Metric Depth and Surface Normal Estimation | [![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10638254) |
| MiDaS | Towards Robust Monocular Depth Estimation: Mixing Datasets for Zero-Shot Cross-Dataset Transfer | [![TPAMI](https://img.shields.io/badge/2022-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/9178977) |
| MiDaS v3.1 | MiDaS v3.1 – A Model Zoo for Robust Monocular Relative Depth Estimation | [![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2307.14460) |
| NeWCRFs | Neural Window Fully-connected CRFs for Monocular Depth Estimation | [![CVPR](https://img.shields.io/badge/2022-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2022/html/Yuan_Neural_Window_Fully-Connected_CRFs_for_Monocular_Depth_Estimation_CVPR_2022_paper.html) |
| NVDS | Neural Video Depth Stabilizer | [![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_Neural_Video_Depth_Stabilizer_ICCV_2023_paper.html) |
| NVDS<sup>+</sup> | NVDS<sup>+</sup>: Towards Efficient and Versatile Neural Stabilizer for Video Depth Estimation | [![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10707178) |
| PatchFusion | PatchFusion: An End-to-End Tile-Based Framework for High-Resolution Monocular Metric Depth Estimation | [![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Li_PatchFusion_An_End-to-End_Tile-Based_Framework_for_High-Resolution_Monocular_Metric_Depth_CVPR_2024_paper.html) |
| UniDepth | UniDepth: Universal Monocular Metric Depth Estimation | [![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Piccinelli_UniDepth_Universal_Monocular_Metric_Depth_Estimation_CVPR_2024_paper.html) |
| ZoeDepth | ZoeDepth: Zero-shot Transfer by Combining Relative and Metric Depth | [![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2302.12288) |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)
