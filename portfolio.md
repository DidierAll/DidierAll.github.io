### **| [Home](./README.md)  |  [Resume](./resume.md)     |  [Portfolio](./portfolio.md)  |  [Research](./research.md)  |** 

# Data Science Portfolio (Selected Projects)

## Atrial Fibrillation Classification from short ECG recordings (CINC 2017 Challenge)

This project based on the [CINC 2017 challenge](https://physionet.org/content/challenge-2017/1.0.0), aimed to develop machine learning algorithms to classify cardiac arrhytmia from short single lead ECG recordings (between 30 s and 60 s in length) into normal sinus rhythm, atrial fibrillation (AF), alternative rhythm, or data which is too noisy to be classified. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
**Figure 1.** _Example of short ECG waveforms recordings_ <br /> 
![Figure 1. Example of the ECG waveforms](/images/example_waveforms.svg) 

<!-- Commenting this: 
<figure>
  <img src="/images/example_waveforms.svg" alt="Trulli" style="width:100%">
  <figcaption>Figure 1. Example of short ECG waveforms recordings.</figcaption>
</figure>
-->

Skills and concepts covered:
1. Data processing and RR peaks extraction from ECG timeseries using an implementation of the Pan-Tompkins algorithm
2. Time and frequency domain features extraction 
3. Model fitting and Hyperparameter tuning using stratified k-fold (k=5) cross-validation
4. Performance comparison between 9 common classifiers: Nearest Neighbors, Decision Tree, Random Forest, Random Forest (Balanced), Neural Net, AdaBoost, Naive Bayes, QDA, and RBF SVM.
5. Discussion and considerations related to challenges associated with an unbalanced dataset (Afib representing 8.4% of the data)

Python libraries: numpy, pandas, matplotlib, seaborn, scipy, sklearn 

The project notebook can be found in my [github repository](https://github.com/DidierAll/ShortECG_AF-Classification_CINC2017/blob/main/AF_Classification.ipynb)

**Figure 2.** _Confusion Matrices comparing Model Performances highlighting the Balanced Random Forest having a more "balanced" accuracy across the 3 classes at aroud 60-80%_ <br />
![Figure 2. Confusion Matrices](/images/CINC2017_ConfusionMatrices.png)  


##  Activity Classification from IMU data 
This project aimed to classify biking, running and walking activity from wrist accelerometers and gyroscopes recording using the ["Wrist PPG During Exercise" dataset in physionet](https://physionet.org/content/wrist/1.0.0/)

Skills and concepts used:
1. Exploratory data analysis
2. Time and frequency domain feature extraction 
3. Model fitting using Random Forest a classifier
4. Hyperparameter tuning using grid search and a double nested leave-one-group-out cross-validation (logoCV)
5. Performance visualization using PCA and t-NSE 
6. Discussion of challenges and limitations associated with a small dataset (N=8)

Python libraries: numpy, pandas, matplotlib, seaborn, scipy, sklearn

The project notebook can be found in my [github repository](https://github.com/DidierAll/Activity_Classification-Biking/blob/main/Activity%20Classification%20-%20Biking.ipynb)

**Figure 1.** _Raw Data from Subject s3_ <br /> 
![Figure 1. Confusion Matrices](/images/RawData_s3.JPG) 


**Figure 2.** _Final Model logo CV accuracy performance_ <br /> 
![Figure 2. Confusion Matrices](/images/FinalModel_logoCV_Results.JPG) <br /> 


**Figure 3.** _Decision Boundary for t-NSE" title="Decision Boundaries when keeping the top 10 features_ <br /> 
![Figure 3. Confusion Matrices](/images/DecisionBoundaryTop10Features.JPG) 

<!-- Commenting this:
<img src="/figures/RawData_s3.JPG" alt="Raw Data" title="Raw Data from Subject s3">
<br/>
<br/>
<img src="/figures/FinalModel_logoCV_Results.JPG" alt="logo CV Results" title="Final Model logo CV accuracy performance">
<br/>
<br/>
<img src="/figures/DecisionBoundaryTop10Features.JPG" alt="Decision Boundary for t-NSE" title="Decision Boundaries when keeping the top 10 features">
-->

## SignalBrowser

SignalBrowser is a graphic user interface software tool, I developed in Matlab to load, process and analyze psychophysiological data (ECG, respiration and skin conductance). 

This tool was used to process and analyze psychophysiological data for several research projects conducted at the Cleveland Clinic looking at the autonomic nervous system and molecular/inflammatory response of stress and relaxation (see _resume_ and _research projects_ pages)

Mode details can be found in [my github repository](https://github.com/DidierAll/SignalBrowser/edit/main/README.md)

**Figure 1.** _Signal Browser main RR Editing View_ <br /> 
![RREditingView1](/images/SignalBrowser_RREditingView1.jpg)

<!-- Commenting this:
![RREditingView2](/images/SignalBrowser_RREditingView2.jpg)
-->
**Figure 2.** _Signal Browser All Signal View showing RR, Respiration rate, Skin Conductance, HRV/ANS timeseries (left panels) and outcomes (right panels)_ <br /> 
![AllSignalView](/images/SignalBrowser_AllSignalsView.jpg)

