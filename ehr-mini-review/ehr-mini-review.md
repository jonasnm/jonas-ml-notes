# ML and EHRs mini-review

This document provides a list of documents and links to papers and projects dealing with EHRs and "modern" machine learning. 


## Venues 
- [ML for health workshop](https://www.mlforhc.org/accepted-papers)
- [Ml4Health (NeurIPS)](https://ml4health.github.io)


## Some interesting papers

- [Learning the Graphical Structure of ElectronicHealth Records with Graph Convolutional Transformer](https://arxiv.org/abs/1906.04716) -- Edward Choi.
- [Opportunities and challenges in developing deep learning models using electronic health records data: a systematic review](https://academic.oup.com/jamia/article/25/10/1419/5035024) -- Edward Choi.

### From mlforhc 2020
- [Neural Conditional Event Time Models](https://www.mlforhc.org/s/50_CameraReadySubmission_MLHC_2020.pdf)
- [Knowledge-Base Completion for Constructing Problem-Oriented Medical Records](https://www.mlforhc.org/s/48_CameraReadySubmission_camera-ready.pdf)
- [Dynamically Extracting Outcome-Specific Problem Lists from Clinical Notes with Guided Multi-Headed Attention](https://www.mlforhc.org/s/53_CameraReadySubmission_camera_ready.pdf)
- [Time-Aware Transformer-based Network for Clinical Notes Series Prediction](https://www.mlforhc.org/s/104_CameraReadySubmission_Time-Aware-Transformer-based-Network-for-Clinical-Notes-Series-Prediction.pdf)
- [Query-Focused EHR Summarization to Aid Imaging Diagnosis](https://www.mlforhc.org/s/115_CameraReadySubmission_Query_Focused_EHR_Summarization_to_Aid_Imaging_Diagnosis.pdf)

### Tl;dr for some papers

[Learning the Graphical Structure of ElectronicHealth Records with Graph Convolutional Transformer](https://arxiv.org/abs/1906.04716).

- Exploit the underlying graphical structure of EHRs
- **Hypothesis**: can they jointly learn the hidden structure of EHR while performing super-vised prediction tasks on EHR data?
- Model: Transformer -> Graph convolutional transformer
- (Related paper [MiME](https://arxiv.org/abs/1810.09593))
- **Setting**: What if the graph of the EHR is hidden or unknown?
- They propose _guided self attention_, which outperforms self-attention.
- EHRs are represented as a graph, where each visit is a node possibly connected to diagnosis nodes and medicine/treatment nodes:
![](https://i.imgur.com/vXrgLmh.png)


## Public datasets (other than MIMIC)

### [eICU dataset](https://eicu-crd.mit.edu/)

Currently cited by 146 according to [Google Scholar](https://scholar.google.no/scholar?cites=11878669525996073977&as_sdt=2005&sciodt=0,5&hl=en). I have not yet looked trough these completely

Potential papers to look into

- [Gastrointestinal bleeding, using "interpretable" methods](https://journals.lww.com/ajg/Fulltext/2020/10000/Explainable_Machine_Learning_Model_for_Predicting.22.aspx). Is this related to Anastomosis Leakage?
