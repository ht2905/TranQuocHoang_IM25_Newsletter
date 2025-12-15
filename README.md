# 🧠 Micro- and Nanoplastics: Crossing the Blood-Brain Barrier to Drive Sustained Neuroinflammation and HPA Axis Dysregulation

This repository contains the **Quarto** source code and supporting files for an academic paper submitted for the **Immunology (BT335IU)** course. The manuscript was prepared using the **Hikmah Academic Quarto** template for journal-ready formatting, references, and figures.

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

### Manuscript metadata (from YAML)

* **Output format:** `hikmah-manuscript-docx` (table of contents disabled) — renders to `.docx`
* **Citation style:** `elsevier-vancouver.csl`
* **Keywords:** Microplastic, Nanoplastic, Neuroinflammation, Microglia, Gut-Brain-Axis, HPA

---

## ⚠️ Disclaimer

This README intentionally omits an explicit list of system-level packages and platform-specific build commands. Collaborators are expected to manage any required system dependencies appropriate to their environment. The project is reproducible at the R/Quarto level via `renv` and the steps below; however, rendering advanced outputs (e.g., PDF) can require additional system libraries or LaTeX, which are not documented here.

---

## 🛠 Minimal Setup & Rendering Instructions

> Note: system-level dependencies (OS packages, LaTeX, etc.) are **not** listed here. Install them yourself as appropriate for your platform.

### 1️⃣ Restore R project environment

Open R or RStudio in the project folder and run:

```r
install.packages("renv")    # if not already installed
renv::restore()             # installs packages locked in renv.lock
```

This will install the exact R package versions used to create the manuscript (including `knitr`, `rmarkdown`, `tinytex` if present in the lockfile).

### 2️⃣ Install Quarto & Hikmah template

1. Install **Quarto** if you don't have it: [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/). Verify with:

```bash
quarto check install
```

2. Add the **Hikmah Academic Quarto** template to your project:

```bash
quarto add andrewheiss/hikmah-academic-quarto
```

(If you previously used other Quarto extensions like `apaquarto`, you can keep or remove them as desired — this project uses the Hikmah docx format by default.)

### 3️⃣ Render the manuscript (.docx)

From the project root:

```bash
quarto render TranQuocHoang_IM25_Newsletter.qmd
```

The output will be a `.docx` file as configured by the YAML (`hikmah-manuscript-docx`). The generated `.docx` file included in this repository serves as the quick preview.

---

## 📚 Key Sections (Manuscript)

1. **Introduction:** MNP definitions, prevalence, and Gut–Brain Axis framing
2. **MP Transport & BBB Crossing:** Routes of entry, BBB structure, translocation hypotheses (endocytosis, Trojan Horse), and associated toxicants
3. **Microglial Activation & Neuroinflammation:** Frustrated phagocytosis, NLRP3 inflammasome cascade, and cytokine-mediated damage
4. **Gut–Brain Axis & Indirect Effects:** Peripheral inflammation driving central immune activation
5. **Functional Consequences & HPA Disruption:** Behavioural, cognitive, and endocrine outcomes from chronic inflammation
6. **Treatment & Prevention:** Policy, remediation, and therapeutic target (e.g., BBB-permeable NLRP3 inhibitors)
7. **Conclusion & Future Directions:** Epidemiology, mechanistic gaps, and real-world exposure priorities

---

## ⚖️ Declaration of Competing Interest

The author declares no competing interests.

---

## 📂 Data & Code Availability

The Quarto project underlying this paper — manuscript source, figures, and bibliography — is available in this repository. A rendered `.docx` preview is included for quick reference.

Repository: [https://github.com/ht2905/TranQuocHoang_IM25_Newsletter](https://github.com/ht2905/TranQuocHoang_IM25_Newsletter)
