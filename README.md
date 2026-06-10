# Machine Learning–based Separation of the He I 10830 Å Chromospheric Signal

This repository is the official open-source code for our paper, *"Machine Learning–based Separation of the He I 10830 Å Chromospheric Signal: Quantitative Analysis of Chromosphere–Corona Intensity in the Quiet Sun"*, published in **The Astrophysical Journal Supplement Series (ApJS)**.

🔗 **Official Paper Link:** [https://doi.org/10.3847/1538-4365/ae6911](https://doi.org/10.3847/1538-4365/ae6911)

## 📌 About the Project

In solar physics observations, the **He I 10830 Å chromospheric absorption line** serves as a critical diagnostic for investigating chromospheric–coronal coupling and coronal heating. However, observed chromospheric signals are severely contaminated by the intense underlying photospheric background. This non-linear mixing blurs fine chromospheric structures and poses a major challenge for rigorous quantitative physical analysis.

This project proposes a **signal decoupling framework that integrates deep learning with a physical model** to separate the He I 10830 Å chromospheric signal from the strongly coupled photospheric background. **To verify the physical reliability of the separation, we performed a thorough quantitative spatial correlation analysis on the extracted chromospheric data by combining it with extreme ultraviolet (EUV) multi-band observations from SDO/AIA. The results confirm the credibility of the decoupled signal for studying upper-atmospheric activities.**

---

## ✨ Key Features & Methodology

* **Dual-Dataset Strategy:** Accounts for the pronounced variations in morphology, intensity, and evolutionary characteristics between **Active Regions (AR)** and the **Quiet Sun (QS)** by constructing and optimizing two independent network models.
* **Cross-Band Deep Learning:** Employs **TiO continuum images** as input, leveraging the cross-band mapping capabilities of deep convolutional neural networks to precisely infer the pure He I 10830 Å photospheric background.
* **Physical Constraints & Multi-Band Verification:** Couples the neural-network-predicted photospheric background with an **Exponential Absorption Model** for rigorous quantitative reconstruction of the pure chromospheric component. Further cross-verification with **AIA EUV data** breaks free from pure data-driven "black-box" limitations, ensuring solid physical significance for the reconstructed structures.

---

## ⚠️ Scope & Limitations

> **💡 Note:**
> This framework represents an exploratory attempt dedicated specifically to **chromospheric–photospheric signal separation**. Although it yields robust quantitative decoupling results for the He I 10830 Å line and has been validated through multi-band quantitative analysis with AIA/SDO data, it is *not* a universal, catch-all solution for all generic cross-layer spectral line interferences or multi-layer line mixing problems. We aim to provide a targeted framework combining "data-driven + physics-constrained" approaches as a progressive step in model evolution, offering insights for future research into more general multi-layer solar atmospheric signal decoupling.

---

## 📄 Citation

If the code or methodology in this repository is helpful to your academic research, please cite our ApJS paper using the official BibTeX format below:

```bibtex
@article{Li_2026,
  doi       = {10.3847/1538-4365/ae6911},
  url       = {[https://doi.org/10.3847/1538-4365/ae6911](https://doi.org/10.3847/1538-4365/ae6911)},
  year      = {2026},
  month     = {jun},
  publisher = {The American Astronomical Society},
  volume    = {284},
  number    = {2},
  pages     = {79},
  author    = {Li, Huaiming and Xu, Fangyu and Bi, Yi and Jin, Zhenyu},
  title     = {Machine Learning–based Separation of the He I 10830 {\AA} Chromospheric Signal: Quantitative Analysis of Chromosphere–Corona Intensity in the Quiet Sun},
  journal   = {The Astrophysical Journal Supplement Series}
}
