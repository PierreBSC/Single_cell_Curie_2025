This GitHub contains a list of ressources for a better understanding of the single-cell genomic field. These ressources include landmark papers, but also blogs, YouTube videos and channels.


## Websites, videos and blogs

- **Likely one of the most important and valuable ressource in the field**: the list and technical details of every published single-cell protocol aggregated by the Teichman lab available [here](https://teichlab.github.io/scg_lib_structs/).
- The excellent blog of Valentine Svensson that focuses on the computational analysis of single-cell data: [What do you mean 'heterogeneity'](https://www.nxn.se/).
-  An other excellent blog is the [blog of Jean Fan](https://jean.fan/blog) that thends to focus more on spatial analysis.
-  An in-depth description of the different dimensionality reduction methods commonly used in the single-cell genomic field such as t-SNE and UMAP. Available in the [smallvis GitHub](https://jlmelville.github.io/smallvis/). More broadly this GitHub contains a large number of implementations and other valuable ressources.
-  The Broad institute provides a list of very interesting computational biology YouTube videos, including videos dedicated to single-cell data analysis. More than a hundred videos are available [here](https://www.youtube.com/playlist?list=PLlMMtlgw6qNjROoMNTBQjAcdx53kV50cS).

## Tools 

The two most common tools for scRNA-seq analysis are [Seurat](https://satijalab.org/seurat/) and [Scanpy](https://scanpy.readthedocs.io/en/stable/), two R an Python packages respectively. While these two tools are commonly used throughout the field, I personnaly prefer the use of the [Pagoda2](https://github.com/kharchenkolab/pagoda2) package, a lightweight yet extremely efficient R package from the Kharchenko lab. As an alternative, metacell-based approach are also worth noting including the original R package [MetaCell](https://metacells.readthedocs.io/en/latest/) and the recently published [SEACell](https://github.com/dpeerlab/SEACells).

## Landmark papers

### Part I: The prehistory of single-cell analysis.


- If you read spanish: **Estructura de los centros nerviosos de las aves** (Cajal, 1888). Of course the interest is more historical than scientific.
- One of the first example of the interest and power of single-cell analysis:  **The biochemical basis of an all-or-none cell fate switch in Xenopus oocytes** (Ferrel and  Machleder, 1998).
- First paper prooving that cancer cells can switch between various states: **Stochastic State Transitions Give Rise to Phenotypic Equilibrium in Populations of Cancer Cells** (Gupta et al. 2011).
- Analysis of the NF-kB oscillations in individual cells: **Single-cell NF-κB dynamics reveal digital activation and analog information processing in cells** (Tay et al. 2010).




### Part II: How does single-cell genomic work ?

- Optimisation of RNA-seq protocols to reach single-cell resolution : **Full-length mRNA-Seq from single-cell levels of RNA and individual circulating tumor cells** (Ramsköld et al. 2012).
-  An early example of microfluidic used for single-cell PCR: **High-Throughput Droplet Digital PCR System for Absolute Quantitation of DNA Copy Number** (Hindson et al. 2008).
-  The paper introducing Unique Molecular Identifier: **Counting absolute numbers of molecules using unique molecular identifiers** (Kivioja et al 2011).
-   The first large-scale plate-based scRNA-seq protocol (MARS-seq): **Massively Parallel Single-Cell RNA-Seq for Marker-Free Decomposition of Tissues into Cell Types** (Jaitin et al. 2014).  Its second version is published a few years later: **MARS-seq2.0: an experimental and analytical pipeline for indexed sorting combined with single-cell RNA sequencing** (Keren-Shaul et al. 2018)
- First droplet-based scRNA-seq protocol: **Highly Parallel Genome-wide Expression Profiling of Individual Cells Using Nanoliter Droplets** (Macosko et al. 2015).
- The paper introducing the 10X Chromium® platform: **Massively parallel digital transcriptional profiling of single cells** (Zheng et al. 2017).
- A nice summary of the different scRNA-seq techniques: **Exponential scaling of single-cell RNA-seq in the past decade** (Svensson et al. 2018). The paper is of course outdated but is a nice summary of the different technologies available at the time.
- Paper introducing CUT&Tag for single-cell epigenomic: **CUT&Tag for efficient epigenomic profiling of small samples and single cells** (Kaya-Okur et al. 2019).
- The first large-scale scATAC-seq protocol, i.e. droplet-based protocol, **Chromatin accessibility profiling by ATAC-seq** (Grandi et al. 2022).

### Part III: The discoveries enabled by scRNA-seq.

- The first highly sucessful application of scRNA-seq *in-vitro* with two studies from the Regev lab: **Single-cell transcriptomics reveals bimodality in expression and splicing in immune cells**  (Shalek et al. 2013) and **Single-cell RNA-seq reveals dynamic paracrine control of cellular variation** (Shalek et al. 2014). 
- The first applications of scRNA-seq to study cancer *in-vivo*: **Dissecting the multicellular ecosystem of metastatic melanoma by single-cell RNA-seq** (Tirosh et al. 2016). Was followed a few years later by brilliant albeit heavy paper on glioblastoma: **An Integrative Model of Cellular States, Plasticity, and Genetics for Glioblastoma** (Neftel et al. 2019). 
- Probably one of the most impactfull single-cell paper that revelead the progressive activation of brain macrophages in neurodegenerative : **A Unique Microglia Type Associated with Restricting Development of Alzheimer’s Disease** (Keren-Shaul et al. 2017).
- One single-cell atlas among many others: **A high-resolution transcriptomic and spatial atlas of cell types in the whole mouse brain** (Yao et al. 2023).



### Part IV: How to analyze single-cell data ?

- If there is only one paper to read about single-cell data analysis it is the excellent **The triumphs and limitations of computational methods for scRNA-seq** (Kharchenko, 2021).
- First paper introducing graph-based clustering under the name of "Phenograph": **Data-Driven Phenotypic Dissection of AML Reveals Progenitor-like Cells that Correlate with Prognosis** (Levine et al. 2015). While initially designed for the analysis of mass and high-dimensional flow cytometry data, this algorithm is now the standard for single-cell analysis due to its scalability and robustness.
- A simple yet essential paper from Valentine Svensson: **Droplet scRNA-seq is not zero-inflated** (Svensson 2020). Very important message that can be applied to any field: simpler is (very) ofter better !
- The paper introducing the Velocity approach: **RNA velocity of single cells** (La Manno et al, 2018).
- The first paper introducing the concept of MetaCells by the Tanay Lab **MetaCell: analysis of single-cell RNA-seq data using K-nn graph partitions** (Baran et al. 2019). This approach has been implemented and further optimised by the Pe'er lab in **SEACells infers transcriptional and epigenomic cellular states from single-cell genomics data** (Persad et al. 2023). It is worth noting that the first paper is quite technical and hard to read but contains a lot of interesting insights and ideas.

### Part V: The challenges and future of the single-cell field.

- An example of typical single-cell pseudoscience  **A single-cell atlas of the peripheral immune response in patients with severe COVID-19** (Wilk et al. 2020). The problematic part is corresponding to Figure 4.
- A long discussion on the potential flaws of dimensionality reduction applied to single-cell genomic from the Pachter Lab: **The specious art of single-cell genomics** (Chari and Pachter 2023).
- Also from the Pachter lab, an in-depth comparison of the two main single-cell analysis packages (Seurat and Scanpy)  and of the impact of the package versions: **The impact of package selection and versioning on single-cell RNA-seq analysis** (Rich et al. 2024).
- One of the first single-cell annotation tool that unlike other methods is relying on a 'simple' autoencoder and not on a complex and questionable attention-based structure: **A cell atlas foundation model for scalable search of similar human cells** (Heimberg et al. 2024).
- A nice review on the different spatial omic methods: **The emerging landscape of spatial profiling technologies** (Moffit et al. 2022).
- Nice paper on the potential of Raman imaging for single-cell analysis: **Raman2RNA: Live-cell label-free prediction of single-cell RNA profiles by Raman microscopy** (Kobayashi-Kirschvink et al. 2024).




