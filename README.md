# <p align=center>Monocular Video Depth Estimation Rankings<br />and Light Field Video Reconstruction<br />from Monocular Video Rankings</p>

This is a very early version and I will gradually add new rankings and expand the existing ones.

In the near future I will write a little more information about what inspired me to add it and how it relates to my first repository: [Video Frame Interpolation Rankings and Video Deblurring Rankings](https://github.com/AIVFI/Video-Frame-Interpolation-Rankings-and-Video-Deblurring-Rankings)

## <p align=center>List of Rankings</p>
<p align=center>Each ranking includes only the best model for one method.</p>  

### Light Field Video Reconstruction from Monocular Video Rankings
1. :crown: **4DLFVD with up to 10×10 real light field views:heavy_check_mark:: LPIPS:heart_eyes:** (no data)  
*This will be the King of all rankings. We look forward to ambitious researchers.*
1. **4DLFVD with up to 10×10 real light field views:heavy_check_mark:: PSNR:disappointed:** (no data)
1. **Hybrid with 7×7 synthetic light field views:bangbang:: LPIPS:heart_eyes:** (no data) 
1. [**Hybrid with 7×7 synthetic light field views:bangbang:: PSNR:disappointed:>=32dB**](#hybrid-with-77-synthetic-light-field-viewsbangbang-psnrdisappointed32db)
### Monocular Video Depth Estimation Rankings
1. **NYU-Depth V2: OPW**
1. [**NYU-Depth V2: AbsRel<=0.054**](#nyu-depth-v2-absrel0054)
### Appendices
- **Rules for qualifying models for the rankings** (to do)

--------------------

## Hybrid with 7×7 synthetic light field views:bangbang:: PSNR:disappointed:>=32dB
| Rank | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;PSNR&nbsp;↑&nbsp;&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | VapourSynth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | LFVRT<br />[![ECCV](https://img.shields.io/badge/2022-ECCV-67cd84)](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/4122_ECCV_2022_paper.php)<br />*MDE:* DPT<br />[![ICCV](https://img.shields.io/badge/2021-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2021/html/Ranftl_Vision_Transformers_for_Dense_Prediction_ICCV_2021_paper.html)<br />*Backbone:*<br />ViT<br />[![ICLR](https://img.shields.io/badge/2021-ICLR-d5df32)](https://openreview.net/forum?id=YicbFdNTTy) | **32.66** {3+1D}<br />[![ECCV](https://img.shields.io/badge/2022-ECCV-67cd84)](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/4122_ECCV_2022_paper.php) | GoPro & TAMULF | [![GitHub Stars](https://img.shields.io/github/stars/ShrisudhanG/Synthesizing-Light-Field-Video-from-Monocular-Video?logo=GitHub&label=Stars)](https://github.com/ShrisudhanG/Synthesizing-Light-Field-Video-from-Monocular-Video)<br />*MDE:*<br />[![GitHub Stars](https://img.shields.io/github/stars/isl-org/DPT?logo=GitHub&label=Stars)](https://github.com/isl-org/DPT)<br />*Backbone:*<br />[![GitHub Stars](https://img.shields.io/github/stars/google-research/vision_transformer?logo=GitHub&label=Stars)](https://github.com/google-research/vision_transformer) | - | - |

Note: The above ranking includes only one model, as the other methods are image-based and don't have any temporal information making them unsuitable for light field video reconstruction from monocular video.

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-video-depth-estimation-rankingsand-light-field-video-reconstructionfrom-monocular-video-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## NYU-Depth V2: AbsRel<=0.054
| Rank | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | VapourSynth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | Metric3D CSTM_label (manually aligned the scale and shift)<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Yin_Metric3D_Towards_Zero-shot_Metric_3D_Prediction_from_A_Single_Image_ICCV_2023_paper.html)<br />*Backbone:*<br />ConvNeXt-L<br />[![CVPR](https://img.shields.io/badge/2022-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2022/html/Liu_A_ConvNet_for_the_2020s_CVPR_2022_paper.html) | **0.050** {1}<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Yin_Metric3D_Towards_Zero-shot_Metric_3D_Prediction_from_A_Single_Image_ICCV_2023_paper.html) | DDAD & Lyft & Driving Stereo & DIML & Arogoverse2 & Cityscapes & DSEC & Mapillary PSD & Pandaset & UASOL & Taskonomy | [![GitHub Stars](https://img.shields.io/github/stars/YvanYin/Metric3D?logo=GitHub&label=Stars)](https://github.com/YvanYin/Metric3D)<br />*Backbone:*<br />[![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/ConvNeXt?logo=GitHub&label=Stars)](https://github.com/facebookresearch/ConvNeXt) | - | - |
| 2 | DPT<br />[![ICCV](https://img.shields.io/badge/2021-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2021/html/Ranftl_Vision_Transformers_for_Dense_Prediction_ICCV_2021_paper.html)<br />*Backbone:*<br />BEiT-L<br />[![ICLR](https://img.shields.io/badge/2022-ICLR-d5df32)](https://openreview.net/forum?id=p-BhZSz59o4) | **0.054** {1}<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Spencer_Kick_Back__Relax_Learning_to_Reconstruct_the_World_by_ICCV_2023_paper.html) | DIML Indoor & MegaDepth & ReDWeb & WSVD & 3D Movies & ApolloScape & IRS & TartanAir & HR-WSI & BlendedMVS & NYU-Depth V2 | [![GitHub Stars](https://img.shields.io/github/stars/isl-org/DPT?logo=GitHub&label=Stars)](https://github.com/isl-org/DPT)<br />*Backbone:*<br />[![GitHub Stars](https://img.shields.io/github/stars/microsoft/unilm?logo=GitHub&label=Stars)](https://github.com/microsoft/unilm/tree/master/beit) | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-video-depth-estimation-rankingsand-light-field-video-reconstructionfrom-monocular-video-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)
