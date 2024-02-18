### **| [Home](./README.md)  |  [Resume](./resume.md)     |  [Portfolio](./portfolio.md)  |  [Research](./research.md)  |** 

# Data Science Portfolio (Selected Projects)

## Atrial Fibrillation Classification from short ECG recordings (CINC 2017 Challenge)

This project is inspired by the Udacity course on Wearables that uses the CINC 2017 challenge. The CINC challenge aimed to develop machine learning algorithms to classify cardiac arrhytmia from short single lead ECG recordings (between 30 s and 60 s in length) into normal sinus rhythm, atrial fibrillation (AF), alternative rhythm, or data which is too noisy to be classified. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
**Figure 1.** _Example of short ECG waveforms recordings_ <br /> 
![Figure 1. Example of the ECG waveforms](/images/example_waveforms.svg) 

<!-- Commenting this: 
<figure>
  <img src="/images/example_waveforms.svg" alt="Trulli" style="width:100%">
  <figcaption>Figure 1. Example of short ECG waveforms recordings.</figcaption>
</figure>
-->

First a two-class classifier was built to distinguish between normal sinus rhythm and abnormal rhythm (atrial fibrillation included). Then a three-class classifier was built to distinguish between normal sinus rhythm, atrial fibrillation and other abnormal rhythm. 

In all cases, noisy recordings were excluded, keeping 7,418 out of the original 8,528 training data recordings.

The following was performed
1. Even though, RR intervals are already provided, an algorithm was first build to extract RR intervals using the Pan-Tompkins method and measure the accuracy performance of the algorithm.
2. Features were processed and extracted from the RR intervals data for our classifier.
3. We built, hypertuned, and compared performance among 9 common classifiers: Nearest Neighbors, Decision Tree, Random Forest, Random Forest (Balanced), Neural Net, AdaBoost, Naive Bayes, QDA, RBF SVM,

Skills and concepts used:
1. Data processing and RR peaks extraction from ECG timeseries using Pan-Tompkins algorithm
2. Time and frequency domain feature extraction 
3. Model fitting using stratified k-fold (k=5) cross-validation
4. Hyperparameter tuning and classifier performance comparison using grid search
5. Challenges associated with an unbalanced dataset (Afib representing 8.4% of the data)

The Notebook can be found in my github profile at [this link](https://github.com/DidierAll/ShortECG_AF-Classification_CINC2017/blob/main/AF_Classification.ipynb)

**Figure 2.** _Confusion Matrices comparing Model Performances highlighting the Balanced Random Forest having a more "balanced" accuracy across the 3 classes at aroud 60-80%_ <br />
![Figure 2. Confusion Matrices](/images/CINC2017_ConfusionMatrices.png)  


##  Activity Classification from IMU data 
Classification of biking, running and walking activity using a Random Forest Classifier with hyperparameters tuning using a grid search and a double nested leave-one-group-out cross-validation loop.  

This project makes use of the ["Wrist PPG During Exercise" dataset in physionet](https://physionet.org/content/wrist/1.0.0/)
containing wrist PPGs, accelerometers and gyroscopes recorded during walking, running and bike riding. The data was recorded from 8 participants (3 male, 5 female), aged 22--32 (mean 26.5).



Skills and concepts used:
1. Time and frequency domain feature extraction 
2. Model fitting using Random Forest
3. Hyperparameter tuning using grid search and a double nested leave-one-group-out cross-validation (logoCV)
4. Challenges associated with a small dataset

The Notebook can be found in my github profile at [this link](https://github.com/DidierAll/Activity_Classification-Biking/blob/main/Activity%20Classification%20-%20Biking.ipynb)

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

## Signal Browser

SignalBrowser is a graphic user interface software tool written in Matlab to load, process and analyze psychophysiological data (ECG, respiration and skin conductance).

This tool was developped and used to process psychophysiological data for the stress and relaxation research projects at the Cleveland Clinic (see _resume_ and _research projects_ pages)

Mode details can be found in my github [Readme](https://github.com/DidierAll/SignalBrowser/edit/main/README.md)

**Figure 1.** _Signal Browser main RR Editing View_ <br /> 
![RREditingView1](/images/SignalBrowser_RREditingView1.jpg)

<!-- Commenting this:
![RREditingView2](/images/SignalBrowser_RREditingView2.jpg)
-->
**Figure 2.** _Signal Browser All Signal View showing RR, Respiration rate, Skin Conductance, HRV/ANS timeseries (left panels) and outcomes (right panels)_ <br /> 
![AllSignalView](/images/SignalBrowser_AllSignalsView.jpg)

