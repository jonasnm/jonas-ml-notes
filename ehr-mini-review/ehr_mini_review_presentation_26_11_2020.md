---
marp: true
# theme: gaia
_class: invert
---

# ML EHR update - Summary of mini-review

---
# Outline 

1. Interesting papers and directions
2. Data sets
    * Quick update about Quake?
3. What should be our way forward?

---
# Interesting papers and directions
After reviewing a lot of papers... :

- Time series (multivariate, missing etc), a la KKW and KØM
- NLP
- Graph based methods
- (Combinations of the above)

---
# Time series

- [A REVIEW OF DEEP LEARNING METHODS FOR IRREGULARLY
SAMPLED MEDICAL TIME SERIES DATA](https://arxiv.org/pdf/2010.12493.pdf) -- Sun et al. 2020, arXiv preprint

- [Explainable Uncertainty-Aware ConvolutionalRecurrent Neural Network for IrregularMedical Time Series](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9224838)
- [Neural Conditional Event Time Models](https://www.mlforhc.org/s/50_CameraReadySubmission_MLHC_2020.pdf)

---
# NLP

- [Dynamically Extracting Outcome-Specific Problem Lists from Clinical Notes with Guided Multi-Headed Attention](https://www.mlforhc.org/s/53_CameraReadySubmission_camera_ready.pdf)
- [Query-Focused EHR Summarization to Aid Imaging Diagnosis](https://www.mlforhc.org/s/115_CameraReadySubmission_Query_Focused_EHR_Summarization_to_Aid_Imaging_Diagnosis.pdf)
- [Attention is not explanation](https://arxiv.org/pdf/1902.10186.pdf) -> learned  attention  weights  are  frequently uncorrelated with gradient-based measures of feature importance"
- [Time-Aware Transformer-based Network for Clinical Notes Series Prediction](https://www.mlforhc.org/s/104_CameraReadySubmission_Time-Aware-Transformer-based-Network-for-Clinical-Notes-Series-Prediction.pdf)
- [Query-Focused EHR Summarization to Aid Imaging Diagnosis](https://www.mlforhc.org/s/115_CameraReadySubmission_Query_Focused_EHR_Summarization_to_Aid_Imaging_Diagnosis.pdf)


---
# NLP

[BlueBert](https://github.com/ncbi-nlp/bluebert) is now in Huggingface.
    
---
# Graph based methods
- [Learning the Graphical Structure of ElectronicHealth Records with Graph Convolutional Transformer](https://arxiv.org/abs/1906.04716) -- Edward Choi.
- [Knowledge-Base Completion for Constructing Problem-Oriented Medical Records](https://www.mlforhc.org/s/48_CameraReadySubmission_camera-ready.pdf)


---
# Other interesting papers

- [DPSOM: Deep Probabilistic Clusteringwith Self-Organizing Maps](https://arxiv.org/pdf/1910.01590.pdf)
- [Unsupervised Representation for EHR Signals andCodes as Patient Status Vector](https://arxiv.org/pdf/1910.01803.pdf)
- [Improved recurrent generative adversarial networks with regularization techniques and a controllable framework](https://www.sciencedirect.com/science/article/pii/S0020025520305417)
- [Analyzing the role of model uncertainty for electronic health records](https://dl.acm.org/doi/abs/10.1145/3368555.3384457?casa_token=1DOErfF0Tp8AAAAA%3ALZeYTElWlay0z0n0OcCyFQwH5z7O733H0Bsyp6Lj5LvG6QMqBTieBWD1RtLWtAoAGKgMVBrwH9yrLg) -- [PDF](https://dl.acm.org/doi/pdf/10.1145/3368555.3384457)

---
# Data sets

[eICU dataset](https://eicu-crd.mit.edu/)

[Mimic](https://mimic.physionet.org/)

[Mimic 4](https://physionet.org/content/mimiciv/0.4/) -- August 2020. Also has "hospital-wide" data, which might be worthwhile checking.

"Quake 2" -- In progress
