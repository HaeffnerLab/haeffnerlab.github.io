---
title: Trap Technology
---

# {{ page.title }}

We develop novel ion trap technology that supports quantum information tasks such as computing and sensing. 
<br>

## 3D-Printed Ion Traps

In collaboration with Lawrence Livermore National Laboratories, UC Santa Barbara, and UC Riverside, we pioneered ion traps manufactured via two-photon-direct laser writing.
This technology allows to print complex three-dimensional structures with sub-micrometer resolution. Theses 3D-printed ion traps combine the advantages, such as strong radial confinement, of traditionally machined 3D traps with on-chip miniaturization. The tight confinement eases ion cooling requirements and speeds up a variety of important operations. More importantly, the design freedom of these 3D printed traps allows the researcher to customize these traps to their needs in quantum information science, precision metrology, and mass spectrometry.  

For more information see:

**"3D-Printed Micro Ion Trap Technology for Scalable Quantum Information Processing"**  
S. Xu, X. Xia, Q. Yu, S. Khan, E. Megidish, B. You, B. Hemmerling, A. Jayich, J. Biener, H. Häffner  
[Nature 645, 362-368 (2025)](https://www.nature.com/articles/s41586-025-09474-1), [arXiv:2310.00595](https://arxiv.org/abs/2310.00595).

<figure>
	<img src="/research/trap-technology/paul-trap-comparison.jpg" alt="Schematics and photographs comparing conventional, surface, and 3D-printed Paul traps" width="700" />
	<figcaption>
		Schematics and representative pictures of (a) a conventional 3D Paul trap, (b) a planar surface trap, and (c) our 3D-printed vertical Paul trap. The 3D-printed design retains the deep trapping potential and high trap frequency of macroscopic 3D traps while remaining as scalable as surface traps. Figure from Xu <i>et al.</i>, Nature <b>645</b>, 362-368 (2025).
	</figcaption>
</figure>

## Integrated Photonics

Scaling trapped-ion quantum processors requires delivering laser light to many ions simultaneously with high precision and stability. We pursue two complementary on-chip technologies for this control &mdash; one built around 3D-printed micro-optics, the other around grating couplers.

### 3D-Printed Micro-Optics

Together with Ming Wu's group (UC Berkeley EECS) and collaborators at UCLA, we develop a hybrid 2D-3D photonic integrated circuit that pairs a planar waveguide lens with a 3D-printed mirror in a 4-F configuration. This design delivers diffraction-limited, multi-spot focusing across an unusually broad band (405-950 nm), covering nearly all wavelengths used in trapped-ion experiments while minimizing chromatic aberrations. The surface-electrode trap is patterned monolithically on top of the PIC, restricting light-dielectric interfacing to a metal-shielded vertical facet and mitigating photoinduced charging &mdash; a long-standing obstacle to scaling integrated-photonic ion traps. The Gen 1.0 device has been deployed in a UHV chamber and used to trap single <sup>40</sup>Ca<sup>+</sup> ions, with Gen 1.1 and Gen 2.0 designs targeting reduced surface scattering and aberrations. This effort is supported by the [Challenge Institute for Quantum Computation (CIQC)](https://ciqc.berkeley.edu/).

**"Characterization of A Novel 2D-3D Photonic Integrated Circuit for Broadband, High-Efficiency Control of Trapped Ion Qubits"**  
D. Klawson, B. You, K. Sun, Q. Wu, Y. Zhi, L. Jiang, W. Ke, J. Lee, C.Y. Fan, A. Roy, S. Tang, J. Luo, B. Saarel, S. Xu, M. Bareian, M. C. Wu, H. H&auml;ffner  
DAMOP 2025 (poster).

<figure>
	<img src="/research/trap-technology/2d3d-pic-sem.jpg" alt="False-color scanning-electron micrograph of the 2D-3D photonic integrated circuit" height="230" />
	<img src="/research/trap-technology/2d3d-pic-wavelengths.png" alt="Top-down focal-plane images of the focused beam from 405 nm to 950 nm" height="230" />
	<figcaption>
		<i>Top:</i> false-color electron micrograph of one PIC element, with the planar waveguide lens (blue) and the 3D-printed biconic mirror (teal) underneath the surface-trap electrodes.
		<br/>
		<i>Bottom:</i> top-down focal-plane images of the focused beam at eight wavelengths from 405 nm to 950 nm, demonstrating broadband, near diffraction-limited focusing covering nearly all wavelengths used in trapped-ion experiments.
	</figcaption>
</figure>

### Grating Couplers

In collaboration with UC Irvine, UC Davis, and UC Santa Barbara, we are also exploring focusing grating couplers embedded in a surface-electrode trap to individually address closely-spaced ions through openings in the trap electrodes. By tailoring the coupler geometry with adjoint optimization and controlling the interference of higher-order TE modes, the device delivers diffraction-limited focal spots with simulated crosstalk down to -60 dB at ion separations of 5-8 &micro;m. The higher-order modes themselves provide a new handle for driving spin-motion-coupling transitions, suggesting alternative routes to quantum gates and simulations. This effort is supported by the [UC Noyce Initiative](https://ucnoyce.org/).

**"Individual trapped-ion addressing with adjoint-optimized multimode photonic circuits"**  
M. Momenzadeh, K. Sun, Q. Wu, B. You, Y.-L. Tang, H. H&auml;ffner, M. R. Shcherbakov  
[npj Nanophotonics 3, 3 (2026)](https://www.nature.com/articles/s44310-025-00102-4), [arXiv:2505.08997](https://arxiv.org/abs/2505.08997).

<figure>
	<img src="/research/trap-technology/grating-coupler-concept.jpg" alt="Conceptual rendering and material stack of the multimode grating-coupler ion trap" width="750" />
	<figcaption>
		<i>Left:</i> conceptual rendering of the surface-electrode trap with adjoint-optimized multimode grating couplers individually addressing three closely-spaced <sup>40</sup>Ca<sup>+</sup> ions through openings in the electrodes.
		<br/>
		<i>Right:</i> cross-section of the device stack &mdash; apodized SiN gratings beneath SiO<sub>2</sub> and Au layers, with an ITO film shielding the ions from interface charging. Figure from Momenzadeh <i>et al.</i>, npj Nanophotonics <b>3</b>, 3 (2026).
	</figcaption>
</figure>
