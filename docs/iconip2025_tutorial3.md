---
layout: default
title: ICONIP2025 Tutorial 3
---

# AI for Human Neuroscience Research: Generative AI Modeling and Large-Scale Analysis

**Date:** November 20, 2025  
**Time:** 10:00–13:00  
**Location:** Seminar room C209 (Main campus Level C) [Map](https://iconip2025.apnns.org/venue/#:~:text=campus%20Level%20C)  
**Tutorial Organizers:**
- Saori Tanaka (ATR / NAIST)  
- Okito Yamashita (ATR / RIKEN AIP)  
- Yu Takagi (Nagoya Institute of Technology)  

**Abstract:**
This tutorial introduces recent advances in human neuroscience empowered by artificial intelligence, with a focus on generative modeling and large-scale brain data analysis. It consists of three integrated sessions, each led by a domain expert.

---

## Note to participant:

- **This tutorial allows pre-registered participants to join via Zoom. However, the tutorial cannot be conducted in exactly the same manner for Zoom participants and on-site participants. Support for exercises and responses to questions will be provided only to on-site participants.**

- **Please read this document and complete "Preparation" before the tutorial.**
[https://vbmeg.atr.jp/docs/iconip2025/static/iconip2025.html](https://vbmeg.atr.jp/docs/iconip2025/static/iconip2025.html)

- **Please note that Session 3-3 also includes several required preparation steps. Please carefully review the instructions in the “Hands-on Materials” section for Session 3-3 and complete them in advance.**

---

## News & Updates

Please check this page regularly for the latest updates regarding the tutorial.

- **November 18, 2025** - Notice to participants and Hands-on materials for 3-1 and 3-3 updated
- **November 13, 2025** - Notice to participants updated
- **November 11, 2025** - Preparation for hands-on updated
- **November 4, 2025** - Preparation for hands-on updated
- **November 4, 2025** - Information for Zoom participants 
- **August 1, 2025** — Tutorial page released

---

## Preparation　**【IMPORTANT】**

This hands-on session will be conducted using **Google Colab for 3-1 and 3-3** and **MATLAB for 3-2** on each participant’s laptop. Participants must bring their own laptop confirmed to run Google Colab and MATLAB. No laptops will be provided to participants. For participants who do not have MATLAB license, please use MATLAB online basic which is free cloud service provided by Mathwork Inc. (https://jp.mathworks.com/products/matlab-online.html).

---

## Description and Outline

### 3-1. Population Analysis of Large-Scale Human MRI Datasets  
**Speaker:** Saori Tanaka (ATR / NAIST)

This session will cover techniques for extracting population-level brain features from large-scale MRI datasets, including preprocessing, dimensionality reduction, and population inference using machine learning.

1. Introduction to Large-Scale Human MRI Datasets  
2. Dataset Overview  
3. Preprocessing Pipeline  
4. Statistical Analysis and Visualization
5. Hands-on

Hands-on Materials:  
[https://www.notion.so/ICONIP2025-Tutorial-3-2a14e529b79180a28edfe575cfa6b185?source=copy_link](https://www.notion.so/ICONIP2025-Tutorial-3-2a14e529b79180a28edfe575cfa6b185?source=copy_link)

### 3-2. Human Brain Dynamics via Multi-Modal Integration and Machine Learning 
**Speaker:** Dr. Okito Yamashita (ATR / RIKEN AIP)

This session will explore methods for analyzing human brain dynamics by integrating multiple neuroimaging modalities (e.g., fMRI, MEG) using advanced machine learning techniques. More specifically, the MEG/EEG current source imaging method using the Bayesian learning will be introduced.

1. Intoduction to MEG/EEG current source imaging
2. Foward modeling
3. Inverse modeling
4. Applications
5. Hands-on

Hands-on Materials:  
[https://vbmeg.atr.jp/docs/iconip2025/static/iconip2025.html](https://vbmeg.atr.jp/docs/iconip2025/static/iconip2025.html)

### 3-3. Modeling Human Brain Activity with Deep Neural Networks  
**Speaker:** Yu Takagi (Nagoya Institute of Technology)

This session will introduce the neural encoding model as a method for identifying alignment between the latent representations of deep neural networks and human brain activity.

1. Introduction to modeling brain data with deep neural networks
2. Hands‑on session: modeling neural data while watching visual images

Hands-on Materials:  
[https://colab.research.google.com/drive/1JCp3bfKYnn-rezfMXO-gCDBShd5PhmBM?usp=sharing](https://colab.research.google.com/drive/1JCp3bfKYnn-rezfMXO-gCDBShd5PhmBM?usp=sharing)  

Before participating in the tutorial, please complete the following consent form and select “Agree”. This step is required in order to access a Google Drive public folder called algonauts_2023_tutorial_data.  
Consent form:
[https://docs.google.com/forms/d/e/1FAIpQLSehZkqZOUNk18uTjRTuLj7UYmRGz-OkdsU25AyO3Wm6iAb0VA/viewform?usp=sf_link](https://docs.google.com/forms/d/e/1FAIpQLSehZkqZOUNk18uTjRTuLj7UYmRGz-OkdsU25AyO3Wm6iAb0VA/viewform?usp=sf_link)  

Before running the tutorial code, you need to select this folder in Google Drive (algonauts_2023_tutorial_data) and choose “Add a shortcut to Drive.” This will create a shortcut (without copying or taking space) of the folder to a desired path in your Google Drive, from which you can read the content after mounting using drive.mount(). Please make sure that the following commands run without errors in Google Colab:  
from google.colab import drive  
drive.mount('/content/drive/', force_remount=True)  
data_dir = '/content/drive/MyDrive/algonauts_2023_tutorial_data'  # @param {type:"string”} # Please edit the `data_dir` variable below with the path on your Drive to the `algonauts_2023_tutorial_data` shortcut folder  
fmri_dir = os.path.join(data_dir, 'training_split', 'training_fmri’)  
lh_fmri = np.load(os.path.join(fmri_dir, 'lh_training_fmri.npy'))  
rh_fmri = np.load(os.path.join(fmri_dir, 'rh_training_fmri.npy'))  

---

## Target Audience

This tutorial is intended for researchers interested in applying AI techniques to human brain imaging data such as MRI and MEG. It is particularly suited for those who wish to perform AI-based analyses using publicly available open neuroimaging datasets or their own recorded data. 

No prior experience with neuroimaging analysis is required. Sample brain data will be provided in advance for hands-on demonstrations. For Session 3-2, access to a MATLAB license is recommended for smoother participation.

---

## Organizer Biographies

### Saori Tanaka (ATR / NAIST)  

[Website](https://xsaori.github.io/)

Dr. Saori Tanaka is a professor of Division of Information Science, Nara Institute of Science and Technology and a department head of ATR Brain Information Communication Research Lab. Group.
<details>
<summary>Click for detailsく</summary>

Dr. Saori Tanaka began her research career in 2001 as a graduate student in computational neuroscience at the Nara Institute of Science and Technology (NAIST). Her early work contributed foundational computational models of human decision-making, particularly in the area of temporal discounting. Her 2004 publication in Nature Neuroscience on this topic has been cited over 1,000 times and has had a significant impact on the development of the field. In recognition of this achievement, she received the Best Paper Award, Best Research Award, and Encouragement Award from the Japan Neural Networks Society in 2005.

As data science rapidly advanced, Dr. Tanaka became increasingly interested in integrating hypothesis-driven and data-driven approaches. In recent years, she has played a leading role in several national neuroscience flagship projects funded by MEXT and AMED. In particular, she has spearheaded the construction of open-access MRI data repositories comprising thousands of patients with brain disorders (Tanaka et al., 2022, Scientific Data). Recognizing the need for improved infrastructure and policy, she has actively advocated for enhanced data-sharing practices in Japan.
</details>

### Okito Yamashita (ATR / RIKEN AIP)  

[Website](https://bicr.atr.jp/~oyamashi/?lang=en)

Dr. Okito Yamashita is a head of the department of the computational brain imaging in ATR. He also holds a concurrent position (team leader) at the computational brain dynamics team in RIKEN-AIP. His reaserch interests are brain dynamics and its relationship to brain function using combinations of the data-driven statistical modeling and biophysical modeling. He has published more than 50 papers in the field of human neuroimaging.


### Yu Takagi (Nagoya Institute of Technology)  

[Website](https://yu-takagi.github.io/)

Dr. Yu Takagi is an Associate Professor at Nagoya Institute of Technology. His research interests lie at the intersection of Artificial Intelligence and Neuroscience. Recently, he has combined generative AI with neuroscience data to explore the alignment between artificial and biological representations, employing encoding–decoding frameworks alongside newer methods that build on and extend these models.

---

## Contact 

[Inquiry form](https://forms.gle/5KYfL9SSJBtBAwcEA)

---
[ICONIP2025 Official Website](https://iconip2025.org)