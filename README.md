# 🧠 Micro- and Nanoplastics: Crossing the Blood-Brain Barrier to Drive Sustained Neuroinflammation and HPA Axis Dysregulation

This repository contains the **Quarto** source code and supporting files for an academic paper submitted for the **Immunology (BT335IU)** course. The manuscript is rendered using a **locally vendored and modified version of the Hikmah Academic Quarto template**, ensuring consistent formatting, citations, and figure handling across systems.

> **Document Preview:** A rendered `.docx` version of the manuscript is included in this repository for quick viewing without rendering the source files.

---

## 🎯 Project Overview

This paper examines the neurotoxic potential of **Micro- and Nanoplastics (MNPs)**, focusing on their ability to traverse the Blood–Brain Barrier (BBB) and induce chronic neuroinflammation and dysregulation of the Hypothalamic–Pituitary–Adrenal (HPA) axis.

* **Topic:** Immune Response Under Environmental Stress
* **Course:** Immunology (BT335IU)
* **Author:** Tran Quoc Hoang
* **Student ID:** BTBTWE24036
* **Professor:** Assoc. Prof. Hoai T. T. Nguyen
* **Due Date:** 12/22/2025

**Abstract Highlights:**

* Nanoplastics can enter the body via ingestion and inhalation and cross the BBB through mechanisms such as endocytosis and the “Trojan Horse” effect.
* Persistent microglial activation (frustrated phagocytosis) and NLRP3 inflammasome activation drive sustained neuroinflammation.
* Peripheral MNP exposure through the Gut–Brain Axis (GBA) can cause systemic inflammation that secondarily activates microglia and dysregulates the HPA axis.
* Consequences include anxiety-like behaviours, cognitive impairment, and endocrine disruption; therapeutic targets such as BBB-permeable NLRP3 inhibitors are discussed.

---

## 💻 Technical Environment

This project uses **Quarto (CLI)** and **R (RStudio)** to dynamically generate the manuscript. The R package environment is managed by **`renv`** for exact reproducibility.

### Main Files

* **Manuscript Source:** `TranQuocHoang_IM25_Newsletter.qmd`
* **Bibliography:** `bibliography.bib`
* **Figures / Images:** `photos/`
* **Project Lockfile:** `renv.lock`
* **Quarto Extensions:** `_extensions/` (includes a modified Hikmah Academic template)

### Manuscript Metadata (from YAML)

* **Output format:** `hikmah-manuscript-docx` (table of contents disabled)
* **Citation style:** `elsevier-vancouver.csl`
* **Keywords:** Microplastic, Nanoplastic, Neuroinflammation, Microglia, Gut-Brain-Axis, HPA

---

## ⚠️ Disclaimer

This README intentionally omits an explicit list of system-level packages and platform-specific build commands. Collaborators are expected to manage any required system dependencies appropriate to their environment.

The project is reproducible at the **R/Quarto level** via `renv` and the vendored Quarto extension included in this repository.

---

## 🛠 Minimal Setup & Rendering Instructions

### 1️⃣ Restore R project environment

Open R or RStudio in the project directory and run:

```r
install.packages("renv")    # if not already installed
renv::restore()             # installs exact versions from renv.lock
```

This installs all R packages required to render the manuscript, including rendering and LaTeX support where applicable.

---

### 2️⃣ Install Quarto

Install **Quarto** if not already available:
[https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/)

Verify installation:

```bash
quarto check install
```

> No additional Quarto extensions are required — the modified Hikmah template is already included in `_extensions/`.

---

### 3️⃣ Render the manuscript (.docx)

From the project root:

```bash
quarto render TranQuocHoang_IM25_Newsletter.qmd
```

The output `.docx` file is generated using the local Hikmah-based format defined in the YAML. A rendered preview is already included in the repository.

---

## 📚 Key Sections (Manuscript)

1. **Introduction:** MNP definitions, prevalence, and Gut–Brain Axis framing
2. **MP Transport & BBB Crossing:** Routes of entry, BBB structure, translocation hypotheses, associated toxicants
3. **Microglial Activation & Neuroinflammation:** Frustrated phagocytosis, NLRP3 inflammasome cascade
4. **Gut–Brain Axis & Indirect Effects:** Peripheral inflammation driving central immune activation
5. **Functional Consequences & HPA Disruption:** Behavioural, cognitive, and endocrine outcomes
6. **Treatment & Prevention:** Policy, remediation, and therapeutic targets
7. **Conclusion & Future Directions:** Epidemiology, mechanistic gaps, real-world exposure priorities

---

## ⚖️ Declaration of Competing Interest

The author declares no competing interests.

---

## 📂 Data & Code Availability

The complete Quarto project — manuscript source, figures, bibliography, and modified template — is available in this repository. A rendered `.docx` preview is included for convenience.

Repository:
[https://github.com/ht2905/TranQuocHoang_IM25_Newsletter](https://github.com/ht2905/TranQuocHoang_IM25_Newsletter)