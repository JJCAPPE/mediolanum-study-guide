# Banca Mediolanum Internship Study Guide

This repository contains a LaTeX study guide for preparing for a Banca Mediolanum Marketing Clienti internship. The guide is aimed at a computer engineering student and focuses on the business, CRM, segmentation, campaign automation, analytics, machine learning, and compliance context needed to understand a client-marketing role in a bank.

The generated PDF is `mediolanum_study_guide.pdf`.

## Contents

- `main.tex` - main LaTeX source for the complete study guide.
- `LegrandOrangeBook.cls` - bundled Legrand Orange Book document class used by the guide.
- `sample.bib` - BibLaTeX bibliography file currently included by the document.
- `Images/` - template images, title-page background, logos, and header source imagery.
- `build_preview/` - selected rendered page previews as PNG files.
- `logs/` - LaTeX build log files.
- `mediolanum_study_guide.pdf` - compiled output artifact.

The top-level `mediolanum_study_guide.*` files with extensions such as `.aux`, `.bcf`, `.toc`, `.lof`, `.lot`, `.idx`, `.ptc`, and `.run.xml` are generated LaTeX build artifacts.

## Build Requirements

Install a full LaTeX distribution such as MacTeX or TeX Live. The document uses common LaTeX packages plus the bundled `LegrandOrangeBook.cls` template. `latexmk` is recommended for repeatable builds.

## Build

From the repository root:

```sh
latexmk -pdf -interaction=nonstopmode -file-line-error -jobname=mediolanum_study_guide main.tex
```

If you want to keep build logs grouped after compiling:

```sh
mkdir -p logs
mv -f mediolanum_study_guide.log logs/
```

The output PDF is written as `mediolanum_study_guide.pdf`.

## Document Scope

The guide is structured as a one-week preparation plan:

- Days 1-2: Mediolanum, banking basics, retail banking, wealth management, and bancassurance.
- Day 3: organizational context, client marketing, and CRM systems.
- Day 4: segmentation, personalization, and marketing automation.
- Day 5: machine learning use cases and data pipelines.
- Day 6: metrics, experimentation, compliance, privacy, and governance.
- Day 7: technical bridge, integrated case study, resources, glossary, interview prep, and final cheat sheet.

The content is for internship preparation only. It is not investment, legal, compliance, or employment advice.
