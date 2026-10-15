---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

## Research Profile

My research focuses on source separation: recovering and characterizing latent components from mixed observations. I develop methods that use spectral structure, multiscale statistics, and knowledge of the acquisition system. During my Ph.D., I studied joint demosaicing and spectral unmixing for multispectral cameras. My current work investigates wavelet-based demixing of multivariate self-similar processes, including correlated sources.

A central question in my research is what makes sources distinguishable when statistical independence cannot be assumed and measurements are incomplete or distorted. I am interested in combining physical observation models with multiscale statistical constraints and learned priors to address these situations. My work on generative models for multifractal textures provides a basis for exploring priors that preserve the statistical properties of the signals to be separated.

## Source Separation of Multivariate Fractional Brownian Motion

In collaboration with [Patrice Abry](https://perso.ens-lyon.fr/patrice.abry/){:target="_blank"}, [Herwig Wendt](https://www.irit.fr/~Herwig.Wendt/){:target="_blank"}, and [Gustavo Didier](https://sse.tulane.edu/gustavo-didier){:target="_blank"}, I am currently working on blind source separation for multivariate self-similar Gaussian processes, with a particular focus on multivariate fractional Brownian motion (mfBm).

Multivariate fractional Brownian motions provide models for multivariate stochastic phenomena exhibiting long-range dependence and scale-invariant properties. When only linear mixtures of latent processes are observed, the challenge is to recover the underlying sources together with their scaling and dependence structures.

In this setting, the observed multivariate process can be written as

$$
X(t) = W Y(t),
$$

where \(X(t)\) denotes the observed mixtures, \(Y(t)\) the latent self-similar sources, and \(W\) the unknown mixing matrix. At the wavelet scale \(2^j\), the covariance structure of the observations can be modeled through

$$
\mathrm{Cov}(d_X(j, k)) = W \, \mathrm{Cov}(d_Y(j, k)) \, W^\top,
$$

where \(d_X(j,k)\) and \(d_Y(j,k)\) denote wavelet coefficients at scale \(2^j\) and location \(k\).

Our work develops wavelet- and covariance-based source separation methodologies that exploit the multiscale statistical structure of these processes. The objective is to jointly estimate the mixing matrix, the scaling parameters, and the covariance structure of the latent Gaussian sources.

This research provides a framework for blind source separation when classical assumptions such as statistical independence are not necessarily appropriate, by instead exploiting second-order statistics and multiscale scaling structures.

A first article resulting from this work, ["Wavelet-based Demixing for Multivariate Fractional Brownian Motion"](https://kinan3bb3s.github.io/files/Eusipco26_OfBm_Demix.pdf){:target="_blank"}, appears in the proceedings of the 34th European Signal Processing Conference (EUSIPCO 2026).

## Ph.D. Research: Joint Demosaicing and Unmixing of Multispectral Images

I conducted my Ph.D. research at [LISIC](https://lisic-prod.univ-littoral.fr/){:target="_blank"}, [Université du Littoral Côte d'Opale](https://www.univ-littoral.fr/){:target="_blank"}, under the supervision of [Matthieu Puigt](https://www-lisic.univ-littoral.fr/~puigt/){:target="_blank"} and [Gilles Roussel](https://scholar.google.com/citations?user=gtdZ87MAAAAJ&hl=fr){:target="_blank"}. My research focused on inverse problems and spectral unmixing for snapshot multispectral imaging.

Snapshot multispectral cameras acquire images in a single exposure, but provide spatially and spectrally incomplete measurements. Demosaicing reconstructs the full multispectral image, while spectral unmixing estimates the spectra of the materials present and their proportions at each location. My Ph.D. investigated solving these two problems jointly from the acquired measurements.

I developed two complementary frameworks using sparsity, non-negativity, and low-rank structures: one based on matrix completion, and another based on spectral deconvolution that accounts for the Fabry-Perot filters of the snapshot camera. These were published in *IEEE Transactions on Computational Imaging*: [Part I: A Matrix-Completion Framework]({{ '/publication/2024-01-01-locally-rank-one-based-joint-unmixing-and-demosaicing-methods-for-snapshot-spectral-images' | relative_url }}) and [Part II: A Filtering-Based Framework]({{ '/publication/2024-02-01-locally-rank-one-based-joint-unmixing-and-demosaicing-methods-for-snapshot-spectral-images-part-ii' | relative_url }}).

The resulting methods improved the quality of spectral unmixing while maintaining competitive reconstruction performance compared with conventional sequential approaches.

A further contribution was an entropy-weighted regularization strategy for Fabry-Perot spectral deconvolution. It accounts for the harmonic structure of the filters and improves spectral restoration compared with conventional deconvolution and the manufacturer's reconstruction approach. This work was published in *IEEE Sensors Letters*: [Fabry-Perot Spectral Deconvolution with Entropy-weighted Penalization]({{ '/publication/10631300' | relative_url }}).

<figure style="text-align: center;">
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(130px, 1fr)); gap: 20px;">
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
  <figcaption>Snapshot input (SSI) and segmentation results for a Hyko 2 database image. PPID and GRMR use demosaicing followed by unmixing; the proposed methods (KPWNMF, VPWNMF, FPKmeans, FPVCA, and Naive) solve both jointly. Compare the spatial extent and boundaries of the recovered regions.</figcaption>
</figure>

## Generative Models for Multifractal Texture Synthesis

In parallel with my research on source separation, I investigate generative modeling of scale-free and multifractal stochastic processes at the [Physics Laboratory of ENS Lyon](https://www.ens-lyon.fr/PHYSIQUE/){:target="_blank"}, in collaboration with [Patrice Abry](https://perso.ens-lyon.fr/patrice.abry/){:target="_blank"} and [Stéphane Roux](https://perso.ens-lyon.fr/stephane.roux/){:target="_blank"}.

The objective is to generate textures that reproduce the multiscale statistical properties of the training data.

I have investigated diffusion models, latent diffusion models, and generative adversarial networks for the synthesis of univariate and multivariate multifractal textures. Their performance is evaluated using multiscale statistical tools, including wavelet leaders and wavelet-based cumulants, allowing us to assess whether generated samples reproduce the scaling and multifractal properties of the target processes.

Our diffusion-model results were presented at [EUSIPCO 2025](https://kinan3bb3s.github.io/files/EUSIPCO_2025.pdf){:target="_blank"} and [GRETSI 2025](https://kinan3bb3s.github.io/files/GRETSI_2025_Diffusion_Models_Anisotropic.pdf){:target="_blank"}.

Starting from April 2026, M2 intern [Jhonatan Ancco Cerda](https://kinan3bb3s.github.io/advising/){:target="_blank"} has worked on this project, focusing on generative AI, diffusion models, and the generation of multivariate, multifractal, and anisotropic textures.

With Jhonatan, Stéphane Roux, and Patrice Abry, we submitted ["Large-size multivariate scale-free texture generation from small-size learning sets with self-attention Wasserstein-GAN"]({{ '/publication/2026-10-15-large-size-multivariate-scale-free-texture-generation' | relative_url }}) to <span style="color: red; font-weight: bold;">ICASSP 2027</span>. In this work, a fully convolutional Wasserstein-GAN with self-attention generates multivariate textures at sizes larger than the training images. We assess how well the generated textures preserve multiscale and cross-component statistics.

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

## Texture Authentication through Multiscale Representations and Siamese Learning

As part of my post-Ph.D. research at the [Physics Laboratory of ENS Lyon](https://www.ens-lyon.fr/PHYSIQUE/){:target="_blank"}, in collaboration with [Pulsalys](https://www.pulsalys.fr/){:target="_blank"} and [XMBauble](https://xmbauble.com/){:target="_blank"}, I worked on statistical texture analysis and machine-learning methodologies for the detection of counterfeit luxury products, together with [Patrice Abry](https://perso.ens-lyon.fr/patrice.abry/){:target="_blank"} and [Stéphane Roux](https://perso.ens-lyon.fr/stephane.roux/){:target="_blank"}.

The objective was to compare a newly acquired texture image with a reference to assess the authenticity of a product, despite changes in camera, illumination, and viewing angle. Applications included leather, carpets, and textiles.

I designed a Siamese neural network to compare texture representations with limited reference data. The approach combined hyperbolic wavelet representations and multiscale texture descriptors with few-shot learning.

I also contributed to an in-situ acquisition prototype combining optical, mechanical, and software components for capturing and comparing textures on products.

## Master's Research: Fog Computing Scheduling and Placement

My Master's degree in Computer Engineering, specializing in Networks and Computer Systems, was completed at Latakia University (formerly Tishreen University) in Syria. The program consisted of one year of advanced coursework followed by two years of research.

My research focused on resource placement and scheduling for real-time IoT applications in fog-computing environments. Different placement policies were evaluated through simulations of smart-city scenarios, with particular attention to service latency and cloud-resource utilization.

The study compared eight placement strategies and showed that HAFA and iFogStor-G provided favorable performance in terms of service time and reduced cloud-processor usage.
