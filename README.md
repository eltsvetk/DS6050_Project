<h2 align="center">
  <strong>6050 Deep Learning, University of Virginia Data Science - Landslide Detection Project Fall Semester 2024</strong>
</h2>

<h3 align="center">
  <strong>Members</strong>
</h3>

<p align="center">
  <strong>Harold Haugen</strong><br>
  <strong>Max Pearton</strong><br>
  <strong>Elena Tsvetkova</strong><br>
  <strong>Daniel Sery</strong>
</p>

---

## Introduction
Landslide detection using deep learning models is a challenging yet critical task for disaster management and mitigation. This study explores the application of EfficientNetB3 and other Convolutional Neural Network (CNN) architectures to classify satellite imagery into landslide and non-landslide categories. We employed techniques such as data augmentation (e.g., saturation, contrast, cropping adjustments, etc.) and fine-tuning with layer unfreezing to improve model performance. Among tested architectures, EfficientNetB3 demonstrated superior results in identifying landslide features when trained with high-level layer unfreezing and transfer learning strategies. Grad-CAM visualizations provided valuable interpretability by highlighting spatial regions critical to the model's predictions. Our results indicate that diverse datasets, careful augmentation, and transfer learning significantly enhance the model's ability to generalize, offering a promising approach to landslide detection tasks.

---

## Presentations & Reports
We presented the following presentations to our peers over course of the semester. 
1. **Landslide_Project_Proposal**  Overview of our project proposal highlighting our motivation for the project, proposed data to be used, related literature review on the subject and intended machine learning methods to be explored.
2. **Landslide_Project_Final** Final presentation highlighting the data process used, initial CNN model performance and our selection of EfficientNet for a phase II exploration process, experimentation results across various scenarios of data and model methods, and a summary of our results and viewpoints.
3. **Landslide_Project_Final_Report** Final report detailing our 

---

## Notebook Contents
The following notebooks were created to support our project objectives including data acquisition, experimentation and visualization of results.  

1. **Image_Data_Loading.ipynb**   Descriptions, links and examples of aerial images as well as direct links to data sources for CNN modeling (on the team's DropBox location). 
2. **Landslide_SatImage_Tracker.ipynb** Accessing the NASA_SatImage_Log.csv file, where the team identified NASA landslide events and their lat./long. information for searching and obtaining Google Earth images of known landsildes.
3. **Landslide_Visuals** - Notebook building dataframes and plots for the report based on experimentation results. 
4. **Model_Design_FirstPhase_hh** - Initial development of a baseline CNN model and basic EfficientNetB3 implementation to assess performance
5. **Model_SecondPhase_NasNet_hh** - Notebook assessing NasNetLarge due to its deeper architecture. 
6. **Model_SecondPhase_EFB3_hh** - Exploratory notebook running the EfficientNetB3 model, base and fine-tuning including augmentation.  Weights and model saved to a .Keras file. 
7. **Model_SecondPhase_EFB3_hh-combdata** - Use of the final combined dataset (Set 4) Exploratory notebook running the EfficientNetB3 model, base and fine-tuning including augmentation.
8. **Model_SecondPhase_ReconstModel_hh** - Transition of EfficientNetB3 weights saved from the Model_SecondPhase_EFB3_hh notebook, and placed into a new model for specific training.
9. **Model_Design_FirstPhase_GradCam_EfficientNet_and_Simple.ipynb** - Built out the architecture for Grad CAM using the models for the simple CNN and original EFB3 model.
10. **Model_SecondPhase_GradCam_EFB3.ipynb** - Applied Grad CAM to our final EFB3 model. Compared results before vs after tuning. For the final EFB3 after tuning, applied GradCAM to the false positives, false negatives, and true positives. Also converted the lambda layer in original data augmentation code to a subclass of keras layers.
11. **phase 2 finetuning DS-2.ipynb** - Testing of various additional fine-tuning approaches, differences between going layer-by-layer vs by block, performance of deeper models
12. **Phase 2 MultiModal Testing DS.ipynb** - Rough initial implementation of a multi-modal approach to attempt both identification of landslides and classification of size
13. **densenetnewdataset.ipynb** - Applied Densenet model, base and hyperparameter tuning. Included data augmentation. 
14. **mobilenetnewdataset.ipynb** - Applied Mobilenet model
15. **USGS_Landslide.ipynb** - Initial EDA on USGS landslide data. This helped us understand the regions in the world that encounter the most landslides.
