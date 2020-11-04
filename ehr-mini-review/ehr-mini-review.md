# ML and EHRs mini-review

This document provides a list of documents and links to papers and projects dealing with EHRs and "modern" machine learning. 


## Venues 
- [ML for health workshop](https://www.mlforhc.org/accepted-papers)
- [Ml4Health (NeurIPS)](https://ml4health.github.io)


## Some interesting papers

- [Learning the Graphical Structure of ElectronicHealth Records with Graph Convolutional Transformer](https://arxiv.org/abs/1906.04716) -- Edward Choi.
- [Opportunities and challenges in developing deep learning models using electronic health records data: a systematic review](https://academic.oup.com/jamia/article/25/10/1419/5035024) -- Edward Choi.
- [A REVIEW OF DEEP LEARNING METHODS FOR IRREGULARLY
SAMPLED MEDICAL TIME SERIES DATA](https://arxiv.org/pdf/2010.12493.pdf) -- Sun et al. 2020, arXiv preprint

### From mlforhc 2020
- [Neural Conditional Event Time Models](https://www.mlforhc.org/s/50_CameraReadySubmission_MLHC_2020.pdf)
- [Knowledge-Base Completion for Constructing Problem-Oriented Medical Records](https://www.mlforhc.org/s/48_CameraReadySubmission_camera-ready.pdf)
- [Dynamically Extracting Outcome-Specific Problem Lists from Clinical Notes with Guided Multi-Headed Attention](https://www.mlforhc.org/s/53_CameraReadySubmission_camera_ready.pdf)
- [Time-Aware Transformer-based Network for Clinical Notes Series Prediction](https://www.mlforhc.org/s/104_CameraReadySubmission_Time-Aware-Transformer-based-Network-for-Clinical-Notes-Series-Prediction.pdf)
- [Query-Focused EHR Summarization to Aid Imaging Diagnosis](https://www.mlforhc.org/s/115_CameraReadySubmission_Query_Focused_EHR_Summarization_to_Aid_Imaging_Diagnosis.pdf)


### Tl;dr for some papers

#### [Learning the Graphical Structure of ElectronicHealth Records with Graph Convolutional Transformer](https://arxiv.org/abs/1906.04716).

- Exploit the underlying graphical structure of EHRs
- **Hypothesis**: can they jointly learn the hidden structure of EHR while performing super-vised prediction tasks on EHR data?
- Model: Transformer -> Graph convolutional transformer
- (Related paper [MiME](https://arxiv.org/abs/1810.09593))
- **Setting**: What if the graph of the EHR is hidden or unknown?
- They propose _guided self attention_, which outperforms self-attention.
- EHRs are represented as a graph, where each visit is a node possibly connected to diagnosis nodes and medicine/treatment nodes:
![](https://i.imgur.com/vXrgLmh.png)

---

#### [Opportunities and challenges in developing deep learning models using electronic health records data: a systematic review](https://academic.oup.com/jamia/article/25/10/1419/5035024)

Surveyed 98 articles, found the following tasks:
![](https://i.imgur.com/z7jXcB7.png)


How are deep models applied to these tasks? What are some special challenges arising from modeling EHR data? 

Interesting paper! [Explainable Prediction of Medical Codes from Clinical Text
](https://arxiv.org/abs/1802.05695) -- James Mullenbach, Sarah Wiegreffe, Jon Duke, Jimeng Sun, Jacob Eisenstein

EHR privacy = De-Identification measures.

Summary of DL techniques and EHR related challenges:
![](https://i.imgur.com/ZHokqgZ.png)

---

#### [A REVIEW OF DEEP LEARNING METHODS FOR IRREGULARLY
SAMPLED MEDICAL TIME SERIES DATA](https://arxiv.org/pdf/2010.12493.pdf) -- Sun et al. 2020, arXiv preprint



## Public datasets (other than MIMIC)

### [eICU dataset](https://eicu-crd.mit.edu/)

Currently cited by 146 according to [Google Scholar](https://scholar.google.no/scholar?cites=11878669525996073977&as_sdt=2005&sciodt=0,5&hl=en). I have not yet looked trough these completely

Potential papers to look into

- [Gastrointestinal bleeding, using "interpretable" methods](https://journals.lww.com/ajg/Fulltext/2020/10000/Explainable_Machine_Learning_Model_for_Predicting.22.aspx). Is this related to Anastomosis Leakage?
- [Explainable Uncertainty-Aware ConvolutionalRecurrent Neural Network for IrregularMedical Time Series](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9224838)
- [Unsupervised Representation for EHR Signals andCodes as Patient Status Vector](https://arxiv.org/pdf/1910.01803.pdf)
- [Improved recurrent generative adversarial networks with regularization techniques and a controllable framework](https://www.sciencedirect.com/science/article/pii/S0020025520305417)
- [DPSOM: Deep Probabilistic Clusteringwith Self-Organizing Maps](https://arxiv.org/pdf/1910.01590.pdf)

## Rantings and ravings

Update 02.11.2020: as is common for most recent deep learning developments, much of the recent work seems to be quite incremental, at least if one looks at the results (e.g. classification scores etc). My guess is that this is mostly due to the limitations, both in availability and data quality, of the data sets. 

I would vote for a deep dive into the old Quake database to try to identify new problems related to our data. Trying to fit our data to whatever other people are doing with their data is going to be a lot of work and, at best, incremental. Or is that putting it too harshly?

