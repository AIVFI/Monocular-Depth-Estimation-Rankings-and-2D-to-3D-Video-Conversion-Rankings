# <p align=center>Monocular Video Depth Estimation Rankings<br />and Light Field Video Reconstruction<br />from Monocular Video Rankings</p>

This is a very early version and I will gradually add new rankings and expand the existing ones.

In the near future I will write a little more information about what inspired me to add it and how it relates to my first repository: [Video Frame Interpolation Rankings and Video Deblurring Rankings](https://github.com/AIVFI/Video-Frame-Interpolation-Rankings-and-Video-Deblurring-Rankings)

## <p align=center>List of Rankings</p>
<p align=center>Each ranking includes only the best model for one method.</p>  

### Light Field Video Reconstruction from Monocular Video Rankings
1. :crown: **4DLFVD with up to 10×10 real light field views:heavy_check_mark:: LPIPS:heart_eyes:** (no data)  
_This will be the King of all rankings. We look forward to ambitious researchers._
1. **4DLFVD with up to 10×10 real light field views:heavy_check_mark:: PSNR:disappointed:** (no data)
1. **Hybrid with 7×7 synthetic light field views:bangbang:: LPIPS:heart_eyes:** (no data) 
1. [**Hybrid with 7×7 synthetic light field views:bangbang:: PSNR:disappointed:>=32dB**](#hybrid-with-77-synthetic-light-field-viewsbangbang-psnrdisappointed32db)
### Monocular Video Depth Estimation Rankings
- (to do)
### Appendices
- **Rules for qualifying models for the rankings** (to do)

--------------------

## Hybrid with 7×7 synthetic light field views:bangbang:: PSNR:disappointed:>=32dB
| Rank | Model | PSNR ↑ | Originally<br />announced | Official<br />repository | Practical<br />models | VapourSynth |
|:----:|:----|:----:|:----:|:----:|:----:|:----:|
| 1 | LFVRT |  **32.66dB** [^1] | July 2022 [^1] | [PyTorch](https://github.com/ShrisudhanG/Synthesizing-Light-Field-Video-from-Monocular-Video) ![Github stars](https://img.shields.io/github/stars/ShrisudhanG/Synthesizing-Light-Field-Video-from-Monocular-Video) | - | - |

Note: The above ranking includes only one model, as the other methods are image-based and don't have any temporal information making them unsuitable for light field video reconstruction from monocular video.

[[Back to Top]](#monocular-video-depth-estimation-rankingsand-light-field-video-reconstructionfrom-monocular-video-rankings)
[[Back to the List of Rankings]](#list-of-rankings)

[^1]: Synthesizing Light Field Video from Monocular Video [[ECCV 2022]](https://www.ecva.net/papers/eccv_2022/papers_ECCV/html/4122_ECCV_2022_paper.php) [[arXiv]](https://arxiv.org/abs/2207.10357)
