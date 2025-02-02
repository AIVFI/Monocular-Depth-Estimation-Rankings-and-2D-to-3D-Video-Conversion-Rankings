# <p align=center>Monocular Depth Estimation Rankings<br />and 2D to 3D Video Conversion Rankings</p>

**Researchers!** On **19 December 2024**, a preprint paper was published that focuses on "evaluating self-supervised learning on non-semantic vision tasks that are **more spatial (3D) and temporal (+1D = 4D)**, such as camera pose estimation, point and object tracking, and depth estimation." The **4DS-j model** presented there achieves significantly better monocular depth estimation results than DINOv2 ViT-g, making it a **better backbone than DINOv2** for specialised video depth estimation models that can be the basis for better 2D to 3D video conversion, too! Please try to implement the 4DS-j backbone instead of DINOv2 ViT-g for your future breakthrough video depth estimation models! Below is a special ranking showing the capabilities of 4DS-j:

## ScanNet: AbsRel (TOP2 best backbone for monocular depth estimation )
| RK | Model <br />*Links:*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;Repository&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />(frozen<br />backbone)<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2412.15212)<br />4DS | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />(short<br />finetuning)<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2412.15212)<br />4DS | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />(medium<br />finetuning)<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2412.15212)<br />4DS | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />(long<br />finetuning)<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2412.15212)<br />4DS |
|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | **4DS-j**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2412.15212) | **0.85** | **0.63** | **0.59** | **0.57** |
| 2 | **DinoV2-g**<br />[![TMLR](https://img.shields.io/badge/2024-TMLR-bfcaef)](https://openreview.net/forum?id=a68SUt6zFt) [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/dinov2?logo=GitHub&label=Stars)](https://github.com/facebookresearch/dinov2) | **0.92** | **0.76** | **0.69** | **0.66** |

Due to the recent number of new models that I am unable to add to the rankings immediately, I have decided to add a waiting list of new models:

| Method | Paper | &nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;&nbsp; | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; |
|:---:|:---:|:---:|:---:|
| Align3R | Align3R: Aligned Monocular Depth Estimation for Dynamic Videos | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2412.03079) | [![GitHub Stars](https://img.shields.io/github/stars/jiah-cloud/Align3R?logo=GitHub&label=Stars)](https://github.com/jiah-cloud/Align3R) |
| FiffDepth | FiffDepth: Feed-forward Transformation of Diffusion-Based Generators for Detailed Depth Estimation | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2412.00671) | - |
| ImmersePro | ImmersePro: End-to-End Stereo Video Synthesis Via Implicit Disparity Learning | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2410.00262) | [![GitHub Stars](https://img.shields.io/github/stars/shijianjian/ImmersePro?logo=GitHub&label=Stars)](https://github.com/shijianjian/ImmersePro) |
| MegaSaM | MegaSaM: Accurate, Fast, and Robust Structure and Motion from Casual Dynamic Videos | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2412.04463) | [![GitHub Stars](https://img.shields.io/github/stars/mega-sam/mega-sam?logo=GitHub&label=Stars)](https://github.com/mega-sam/mega-sam) |
| RollingDepth | Video Depth without Video Models | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2411.19189) | [![GitHub Stars](https://img.shields.io/github/stars/prs-eth/RollingDepth?logo=GitHub&label=Stars)](https://github.com/prs-eth/RollingDepth) |
| SpatialMe | SpatialMe: Stereo Video Conversion Using Depth-Warping and Blend-Inpainting | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2412.11512) | - |

## <p align=center>List of Rankings</p>

### 2D to 3D Video Conversion Rankings
1. [**Qualitative comparison of four 2D to 3D video conversion methods: Rank (human perceptual judgment)**](#qualitative-comparison-of-four-2d-to-3d-video-conversion-methods-rank-human-perceptual-judgment)
### Monocular Depth Estimation Rankings
#### I. Rankings based on temporal consistency metrics
1. [**ScanNet (170 frames): TAE<=2.2**](#scannet-170-frames-tae22)
1. [**Bonn RGB-D Dynamic (5 video clips with 110 frames each): OPW<=0.1**](#bonn-rgb-d-dynamic-5-video-clips-with-110-frames-each-opw01)
1. [**ScanNet++ (98 video clips with 32 frames each): TAE**](#scannet-98-video-clips-with-32-frames-each-tae)
1. [**NYU-Depth V2: OPW<=0.37**](#nyu-depth-v2-opw037)
#### II. Rankings based on 3D metrics
1. [**Direct comparison of 9 metric depth models (each with each) on 5 datasets: F-score**](#direct-comparison-of-9-metric-depth-models-each-with-each-on-5-datasets-f-score)
#### III. Rankings based on 2D metrics
1. [**Bonn RGB-D Dynamic (5 video clips with 110 frames each): AbsRel<=0.078**](#bonn-rgb-d-dynamic-5-video-clips-with-110-frames-each-absrel0078)
1. [**NYU-Depth V2: AbsRel<=0.045 (relative depth)**](#nyu-depth-v2-absrel0045-relative-depth)
1. [**NYU-Depth V2: AbsRel<=0.051 (metric depth)**](#nyu-depth-v2-absrel0051-metric-depth)
#### IV. Old layout - currently no longer up to date
1. [**NYU-Depth V2 (640×480): AbsRel<=0.058 (old layout - currently no longer up to date)**](#nyu-depth-v2-640480-absrel0058-old-layout---currently-no-longer-up-to-date)
1. [**UnrealStereo4K (3840×2160): AbsRel<=0.04 (old layout - currently no longer up to date)**](#unrealstereo4k-38402160-absrel004-old-layout---currently-no-longer-up-to-date)
### Appendices
- **Appendix 1: Rules for qualifying models for the rankings** (to do)
- **Appendix 2: Metrics selection for the rankings** (to do)
- [**Appendix 3: List of all research papers from the above rankings**](#appendix-3-list-of-all-research-papers-from-the-above-rankings)

--------------------

## Qualitative comparison of four 2D to 3D video conversion methods: Rank (human perceptual judgment)
📝 **Note:** There are no quantitative comparison results of StereoCrafter yet, so this ranking is based on my own perceptual judgement of the qualitative comparison results shown in [Figure 7](https://arxiv.org/abs/2409.07447). One output frame (right view) is compared with one input frame (left view) from the video clip: [22_dogskateboarder](https://github.com/stereocrafter/stereocrafter.github.io/releases/V0.0.1) and one output frame (right view) is compared with one input frame (left view) from the video clip: [scooter-black](https://davischallenge.org/davis2016/code.html)
| RK | Model <br />*Links:*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;Repository&nbsp;&nbsp;&nbsp;&nbsp; | Rank&nbsp;↓<br />(human&nbsp;perceptual<br />judgment) |
|:---:|:---:|:---:|
| 1 | **StereoCrafter**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2409.07447) [![GitHub Stars](https://img.shields.io/github/stars/TencentARC/StereoCrafter?logo=GitHub&label=Stars)](https://github.com/TencentARC/StereoCrafter) | **1** |
| 2-3 | **Immersity AI** | **2-3** |
| 2-3 | **Owl3D** | **2-3** |
| 4 | **Deep3D**<br />[![ECCV](https://img.shields.io/badge/2016-ECCV-67cd84)](https://link.springer.com/chapter/10.1007/978-3-319-46493-0_51) [![GitHub Stars](https://img.shields.io/github/stars/piiswrong/deep3d?logo=GitHub&label=Stars)](https://github.com/piiswrong/deep3d) | **4** |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## ScanNet (170 frames): TAE<=2.2
| RK | Model <br />*Links:*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;Repository&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;TAE&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![arXiv](https://img.shields.io/badge/2025-arXiv-b31b1b)](https://arxiv.org/abs/2501.12375)<br />VDA |
|:---:|:---:|:---:|
| 1 | **VDA-L**<br />[![arXiv](https://img.shields.io/badge/2025-arXiv-b31b1b)](https://arxiv.org/abs/2501.12375) [![GitHub Stars](https://img.shields.io/github/stars/DepthAnything/Video-Depth-Anything?logo=GitHub&label=Stars)](https://github.com/DepthAnything/Video-Depth-Anything) | **0.570** {MF} |
| 2 | **DepthCrafter**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2409.02095) [![GitHub Stars](https://img.shields.io/github/stars/Tencent/DepthCrafter?logo=GitHub&label=Stars)](https://github.com/Tencent/DepthCrafter) | **0.639** {MF} |
| 3 | **Depth Any Video**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2410.10815) [![GitHub Stars](https://img.shields.io/github/stars/Nightmare-n/DepthAnyVideo?logo=GitHub&label=Stars)](https://github.com/Nightmare-n/DepthAnyVideo) | **0.967** {MF} |
| 4 | **ChronoDepth**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2406.01493) [![GitHub Stars](https://img.shields.io/github/stars/jhaoshao/ChronoDepth)](https://github.com/jhaoshao/ChronoDepth) | **1.022** {MF} |
| 5 | **Depth Anything V2 Large**<br />[![NeurIPS](https://img.shields.io/badge/2024-NeurIPS-68448a)](https://arxiv.org/abs/2406.09414) [![GitHub Stars](https://img.shields.io/github/stars/DepthAnything/Depth-Anything-V2?logo=GitHub&label=Stars)](https://github.com/DepthAnything/Depth-Anything-V2) | **1.140** {1} |
| 6 | **NVDS**<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_Neural_Video_Depth_Stabilizer_ICCV_2023_paper.html) [![GitHub Stars](https://img.shields.io/github/stars/RaymondWang987/NVDS?logo=GitHub&label=Stars)](https://github.com/RaymondWang987/NVDS) | **2.176** {4} |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## Bonn RGB-D Dynamic (5 video clips with 110 frames each): OPW<=0.1
| RK | Model <br />*Links:*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;Repository&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;OPW&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2411.17249)<br />BA |
|:---:|:---:|:---:|
| 1 | **Buffer Anytime (DA V2)**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2411.17249) | **0.028** {MF} |
| 2 | **DepthCrafter**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2409.02095) [![GitHub Stars](https://img.shields.io/github/stars/Tencent/DepthCrafter?logo=GitHub&label=Stars)](https://github.com/Tencent/DepthCrafter) | **0.029** {MF} |
| 3 | **ChronoDepth**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2406.01493) [![GitHub Stars](https://img.shields.io/github/stars/jhaoshao/ChronoDepth)](https://github.com/jhaoshao/ChronoDepth) | **0.035** {MF} |
| 4 | **Marigold + E2E FT**<br />[![WACV](https://img.shields.io/badge/2025-WACV-2e0094)](https://arxiv.org/abs/2409.11355) [![GitHub Stars](https://img.shields.io/github/stars/VisualComputingInstitute/diffusion-e2e-ft)](https://github.com/VisualComputingInstitute/diffusion-e2e-ft) | **0.053** {1} |
| 5 | **Depth Anything V2 Large**<br />[![NeurIPS](https://img.shields.io/badge/2024-NeurIPS-68448a)](https://arxiv.org/abs/2406.09414) [![GitHub Stars](https://img.shields.io/github/stars/DepthAnything/Depth-Anything-V2?logo=GitHub&label=Stars)](https://github.com/DepthAnything/Depth-Anything-V2) | **0.059** {1} |
| 6 | **NVDS**<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_Neural_Video_Depth_Stabilizer_ICCV_2023_paper.html) [![GitHub Stars](https://img.shields.io/github/stars/RaymondWang987/NVDS?logo=GitHub&label=Stars)](https://github.com/RaymondWang987/NVDS) | **0.068** {4} |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

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
| RK | Model <br />*Links:*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;Repository&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;OPW&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![ECCV](https://img.shields.io/badge/2024-ECCV-67cd84)](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/828_ECCV_2024_paper.php)<br />FD | &nbsp;&nbsp;&nbsp;OPW&nbsp;↓&nbsp;&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10707178)<br />NVDS<sup>+</sup> | &nbsp;&nbsp;OPW&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_Neural_Video_Depth_Stabilizer_ICCV_2023_paper.html)<br />NVDS |
|:---:|:---:|:---:|:---:|:---:|
| 1 | **FutureDepth**<br />[![ECCV](https://img.shields.io/badge/2024-ECCV-67cd84)](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/828_ECCV_2024_paper.php) | **0.303** {4} | - | - |
| 2 | **NVDS<sup>+</sup>**<br />[![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10707178) [![GitHub Stars](https://img.shields.io/github/stars/RaymondWang987/NVDS?logo=GitHub&label=Stars)](https://github.com/RaymondWang987/NVDS) | - | **0.339** {4} | - |
| 3 | **NVDS**<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_Neural_Video_Depth_Stabilizer_ICCV_2023_paper.html) [![GitHub Stars](https://img.shields.io/github/stars/RaymondWang987/NVDS?logo=GitHub&label=Stars)](https://github.com/RaymondWang987/NVDS) | **0.364** {4} | - | **0.364** {4} |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## Direct comparison of 9 metric depth models (each with each) on 5 datasets: F-score
📝 **Note:** This ranking is based on data from [Table 4](https://arxiv.org/abs/2410.02073). The example result 3:0:2 (first left in the first row) means that Depth Pro has a better F-score than UniDepth-V in 3 datasets, in no dataset has the same F-score as UniDepth-V and has a worse F-score compared to UniDepth-V in 2 datasets.
| RK | Model <br />*Links:*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;Repository&nbsp;&nbsp;&nbsp;&nbsp; | DP | UD | M3D v2 | DA V2 | DA | ZoeD | M3D | PF | ZD |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | **Depth Pro**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2410.02073) [![GitHub Stars](https://img.shields.io/github/stars/apple/ml-depth-pro?logo=GitHub&label=Stars)](https://github.com/apple/ml-depth-pro) | - | **3:0:2** | **3:1:1** | **5:0:0** | **5:0:0** | **5:0:0** | **5:0:0** | **5:0:0** | **3:0:0** |
| 2 | **UniDepth-V**<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Piccinelli_UniDepth_Universal_Monocular_Metric_Depth_Estimation_CVPR_2024_paper.html) [![GitHub Stars](https://img.shields.io/github/stars/lpiccinelli-eth/UniDepth?logo=GitHub&label=Stars)](https://github.com/lpiccinelli-eth/UniDepth) | **2:0:3** | - | **4:0:1** | **5:0:0** | **5:0:0** | **5:0:0** | **5:0:0** | **5:0:0** | **3:0:0** |
| 3 | **Metric3D v2 ViT-giant**<br />[![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10638254) [![GitHub Stars](https://img.shields.io/github/stars/YvanYin/Metric3D?logo=GitHub&label=Stars)](https://github.com/YvanYin/Metric3D) | **1:1:3** | **1:0:4** | - | **4:1:0** | **5:0:0** | **5:0:0** | **5:0:0** | **5:0:0** | **3:0:0** |
| 4 | **Depth Anything V2**<br />[![NeurIPS](https://img.shields.io/badge/2024-NeurIPS-68448a)](https://arxiv.org/abs/2406.09414) [![GitHub Stars](https://img.shields.io/github/stars/DepthAnything/Depth-Anything-V2?logo=GitHub&label=Stars)](https://github.com/DepthAnything/Depth-Anything-V2) | **0:0:5** | **0:0:5** | **0:1:4** | - | **4:1:0** | **4:0:1** | **5:0:0** | **4:0:1** | **3:0:0** |
| 5 | **Depth Anything**<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Depth_Anything_Unleashing_the_Power_of_Large-Scale_Unlabeled_Data_CVPR_2024_paper.html) [![GitHub Stars](https://img.shields.io/github/stars/LiheYoung/Depth-Anything?logo=GitHub&label=Stars)](https://github.com/LiheYoung/Depth-Anything) | **0:0:5** | **0:0:5** | **0:0:5** | **0:1:4** | - | **3:0:2** | **3:1:1** | **3:0:2** | **2:1:0** |
| 6 | **ZoeD-M12-NK**<br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2302.12288) [![GitHub Stars](https://img.shields.io/github/stars/isl-org/ZoeDepth?logo=GitHub&label=Stars)](https://github.com/isl-org/ZoeDepth) | **0:0:5** | **0:0:5** | **0:0:5** | **1:0:4** | **2:0:3** | - | **3:0:2** | **3:1:1** | **2:0:1** |
| 7 | **Metric3D**<br />[![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Yin_Metric3D_Towards_Zero-shot_Metric_3D_Prediction_from_A_Single_Image_ICCV_2023_paper.html) [![GitHub Stars](https://img.shields.io/github/stars/YvanYin/Metric3D?logo=GitHub&label=Stars)](https://github.com/YvanYin/Metric3D) | **0:0:5** | **0:0:5** | **0:0:5** | **0:0:5** | **1:1:3** | **2:0:3** | - | **3:0:2** | **2:1:0** |
| 8 | **PatchFusion**<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Li_PatchFusion_An_End-to-End_Tile-Based_Framework_for_High-Resolution_Monocular_Metric_Depth_CVPR_2024_paper.html) [![GitHub Stars](https://img.shields.io/github/stars/zhyever/PatchFusion?logo=GitHub&label=Stars)](https://github.com/zhyever/PatchFusion) | **0:0:5** | **0:0:5** | **0:0:5** | **1:0:4** | **2:0:3** | **1:1:3** | **2:0:3** | - | **2:0:1** |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## Bonn RGB-D Dynamic (5 video clips with 110 frames each): AbsRel<=0.078
📝 **Note:** This Ranking will temporarily not be updated due to - see [Figure 4](https://arxiv.org/abs/2501.12375)
| RK | Model <br />*Links:*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;Repository&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2410.03825)<br />MonST3R | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2409.02095)<br />DC |
|:---:|:---:|:---:|:---:|
| 1 | **MonST3R**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2410.03825) [![GitHub Stars](https://img.shields.io/github/stars/Junyi42/monst3r?logo=GitHub&label=Stars)](https://github.com/Junyi42/monst3r) | **0.063** {MF} | - |
| 2 | **DepthCrafter**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2409.02095) [![GitHub Stars](https://img.shields.io/github/stars/Tencent/DepthCrafter?logo=GitHub&label=Stars)](https://github.com/Tencent/DepthCrafter) | **0.075** {MF} | **0.075** {MF} |
| 3 | **Depth Anything**<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Depth_Anything_Unleashing_the_Power_of_Large-Scale_Unlabeled_Data_CVPR_2024_paper.html) [![GitHub Stars](https://img.shields.io/github/stars/LiheYoung/Depth-Anything?logo=GitHub&label=Stars)](https://github.com/LiheYoung/Depth-Anything) | - | **0.078** {1} |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## NYU-Depth V2: AbsRel<=0.045 (relative depth)
| RK | Model <br />*Links:*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;Repository&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2410.19115)<br />MoGe | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2407.17952)<br />BD | &nbsp;&nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10638254)<br />M3D v2 | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Depth_Anything_Unleashing_the_Power_of_Large-Scale_Unlabeled_Data_CVPR_2024_paper.html)<br />DA | &nbsp;&nbsp;&nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![NeurIPS](https://img.shields.io/badge/2024-NeurIPS-68448a)](https://arxiv.org/abs/2406.09414)<br />DA V2 |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | **MoGe**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2410.19115) [![GitHub Stars](https://img.shields.io/github/stars/microsoft/MoGe?logo=GitHub&label=Stars)](https://github.com/microsoft/MoGe) | **0.0341** {1} | - | - | - | - |
| 2 | **UniDepth**<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Piccinelli_UniDepth_Universal_Monocular_Metric_Depth_Estimation_CVPR_2024_paper.html) [![GitHub Stars](https://img.shields.io/github/stars/lpiccinelli-eth/UniDepth?logo=GitHub&label=Stars)](https://github.com/lpiccinelli-eth/UniDepth) | **0.0380** {1} | - | - | - | - |
| 3-4 | **BetterDepth**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2407.17952) | - | **0.042** {1} | - | - | - |
| 3-4 | **Metric3D v2 ViT-Large**<br />[![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10638254) [![GitHub Stars](https://img.shields.io/github/stars/YvanYin/Metric3D?logo=GitHub&label=Stars)](https://github.com/YvanYin/Metric3D) | **0.134** {1} | - | **0.042** {1} | - | - |
| 5 | **Depth Anything Large**<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Depth_Anything_Unleashing_the_Power_of_Large-Scale_Unlabeled_Data_CVPR_2024_paper.html) [![GitHub Stars](https://img.shields.io/github/stars/LiheYoung/Depth-Anything?logo=GitHub&label=Stars)](https://github.com/LiheYoung/Depth-Anything) | **0.0424** {1} | **0.043** {1} | **0.043** {1} | **0.043** {1} | **0.043** {1} |
| 6 | **Depth Anything V2 Large**<br />[![NeurIPS](https://img.shields.io/badge/2024-NeurIPS-68448a)](https://arxiv.org/abs/2406.09414) [![GitHub Stars](https://img.shields.io/github/stars/DepthAnything/Depth-Anything-V2?logo=GitHub&label=Stars)](https://github.com/DepthAnything/Depth-Anything-V2) | **0.0420** {1} | - | - | - | **0.045** {1} |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## NYU-Depth V2: AbsRel<=0.051 (metric depth)
| RK | Model <br />*Links:*<br />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;Repository&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10638254)<br />M3D v2 | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.}<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2409.09896)<br />GRIN | - | - | - |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | **Metric3D v2 ViT-giant**<br />[![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10638254) [![GitHub Stars](https://img.shields.io/github/stars/YvanYin/Metric3D?logo=GitHub&label=Stars)](https://github.com/YvanYin/Metric3D) | **0.045** {1} | - | - | - | - |
| 2 | **GRIN_FT_NI**<br />[![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2409.09896) | - | **0.051** {1} | - | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## NYU-Depth V2 (640×480): AbsRel<=0.058 (old layout - currently no longer up to date)
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

## UnrealStereo4K (3840×2160): AbsRel<=0.04 (old layout - currently no longer up to date)
| RK | &nbsp;&nbsp;&nbsp;&nbsp;Model&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;AbsRel&nbsp;↓&nbsp;&nbsp;<br />{Input&nbsp;fr.} | Training<br />dataset | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; | Practical<br />model | Vapour-<br />Synth |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 1 | ZoeDepth +PF<sub>R=128</sub><br />[![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2302.12288)<br />*ENH:*<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Li_PatchFusion_An_End-to-End_Tile-Based_Framework_for_High-Resolution_Monocular_Metric_Depth_CVPR_2024_paper.html) | **0.0388** {1}<br />[![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Li_PatchFusion_An_End-to-End_Tile-Based_Framework_for_High-Resolution_Monocular_Metric_Depth_CVPR_2024_paper.html) | *ENH:*<br />UnrealStereo4K | [![GitHub Stars](https://img.shields.io/github/stars/isl-org/ZoeDepth?logo=GitHub&label=Stars)](https://github.com/isl-org/ZoeDepth)<br />*ENH:*<br />[![GitHub Stars](https://img.shields.io/github/stars/zhyever/PatchFusion?logo=GitHub&label=Stars)](https://github.com/zhyever/PatchFusion) | - | - |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)

## Appendix 3: List of all research papers from the above rankings

2025:
| Method | Abbr. | Paper | &nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;&nbsp;<br />(Alt link) | Official<br />&nbsp;&nbsp;repository&nbsp;&nbsp; |
|:---:|:---:|:---:|:---:|:---:|
| Video Depth Anything | VDA | Video Depth Anything: Consistent Depth Estimation for Super-Long Videos | [![arXiv](https://img.shields.io/badge/2025-arXiv-b31b1b)](https://arxiv.org/abs/2501.12375) | [![GitHub Stars](https://img.shields.io/github/stars/DepthAnything/Video-Depth-Anything?logo=GitHub&label=Stars)](https://github.com/DepthAnything/Video-Depth-Anything) |

2024 and older:
| Method | Paper | &nbsp;&nbsp;&nbsp;&nbsp;Venue&nbsp;&nbsp;&nbsp;&nbsp; |
|:---:|:---:|:---:|
| 4DS | Scaling 4D Representations | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2412.15212) | - |
| BetterDepth | BetterDepth: Plug-and-Play Diffusion Refiner for Zero-Shot Monocular Depth Estimation | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2407.17952) |
| Buffer Anytime | Buffer Anytime: Zero-Shot Video Depth and Normal from Image Priors | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2411.17249) | - |
| ChronoDepth | Learning Temporally Consistent Video Depth from Video Diffusion Priors | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2406.01493) |
| Deep3D | Deep3D: Fully Automatic 2D-to-3D Video Conversion with Deep Convolutional Neural Networks | [![ECCV](https://img.shields.io/badge/2016-ECCV-67cd84)](https://link.springer.com/chapter/10.1007/978-3-319-46493-0_51) |
| Depth Any Video | Depth Any Video with Scalable Synthetic Data | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2410.10815) |
| Depth Anything | Depth Anything: Unleashing the Power of Large-Scale Unlabeled Data | [![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Depth_Anything_Unleashing_the_Power_of_Large-Scale_Unlabeled_Data_CVPR_2024_paper.html) |
| Depth Anything V2 | Depth Anything V2 | [![NeurIPS](https://img.shields.io/badge/2024-NeurIPS-68448a)](https://arxiv.org/abs/2406.09414) |
| Depth Pro | Depth Pro: Sharp Monocular Metric Depth in Less Than a Second | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2410.02073) |
| DepthCrafter | DepthCrafter: Generating Consistent Long Depth Sequences for Open-world Videos | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2409.02095) |
| DINOv2 | DINOv2: Learning Robust Visual Features without Supervision | [![TMLR](https://img.shields.io/badge/2024-TMLR-bfcaef)](https://openreview.net/forum?id=a68SUt6zFt) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/dinov2?logo=GitHub&label=Stars)](https://github.com/facebookresearch/dinov2) |
| Diffusion E2E FT | Fine-Tuning Image-Conditional Diffusion Models is Easier than You Think | [![WACV](https://img.shields.io/badge/2025-WACV-2e0094)](https://arxiv.org/abs/2409.11355) |
| FutureDepth | FutureDepth: Learning to Predict the Future Improves Video Depth Estimation | [![ECCV](https://img.shields.io/badge/2024-ECCV-67cd84)](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/828_ECCV_2024_paper.php) |
| GenPercept | Diffusion Models Trained with Large Data Are Transferable Visual Models | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2403.06090) |
| GeoWizard | GeoWizard: Unleashing the Diffusion Priors for 3D Geometry Estimation from a Single Image | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2403.12013) |
| GRIN | GRIN: Zero-Shot Metric Depth with Pixel-Level Diffusion | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2409.09896) |
| LightedDepth | LightedDepth: Video Depth Estimation in light of Limited Inference View Angles | [![CVPR](https://img.shields.io/badge/2023-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2023/html/Zhu_LightedDepth_Video_Depth_Estimation_in_Light_of_Limited_Inference_View_CVPR_2023_paper.html) |
| Marigold | Repurposing Diffusion-Based Image Generators for Monocular Depth Estimation | [![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Ke_Repurposing_Diffusion-Based_Image_Generators_for_Monocular_Depth_Estimation_CVPR_2024_paper.html) |
| Metric3D | Metric3D: Towards Zero-shot Metric 3D Prediction from A Single Image | [![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Yin_Metric3D_Towards_Zero-shot_Metric_3D_Prediction_from_A_Single_Image_ICCV_2023_paper.html) |
| Metric3D v2 | Metric3D v2: A Versatile Monocular Geometric Foundation Model for Zero-shot Metric Depth and Surface Normal Estimation | [![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10638254) |
| MiDaS | Towards Robust Monocular Depth Estimation: Mixing Datasets for Zero-Shot Cross-Dataset Transfer | [![TPAMI](https://img.shields.io/badge/2022-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/9178977) |
| MiDaS v3.1 | MiDaS v3.1 – A Model Zoo for Robust Monocular Relative Depth Estimation | [![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2307.14460) |
| MoGe | MoGe: Unlocking Accurate Monocular Geometry Estimation for Open-Domain Images with Optimal Training Supervision | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2410.19115) | [![GitHub Stars](https://img.shields.io/github/stars/microsoft/MoGe?logo=GitHub&label=Stars)](https://github.com/microsoft/MoGe) |
| MonST3R | MonST3R: A Simple Approach for Estimating Geometry in the Presence of Motion | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2410.03825) |
| NeWCRFs | Neural Window Fully-connected CRFs for Monocular Depth Estimation | [![CVPR](https://img.shields.io/badge/2022-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2022/html/Yuan_Neural_Window_Fully-Connected_CRFs_for_Monocular_Depth_Estimation_CVPR_2022_paper.html) |
| NVDS | Neural Video Depth Stabilizer | [![ICCV](https://img.shields.io/badge/2023-ICCV-fcb900)](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_Neural_Video_Depth_Stabilizer_ICCV_2023_paper.html) |
| NVDS<sup>+</sup> | NVDS<sup>+</sup>: Towards Efficient and Versatile Neural Stabilizer for Video Depth Estimation | [![TPAMI](https://img.shields.io/badge/2024-TPAMI-fefd02)](https://ieeexplore.ieee.org/document/10707178) |
| PatchFusion | PatchFusion: An End-to-End Tile-Based Framework for High-Resolution Monocular Metric Depth Estimation | [![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Li_PatchFusion_An_End-to-End_Tile-Based_Framework_for_High-Resolution_Monocular_Metric_Depth_CVPR_2024_paper.html) |
| StereoCrafter | StereoCrafter: Diffusion-based Generation of Long and High-fidelity Stereoscopic 3D from Monocular Videos | [![arXiv](https://img.shields.io/badge/2024-arXiv-b31b1b)](https://arxiv.org/abs/2409.07447) |
| UniDepth | UniDepth: Universal Monocular Metric Depth Estimation | [![CVPR](https://img.shields.io/badge/2024-CVPR-1e407f)](https://openaccess.thecvf.com/content/CVPR2024/html/Piccinelli_UniDepth_Universal_Monocular_Metric_Depth_Estimation_CVPR_2024_paper.html) |
| ZoeDepth | ZoeDepth: Zero-shot Transfer by Combining Relative and Metric Depth | [![arXiv](https://img.shields.io/badge/2023-arXiv-b31b1b)](https://arxiv.org/abs/2302.12288) |

[![Back to Top](https://img.shields.io/badge/Back_to_Top-555555)](#monocular-depth-estimation-rankingsand-2d-to-3d-video-conversion-rankings)
[![Back to the List of Rankings](https://img.shields.io/badge/Back_to_the_List_of_Rankings-555555)](#list-of-rankings)
