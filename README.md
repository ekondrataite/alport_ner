# Medical Entity Extraction from Electronic Health Records for Alport Syndrome Patients

This repository contains the code of **Eglė Kondrataitė Master's thesis** about the use of unstructured medical text and natural language processing techniques for analysis of Alport syndrome.

# Abstract

This Master's thesis demonstrates the development and evaluation of a rule-based **Named Entity Recognition (NER)** system for extracting clinically relevant information about **Alport Syndrome (AS)** patients from unstructured medical text in **electronic health records (EHRs)**. A specialised dictionary of 33 standardised AS-related terms, validated by a medical expert, was created using an ontology and medical text analysis. The dictionary included three types of medical entities: diseases, symptoms and procedures. The developed NER system included 78 custom pattern rules to detect synonyms, abbreviations and alternative phrasing. In addition, the system recognised context-specific expressions to extract relevant information. When extracting information from medical notes, the system identified 18 terms out of 33 dictionary terms. Clustering analyses validated the clinical accuracy and interpretability of the extracted information, with algorithms such as K-Means, hierarchical clustering and DBSCAN identifying meaningful patient groups. The algorithms were able to distinguish between patients with pre-renal failure and those with renal failure. The results showed that clustering of all extracted entity terms provided the most interpretable insights, while separate entity terms provided limited interpretability. Comparative analysis with patients with chronic kidney disease demonstrated the system's ability to distinguish between similar diseases, but also identified overlapping symptoms of similar diseases, which poses difficulties in diagnosing the diseases. This work provides a novel framework for using unstructured medical text and **natural language processing (NLP)** techniques to advance research into rare diseases such as AS.

**Keywords:** natural language processing, electronic health records, Alport syndrome, medical named entity recognition

# Content

The python code consists of **3** files:

- **alport_primary_analysis** and this file contains:
  - the primary analysis of alport patient dataset,
  - the most common word and phrases analysis for dictionary development.
 
- **alport_ehr_ner** and this file contains:
  - the developed rule-based NER system,
  - analysis of the extracted terms.
 
- **alport_clustering** and this file contains:
  - the text vectorisation using TF-IDF,
  - the dimension reduction using Singular Value Decomposition,
  - the clustering analysis using K-Means, DBSCAN and hierarchical clustering
