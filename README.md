# Skin-Cancer-Detection-A-Comparative-Analysis-of-SVM-and-CNN-on-Melanoma-Image-Classification

(Done in a university setting as project part of a Machine Learning and Deep Learning class together with other three students.)

Machine Learning is the most important branch of Artificial Intelligence and it’s the capacity of the machine to constantly improve its performance autonomously without the need for a human to explain and guide it through the tasks (Brynjolfsson&McAfee, 2017).
Since the discovery of ML, several fields decided to implement it to improve efficiency, productivity, forecasting, and predictions. One of the sectors that is currently benefitting from technological innovation, and in particular machine learning, is healthcare, from research to personalized medicine to the diagnostic process.
The innovation has in fact proven extremely effective in predicting different types of cancer, such as breast, brain, lung, liver, and prostate cancer (Zhang, Shi&Wang,2023).

In this paper, we will focus on a dataset of pictures of melanoma, a type of skin tumor, and we will build different models of machine learning to achieve great reliability in identifying if the tumor is benign or malignant.

The No Free Lunch (NFL) Theorem explains that if no assumption is about the data, then there is no reason to prefer a specific model, they all need to be tested. In practice, this is not possible, so some assumptions have to be made about the data and only reasonable models are tested (Géron, 2019). In this paper, the dataset will be manipulated with Random Forest, Principal Component Analysis, Naive Bayes, Support Vector Machines, and Convolutional Neural Networks and the results of the different models will be compared in an analysis for efficiency and accuracy.

# Introduction

Cancer is a disease that causes the body’s cells located in an area to grow uncontrollably and spread also to other parts. Usually, human cells grow and multiply in an orderly fashion and when old or damaged they die, but if an individual gets sick they keep on growing even when damaged and they multiply causing lumps. These masses can be benign or malignant, then called cancer. When a tumor is cancerous it will attack other organs or tissues forming new tumors (the process of metastasis).
In the opinion of experts, cancer is the second leading cause of death in the world, following heart disease. Melanoma skin cancer is the fifth most common type (Morgan&Khatri, 2022). Melanoma is a skin cancer of the melanocytes, which are the cells engaged in the production of the pigment melanin for skin colour.

To improve prediction and reduce invasive diagnostic procedures, machine learning (ML) has been increasingly implemented in medicine. With decreasing storage and computation costs, ML models have been applied to achieve more accurate results in oncology, cardiology, and other fields (Burton, Fathieh, Nemati et al., 2024). Previous studies have demonstrated the potential of ML algorithms in various medical fields, including the classification of skin lesions (Esteva et al., 2017; Haenssle et al., 2018). These studies have shown that ML models, particularly those based on deep learning, can achieve diagnostic performance comparable to or exceeding that of dermatologists.
Image analysis will be the particular focus of our project, implemented on a dataset of images of melanoma both benign and malignant. Different models will be trained to recognized the type of melanoma through its image, with efficiency, accuracy and other parameters taken under consideration and compared.

# Motivation

The risk of melanoma has been on the rise recently, so it’s important to invest in better diagnosis practices. This is because when melanoma is diagnosed early, it can be treated. However if not, it can reach a metastatic state and treatment becomes less effective (Lapides, Saravi, Mueller&al, 2023). According to the American Cancer Society, melanoma accounts for only about 1% of skin cancers but causes a significant majority of skin cancer deaths, highlighting the need for early and accurate detection (American Cancer Society, 2021).

Diagnosis is fundamental for patient care, research, and guidelines. Unfortunately, there are risks associated with diagnostic testing, both with underuse as said above, but also with overuse. Aggressive testing, which is often linked to physicians’ fear of missing some signals about the possible disease, is putting patients at risk, and not improving certainty (Committee on Diagnostic Error in Health Care; Board on Health Care Services; Institute of Medicine; The National Academies of Sciences, Engineering, and Medicine, 2015).

The motivation behind this study is to leverage the advancements in ML to develop a reliable model, to predict whether a melanoma is benign or malignant. With our dataset composed of images of nevis and bruises, we aim to train a model that can assist dermatologists in making faster and more accurate diagnoses. This approach has the potential to reduce the workload on healthcare professionals but also to provide diagnostic support in regions with limited access to preventive medicine.

# Research Question

"What is the effectiveness of Convolutional Neural Networks (CNNs) and Support Vector Machines (SVMs) in accurately detecting and classifying skin cancer, and how do these models perform in terms of balancing false positives and false negatives in clinical diagnostics?”

This question aims to explore the effectiveness of the two machine learning techniques in identifying the type of melanoma through image analysis. The goal is to develop a reliable model that can assist dermatologists in making faster and more accurate diagnoses, ultimately improving patient care and reducing the risks associated with both underuse and overuse of diagnostic testing.
