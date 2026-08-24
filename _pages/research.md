---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

## Research Profile

> The observed world is often incomplete and mixed. My research asks which statistical, spectral, and multiscale structures make it possible to reconstruct what is missing and recover the hidden sources behind complex data.

My research lies at the intersection of statistical signal and image processing, source separation, inverse problems, multiscale analysis, and machine learning. A central direction of my work concerns the recovery and characterization of latent sources from complex observations by exploiting their structural, statistical, and multiscale properties.

During my Ph.D., I investigated spectral unmixing and source separation in multispectral imaging, developing methods based on sparse component analysis, nonnegative matrix factorization, low-rank models, and inverse problems. More recently, my research has focused on blind source separation of multivariate stochastic processes, where multiscale and covariance structures are exploited to recover latent sources and their statistical properties.

In parallel, I investigate statistical learning and generative models for complex signals and textures, particularly diffusion models and generative adversarial networks for scale-free and multifractal processes. Across these topics, the common thread is the same: building models that turn partial, mixed, or highly structured observations into interpretable representations.

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

Unlike conventional multispectral cameras that acquire spectral bands sequentially, snapshot multispectral cameras enable instantaneous acquisition and are therefore suitable for dynamic scenes and videos. However, miniaturized snapshot sensors provide spatially and spectrally incomplete measurements, requiring a reconstruction step known as demosaicing to recover the complete multispectral data cube.

At the same time, the spectrum observed at each spatial location can often be modeled as a mixture of spectra associated with pure materials, called endmembers, with corresponding spatial proportions known as abundances. Recovering these latent components constitutes a spectral unmixing problem.

Rather than following the conventional pipeline in which the multispectral image is first demosaiced and subsequently unmixed, my Ph.D. investigated joint demosaicing and unmixing, incorporating the source-separation problem directly into the reconstruction of the acquired measurements.

Conceptually, this problem links inverse problems and source separation: the measurements are both incomplete because of the sensor acquisition model and mixed because each pixel can contain several latent spectral components.

Building upon assumptions from Sparse Component Analysis (SCA), Nonnegative Matrix Factorization (NMF), and hyperspectral unmixing, I developed several approaches exploiting sparsity, non-negativity, and low-rank structures. Two complementary frameworks were investigated: one based on low-rank matrix completion, and another based on spectral deconvolution, specifically accounting for the Fabry-Perot filters used by the considered snapshot camera.

The resulting methods improved the quality of spectral unmixing while maintaining competitive reconstruction performance compared with conventional sequential approaches.

A further contribution of the thesis concerned spectral deconvolution for Fabry-Perot imaging systems. I developed an entropy-weighted regularization strategy that accounts for the harmonic structure of the filters and improves spectral restoration compared with conventional deconvolution and the manufacturer's reconstruction approach.

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

## Generative Models for Multifractal Texture Synthesis

In parallel with my research on source separation, I investigate generative modeling of scale-free and multifractal stochastic processes at the [Physics Laboratory of ENS Lyon](https://www.ens-lyon.fr/PHYSIQUE/){:target="_blank"}, in collaboration with [Patrice Abry](https://perso.ens-lyon.fr/patrice.abry/){:target="_blank"} and [Stéphane Roux](https://perso.ens-lyon.fr/stephane.roux/){:target="_blank"}.

The objective is to determine whether modern generative models can reproduce not only the visual appearance of complex textures, but also their multiscale statistical properties.

I have investigated diffusion models, latent diffusion models, and generative adversarial networks for the synthesis of univariate and multivariate multifractal textures. Their performance is evaluated using multiscale statistical tools, including wavelet leaders and wavelet-based cumulants, allowing us to assess whether generated samples reproduce the scaling and multifractal properties of the target processes.

In this line of work, the goal is not only to generate visually plausible samples, but also to preserve the hidden statistical organization of the data across scales.

A further direction of this research concerns the generation of textures on spatial supports larger than those used during training, through fully convolutional generative architectures and self-attention mechanisms.

This research has resulted in work presented at [EUSIPCO 2025](https://kinan3bb3s.github.io/files/EUSIPCO_2025.pdf){:target="_blank"} and [GRETSI 2025](https://kinan3bb3s.github.io/files/GRETSI_2025_Diffusion_Models_Anisotropic.pdf){:target="_blank"}, and continues through the study of multivariate multifractal texture generation and super-resolution.

Starting from April 2026, M2 intern [Jhonatan Ancco Cerda](https://kinan3bb3s.github.io/advising/){:target="_blank"} has worked on this project, focusing on generative AI, diffusion models, and the generation of multivariate, multifractal, and anisotropic textures.

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

## Multiscale Texture Analysis and Machine Learning for Counterfeit Detection

As part of my post-Ph.D. research at the [Physics Laboratory of ENS Lyon](https://www.ens-lyon.fr/PHYSIQUE/){:target="_blank"}, in collaboration with [Pulsalys](https://www.pulsalys.fr/){:target="_blank"} and [XMBauble](https://xmbauble.com/){:target="_blank"}, I worked on statistical texture analysis and machine-learning methodologies for the detection of counterfeit luxury products, together with [Patrice Abry](https://perso.ens-lyon.fr/patrice.abry/){:target="_blank"} and [Stéphane Roux](https://perso.ens-lyon.fr/stephane.roux/){:target="_blank"}.

The objective was to characterize and recognize material textures under realistic acquisition variability, including changes in cameras, illumination conditions, viewing angles, and other environmental factors. Applications included leather, carpets, and textiles.

Our approach combined hyperbolic wavelet representations and multiscale texture descriptors with machine-learning methods, including few-shot learning and Siamese neural networks, with the objective of achieving robust material recognition from limited reference data.

This work illustrates a broader aspect of my research: combining multiscale statistical representations with modern machine-learning approaches to extract reliable structure from complex signals and images under real acquisition constraints.

## Master's Research: Fog Computing Scheduling and Placement

My Master's degree in Computer Engineering, specializing in Networks and Computer Systems, was completed at Latakia University (formerly Tishreen University) in Syria. The program consisted of one year of advanced coursework followed by two years of research.

My research focused on resource placement and scheduling for real-time IoT applications in fog-computing environments. Different placement policies were evaluated through simulations of smart-city scenarios, with particular attention to service latency and cloud-resource utilization.

The study compared eight placement strategies and showed that HAFA and iFogStor-G provided favorable performance in terms of service time and reduced cloud-processor usage.
