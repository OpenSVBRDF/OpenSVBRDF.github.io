---
layout: default
---
<!-- 
Text can be **bold**, _italic_, or ~~strikethrough~~. -->

<!-- [Link to another page](./another-page.html). -->

<!-- There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project. -->

## Introduction

OpenSVBRDF is the **first** large-scale database of **measured** spatially-varying **anisotropic** reflectance, consisting of **1,000** high-quality near-planar SVBRDFs, spanning 9 material categories.

Please click on the left image to view rendering results of 108 (out of 1,000) high-resolution SVBRDFs captured and reconstructed in the database. Each row represents one category, from the top row to bottom: satin, wood, paper, metal, leather, ceramic, woven, fabric and wallpaper.

## Data organization
The database consists of three components. For different research purposes, you can choose data that suits your needs for downloading. We support both individual downloads for each sample and bulk downloads.

#### 1. Texture maps (50GB)
For each sample in the database, we store 6 texture maps, including GGX parameters (diffuse albedo, specular albedo, anisotropic roughness, normal, tangent) and transparency. The spatial resolution
is 1,024×1,024 for all texture maps of 1,000 samples. The data size for each sample is 50MB, totaling 50GB.

#### 2. Neural representation (283GB)
We store the intermediate neural representations of all SVBRDFs (also described as latent vectors in the <a href="{{ site.github.repository_url }}">paper</a>), with spatial resolution 1,024×1,024. The data size for each sample is 290MB, totaling 283GB.

#### 3. Raw images (15TB)
We also store the 193 raw HDR photographs (with resolution of 24MP) for each sample. The data size for each sample is 15GB, totaling 15TB.

Please visit the <a href="http://www.cad.zju.edu.cn/home/opensvbrdf">database website</a> to see the preview of 1,000 samples and get download links. In order to get full access to the data on the website, it is required to apply for an account with your e-mail. We will review the application within a few working days.


## License

Our source code is released under the GPL-3.0 license for academic purposes. The only requirement for using the code in your research is to cite our paper:
```
@article{Ma:2023:OpenSVBRDF,
        author = {Ma, Xiaohe and Xu, Xianmin and Zhang, Leyao and Zhou, Kun and Wu, Hongzhi},
        title = {OpenSVBRDF: A Database of Measured
        Spatially-Varying Reflectance},
        year = {2023},
        issue_date = {December 2023},
        publisher = {Association for Computing Machinery},
        address = {New York, NY, USA},
        volume = {42},
        number = {6},
        doi = {10.1145/3618358},
        journal = {ACM Trans. Graph.}
        articleno = {254},
}
```
For commercial licensing options, please email hwu at acm.org. See <a href="COPYING.txt">COPYING</a> for the open source license.

## Challenges

In the future, We are going to set up open challenges (e.g., on material estimation, classification, generation) because standardized benchmarks based on our growing dataset might be useful to quantitatively evaluate existing as well as future research on a common ground.<br><br>
Further information will be added to the <a href="http://www.cad.zju.edu.cn/home/opensvbrdf">database website</a>.

<iframe width="480" height="270" src="https://www.youtube.com/embed/tDccO4-SQQE?rel=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## Acknowledgements

Thanks to the contributions by <a href="https://xiaohema98.com">Xiaohe Ma</a>, Xianmin Xu, Leyao Zhang, and supervision by <a href="http://kunzhou.net/">Kun Zhou</a> and <a href="http://hongzhiwu.com/">Hongzhi Wu</a>. Additionally, we would like to thanks Yaxin Yu and <a href="https://cocoakang.cn/">Kaizhang Kang</a> for help in building the prototype, <a href="https://yuedong.shading.me/">Yue Dong</a>, <a href="https://www.microsoft.com/en-us/research/people/xtong/">Xin Tong</a>, <a href="https://graphics.cs.yale.edu/people/julie-dorsey">Julie Dorsey</a> and <a href="https://graphics.cs.yale.edu/people/holly-rushmeier">Holly Rushmeier</a> for their support.<br>

This work is partially supported by NSF China (62022072 & 62227806), Zhejiang Provincial Key R&D Program (2022C01057), the Fundamental Research Funds for the Central Universities, the XPLORER PRIZE and Information Technology Center and State Key Lab of CAD&CG, Zhejiang University.