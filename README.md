# <p align=center>Monocular Depth Estimation Rankings<br />and 2D to 3D Video Conversion Rankings</p>

## <p align=center>List of Rankings</p>
<p align=center>Each ranking includes only the best model for one method.</p>  

### Monocular Depth Estimation Rankings
1. [**UnrealStereo4K (3840×2160): AbsRel<=0.04**](#unrealstereo4k-38402160-absrel004)
1. [**MVS-Synth (1920×1080): AbsRel<=0.06**](#mvs-synth-19201080-absrel006)
1. [**HRSD (1920×1080): AbsRel<=0.08**](#hrsd-19201080-absrel008)
1. [**Middlebury2021 (1920×1080): SqRel<=0.5**](#middlebury2021-19201080-sqrel05)
1. [**NYU-Depth V2 (640×480): AbsRel<=0.056**](#nyu-depth-v2-640480-absrel0056)
### 2D to 3D Video Conversion Rankings
#### I. Video Inpainting Rankings
- (to do)
#### II. Light Field Video Reconstruction from Monocular Video Rankings
1. :crown: **4DLFVD with up to 10×10 real light field views✔️: LPIPS😍** (no data)  
*This will be the King of all rankings. We look forward to ambitious researchers.*
1. **4DLFVD with up to 10×10 real light field views✔️: PSNR😞** (no data)
1. **Hybrid with 7×7 synthetic light field views✖️: LPIPS😍** (no data) 
1. [**Hybrid with 7×7 synthetic light field views✖️: PSNR😞>=32dB**](#hybrid-with-77-synthetic-light-field-views%EF%B8%8F-psnr32db)
### Appendices
- **Appendix 1: Rules for qualifying models for the rankings** (to do)

--------------------

## UnrealStereo4K (3840×2160): AbsRel<=0.04
| RK | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | VapourSynth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | ZoeDepth +PF<sub>R=128</sub><br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2302.12288)<br />*ENH:*<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f "The link to the conference paper will be available in June. CVPR 2024: June 17th – 21st")](https://cvpr.thecvf.com/Conferences/2024) | **0.0388** {1}<br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2312.02284) | *ENH:*<br />UnrealStereo4K | [![GitHub Stars](https://img.shields.io/github/stars/isl-org/ZoeDepth?logo=GitHub&label=Stars)](https://github.com/isl-org/ZoeDepth)<br />*ENH:*<br />[![GitHub Stars](https://img.shields.io/github/stars/zhyever/PatchFusion?logo=GitHub&label=Stars)](https://github.com/zhyever/PatchFusion) | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## MVS-Synth (1920×1080): AbsRel<=0.06
| RK | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | VapourSynth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | ZoeDepth +PF<sub>R=128</sub><br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2302.12288)<br />*ENH:*<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f "The link to the conference paper will be available in June. CVPR 2024: June 17th – 21st")](https://cvpr.thecvf.com/Conferences/2024) | **0.0589** {1}<br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2312.02284) | *ENH:*<br />MVS-Synth | [![GitHub Stars](https://img.shields.io/github/stars/isl-org/ZoeDepth?logo=GitHub&label=Stars)](https://github.com/isl-org/ZoeDepth)<br />*ENH:*<br />[![GitHub Stars](https://img.shields.io/github/stars/zhyever/PatchFusion?logo=GitHub&label=Stars)](https://github.com/zhyever/PatchFusion) | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## HRSD (1920×1080): AbsRel<=0.08
| RK | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | VapourSynth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | DPT-B + R + AL<br />[![ICCV](https://img.shields.io/badge/2021-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2021/html/Ranftl_Vision_Transformers_for_Dense_Prediction_ICCV_2021_paper.html)<br />*ENH:*<br />[![CVPRW](https://img.shields.io/badge/2023-CVPRW-1e407f)](https://openaccess.thecvf.com/content/CVPR2023W/NTIRE/html/Rajpal_High-Resolution_Synthetic_RGB-D_Datasets_for_Monocular_Depth_Estimation_CVPRW_2023_paper.html) | **0.074** {1}<br />[![CVPRW](https://img.shields.io/badge/2023-CVPRW-1e407f)](https://openaccess.thecvf.com/content/CVPR2023W/NTIRE/html/Rajpal_High-Resolution_Synthetic_RGB-D_Datasets_for_Monocular_Depth_Estimation_CVPRW_2023_paper.html) | *ENH:*<br />HRSD | [![GitHub Stars](https://img.shields.io/github/stars/isl-org/DPT?logo=GitHub&label=Stars)](https://github.com/isl-org/DPT)<br />*ENH:*<br />- | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## Middlebury2021 (1920×1080): SqRel<=0.5
| RK | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;SqRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | VapourSynth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | LeReS-GBDMF<br />[![CVPR](https://img.shields.io/badge/2021-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2021/html/Yin_Learning_To_Recover_3D_Scene_Shape_From_a_Single_Image_CVPR_2021_paper.html)<br />*ENH:*<br />[![AAAI](https://img.shields.io/badge/2023-AAAI-fddfa0)](https://ojs.aaai.org/index.php/AAAI/article/view/25123) | **0.444** {1}<br />[![AAAI](https://img.shields.io/badge/2023-AAAI-fddfa0)](https://ojs.aaai.org/index.php/AAAI/article/view/25123) | *ENH:*<br />HR-WSI | [![GitHub Stars](https://img.shields.io/github/stars/aim-uofa/AdelaiDepth?logo=GitHub&label=Stars)](https://github.com/aim-uofa/AdelaiDepth)<br />*ENH:*<br />[![GitHub Stars](https://img.shields.io/github/stars/YuiNsky/Gradient-based-depth-map-fusion?logo=GitHub&label=Stars)](https://github.com/YuiNsky/Gradient-based-depth-map-fusion) | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## NYU-Depth V2 (640×480): AbsRel<=0.056
| RK | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | VapourSynth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | Metric3D v2 CSTM_label<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Yin_Metric3D_Towards_Zero-shot_Metric_3D_Prediction_from_A_Single_Image_ICCV_2023_paper.html)<br />*ENH:*<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2404.15506)<br />*Backbone:*<br />DINOv2 with registers (ViT-L/14) | **0.042** {1}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2404.15506) | DDAD & Lyft & Driving Stereo & DIML & Arogoverse2 & Cityscapes & DSEC & Mapillary PSD & Pandaset & UASOL & Virtual KITTI & Waymo & Matterport3d & Taskonomy & Replica & ScanNet & HM3d & Hypersim | [![GitHub Stars](https://img.shields.io/github/stars/YvanYin/Metric3D?logo=GitHub&label=Stars)](https://github.com/YvanYin/Metric3D) | - | - |
| 2 | Depth Anything Large<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f "The link to the conference paper will be available in June. CVPR 2024: June 17th – 21st")](https://cvpr.thecvf.com/Conferences/2024)<br />*Backbone:*<br />DINOv2 (ViT-L/14) | **0.043** {1}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2401.10891) | *Pretraining*: BlendedMVS & DIML & HR-WSI & IRS & MegaDepth & TartanAir<br />*Training*: BDD100K & Google Landmarks & ImageNet-21K & LSUN & Objects365 & Open Images V7 & Places365 & SA-1B | [![GitHub Stars](https://img.shields.io/github/stars/LiheYoung/Depth-Anything?logo=GitHub&label=Stars)](https://github.com/LiheYoung/Depth-Anything) | - | - |
| 3 | MiDaS v3.1 BEiT<sub>L-512</sub><br />[![TPAMI](https://img.shields.io/badge/2022-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/9178977)<br />*ENH:*<br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2307.14460)<br />*Backbone:*<br />BEiT<sub>512</sub>-L (ViT-L/16) | **0.048** {1}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2401.10891) | *Pretraining*: ReDWeb & HR-WSI & BlendedMVS & NYU-Depth V2 & KITTI<br />*Training*: ReDWeb & DIML & 3D Movies & MegaDepth & WSVD & TartanAir & HR-WSI & ApolloScape & BlendedMVS & IRS & NYU-Depth V2 & KITTI | [![GitHub Stars](https://img.shields.io/github/stars/isl-org/MiDaS?logo=GitHub&label=Stars)](https://github.com/isl-org/MiDaS) | - | [![PyTorch](https://img.shields.io/badge/PyTorch-ee4c2c?logo=PyTorch&logoColor=white)](https://github.com/HolyWu/vs-midas)<br />[![GitHub Stars](https://img.shields.io/github/stars/HolyWu/vs-midas?logo=GitHub&label=Stars)](https://github.com/HolyWu/vs-midas) |
| 4 | Marigold<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f "The link to the conference paper will be available in June. CVPR 2024: June 17th – 21st")](https://cvpr.thecvf.com/Conferences/2024)<br />*Backbone:*<br />text-to-image LDM (Stable Diffusion v2) | **0.055** {1}<br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2312.02145) | Hypersim & Virtual KITTI | [![GitHub Stars](https://img.shields.io/github/stars/prs-eth/Marigold?logo=GitHub&label=Stars)](https://github.com/prs-eth/Marigold) | - | - |
| 5 | GenPercept<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2403.06090)<br />*Backbone:*<br />VAE & U-Net (Stable Diffusion v2.1) | **0.056** {1}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2403.06090) | Hypersim & Virtual KITTI | [![GitHub Stars](https://img.shields.io/github/stars/aim-uofa/GenPercept?logo=GitHub&label=Stars)](https://github.com/aim-uofa/GenPercept) | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## Hybrid with 7×7 synthetic light field views✖️: PSNR😞>=32dB
| RK | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;PSNR&nbsp;↑&nbsp;&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | VapourSynth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | LFVRT<br />[![ECCV](https://img.shields.io/badge/2022-ECCV-67cd84)](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/4122_ECCV_2022_paper.php)<br />*MDE:* DPT<br />[![ICCV](https://img.shields.io/badge/2021-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2021/html/Ranftl_Vision_Transformers_for_Dense_Prediction_ICCV_2021_paper.html)<br />*Backbone:*<br />ViT | **32.66** {3+1D}<br />[![ECCV](https://img.shields.io/badge/2022-ECCV-67cd84)](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/4122_ECCV_2022_paper.php) | GoPro & TAMULF | [![GitHub Stars](https://img.shields.io/github/stars/ShrisudhanG/Synthesizing-Light-Field-Video-from-Monocular-Video?logo=GitHub&label=Stars)](https://github.com/ShrisudhanG/Synthesizing-Light-Field-Video-from-Monocular-Video)<br />*MDE:*<br />[![GitHub Stars](https://img.shields.io/github/stars/isl-org/DPT?logo=GitHub&label=Stars)](https://github.com/isl-org/DPT) | - | - |

📝 **Note:** The above ranking includes only one model, as the other methods are image-based and don't have any temporal information making them unsuitable for light field video reconstruction from monocular video.

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)
