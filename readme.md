# Evaluating Elements of Empathic Communication with Experts, Crowds, and Large Language Models

This project investigates the inter-rater reliability of experts, crowds, and large language models (LLMs) in evaluating empathic communication. We analyze annotations of 21 empathy-related features across 200 conversations from four datasets, where one partner shares a problem and the other offers support.    

### Data
We use 50 conversations from four conversation datasets:
- EmpatheticDialogues: 24,850 crowdsourced conversations with annotations on empathy, fluency, and relevance.    
- EPITOME: 3,081 Reddit conversations with annotations on emotional reactions, interpretations, and explorations.   
- Perceived Empathy: 501 conversations with human responses to personal troubles, rated on various dimensions of perceived empathy.  
- Lend an Ear Pilot: 150 workplace trouble conversations with annotations on validating emotions, encouraging elaboration, demonstrating understanding, providing unsolicited advice,self-orientation, and dismissing emotions.    

### Download the Dataset
You can find the combined annotations for all four datasets in data/combined_annotations_across_methods_and_datasets.csv. This file contains annotations from experts, crowds, and LLMs (GPT-4o, Gemini 1.5 Pro) for each of the 21 dimensions.

The original annotations for each 50 conversation sample is stored in the original_samples directory. You can find the conversations and annotationsin the following files:

- EmpatheticDialogues: sample_empatheticdialogues.csv
- EPITOME: sample_epitome.csv
- Perceived Empathy: sample_perceived_empathy_annotations.csv (conversations available on request)
- Lend an Ear Pilot: sample_rpg_conversations.csv and sample_rpg_annotations.csv 

### Analysis
We compare inter-rater reliability between experts, crowds, and LLMs (GPT-4o, Gemini 1.5 Pro) using Spearman's rank correlation, Cohen's Kappa with quadratic weighting, and F1 scores.  We also conduct a qualitative analysis of conversations with high and low agreement between annotators.    

### Replicate our Analysis
You can replicate the results from our paper using the jupyter notebook analysis.ipynb in the repository.