# ICP-for-Clinical-Reasoning

This repository contains the code and resources for the paper: 
**《Guiding Clinical Reasoning with Large Language Models via Knowledge Seeds》**

**Authors:** Jiageng Wu*, Xian Wu, and Jie Yang\#, PhD

*Contribute equally to this paper, \# Correspondence: 

## Introduction

Clinical reasoning refers to the cognitive process that physicians employ in evaluating and managing patients. This process typically involves suggesting necessary examinations, diagnosing patients’ diseases, and selecting appropriate therapies, etc. Accurate clinical reasoning requires extensive medical knowledge and rich clinical experience, setting a high bar for physicians. This is particularly challenging in developing countries due to the overwhelming number of patients and limited physician resources, contributing significantly to global health inequity and necessitating automated clinical reasoning approaches. Recently, the emergence of large language models (LLMs) such as ChatGPT and GPT-4 have demonstrated their potential in clinical reasoning. However, these LLMs are prone to hallucination problems, and the reasoning process of LLMs may not align with the clinical decision pathways of physicians. In this study, we introduce a novel framework, In-Context Padding (ICP), to enhance LLMs reasoning with medical knowledge. Specifically, we infer critical clinical reasoning elements (referred to as knowledge seeds) and use these as anchors to guide the generation process of LLMs. Experiments on two clinical question datasets validate that ICP significantly improves the clinical reasoning ability of LLMs.

## Method

We will upload all the code once our paper is published.

If there is any question, please feel free to contact me (jiagengwu@zju.edu.cn)

## Dataset
There are different examinations for different clinical disciplines, so we selected two datasets for model evaluation. 
1. [CMExam](https://github.com/williamliujl/CMExam), is a more comprehensive collection encompassing the six types of medical licensing examination: clinical medicine, traditional Chinese medicine (TCM), integrated TCM and Western medicine, dentistry, public health, pharmacy, and traditional Chinese pharmacy. The CMExam incorporates 68,119 medical questions sourced from past examinations and medical books. To ensure consistency with the genuine examination, we only included 57,565 questions that have five options, a singular correct answer, and an analysis exceeding 30 words. Lastly, we randomly selected 600 questions to serve as the testing set, while the remaining questions in CMExam were designated as the training set. 
2. CNMLE-Clinical (Confidential due to copyright issues), focuses on CNMLE for clinical medicine. The CNMLE-Clinical evaluates four parts of medicine: preventive medicine, preclinical medicine, clinical medicine, and medical humanities, which cover over twenty distinct medical subjects. We gathered questions from past examinations and various reference books, accumulating a total of 15,255 questions. Out of these, we randomly selected 600 questions, consistent with the number in the official examination, to serve as our testing set, while the remainder were used as the training set. Each instance in CNMLEClinical consists of a question, five candidate options, the correct answer, and a detailed explanation for the answer.
