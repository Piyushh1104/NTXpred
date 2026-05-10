# NTXpred: Prediction of Neurotoxins Based on Their Function and Source

## Overview

NTXpred is a computational platform developed for predicting neurotoxins and classifying them based on their biological source and functional activity.

The system uses multiple machine learning and sequence-analysis approaches including:

- Support Vector Machine (SVM)
- Feed Forward Neural Network (FNN)
- Recurrent Neural Network (RNN)
- PSI-BLAST
- MEME/MAST

The platform predicts:

- Neurotoxin proteins
- Source of neurotoxins
- Functional class of neurotoxins
- Ion channel blocker subclasses

Web Server:

http://www.imtech.res.in/raghava/ntxpred/

---

## Research Paper

**Title:** Prediction of neurotoxins based on their function and source

**Authors:**  
Sudipto Saha and Gajendra P. S. Raghava

**Journal:** In Silico Biology (2007)

**DOI:** https://doi.org/10.3233/ISB-2007-7104

---

## Background

Neurotoxins are toxic proteins that affect the nervous system by blocking nerve impulses and interfering with ion channels or neurotransmitter release.

Major biological sources include:

- Eubacteria
- Cnidaria
- Mollusca
- Arthropoda
- Chordata

Neurotoxins are important for:

- Drug discovery
- Pain research
- Epilepsy therapeutics
- Ion channel studies
- Functional proteomics

---

## Dataset Information

The dataset was collected from Swiss-Prot/Tox-Prot databases.

### Initial Dataset

- 932 experimentally validated neurotoxin proteins

### Final Non-Redundant Dataset

- 582 neurotoxin sequences

Redundancy reduction was performed using PROSET software with 90% sequence identity cutoff.

---

## Classification Categories

### Based on Source

- Eubacteria
- Cnidaria
- Mollusca
- Arthropoda
- Chordata

### Based on Function

- Ion channel blockers
- Acetylcholine receptor blockers
- Inhibitors of acetylcholine release
- Facilitators of acetylcholine release

### Ion Channel Subclassification

- Sodium channel blockers
- Potassium channel blockers
- Calcium channel blockers
- Chloride channel blockers

---

## Machine Learning Approaches

### Support Vector Machine (SVM)

SVM models were developed using:

- Amino acid composition
- Dipeptide composition
- Sequence length

### Artificial Neural Networks

#### Feed Forward Neural Network (FNN)

- Accuracy: 84.19%

#### Recurrent Neural Network (RNN)

- Accuracy: 92.75%

### PSI-BLAST

Used for similarity-based neurotoxin prediction.

### MEME/MAST

Used for motif discovery and motif-based classification.

---

## Best Prediction Performance

| Method | Accuracy | MCC |
|--------|----------|------|
| SVM Composition | 97.72% | 0.9416 |
| SVM Dipeptide | 96.05% | 0.9247 |
| RNN | 92.75% | 0.8572 |
| FNN | 84.19% | 0.6890 |

---

## Source Classification Performance

### Best Hybrid Model

- Overall Accuracy: 92.10%

The hybrid model combined:

- PSI-BLAST
- SVM Composition + Length

---

## Functional Classification Performance

### Best Hybrid Model

- Overall Accuracy: 96.00%

The hybrid model combined:

- MEME/MAST
- SVM Dipeptide + Length

---

## Ion Channel Blocker Prediction

Maximum overall prediction accuracy:

- 75.08%

Classes predicted:

- Sodium channel blockers
- Potassium channel blockers
- Calcium channel blockers
- Chloride channel blockers

---

## Sequence Analysis

The study observed that neurotoxins contain:

- High cysteine content
- Conserved amino acid patterns
- Distinct amino acid composition compared to non-toxin proteins

Important enriched residues include:

- Cysteine
- Glycine
- Lysine
- Tyrosine

---

## Hybrid Prediction Strategy

Hybrid approaches combined:

- SVM + PSI-BLAST
- SVM + MEME/MAST

These hybrid systems improved prediction accuracy significantly over individual methods.

---

## Technologies Used

- SVM_light
- SNNS Neural Networks
- PSI-BLAST
- MEME/MAST
- PROSET
- Perl
- CGI
- Linux

---

## Applications

NTXpred can be used for:

- Neurotoxin prediction
- Venom protein analysis
- Drug discovery
- Functional proteomics
- Ion channel research
- Therapeutic peptide studies

---

## Web Server Features

The server allows users to:

- Predict neurotoxins
- Identify toxin source
- Predict toxin function
- Predict ion channel blocker subclasses
- Submit sequences in FASTA format
- Analyze proteins using multiple prediction methods

---

## Availability

Web Server:

http://www.imtech.res.in/raghava/ntxpred/

Mirror Server:

http://bioinformatics.uams.edu/mirror/ntxpred

---

## Contact

### Prof. Gajendra P. S. Raghava

Department of Computational Biology  
Indraprastha Institute of Information Technology Delhi  
New Delhi, India

Email: raghava@iiitd.ac.in

---

## License

Creative Commons Attribution License

---

## Source

Generated from the uploaded NTXpred research paper. :contentReference[oaicite:0]{index=0}
