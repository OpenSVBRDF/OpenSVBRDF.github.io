---
layout: default
---

## Introduction

OpenSVBRDF is the first large-scale database of measured spatially-varying anisotropic reflectance, consisting of 1,000+ high-quality near-planar SVBRDFs, spanning 9 material categories such as wood, fabric and metal. To build this database, we develop a novel integrated system for robust, high-quality and -efficiency reflectance acquisition and reconstruction. Each sample is captured in 15 minutes, and represented as a set of high-resolution texture maps that correspond to spatially-varying BRDF parameters and local frames.

For more technical details, please refer to our <a href="https://svbrdf.github.io/publications/OpenSVBRDF/project.html/">journal-track paper</a > accepted to ACM SIGGRAPH Asia.


## Download 

We provide three components of data and the source code in the <a href="http://www.cad.zju.edu.cn/home/opensvbrdf/">database website</a>. You can download different contents based on your research needs.

Due to government regulations, the website may experience occasional unavailability. In such cases, please feel free to <a href="mailto:xiaohema1998@gmail.com?subject=Restricted%20Access%20to%20OpenSVBRDF&body=Please%20provide%20the%20following%20information.%0D%0A%0D%0AFirst%20name%3A%20%0D%0ALast%20name%3A%20%0D%0AYour%20institution%3A%20%0D%0AYour%20region%3A%20%0D%0AHave%20you%20registered%20before%3F%20%28y%2Fn%29%20">contact us</a> for assistance.

#### 1. Texture maps (50GB)
We store 6 texture maps for each sample in the database, which include GGX parameters (diffuse albedo, specular albedo, anisotropic roughness, normal and tangent), as well as transparency. All texture maps have a spatial resolution of 1,024×1,024. The total size is 50GB (each sample is 50MB).

#### 2. Neural representations (283GB)
We store the intermediate neural representations of all SVBRDFs (also described as latent vectors in the paper), with spatial resolution 1,024×1,024. The total size is 283GB (each sample is 290MB).

#### 3. Raw images (15TB)
We also store the 193 raw HDR photographs (with resolution of 24MP) for each sample. The total size is 15TB (each sample is 15GB).

#### 4. Code (Coming Soon)
The code encompasses all the steps from processing the original captured photographs to fine-tuning neural representations. You can also separately download the portion of the code that converts neural representations into lumitexel vectors.

## Benchmarks
In the future, We are going to set up open challenges (e.g., on material estimation, classification, generation) because standardized benchmarks based on our growing dataset might be useful to quantitatively evaluate existing as well as future research on a common ground. Further information will be added to the <a href="http://www.cad.zju.edu.cn/home/opensvbrdf/">database website</a>.

If you are interested in participating in setting up the benchmarks, please don't hesitate to <a href="mailto:xiaohema1998@gmail.com?subject=Setting%20Up%20Benchmarks%20Together!&body=Please%20provide%20the%20following%20information.%0D%0A%0D%0AFirst%20name%3A%0D%0ALast%20name%3A%0D%0AYour%20institution%3A%0D%0APlease%20describe%20your%20project%20experience%20or%20any%20helpful%20ideas%3A">contact us</a>.

## Acknowledgements

We would like to thank anonymous reviewers for their comments, Yaxin Yu and <a href="https://cocoakang.cn/">Kaizhang Kang</a> for help in building the prototype, and <a href="https://yuedong.shading.me/">Yue Dong</a>, <a href="https://www.microsoft.com/en-us/research/people/xtong/">Xin Tong</a>, <a href="https://graphics.cs.yale.edu/people/julie-dorsey">Julie Dorsey</a> and <a href="https://graphics.cs.yale.edu/people/holly-rushmeier">Holly Rushmeier</a> for their support. This work is partially supported by NSF China (62022072 & 62227806), Zhejiang Provincial Key R&D Program (2022C01057),the Fundamental Research Funds for the Central Universities, the XPLORER PRIZE and Information Technology Center and State Key Lab of CAD&CG, Zhejiang University.