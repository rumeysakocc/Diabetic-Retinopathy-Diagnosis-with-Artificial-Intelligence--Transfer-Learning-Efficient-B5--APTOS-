# Diabetic-Retinopathy-Diagnosis-with-Artificial-Intelligence

## First of all, let's talk about why Ophthalmology and Artificial Intelligence overlap so much:

<img src="https://github.com/KocHanim/Diabetic-Retinopathy-Diagnosis-with-Artificial-Intelligence--Transfer-Learning-Efficient-B5--APTOS-/assets/115664157/754cabb4-d149-472d-962a-414028b5fee8" alt="images" align="left" width="500" height="300">

<p>The most important feature that distinguishes ophthalmology from other branches is that it uses especially the sense of sight in the clinic. 
They see pathological findings in patients and make a diagnosis by analysing them. Nowadays, with the increase in the computing power of computers, deep learning models have become able to analyse images. 
Since most of the data to be analysed in ophthalmology is image-based and therefore the analysis of the data is related to image recognition,
processing the data and making a diagnosis with decision mechanisms appropriate to the processed data is a very suitable area for ophthalmology Artificial Intelligence cooperation.
The integration of artificial intelligence in ophthalmology not only revolutionizes diagnostic accuracy but also amplifies the speed of identifying and treating ocular conditions. By harnessing cutting-edge algorithms and machine learning, ophthalmologists now have the capability to swiftly process vast amounts of image-based data, unveiling nuanced patterns and subtleties in ocular scans and images. This marriage between technology and medical expertise enhances the precision of diagnoses, enabling earlier interventions and tailored treatment plans for patients. As ophthalmology becomes increasingly intertwined with the advancements in artificial intelligence, the field paves the way for a new era where swift, accurate, and personalized care in eye healthcare is at the forefront [1][2]</p>

## So why is Artificial Intelligence research in the literature particularly focused on Diabetic Retinopathy, although there are dozens of eye-related diseases? 

According to research, Diabetic Retinopathy affects one in every 3 people with diabetes and is one of the leading causes of preventable blindness. 
Of the more than 400 million people with diabetes worldwide, 10%, or about 40 million, have vision-threatening Diabetic retinopathy. 
Diabetic patients generally do not visit a doctor for regular retinal screening unless there is a symptom affecting their vision. However, 
the importance of regular eye check-ups to prevent vision loss with the early diagnosis of Diabetic Retinopathy has become evident, as a significant portion of the development of the disease progresses stealthily. 
The increasing number of diabetic individuals worldwide, along with a shortage of trained eye doctors, has drawn the attention of the healthcare sector to the use of artificial intelligence technology for retinopathy diagnosis. 
In various research studies using successful artificial intelligence algorithms, when we examine the values of sensitivity and specificity on paper, 
it is observed that artificial intelligence can make more successful diagnoses than even eye specialists.

## What is Diabetic Retinopathy?
Our eye transmits the image it sees to the brain through nerves. These nerves are located in the area of the eye we call Retina. We call "Diabetic Retinopathy" when diabetes affects the structure of the capillaries in this retina and disrupts the functioning of the retina and impairs the visual function. There are 5 classes to be used in this model.

 0 - No DR-> Healthy eye.

1 - Mild-> Microaneurysm

2 - Moderate-> Microaneurysm or haemorrhage should be present in at least 1 quadrant. Retinal haemorrhage, hard exudate, soft exudate and venous lumen irregularity may also be seen.

3 - Severe->More than 20 retinal haemorrhages in each quadrant, marked venous lumen irregularity in at least 2 quadrants and abnormal branching or dilation of capillaries in at least one quadrant.

4 - Proliferative DR-> Neovascularisation or preretinal haemorrhage

In order to make this classification, I would like to talk about the basic features of pathological findings.
Diabetes disrupts the structure of the capillaries in the retina, leads to cell loss, disruption of vascular permeability, accumulation of fluid and oily substances in the yellow spot area, and causes the capillaries to be blocked and non-nourished areas to appear. It forms new vessels in the retina that can bleed spontaneously. Haemorrhages in front of and inside the retina can leak into the posterior cavity of the eye. Vascularised membranes form in the retina and can lead to severe visual loss and painful eye pressure increases. All these findings distinguish the healthy eye from the sick eye.

<img src="https://gadsdeneye.com/wp-content/uploads/diabetic-retinopathy-vector.jpg">

## The dataset used in the project
In the project, the data set of the APTOS 2019 Blindness Detection competition on the kaggle site was used. 
The reason for using this dataset in particular; APTOS contains 5590 retinal images and was taken using different camera models and types.
https://www.kaggle.com/datasets/benjaminwarner/resized-2015-2019-blindness-detection-images/data

## Techniques used in the project

-> CLAHE is an adaptive extension of Histogram Equalisation that helps to dynamically preserve the local contrast characteristics of an image. CLAHE is followed by median filtering of DR images to smooth out background noise. The algorithms used have led to significant improvements in the enhancement of DR images.[3]

The proposed method improves the quality of the DR image while preserving sharpness and small details. Qualitative analysis clearly shows that the diabetic retinopathy image is significantly improved. 



-> Transfer Learning, suppose you are building a deep learning model but you do not have enough data. For example, you are trying to identify a rare skin disease and you have only 100 images. Meanwhile, for another project, you trained a classification model with a dataset containing 100,000 cat-dog photos and achieved a high accuracy score.  Although these two examples seem unrelated to each other, they are actually related. Because basically all computer vision models try to detect similar patterns. When you train a model with thousands of data, it becomes able to identify image features such as weights, edges, shapes, patterns and pixels of different densities in different layers. Thanks to these learned features, the model trained for cat-dog classification can even diagnose a rare skin disease.  You only need to remove the last layer of the cat-dog model, which calculates probabilities, and replace it with the classification layer appropriate to your data.
The most important feature of Transfer Learning:
-Short time
-Low data 
-High Accuracy
Ability to create models.

References:
[1]https://www.thehindu.com/sci-tech/science/seeing-the-magic-of-artificial-intelligence-applications-in-ophthalmology/article67437234.ece

[2]https://www.telefonica.com/en/communication-room/news/what-are-the-benefits-of-artificial-intelligence-in-ophthalmology/

[3]https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=7e0f9ed873453a92c21ae1427137ac501608f1ed


