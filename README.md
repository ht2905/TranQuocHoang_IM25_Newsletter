# 🧠 Micro- and Nanoplastics: Crossing the Blood-Brain Barrier to Drive Sustained Neuroinflammation and HPA Axis Dysregulation

This repository contains the Quarto source code and supporting files for an academic paper submitted for the **Immunology (BT335IU)** course.

-----

## 🎯 Project Overview

This paper explores the neurotoxic potential of Micro- and Nanoplastics (MNPs), focusing on their ability to traverse the Blood-Brain Barrier (BBB) and induce chronic inflammation and HPA Axis dysregulation.

  * **Topic:** Immune Response Under Environmental Stress.
  * **Course:** Immunology (BT335IU)
  * **Author:** Tran Quoc Hoang
  * **Submission Deadline:** 31 October 2025

-----

## 💻 Technical Environment

This project is built using **Quarto** and **R (RStudio)** for dynamic document generation. To ensure true reproducibility, the R environment is managed by **`renv`**.

### Source Files

  * **Main Document Source:** `TranQuocHoang_IM25_Newsletter.qmd`
  * **Bibliography:** `IM25_Newsletter.bib` (Managed via Zotero + Better BibTeX)

### Operating System (For Reference)

The environment used for initial development was:

  * **Host OS:** Windows 11
  * **Virtualization:** WSL2
  * **Linux Distribution:** Ubuntu 22.04 LTS

-----

## 🚀 Setup & Rendering Instructions (3-Step Guide)

To compile this document and reproduce the final output, please follow these steps sequentially.

### 1\. R Environment and Package Setup

The R version and all package dependencies are managed by the **`renv.lock`** file.

| Action | Command (in **R Console**) | Description |
| :--- | :--- | :--- |
| **A. Activate Environment** | **Open the `.Rproj` file** in RStudio. | This automatically activates the `renv` environment. |
| **B. Install Packages** | `renv::restore()` | Reads `renv.lock` and installs the **exact package versions** required, including `yaml`. |

### 2\. Quarto Extensions and System Dependencies

These required external tools are **not** managed by `renv` and must be installed via the Terminal.

| Dependency | Command (in **Terminal** Pane) | Description |
| :--- | :--- | :--- |
| **APA Quarto Format** | `quarto add wjschne/apaquarto` | Installs the necessary extension for APA citation formatting. |
| **TinyTeX** | `quarto install tinytex` | Essential for compiling PDF output via LaTeX. |
| **R Development Tools** | `sudo apt install r-base-dev` | Required on Linux systems (like WSL) to successfully compile some R packages from source. |

### 3\. Render the Document

Once all dependencies are set up, run the render command from the R Console:

```r
quarto::quarto_render("TranQuocHoang_IM25_Newsletter.qmd")
```

Alternatively, simply click the **Render** button in RStudio while the `.qmd` file is open.