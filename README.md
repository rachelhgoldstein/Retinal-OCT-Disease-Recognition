# Retinal-OCT-Disease Recognition

## Overview: 

Retinal optical coherence tomography (OCT) is a noninvasive imaging technique that essentially takes pictures of your retinas by measuring how much light reflects off the retina and optic nerve. It can be used to diagnose and manage diseases like diabetes-related retinopathy and age-related macular degeneration (AMD), amongst others. Millions of OCT scans are performed each year, and the analysis and interpretation of the images can take up a tremendous amount of time.

## Business Problem:

OCT imaging is crucial step in capturing a retinal disease early, and the analysis and interpretation of the images can be quite time-consuming and resource intensive. To address this challenge and optimize the use of resources, the goal is to develop a model capable of predicting whether a patient’s retinal scan is normal, or exhibits signs of CNV, DME, or Drusen diseases. Given that these diseases can lead to vision loss, the primary objective is to provide a more efficient method for medical professionals, particularly ophthalmologists, in their interpretation and analysis of retinal scans. 

## Data:

The data for this project comes from [Kaggle](https://www.kaggle.com/datasets/paultimothymooney/kermany2018/data). It contains approximately 85,000 images, each representing a distinct category - Normal, CNV, DME, or Drusen.

The data is split into separate train, test, and validation folders. Within each of these, there are labeled sub-folders for each category, with each individual image labeled as such: (disease)-(randomized patient ID)-(image number by this patient).

The images were selected from adult patients from the Shiley Eye Institute of the University of California San Diego, the California Retinal Research Foundation, Medical Center Ophthalmology Associates, the Shanghai First People’s Hospital, and Beijing Tongren Eye Center between July 1, 2013 and March 1, 2017. 

It was then subjected to a meticulous tiered grading system. The first tier involved undergraduate and medical students who had completed an OCT interpretation course, ensuring basic quality control. The second tier included four ophthalmologists who independently labeled each image passing the initial review, recording the presence or absence of pathologies. Finally, the third tier comprised of two senior independent retinal specialists, each with over 20 years of clinical retina experience, who verified the true labels for each image.

## Definitions:

According to the National Library of Medicine, the following terms are defined as follows:

CNV: (Choroidal Neovascularization): a condition where abnormal blood vessels grow beneath the retina in the choroid area. These abnormal blood vessels can leak fluid or blood into the retina, which can cause vision loss. Commonly associated with age-related macular degeneration (AMD), which is a leading cause of vision loss in older adults.

DME (Diabetic Macular Edema): a complication of diabetic retinopathy, which is an eye condition that can develop in people with diabetes. DME occurs when fluid builds in the macula, the central part of the retina responsible for our central vision, leading to to vision impairment and distortion.

Drusen: small yellow or white deposits that accumulate in the retina. They can be found in the macula or the peripheral retina. Drusen are a hallmark sign of age-related macular degeneration (AMD).

Treatment options for CNV, DME, and AMD may include medications, laser therapy, or in some cases, surgical interventions, depending on the specific condition and its stage.

## Modeling:


## Evaluation:


## Next Steps:

As with any machine learning project, there are a few next steps I would like to explore:

**1. Gather more data!** I started out with around 85,000 images, and used data augmentation techniques to increase that further. However, more genuine data is always beneficial and encouraged in building successful and accurate models.

**2. Continue tweaking the final model:** Although the final scores achieved are impressive, there is always room for improvement. Given more time, a more powerful computer, and additional memory, I believe these scores could be further optimized. 

**3. Return to Multi-Class classification:** For the purposes of this notebook, and due to time constraints, I have built a binary model that predicts if the image is normal or abnormal. Returning to a multi-class approach will allow for a more nuanced understanding of the individual diseases CNV, DME, and Drusen.

**4. Build a streamlit app and deploy!** this step aims to enhance accessibility for medical professionals, providing them with a convenient tool for obtaining a rapid and accurate initial opinion on a retina scan. The app will allow users to effortlessly upload a retina scan and receive a prediction on its normalcy or the presence of abnormalities.

## Conclusion:

In conclusion, applying the power of machine learning models to the analysis and interpretation of Retinal Optical Coherence Tomography (OCT) scans is a promising path for streamlining the diagnostic and management processes of vision-threatening diseases. The traditional approach, depending solely on manual analysis by medical professionals, is both time-consuming and resource-intensive.

The machine learning model developed in this project offers a valuable solution by significantly reducing the time and energy invested in the interpretation of retinal OCT scans. By serving as a rapid and accurate initial opinion, this model can empower ophthalmologists and other medical professionals, providing them with a reliable tool to aid in the diagnosis and management of eye conditions.

The spread and use of such a model has the capability to revolutionize the medical field, allowing for more efficient and accessible eye care. This innovation stands as a testament to the transformative impact of artificial intelligence in the realm of medical diagnostics, promising improved patient outcomes and contributing to the overall advancement of healthcare practices.

## For More Information:
For more information relating to multi-class modeling, please find the latest [Multi-Class](./Code/Working_Copy_Multiclass_V3.ipynb) notebook here. 

For more information relating to the binary modeling, please find the full analysis in the [Final Jupyter Notebook](./Retinal_OCT_Final_Notebook.ipynb), and the [presentation](./Retinal_OCT_Imaging_Presentation.pdf) here.

For additional information, please contact Rachel Goldstein at [rachelhgoldstein1@gmail.com](mailto:rachelhgoldstein1@gmail.com), or find me on [Linkedin](https://www.linkedin.com/in/rachel-h-goldstein/). 

## Repository Structure:
```
├── code
│   ├── Working_Copy_Binary.ipynb
│   ├── Working_Copy_Multiclass.ipynb
│   ├── Working_Copy_Multiclass_V2.ipynb
│   └── Working_Copy_Multiclass_v3.ipynb
├── .gitignore
├── README.md
├── Retinal_OCT_Final_Notebook.ipynb
└── Retinal_OCT_Imaging_Presentation.pdf
```
