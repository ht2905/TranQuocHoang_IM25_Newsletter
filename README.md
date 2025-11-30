# 🧠 Micro- and Nanoplastics: Crossing the Blood-Brain Barrier to Drive Sustained Neuroinflammation and HPA Axis Dysregulation

This repository contains the **Quarto** source code and supporting files for an academic paper submitted for the **Immunology (BT335IU)** course.

---

## 🎯 Project Overview

This paper explores the neurotoxic potential of **Micro- and Nanoplastics (MNPs)**, focusing on their ability to traverse the Blood-Brain Barrier (BBB) and induce chronic neuroinflammation and HPA Axis dysregulation.

* **Topic:** Immune Response Under Environmental Stress.
* **Course:** Immunology (BT335IU)
* **Author:** Tran Quoc Hoang
* **Submission Deadline:** 31 October 2025

---

## 💻 Technical Environment

This project uses **Quarto (CLI)** and **R (RStudio)** for dynamic document generation. The R package environment is managed by **`renv`** to ensure exact reproducibility.

### Source Files
* **Main Document Source:** `TranQuocHoang_IM25_Newsletter.qmd`
* **Bibliography:** `IM25_Newsletter.bib` (Managed via Zotero + Better BibTeX)

### Development Environment (For Reference)
The project was developed in a Linux environment:
* **Host OS:** Windows 11
* **Virtualization:** WSL2
* **Linux Distribution:** Ubuntu 22.04 LTS (Noble)

---

## 🚀 Setup & Rendering Instructions (A Single, Coherent Guide)

To compile this document and reproduce the final output (`.docx` and potentially `.pdf`), you must install **external system libraries**, **R packages**, and **Quarto extensions** in sequence.

### Step 1: Install Critical Linux System Dependencies (WSL/Ubuntu)

The R packages `ragg` and `systemfonts` require specific **development headers** (build dependencies) to compile successfully in a Linux environment. These **must** be installed via your terminal **before** installing R packages.

| Dependency | Command (in **WSL Terminal**) | Purpose |
| :--- | :--- | :--- |
| **R Dev Tools** | `sudo apt install r-base-dev` | Required for compiling many R packages from source. |
| **Graphics Libs** | `sudo apt install libfontconfig1-dev libfreetype6-dev libwebp-dev` | Essential for `ragg` and `systemfonts` to handle fonts and image formats (WebP). |

### Step 2: R Environment and Package Setup

The R version and all project dependencies are managed by the **`renv.lock`** file.

1. **Activate Environment:** **Open the `.Rproj` file** in RStudio to automatically activate the `renv` environment.  
2. **Install Packages:** Run the following command in the **R Console** to install the exact required versions:
```r
renv::restore()
```

### Step 3: Quarto Extensions and LaTeX

These external tools are required for formatting and PDF compilation.

| Dependency | Command (in **Terminal**) | Description |
| :--- | :--- | :--- |
| **APA Quarto Format** | `quarto install extension wjschne/apaquarto` | Installs the extension for APA citation and document formatting. |
| **TinyTeX** | `quarto install tinytex` | Essential for compiling PDF output via LaTeX (if enabled in the `.qmd` file). |

### Step 4: Render the Document

Once all dependencies are set up, run the render command from the **Terminal** or the **Terminal** pane in RStudio.

```bash
quarto render TranQuocHoang_IM25_Newsletter.qmd