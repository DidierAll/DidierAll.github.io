# About Me

I am dedicated to revolutionizing healthcare and improving health and wellness by advancing research and innovation in neuro-engineering and digital health technologies powered by machine learning, AI, and wearable technology.

I have over 10 years of leadership experience and over 20 years of scientific and clinical research and development expertise in wearable, biosensors, digital health, and neurotechnology. Applications of my work span remote health monitoring, movement disorders, neurorehabilitation, psychophysiological and cardiovascular effect of stress and relaxation, and overall health and wellness.
 
Throughout my career in academia and industry, I have honed my technical skills in neural and cardiac electrophysiology, data science, machine learning, algorithm development, and advanced analysis of clinical and biosensor data. 

I have an extensive clinical and scientific experience measuring, understanding, and improving physiological, health and wellness outcomes across diverse populations, including healthy and elderly as well as cancer survivors, stroke, traumatic brain injury, spinal cord injury, autism, and cardiovascular disease patients.

I am a detail-oriented and cross-functional collaborator with excellent communication & interpersonal skills. I excel at identifying and nurturing individual talents while providing an environment and resource to foster self-development and personal growth. Given my strong technical background, I thrive in leading collaborative effort to solve complex technological challenges to drive research, innovation and product development success.

# Project Portfolio

## Neurophysiological markers of Balance Deficit in Traumatic Brain Injury

As a co-Principal Investigator at the Kessler Foundation to this NJ Commission on Brain Injury Research funded research project, I seeked to investigate the neural and electrophysiological mechanisms of balance deficit of Traumatic Brain Injury using EEG, EMG, fMRI, dMRI and TMS. This ongoing research effort has led to several manuscripts and conference presentations:

1. Shenoy Handiru V., Alivar A., Hoxha A., Saleh S., Selvan S.E., Yue G.H., Allexandre D. (2021) Graph-theoretical Analysis of EEG Functional Connectivity during Balance Perturbation in Traumatic Brain Injury. Human Brain Mapping, (May), 8(14) pp. 4427-4447. doi: 10.1002/hbm.25554
2. Allexandre D., Handiru H.V., Hoxha A., Mark D., Selvan S.E., Yue G.H. (2021) Altered Modulation of the Movement-Related Beta Desynchronization with Force in Stroke – a Pilot Study. IEEE EMBS 2021 pp 6751-6754. 
3. Handiru H.V., Hoxha A., Mark D., Yue G.H., Allexandre D. (2021) An Automated Workflow for the Electric Field Modeling of High-definition Transcranial Direct Current Stimulation (HD-tDCS) in Chronic Stroke with Lesions.
4. Handiru, V. S., Suviseshamuthu, E. S., Saleh, S., Yue, G. H., & Allexandre, D. (2022). Identifying the Neural Correlates of Balance Deficits in Traumatic Brain Injury using the Partial Least Squares Correlation (PLSC) analysis.
Identifying the Neural Correlates of Balance Deficits in Traumatic Brain Injury using the Partial Least Squares Correlation (PLSC) analysis

## Atrial Fibrillation Classification from short ECG (CINC 2017 Challenge)

This project is inspired from CINC challenge which is aimed to develop machine learning algorithms to classify short single lead ECG recordings (between 30 s and 60 s in length) between normal sinus rhythm, atrial fibrillation (AF), or alternative rhythm, or is too noisy to be classified. 

![Figure 1. Example of the ECG waveforms](../../..ShortECG_AF-Classification_CINC2017/tree/main/figures/example_waveforms.svg](https://github.com/DidierAll/ShortECG_AF-Classification_CINC2017/tree/main/figures)

In this project, we start by building a simpler two-class classifier distinguishing between normal sinus rhythm and abnormal rhythm (atrial fibrillation included) by excluding the noisy recordings. We thus used 7,418 out of the original 8,528 training data recordings. 

We performed the following 
1. Even though, RR intervals are already provided, we first build an algorithm to extract RR intervals using the Pan-Tompkins method and measure the accuracy performance of the algorithm.
2. We processed and extracted features from the RR intervals data for our classifier.
3. We performed a grid search for hyperparameter tuning
5. We built, hypertuned, and compared performance among 9 common classifiers: Nearest Neighbors, Decision Tree,Random Forest, Random Forest (Balanced), Neural Net, AdaBoost, Naive Bayes, QDA, RBF SVM,

The Notebook can be found at [this link](https://github.com/DidierAll/ShortECG_AF-Classification_CINC2017/blob/main/AF_Classification.ipynb)
