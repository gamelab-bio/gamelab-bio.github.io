---
layout: page
title: Research
permalink: /research.html
---

## Research

<div class="research-intro">
<div class="research-panel research-intro-figure"><img class="panel-light" src="/assets/panels/00-adaptation.svg" alt="A central cancer cell within a stress gradient, switching between glycolytic, dormant, drug-tolerant and metabolically flexible survival strategies" /><img class="panel-dark" src="/assets/panels/00-adaptation-dark.svg" alt="" /></div>
<div class="research-intro-text" markdown="1">

We study how cancer cells adopt different survival mechanisms upon microenvironmental changes and stress. cancer cells have extraordinary adaptation mechanisms that allow them to acquire adaptive survival strategies — such as a glycolytic switch under hypoxia, senescence or dormancy in hostile environments, drug-tolerant persistence under therapeutic pressure, or metabolic flexibility under nutrient stress. we focus on the genomic and transcriptional strategies that make this adaptation possible, on how those strategies coexist and regulate one another within a single tumor, and on how they shape — and are shaped by — the other cell types that make up the tumor microenvironment.

</div>
</div>

### inter-cellular and inter-strategy games in cancer

<div class="research-panel research-panel-left"><img class="panel-light" src="/assets/panels/01-games.svg" alt="Network of cells of two strategies with a payoff matrix" /><img class="panel-dark" src="/assets/panels/01-games-dark.svg" alt="" /></div>

A tumor is an ecosystem in which cancer cells play games. we model the interactions between cells — and between the strategies they pursue — as games, where each cell's strategy depends on what its neighbors are doing. this game-theoretic view explains how distinct strategies — proliferative, secretory, invasive — coexist, compete, cooperate, and regulate one another; why heterogeneity is stable, when one strategy outcompetes another, and how the rules of the game might be turned against the tumor.

### cell-cell communication between different cellular strategies

<div class="research-panel"><img class="panel-light" src="/assets/panels/02-communication.svg" alt="Two cell groups exchanging secreted factors and a contact junction" /><img class="panel-dark" src="/assets/panels/02-communication-dark.svg" alt="" /></div>

Strategies don't act in isolation — they talk to each other. we study the signaling that passes between cancer cells pursuing different strategies, from secreted factors to contact-dependent cues, and ask how this communication coordinates behavior, hands off advantages between states, and shapes which strategies prevail.

### stress-responsive epigenetic and transcriptional landscapes

<div class="research-panel research-panel-left"><img class="panel-light" src="/assets/panels/03-stress-epigenetics.svg" alt="Nucleosome fiber over an energy landscape" /><img class="panel-dark" src="/assets/panels/03-stress-epigenetics-dark.svg" alt="" /></div>

Stress reshapes how cells behave, and cancer cells are usually under substantial stress. stress also affects how the genome is read. we map the epigenetic and transcriptional landscapes that cancer cells deploy under cellular, metabolic, and microenvironmental stress — and how these regulatory programs prime cells for adaptation. to resolve this at the level of specific genomic loci, we combine quantitative genomic locus proteomics, advanced DNA footprinting and next-generation sequencing.

## our tools

We develop and apply quantitative methods to read out how different cancer strategies coexist, compete, cooperate, and regulate one another, and how stress response reshapes the communication between different cell strategies and cell types.

### genomic locus proteomics & GLproxScape

<div class="research-panel"><img class="panel-light" src="/assets/panels/04-locus-proteomics.svg" alt="A DNA locus with a proximity-labeling capture radius and nearby proteins" /><img class="panel-dark" src="/assets/panels/04-locus-proteomics-dark.svg" alt="" /></div>

We use genomic locus proteomics to capture the proteome associated with specific genomic loci in living cells — identifying transcription factors and chromatin regulators that occupy a promoter or regulatory element of interest. to extract biological meaning from the resulting data, we developed GLproxScape, an R package that performs spatial deconvolution of genomic locus proteomics datasets and generates locus-resolved binding predictions.

### cellMUX-CRISPR screens

<div class="research-panel research-panel-left"><img class="panel-light" src="/assets/panels/05-cellmux-crispr.svg" alt="A multiplexed library demultiplexed into different cell types with distinct barcodes" /><img class="panel-dark" src="/assets/panels/05-cellmux-crispr-dark.svg" alt="" /></div>

Unlike traditional CRISPR screens where we target all cells with the same library, cellMUX-CRISPR screens are designed to target different cell types with different libraries, and employ combined experiments. we use this method with CROP-seq and Perturb-DBiT to understand interdependencies of different cell strategies, and different cell types in cancer tissues.

### single cell methods

<div class="research-panel"><img class="panel-light" src="/assets/panels/06-scrna-spatial.svg" alt="Expression clusters mapped onto a tissue section" /><img class="panel-dark" src="/assets/panels/06-scrna-spatial-dark.svg" alt="" /></div>

We use single cell RNA sequencing (scRNA-seq) and spatial transcriptomics methods to resolve how strategies are distributed across cells and tissue. additionally, we adopt and implement emerging single-cell technologies to broaden the molecular information we extract from individual cells — such as DNA accessibility (SHARE-seq), DNA footprinting (D&D-seq), DNA methylation (ME-seq), surface protein expression (CITE-seq), and phosphorylation (Phospho-seq), according to our experimental questions.
