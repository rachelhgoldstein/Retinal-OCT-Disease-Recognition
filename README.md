# Retinal-OCT-Images

**Overview:**

Retinal optical coherence tomography (OCT) is a noninvasive imaging technique that essentially takes pictures of your retinas by measuring how much light reflects off the retina and optic nerve. It can be used to diagnose and manage diseases like diabetes-related retinopathy and glaucoma, amongst others. Millions of OCT scans are performed each year, and the analysis and interpretation of the images can take up a tremendous amount of time.

**Business Problem:**

In order to save time and resources in analyzing and interpreting OCT scans, the problem at hand is to create a model that can predict whether a patient's retinal scan is normal or shows signs of CNV, DME, or DRUSEN diseases.

The stakeholders are medical professionals, specifically ophthalmologists.

**Data:**

The data for this project comes from Kaggle: https://www.kaggle.com/datasets/paultimothymooney/kermany2018/data. It contains 84,495 images, and 4 categories to predict (NORMAL, CNV, DME, or DRUSEN).

The data is split into separate train, test, and validation folders. Within each of these, there are labeled sub-folders for each category, with each individual image labeled as such: (disease)-(randomized patient ID)-(image number by this patient).

The images were selected from adult patients from the Shiley Eye Institute of the University of California San Diego, the California Retinal Research Foundation, Medical Center Ophthalmology Associates, the Shanghai First People’s Hospital, and Beijing Tongren Eye Center between July 1, 2013 and March 1, 2017.

**Definitions:**

According to the National Library of Medicine, the following terms are defined as follows:

CNV: (Choroidal Neovascularization): a condition where abnormal blood vessels grow beneath the retina in the choroid area. These abnormal blood vessels can leak fluid or blood into the retina, which can cause vision loss. Commonly associated with age-related macular degeneration (AMD), which is a leading cause of vision loss in older adults.

DME (Diabetic Macular Edema): a complication of diabetic retinopathy, which is an eye condition that can develop in people with diabetes. DME occurs when fluid builds in the macula, the central part of the retina responsible for our central vision, leading to to vision impairment and distortion.

Drusen: small yellow or white deposits that accumulate in the retina. They can be found in the macula or the peripheral retina. Drusen are a hallmark sign of age-related macular degeneration (AMD).

Treatment options for CNV, DME, and AMD may include medications, laser therapy, or in some cases, surgical interventions, depending on the specific condition and its stage.

**Modeling:** 

**Evaluation:**


**Next Steps:**

As with any machine learning project, there are a few next steps I would like to explore:

1. Gather more data! I started out with around 85,000 images, and used data augmentation techniques to increase that further. However, more genuine data is always useful and encouraged in building successful and accurate models.

2. Continue tweaking the final model: Although my final scores are pretty good, there is always room for improvement. Given more time, a more powerful computer, and additional memory, I believe these scores could be increased. I would also like to try GridSearching to help with hyperparameter tuning.

3. Return to Multi-Class classification: For the purposes of this notebook, and due to time constraints, I have built a binary model, i.e., is the image normal, or abnormal. The limitations of this is you lose the individuality of the diseases CNV, DME, and Drusen. I would like to return to my earlier versions where I built a multi-class model, and spend some time increasing testing accuracy.

4. Build a streamlit app and deploy! To make it easier and more accessible for medical professionals to get a second opinion on a retina scan, I would like to build a streamlit app that will allow a user to drop a retina scan in, and get a prediction on whether it is normal, or contains an abnormality.

**Conclusion:**

In conclusion, applying the power of machine learning models to the analysis and interpretation of Retinal Optical Coherence Tomography (OCT) scans is a promising path for streamlining the diagnostic and management processes of vision-threatening diseases such as diabetes-related retinopathy and glaucoma. The traditional approach, depending solely on manual analysis by medical professionals, is both time-consuming and resource-intensive.

The machine learning model developed in this project offers a valuable solution by significantly reducing the time and energy invested in the interpretation of retinal OCT scans. By serving as a rapid and accurate second opinion, this model can empower ophthalmologists and other medical professionals, providing them with a reliable tool to aid in the diagnosis and management of eye conditions.

The spread and use of such a model has the capability to revolutionize the medical field, allowing for more efficient and accessible eye care. This innovation stands as a testament to the transformative impact of artificial intelligence in the realm of medical diagnostics, promising improved patient outcomes and contributing to the overall advancement of healthcare practices.

**For More Information:**


**Repository Structure:**
