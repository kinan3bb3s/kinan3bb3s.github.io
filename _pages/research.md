---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---
## Diffusion Models for Multifractal Texture Synthesis

This project is a part of my postdoctoral research at the [Physics Laboratory of ENS Lyon](https://www.ens-lyon.fr/PHYSIQUE/){:target="_blank"}, in collaboration with Prof. [Patrice Abry](https://perso.ens-lyon.fr/patrice.abry/){:target="_blank"} and Dr. [Stéphane Roux](https://perso.ens-lyon.fr/stephane.roux/){:target="_blank"}. We are investigating the degree to which diffusion models can generate univariate and multivariate multifractal, as well as anisotropic textures. We evaluate the performance using advanced multiscale analyses like wavelet-leader and dual-tree complex wavelet transforms, with the final goal of developing a model that can generate better textures. This research has recently resulted in two publications: "Modèles de diffusion pour la synthèse de textures anisotropes" accepted at [GRETSI 2025](https://kinan3bb3s.github.io/files/GRETSI_2025_Diffusion_Models_Anisotropic.pdf){:target="_blank"}, and "Diffusion Models for Multifractal Texture Synthesis" accepted at [EUSIPCO 2025](https://kinan3bb3s.github.io/files/EUSIPCO_2025.pdf){:target="_blank"}.
<div style="text-align: center;">
  <figure>
    <div style="display: flex; gap: 20px; justify-content: center;">
      <div>
        <img src="c1_j.png" alt="Subfigure 1" style="width: 75%;">
        <figcaption>Cumulant C1(2^j)</figcaption>
      </div>
      <div>
        <img src="c2_j.png" alt="Subfigure 2" style="width: 75%;">
        <figcaption>Cumulant C2(2^j)</figcaption>
      </div>
    </div>
    <figcaption>Figure: Cumulants C1(2^j) and C2(2^j) as functions of scales, averaged across the training set (blue) and diffusion model generated texture sets, obtained from different noise schedulers. The dashed black line materializes the theoretical scaling behavior across scales.</figcaption>
  </figure>
</div>


## Texture Analysis for the Detection of Counterfeit Luxury Products

 This work has been done as a part of my Postdoc at the [Physics Laboratory of ENS Lyon](https://www.ens-lyon.fr/PHYSIQUE/){:target="_blank"}, France, since July 15, 2024, in collaboration with [Pulsalys](https://www.pulsalys.fr/){:target="_blank"} and [XMBauble](https://xmbauble.com/){:target="_blank"}, focusing on developing innovative solutions in texture analysis and anti-counterfeiting technologies through machine learning and computer vision, alongside experts Prof. [Patrice Abry](https://perso.ens-lyon.fr/patrice.abry/){:target="_blank"} and Dr. [Stéphane Roux](https://perso.ens-lyon.fr/stephane.roux/){:target="_blank"} . This project targets the analysis of textures for anti-counterfeiting applications, successfully applied to leather, carpets, and textiles, aiming to address challenges posed by **texture variability** due to factors such as differences between cameras, lighting condition variations, shooting angles (*Point of View, POV*), and other environmental or contextual constraints. Our approach leverages **hyperbolic wavelet transforms** combined with deep learning techniques, specifically exploring **few-shot learning** and **Siamese networks** to enhance the methodology.

## Thesis: Joint demosaicing and unmixing of multispectral images

 I did my thesis in the LISIC lab at ULCO University under the supervision of Prof. [Matthieu Puigt](https://www-lisic.univ-littoral.fr/~puigt/){:target="_blank"} and Prof. [Gilles Roussel](https://scholar.google.com/citations?user=gtdZ87MAAAAJ&hl=fr){:target="_blank"}.

 In this work, we consider images sensed by a miniaturized multispectral (MS) snapshot camera. Contrary to classical RGB cameras, MS imaging allows for observing a scene on tens of different wavelengths, allowing a much more precise analysis of the observed content. 

 While most MS cameras require a scan to generate an image, snapshot MS cameras can instantaneously provide images or even videos. When the camera is miniaturized, instead of a 3D data cube, it gets a 2D image, each pixel being associated with a filtered version of the theoretical spectrum it should acquire. Post-processing, called "demosaicing", is then necessary to reconstruct a data cube. Furthermore, in each pixel of the image, the observed spectrum can be considered as a mixture of spectra of pure materials present in the pixel. Estimating these spectra, named endmembers as well as their spatial distribution (named abundances), is called "unmixing''. While a classical pipeline to process MS snapshot images is to first demosaice and then unmix the data, the work introduced in this thesis explores alternative strategies in which demosaicing and unmixing are jointly performed. Extending classical assumptions met in sparse component analysis and in remote sensing MS unmixing, we propose two different frameworks to restore and unmix the acquired scene, based on low-rank matrix completion and deconvolution, respectively, the latter being specifically designed for Fabry-Perot filters used in the considered camera. The four proposed methods exhibit a far better unmixing enhancement than the variants they extend when the latter are applied to demosaiced data. Still, they allow a similar demosaicing performance as state-of-the-art methods.

 The last part of the thesis introduces a deconvolution approach to restore the spectra of such cameras. Our contribution lies in the weights of the penalization term, which are automatically set using the entropy of the Fabry-Perot harmonics. The proposed method exhibits a better spectrum restoration than the strategy proposed by the camera manufacturer and than the classical deconvolution technique it extends.

<figure style="text-align: center;">
  <div style="display: flex; justify-content: center; gap: 20px;">
    <div>
      <img src="SSI.png" alt="SSI Image" style="width: 75%;">
      <figcaption>SSI Image</figcaption>
    </div>
    <div>
      <img src="PPID.png" alt="PPID" style="width: 75%;">
      <figcaption>PPID</figcaption>
    </div>
    <div>
      <img src="GRMR.png" alt="GRMR" style="width: 75%;">
      <figcaption>GRMR</figcaption>
    </div>
    <div>
      <img src="KPWNMF.png" alt="KPWNMF" style="width: 75%;">
      <figcaption>KPWNMF</figcaption>
    </div>
  </div>
  <div style="display: flex; justify-content: center; gap: 20px; margin-top: 20px;">
    <div>
      <img src="VPWNMF.png" alt="VPWNMF" style="width: 75%;">
      <figcaption>VPWNMF</figcaption>
    </div>
    <div>
      <img src="FPKmeans_V4.png" alt="FPKmeans" style="width: 75%;">
      <figcaption>FPKmeans</figcaption>
    </div>
    <div>
      <img src="FPVCA_V2.png" alt="FPVCA" style="width: 75%;">
      <figcaption>FPVCA</figcaption>
    </div>
    <div>
      <img src="Naive.png" alt="Naive" style="width: 75%;">
      <figcaption>Naive</figcaption>
    </div>
  </div>
  <figcaption>Figure: Segmentation of a Hyko 2 database image for different unmixing methods. Demosaicing is applied to the SSI image, followed by the generation of abundance maps and subsequent segmentation. For the proposed methods (VPWNMF, KPWNMF, FPVCA, FPKmeans, and Naive), unmixing and demosaicing were jointly applied.</figcaption>
</figure>


## Master's Work: Evaluating Fog Computing Scheduling and Placement Algorithms.

My Master's degree in **Computer Engineering / Networks and Computer Systems** was completed at Latakia University( Tishreen University before 2025), Latakia, Syria, following a one-year coursework phase and two years of research, a standard path before pursuing a PhD in the country.  My research focused on **Fog Computing** technologies, specifically evaluating algorithms for placement and scheduling of real-time IoT applications. The methods were tested in a simulated smart city, where analysis of eight placement policies demonstrated that HAFA and iFogStor-G approaches provided optimal service times and reduced cloud processor usage.

