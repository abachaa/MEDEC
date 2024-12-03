# MEDEC Dataset

MEDEC is the first dataset for medical error detection and correction in clinical notes (e.g., diagnosis, treatment). It includes a total of 3,848 clinical texts from the MS and UW collections. 

- The training set contains 2,189 MS texts. 
  - The MS Validation Set (#1) contains 574 clinical texts.
  - The UW Validation Set (#2) contains 160 clinical texts.
- The test includes 597 MS texts and 328 UW texts.

Each clinical text is either correct or contains one error. The task consists in: (a) predicting the error flag (1: the text contains an error, 0: the text has no errors), and for flagged texts (with error): (b) extracting the sentence that contains the error, and (c) generating a corrected sentence.


MEDEC Paper
=================
- 

MEDIQA-CORR Shared Task  
=================

The dataset has been introduced for the first shared task on medical error detection and correction: MEDIQA-CORR @ NAACL-ClinicalNLP 2024  

* **Website:** https://sites.google.com/view/mediqa2024/mediqa-corr
* **Shared Task Paper:** https://aclanthology.org/2024.clinicalnlp-1.57.pdf 

Evaluation
=================

Evaluation metrics and scripts: [https://github.com/abachaa/MEDIQA-CORR-2024 ](https://github.com/abachaa/MEDIQA-CORR-2024/tree/main/evaluation) 


Citation
=================
    
        @article{medec,
          author    = {Asma {Ben Abacha} and Wen-wai Yim and Yujuan Fu and Zhaoyi Sun and Meliha Yetisgen and Fei Xia and Thomas Lin},
          title     = {MEDEC: A Benchmark for Medical Error Detection and Correction in Clinical Notes},
          journal      = {CoRR}, 
          eprinttype    = {arXiv},
          year      = {2024}
          }


Contact
=================

    -  Asma Ben abacha (abenabacha at microsoft dot com)
    -  Wen-wai Yim (yimwenwai at microsoft dot com)
----

