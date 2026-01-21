# MEDEC Dataset

MEDEC is the first dataset for medical error detection and correction in clinical notes. 

<a href="url"><img src="https://github.com/abachaa/MEDEC/blob/main/medec-exps" align="right" height="450" width="550" ></a>

It includes 3,848 clinical texts from the MS and UW collections covering five types
of errors (Diagnosis, Management, Treatment, Pharmacotherapy, and Causal Organism).  

  - The Training Set contains 2,189 MS texts. 
  - The MS Validation Set contains 574 clinical texts.
  - The UW Validation Set contains 160 clinical texts.
  - The MS Test includes 597 MS texts
  - The UW Test set includes 328 UW texts.

Each clinical text is either correct or contains one error. The task consists in: 
  - (A) predicting the error flag (1: the text contains an error, 0: the text has no errors)
  - For flagged texts (with error):
    - (B) extracting the sentence that contains the error, and
    - (C) generating a corrected sentence.

**DATA:**
- **MEDEC-MS Collection:** https://github.com/abachaa/MEDEC/tree/main/MEDEC-MS (MEDEC-MS Training, Validation, and Test Sets)
- **MEDEC-UW Collection:** Please send an email to medec-uw@googlegroups.com to receive the UW Data Usage Agreement (DUA) required to have access to the MEDEC-UW Validation & Test sets.


MEDEC Paper
=================

- **PDF**: https://aclanthology.org/2025.findings-acl.1159.pdf 
- **Abstract**: Several studies have shown that Large Language Models (LLMs) can answer medical questions correctly, even outperforming the average human score in some medical exams. However, to our knowledge, no study has been conducted to assess the ability of language models to validate existing or generated medical text for correctness and consistency. In this paper, we introduce MEDEC, the first publicly available benchmark for medical error detection and correction in clinical notes, covering five types of errors (Diagnosis, Management, Treatment, Pharmacotherapy, and Causal Organism). MEDEC consists of 3,848 clinical texts, including 488 clinical notes from three US hospital systems that were not previously seen by any LLM. The dataset has been used in the MEDIQA-CORR 2024 shared task to evaluate seventeen participating systems [Ben Abacha et al., 2024](https://aclanthology.org/2024.clinicalnlp-1.57.pdf). In this paper, we describe the data creation methods and we evaluate recent LLMs (e.g., o1-preview, GPT-4, Claude 3.5 Sonnet, Gemini 2.0 Flash, and DeepSeek-R1) for the tasks of detecting and correcting medical errors requiring both medical knowledge and reasoning capabilities. We also conducted a comparative study where two medical doctors performed the same task on the MEDEC test set. The results showed that MEDEC is a sufficiently challenging benchmark to assess the ability of models to validate existing or generated notes and to correct medical errors. We also found that although recent LLMs have a good performance in error detection and correction, they are still outperformed by medical doctors in these tasks. We discuss the potential factors behind this gap, the insights from our experiments, the limitations of current evaluation metrics, and share potential pointers for future research. 

MEDIQA-CORR Shared Task  
=================

The dataset has been introduced for the first shared task on medical error detection and correction: MEDIQA-CORR @ NAACL-ClinicalNLP 2024  

* **Website:** https://sites.google.com/view/mediqa2024/mediqa-corr
* **Shared Task Paper:** https://aclanthology.org/2024.clinicalnlp-1.57.pdf
* **GitHub:** https://github.com/abachaa/MEDIQA-CORR-2024

Evaluation
=================

Evaluation metrics and scripts: [https://github.com/abachaa/MEDIQA-CORR-2024 ](https://github.com/abachaa/MEDIQA-CORR-2024/tree/main/evaluation) 

MEDEC-MS
=================
**Formatting issues:**  The raw data used to create MEDEC-MS contains some formatting issues (e.g., non-standard characters and unintended line breaks).   

If you are comparing your results with other published work, we recommend using the original MEDEC-MS dataset published here. 

If you prefer an updated version that resolves some of these issues, please refer to Max Kieffer's repo: https://huggingface.co/datasets/mkieffer/MEDEC 

## <h2>License</h2>
- This work is released under the Creative Commons Attribution 4.0 International License ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)). Please cite our paper if you use the full dataset or any subset of MEDEC: 
    
        @inproceedings{medec,
          author       = {Asma {Ben Abacha} and Wen{-}wai Yim and Yujuan Fu and Zhaoyi Sun and Meliha Yetisgen and Fei Xia and Thomas Lin}, 
          title        = {{MEDEC:} {A} Benchmark for Medical Error Detection and Correction in Clinical Notes}, 
          booktitle    = {Findings of the Association for Computational Linguistics, {ACL} 2025, Vienna, Austria, July 27 - August 1, 2025}, 
          pages        = {22539--22550}, 
          publisher    = {Association for Computational Linguistics}, 
          year         = {2025}, 
          url          = {https://aclanthology.org/2025.findings-acl.1159/} 
          }

Contact
=================

    -  Asma Ben abacha (abenabacha at microsoft dot com)
    -  Wen-wai Yim (yimwenwai at microsoft dot com)
----

