

## Workshop overview

Single-cell sequencing technologies are powerful tools used to assess genomic, transcriptomic and proteomics information at the single-cell level. In recent years, the application of techniques that use single-cell sequencing have become increasingly common in several areas of research: including medicine, agriculture, and other life sciences disciplines. Single-cell sequencing may be used to study many aspects of an organism’s biology, both in health and disease, and the results of these studies contribute immensely to advancing the understanding of organisms as a whole. 

The establishment of collaborative scientific endeavors like the [Human Cell Atlas](https://www.humancellatlas.org/) is a testament to the surging enthusiasm and curiosity in this domain. Yet, when we look towards Latin America, we find a gap in the necessary infrastructure, financial support, and subject matter expertise required to harness these cutting-edge technologies. Recognizing this, our workshop is designed to bridge this gap. We provide participants with hands-on experience in the laboratory and in-depth bioinformatics training, ensuring that the region advances in its capabilities with single-cell methodologies.

[Workshop website](https://events.humancellatlas.org/hca_asiaws2024/home)

## Bioinformatics Team (Shalek lab)
- [Nuo "Ivy" Liu](https://nuoliu.github.io/), MIT/Broad Institute/Ragon Institute, US
- [Sergio Triana](https://scholar.google.com/citations?hl=en&user=WxyC26MAAAAJ), MIT/Broad Institute/Ragon Institute, US
- [Son Ngoc Nguyen](https://scholar.google.com/citations?user=j828UUwAAAAJ&hl=en), MIT/Broad Institute/Ragon Institute, US
- [Constantine N Tzouanas](https://scholar.google.com/citations?user=tsly1VQAAAAJ&hl=en), MIT/Broad Institute/Ragon Institute, US

## Introductory slide by Professor Alex Shalek
- [Practical_for_participants](https://docs.google.com/presentation/d/1I-UutDcNhawt584zM1KrLGelXGyWsu2w/edit?usp=sharing&ouid=111891412756444731558&rtpof=true&sd=true)
- [Introduction to single cell genomics](https://docs.google.com/presentation/d/1P-WpnqoHbaEwUtmmP2QiAPI0PjBDNac2/edit?usp=drive_link&ouid=111891412756444731558&rtpof=true&sd=true)

## Hands-On Bioinformatics Training Material

Below, you will find the links to the pre-course videos and Google Colab notebooks for the practical modules. 

### Practical Modules with Google Colab Notebooks:

- [Notebook A - Processing raw scRNA-seq data](https://colab.research.google.com/github/ShalekLab/HCA_Thailand_2024_workshop/blob/main/notebooks/Notebook_A_Processing_RawSeqs_CellRanger.ipynb):
_Processing raw single-cell sequencing data (scRNA-seq) is a crucial step in the whole pipeline analysis of scRNA-Seq experiments. Depending on the library preparation method used, the RNA sequences will be acquired either from 3’ ends (or 5’ ends) of the transcripts (10X Genomics, CEL-seq2, Drop-seq, inDrops) or from full-length transcripts (Smart-seq). The choice of a specific method will depend entirely on the biological question and the downstream analysis to be implemented from a count matrix. In this notebook we will cover theoretical and practical steps in setting up from raw sequences (reads)to count matrix analysis pipelines, as well as explore the basic output of the Cell Ranger tool._
[**Lecture: Preprocessing**](https://github.com/ShalekLab/HCA_Thailand_2024_workshop/blob/main/lectures/Module%201%20-%20preprocessing.pptx).

- [Notebook B - Quality Control, Exploratory Analysis, Data Normalization, Clustering, Differential expression in scRNA-seq experiments](https://colab.research.google.com/github/ShalekLab/HCA_Thailand_2024_workshop/blob/main/notebooks/Notebook_B_scRNA_seq_Analysis_Bioconductor_Seurat.ipynb):
_In that part of the course, we will guide you through the initial steps of scRNA-seq data analysis, including data importing and organization, filtering, and preliminary visualization. These essential steps ensure quality and metadata information control over heterogeneous datasets before using the Seurat package and Bioconductor infrastructure. Once the data is imported, we will focus on assessing dataset quality through various metrics and visualizations, enabling the identification and removal of poor-quality cells. Furthermore, we'll delve into normalization techniques to address technical factors and clustering methods to group cells based on expression similarity, facilitating the interpretation of results and characterization of heterogeneity. Additionally, we learn to dentify the set of features (genes/transcripts) that show distinct patterns of expression when comparing different conditions is an essential part of scRNA-seq analysis. This enables one to explore what processes might be involved in the differentiation between these circumstances. We will discuss mechanisms of analysis that combine differential expression, cell type annotation, and functional analyses to address this issue._
[**Lecture: Preprocessing**](https://github.com/ShalekLab/HCA_Thailand_2024_workshop/blob/main/lectures/Module%201%20-%20preprocessing.pptx) and [**Lecture: Clustering and cell annotation**](https://github.com/ShalekLab/HCA_Thailand_2024_workshop/blob/main/lectures/Module%202%20-%20clustering%20and%20cell%20annotation%20(no_video).pptx).


- [Notebook C - Integrating single-cell transcriptomes from multiple samples](https://colab.research.google.com/github/ShalekLab/HCA_Thailand_2024_workshop/blob/main/notebooks/Notebook_C_scRNAseq_Dataset_Integration.ipynb):
_With the increasing complexity of single-cell data, the integration of multiple datasets has become common. However, it is crucial to account for batch effects resulting from technical and biological variations to perform accurate analyses. These batch effects can stem from differences in sample handling, experimental protocols, sequencing platforms, as well as biological factors like the donor's genetic background and tissue origin. 
By employing computational methods to address these variations when comparing multiple samples, unwanted sources of variation can be eliminated, allowing researchers to focus on biologically meaningful signals. The process of removing batch effects involves making two important choices: selecting the appropriate method and parameterization, and determining the batch covariate. While the parameters are specific to the chosen method, the selection of the batch covariate depends on the goal of the integration task. This notebook will cover the key concepts and methods related to data integration and batch-effect correction, followed by hands-on activities that illustrate the integration of multiple datasets using methods from Seurat and Harmony._
[**Lecture: Batch Correction and Data Integration**](https://github.com/ShalekLab/HCA_Thailand_2024_workshop/blob/main/lectures/Module%203%20-%20integration%20and%20batch%20correction.pptx).



- [Notebook D - Deciphering cell-cell communication in single-cell transcriptomics data](https://colab.research.google.com/github/ShalekLab/HCA_Thailand_2024_workshop/blob/main/notebooks/Notebook_D_Cell_Cell_Communication.ipynb):
_Cell-cell communication plays a crucial role in coordinating cellular activities and maintaining the overall functionality of multicellular organisms. It allows cells to transmit signals, exchange information, and coordinate their behaviors, ultimately contributing to essential biological processes such as development, immune response, and tissue homeostasis. In this context, inferring cell-cell interactions from gene expression data becomes valuable for unraveling the multiple roles and coordination processes that cells perform within multicellular systems. 
In this notebook, main concepts and a general computational workflow will be covered, then hands-on activities will be performed using LIANA, a flexible tool implementing multiple state-of-the-art methods to study cell-cell interactions._
[**Lecture: Batch Correction and Data Integration**](https://github.com/ShalekLab/HCA_Thailand_2024_workshop/blob/main/lectures/Module%204%20-%20cell-cell%20communication.pptx).

- [Notebook E - BCR/TCR Profiling and CITE-Seq in Single-Cell Analysis](https://github.com/ShalekLab/HCA_Thailand_2024_workshop/blob/main/notebooks/Notebook_E_10x_BCR_analysis.ipynb) :  _T cell receptor (TCR) profiling and Cellular Indexing of Transcriptomes and Epitopes by Sequencing (CITE-Seq) are pivotal techniques in single-cell research, offering unparalleled insights into the adaptive immune system and cellular heterogeneity. TCR profiling enables a deep dive into the repertoire and diversity of T cell populations, highlighting the specificity and uniqueness of T cell responses. On the other hand, CITE-Seq facilitates the concurrent assessment of transcriptomic data and protein expression within individual cells, creating a comprehensive portrayal of cellular states.
In this module, participants will explore the profound implications of TCR profiling in understanding immune responses and the synergies it can achieve when coupled with CITE-Seq. We'll initiate with core concepts and theories, and swiftly transition into practical applications using advanced computational tools. Through this hands-on approach, attendees will master the nuances of TCR profiling and CITE-Seq, equipping them with valuable tools for their immunological and single-cell research pursuits._[**Lecture: BCR/TCR and CITE-Seq**](https://github.com/ShalekLab/HCA_Thailand_2024_workshop/blob/main/lectures/Module%205%20-%20BCR%20background%20and%2010x%20analysis.pptx).


- [Notebook F - Trajectory inference and pseudotemporal ordering](https://colab.research.google.com/github/ShalekLab/HCA_Thailand_2024_workshop/blob/main/notebooks/Notebook_F_Pseudotime_Analysis.ipynb):
_Gene expression changes in a dynamic way as cells transition from one state to another. These transitions occur during development and throughout life, which makes them of interest to understand changes in the cellular functions. In each of these states, some genes get activated and others silenced. 
By using scRNA-seq data, computational tools such as Monocle3 can infer the single-cell trajectories that cells undergo when transitioning across the different functional states. Thus, the developmental history (ontogeny) of differentiated cell types can be traced. This notebook will cover the key concepts and methods related to inferring cell-state trajectory and pseudotime ordering, followed by hands-on activities that illustrate the use of Monocle3, a tool devised for this purpose._
**Related Slides:** _[**Lecture: Trajectory inference **](https://github.com/ShalekLab/HCA_Thailand_2024_workshop/blob/main/lectures/Module%205%20-%20Trajectory%20inference.pptx).

  

### Authorship and Acknowledgments:

This comprehensive material has been a result of collaborative efforts since 2021 and has been successfully employed in numerous courses organized by esteemed institutions like the Human Cell Atlas, LatinCells initiative, and Wellcome Connecting Sciences. We extend our heartfelt gratitude to all the individuals listed below, who have actively contributed to the development and refinement of this material over the years. Their dedication and expertise have been instrumental in making this resource valuable for the bioinformatics community.

We appreciate the continuous support and feedback from participants, mentors, and institutions that have made this endeavor possible. Together, we strive to advance the understanding and application of single-cell genomics in Latin America and the Caribbean.

**List of Contributors from the Mahidol university - Listed Alphabetically:**

Benjamaporn Sriwilai; sbenjamaporn19@gmail.com	

Namkhang Leeratsuwan; nleeratsuwan@gmail.com	

Piroon Jenjaroenpun; piroon.jen@mahidol.edu 

Punn Augsornworawat; punn.aug@mahidol.ac.th 

Sarintip Nguantad; sarintip.ng@gmail.com	

Sirawit Srikor; sirawitsrikor@gmail.com	

Tantip Arigul; tantip.ari@mahidol.edu 

Varodom Charoensawan; varodom.cha@mahidol.edu	

Waradon Sungnak; waradon.sun@mahidol.edu	

Yasumin Kerdsri; k.yasuminmeen@gmail.com


******
## License
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
