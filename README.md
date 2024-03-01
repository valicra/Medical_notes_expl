# Extracting Medical Conditions from Electronic Health Records
Semantic Computing Group\
Bielefeld University, Germany


Supervisors: Christoph Düsing, Philipp Cimiano 

## Overview
This project leverages Deep Learning (DL) and Natural Language Processing (NLP) techniques to analyze clinical notes from the MIMIC-III dataset. 
The primary objectives include identifying symptoms and pathogens, classifying clinical notes based on infections, applying models to unlabeled data, 
clustering symptoms, and inferring infection locations.

## Dataset
Source: MIMIC-III
Size: 2,000,000 noteevents, 60,000 discharge letters, 7,500 related to sepsis
Labeled Data: 370 annotated notes
Annotations:\
Text spans for symptoms and pathogens
Labels indicating the source of infection and affected organs

## Tasks
1. **Identifying Symptoms and Pathogens** \
Approach:
Utilize NLP models (spaCy) for Named Entity Recognition (NER).
Train on labeled data to identify and extract symptoms and pathogens from clinical notes.
3. **Classifying Clinical Notes**\
Approach:
Implement a DL classification model (BERT) to categorize clinical notes based on infections.
Train the model using labeled data, allowing it to distinguish between different infections.
4. **Applying Models to Unlabeled Data** \
Transfer Learning:
Fine-tune models on labeled data and apply them to the large corpus of 2,000,000 unlabeled noteevents for comprehensive analysis.
5. **Clustering Symptoms**\
Clustering Algorithm:
Apply clustering techniques (K-means) to group similar symptoms together.
Uncover patterns and relationships within the symptom data.
6. **Inferring Infection Location**\
Inference Model:
Develop a model to infer the location of infection based on individual or sets of symptoms.
Utilize the labeled data to train the model for accurate predictions.
