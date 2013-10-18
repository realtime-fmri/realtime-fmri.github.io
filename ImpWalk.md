---
layout : page
title : Implementation Walkthough
subtitle : 
order : 1
---
## Existing real-time fMRI implementations

There are a variety of ways one can extract fMRI information based on how the brain is responding during an experiment, and then
 use this information to change stimuli (neurofeedback) or controll brain computer interfaces (BCI).  
The majority of real-time fMRI has focused on the use of univariate statistical analysis approaches related to the general linear model
(GLM) [\(Friston et al., 1995b\)](http://spin.ecn.purdue.edu/fmri/PDFLibrary/FristonK_HBM_1995_2_189_210.pdf) or to tracking the 
fMRI signal in one or a few regions of interest (ROIs). However, there are also real-time fMRI approaches that predict brain-states for feedback using distributed brain-state patterns. In other words, it's an approach of brain reading rather than that of localized activation.

In this section we will walkthough the different ways of implementing real-time fMRI.




##Univariate statistical approaches


### Region Of Interest (ROI)


Turbo BrainVoyager



##  Brain state prediction real-time fMRI.


### Temporally Adaptive Brain State (TABS) fMRI.

This part describes brain-state prediction real-time fMRI from [\(LaConte et al., 2007, ](http://www.ncbi.nlm.nih.gov/pubmed/17133383)[ 2011\)] (http://www.ncbi.nlm.nih.gov/pubmed/?term=Decoding+fMRI+brain+states+in+real-time+laConte)

####Advantages
1. No prior assumptions about functional localization and individual performance strategies required
  + the system learns these directly from the volunteer. 
2. Feedback can rely on a direct, intuitive translation of brain state, rather than a representation based on
increasing or decreasing local activity. 

####Highlights

+ "Brain states" [(as in Strother et al., 2002b)](http://www.ncbi.nlm.nih.gov/pubmed/11906218) are essentially the sensory/behavioral events or mental processes for which
a researcher might hope to find neural correlates through neuroimaging.
+ In a mass univariate context, "brain states" are represented as variates of interest in a design matrix. 
+ In a supervised learning context, these regressors serve instead as "labels." 

   When the labels are **categorical** in nature, we can formulate the modeling problem as a classification problem over a set of experimental
   categories. 

   When the labels are **continuous**, the problem can be framed as a regression problem to describe parametrically varying
brain states such as task difficulty, behavioral rate, visual angle, etc. 

   It is important to remember that regardless of the analyses performed
   (supervised, unsupervised, multivariate, mass univariate), the source
   data are exactly the same and come with the same limitations inherent
   to fMRI (e.g. voxel size, temporal sampling, and an indirect
   relationship to cellular brain activity). 

+ Multi voxel pattern analysis (MVPA) settings 
usually require a training data set (to estimate the parameters for the
supervised learning model) and an independent test set (that was
never seen by the training step). 
+Since the MVPA predicts brain states
(which are often designed or measured) and not brain maps (which
are usually not known), the models are easier to validate. 

 
 
### TABS implementation



The minimum required equipment that you will need to run a powerfull rt-fMRI on your scanner could look something like this:

CPU
RAM
etc.. 


