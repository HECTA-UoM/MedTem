<img src="https://github.com/HECTA-UoM/MedTem/blob/main/MedTem_logo.png" width="100">

# MedTem: Medications and Treatments Mining and Temporal Relation Modelling using NLP
We use state-of-the-art NLP models including LLMs and GPTs to extract medication and temporal relations from clinical letters, for supporting healthcare. 

# MedTem1.0:
Abstract:
Clinical texts, represented in electronic medical records (EMRs), contain rich medical information and are essential for disease prediction, personalised information recommendation, clinical decision support, and medication pattern mining and measurement. Relation extractions between medication mentions and temporal information can further help clinicians better understand the patients' treatment history. To evaluate the performances of deep learning (DL) and large language models (LLMs) in medication extraction and temporal relations classification, we carry out an empirical investigation of \textbf{MedTem} project using several advanced learning structures including BiLSTM-CRF and CNN-BiLSTM for a clinical domain named entity recognition (NER), and BERT-CNN for temporal relation extraction (RE), in addition to the exploration of different word embedding techniques. Furthermore, we also designed a set of post-processing roles to generate structured output on medications and the temporal relation. Our experiments show that CNN-BiLSTM slightly wins the BiLSTM-CRF model on the i2b2-2009 clinical NER task yielding 75.67, 77.83, and 78.17 for precision, recall, and F1 scores using Macro Average. BERT-CNN model also produced reasonable evaluation scores 64.48, 67.17, and 65.03 for P/R/F1 using Macro Avg on the temporal relation extraction test set from i2b2-2012 challenges. 


MedTem1.0 goal of output from free text to table representation:

<img src="https://github.com/HECTA-UoM/MedTem/blob/main/input-example-free-text.png" width="900">

<img src="https://github.com/HECTA-UoM/MedTem/blob/main/example-output.png" width="600">


MedTem1.0 Pipeline:

<img src="https://github.com/HECTA-UoM/MedTem/blob/main/MedTem-pipe.png" width="900">



MedTem1.0 used data set sample with labels from i2b2 2009 and 2012:

<img src="https://github.com/HECTA-UoM/MedTem/blob/main/2009-labels.png" width="600">

<img src="https://github.com/HECTA-UoM/MedTem/blob/main/2012-labels.png" width="600">


MedTem1.0 NER scores using BiLSTM-CRF

<img src="https://github.com/HECTA-UoM/MedTem/blob/main/2009-bilstm-crf.png" width="600">

<img src="https://github.com/HECTA-UoM/MedTem/blob/main/2012-bilstm-crf.png" width="600">


MedTem1.0 RE model we re-implemented BERT-CNN:

<img src="https://github.com/HECTA-UoM/MedTem/blob/main/BERT-cnn.png" width="600">


MedTem1.0 RE scores using BERT-CNN on i2b2 2012 train and test set:

<img src="https://github.com/HECTA-UoM/MedTem/blob/main/RE-2012-train.png" width="600">

<img src="https://github.com/HECTA-UoM/MedTem/blob/main/RE-2012-test.png" width="600">


# MedTem2.0 

More details on MedTem2 is hosted at [Here](https://github.com/yang-C23/Third_year_project)

# PBL Template Examples


<img src="https://github.com/HECTA-UoM/MedTem/blob/main/PBL_templates.png" width="500">

# Data creation for MedTem2.0

The i2b2 temporal relations corpus we used contains pre-existing layers of gold standard annotations, such as clinical concepts (problems, tests, treatments) and coreference relations (Uzuneret al. 2011, 2012), which can facilitate temporal reasoning. 'The 2010 i2b2/VA Workshop on Natural Language Processing Challenges for Clinical Records' [challenge page](https://www.i2b2.org/NLP/Relations/).

MedTem2.0 System Pipeline:

<img src="https://github.com/HECTA-UoM/MedTem/blob/main/MedTem2_pipeline.png" width="700">

PBL (prompt-based learning) vs Pre-training+Finetuning

<img src="https://github.com/HECTA-UoM/MedTem/blob/main/PBL_vs_FineTune.png" width="700">

<img src="https://github.com/HECTA-UoM/MedTem/blob/main/scores_PBL_PF.png" width="700">


# Presentations
ACL2023 https://virtual2023.aclweb.org/paper_S57.html
HealTAC2023 http://healtex.org/healtac-2023/programme/ 

# Cite our work: 

Yang Cui, Lifeng Han, Goran Nenadic. 2023. 
MedTem2.0: Prompt-based Temporal Classification of Treatment Events from Discharge Summaries. Accepted to ACL2023: SRW. [paper](https://www.researchgate.net/publication/371575431_MedTem20_Prompt-based_Temporal_Classification_of_Treatment_Events_from_Discharge_Summaries) [poster](https://github.com/HECTA-UoM/MedTem/blob/main/MedTem_poster_Portrait_4ACL.pdf)

MedTem-1:
@misc{tu2023extraction,
      title={Extraction of Medication and Temporal Relation from Clinical Text using Neural Language Models}, 
      author={Hangyu Tu and Lifeng Han and Goran Nenadic},
      year={2023},
      eprint={2310.02229},
      archivePrefix={arXiv},
      url={https://arxiv.org/abs/2310.02229}
      primaryClass={cs.CL}
}

Hangyu Tu. 2022. Extraction of Temporal Information from Clinical Free Text. MSc thesis. Uni Manchester. MSc Advisor: [Prof Goran Nenadic](https://research.manchester.ac.uk/en/persons/gnenadic) and [Dr Lifeng Han](https://research.manchester.ac.uk/en/persons/lifeng.han) | 
[thesis-download](https://www.researchgate.net/publication/369453637_Extraction_of_Temporal_Information_from_Clinical_Free_Text)

# Acknowledgement
Thanks go to Warren for advice on logo design. We are grateful to grant support EP/V047949/1 “Integrating hospital outpatient letters into the healthcare data space” (funder: UKRI/EPSRC).
