# <p align=center>Monocular Depth Estimation Rankings<br />and Light Field Video Reconstruction<br />from Monocular Video Rankings</p>

This is a very early version and I will gradually add new rankings and expand the existing ones.

In the near future I will write a little more information about what inspired me to add it and how it relates to my first repository: [Video Frame Interpolation Rankings and Video Deblurring Rankings](https://github.com/AIVFI/Video-Frame-Interpolation-Rankings-and-Video-Deblurring-Rankings)

## <p align=center>List of Rankings</p>
<p align=center>Each ranking includes only the best model for one method.</p>  

### Light Field Video Reconstruction from Monocular Video Rankings
1. :crown: **4DLFVD with up to 10×10 real light field views✔️: LPIPS😍** (no data)  
*This will be the King of all rankings. We look forward to ambitious researchers.*
1. **4DLFVD with up to 10×10 real light field views✔️: PSNR😞** (no data)
1. **Hybrid with 7×7 synthetic light field views✖️: LPIPS😍** (no data) 
1. [**Hybrid with 7×7 synthetic light field views✖️: PSNR😞>=32dB**](#hybrid-with-77-synthetic-light-field-views%EF%B8%8F-psnr32db)
### Monocular Depth Estimation Rankings
1. [**UnrealStereo4K (3840×2160): AbsRel<=0.04**](#unrealstereo4k-38402160-absrel004)
1. [**NYU-Depth V2 (640×480): AbsRel<=0.055**](#nyu-depth-v2-640480-absrel0055)
### Appendices
- **Appendix 1: Rules for qualifying models for the rankings** (to do)

--------------------

## Hybrid with 7×7 synthetic light field views✖️: PSNR😞>=32dB
| Rank | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;PSNR&nbsp;↑&nbsp;&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | VapourSynth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | LFVRT<br />[![ECCV](https://img.shields.io/badge/2022-ECCV-67cd84)](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/4122_ECCV_2022_paper.php)<br />*MDE:* DPT<br />[![ICCV](https://img.shields.io/badge/2021-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2021/html/Ranftl_Vision_Transformers_for_Dense_Prediction_ICCV_2021_paper.html)<br />*Backbone:*<br />ViT | **32.66** {3+1D}<br />[![ECCV](https://img.shields.io/badge/2022-ECCV-67cd84)](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/4122_ECCV_2022_paper.php) | GoPro & TAMULF | [![GitHub Stars](https://img.shields.io/github/stars/ShrisudhanG/Synthesizing-Light-Field-Video-from-Monocular-Video?logo=GitHub&label=Stars)](https://github.com/ShrisudhanG/Synthesizing-Light-Field-Video-from-Monocular-Video)<br />*MDE:*<br />[![GitHub Stars](https://img.shields.io/github/stars/isl-org/DPT?logo=GitHub&label=Stars)](https://github.com/isl-org/DPT) | - | - |

📝 **Note:** The above ranking includes only one model, as the other methods are image-based and don't have any temporal information making them unsuitable for light field video reconstruction from monocular video.

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-light-field-video-reconstructionfrom-monocular-video-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## UnrealStereo4K (3840×2160): AbsRel<=0.04
| Rank | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | Vapour Synth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | ZoeDepth +PF<sub>R=128</sub><br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2302.12288)<br />*Enhancement:*<br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2312.02284) | **0.0388** {1}<br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2312.02284) | *Pretraining*: NYU-Depth V2<br />*Training*: UnrealStereo4K | [![GitHub Stars](https://img.shields.io/github/stars/isl-org/ZoeDepth?logo=GitHub&label=Stars)](https://github.com/isl-org/ZoeDepth)<br />*Enhancement:*<br />[![GitHub Stars](https://img.shields.io/github/stars/zhyever/PatchFusion?logo=GitHub&label=Stars)](https://github.com/zhyever/PatchFusion) | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-light-field-video-reconstructionfrom-monocular-video-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## NYU-Depth V2 (640×480): AbsRel<=0.055
| Rank | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | VapourSynth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | Depth Anything<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2401.10891)<br />*Backbone:*<br />ViT-L | **0.043** {1}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2401.10891) | BlendedMVS & DIML & HRWSI & IRS & MegaDepth & TartanAir & BDD100K & Google Landmarks & ImageNet-21K & LSUN & Objects365 & Open Images V7 & Places365 & SA-1B | [![GitHub Stars](https://img.shields.io/github/stars/LiheYoung/Depth-Anything?logo=GitHub&label=Stars)](https://github.com/LiheYoung/Depth-Anything) | - | - |
| 2 |  | **0.048** {1}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2401.10891) |  |  | - | - |
| 3 | Metric3D CSTM_label<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Yin_Metric3D_Towards_Zero-shot_Metric_3D_Prediction_from_A_Single_Image_ICCV_2023_paper.html)<br />*Backbone:*<br />ConvNeXt-L | **0.050** {1}<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Yin_Metric3D_Towards_Zero-shot_Metric_3D_Prediction_from_A_Single_Image_ICCV_2023_paper.html) | DDAD & Lyft & Driving Stereo & DIML & Arogoverse2 & Cityscapes & DSEC & Mapillary PSD & Pandaset & UASOL & Taskonomy | [![GitHub Stars](https://img.shields.io/github/stars/YvanYin/Metric3D?logo=GitHub&label=Stars)](https://github.com/YvanYin/Metric3D) | - | - |
| 4 | DPT<br />[![ICCV](https://img.shields.io/badge/2021-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2021/html/Ranftl_Vision_Transformers_for_Dense_Prediction_ICCV_2021_paper.html)<br />*Backbone:*<br />BEiT-L | **0.054** {1}<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Spencer_Kick_Back__Relax_Learning_to_Reconstruct_the_World_by_ICCV_2023_paper.html) | DIML Indoor & MegaDepth & ReDWeb & WSVD & 3D Movies & ApolloScape & IRS & TartanAir & HR-WSI & BlendedMVS & NYU-Depth V2 | [![GitHub Stars](https://img.shields.io/github/stars/isl-org/DPT?logo=GitHub&label=Stars)](https://github.com/isl-org/DPT) | - | - |
| 5 | Marigold<br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2312.02145)<br />*Backbone:*<br />Stable Diffusion v2 | **0.055** {1}<br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2312.02145) | Hypersim & Virtual KITTI | [![GitHub Stars](https://img.shields.io/github/stars/prs-eth/Marigold?logo=GitHub&label=Stars)](https://github.com/prs-eth/Marigold) | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-light-field-video-reconstructionfrom-monocular-video-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)
