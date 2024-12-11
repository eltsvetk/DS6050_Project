<h2 align="center">
  <strong>6050 Deep Learning - Landslide Detection Project Fall Semester 2024</strong>
</h2>

<h3 align="center">
  <strong>Members</strong>
</h3>

<p align="center">
  <strong>Harold Haugen</strong><br>
  <strong>Max Pearton</strong><br>
  <strong>Elena Tsvetkova</strong><br>
  <strong>Daniel Siery</strong>
</p>

---

## Introduction
Landslide detection using deep learning models is a challenging yet critical task for disaster management and mitigation. This study explores the application of EfficientNetB3 and other Convolutional Neural Network (CNN) architectures to classify satellite imagery into landslide and non-landslide categories. We employed techniques such as data augmentation (e.g., saturation, contrast, cropping adjustments, etc.) and fine-tuning with layer unfreezing to improve model performance. Among tested architectures, EfficientNetB3 demonstrated superior results in identifying landslide features when trained with high-level layer unfreezing and transfer learning strategies. Grad-CAM visualizations provided valuable interpretability by highlighting spatial regions critical to the model's predictions. Our results indicate that diverse datasets, careful augmentation, and transfer learning significantly enhance the model's ability to generalize, offering a promising approach to landslide detection tasks.

---

## Notebook Contents
The following notebooks were created to support our project objectives including data acquisition, experimentation and visualization of results.  

1. **Image_Data_Loading.ipynb**  Housing descriptions, links and examples to key data sources on the team's DropBox location. 
2. **Landslide_SatImage_Tracker.ipynb** Accessing the NASA_SatImage_Log.csv file, where the team identified NASA landslide events and their lat./long. information to obtain related Google Earth images.
3. **Model_SecondPhase_NasNet_hh** - Notebook assessing NasNetLarge due to its deeper architecture. 
4. **Landslide_Visuals** - Notebook building dataframes and plots for the report based on experimentation results. 
5. **Model_SecondPhase_EFB3_hh** - Exploratory notebook running the EfficientNetB3 model, base and fine-tuning including augmentation.  Weights and model saved to a .Keras file. 
6. **Model_SecondPhase_EFB3_hh-combdata** - Use of the final combined dataset (Set 4) Exploratory notebook running the EfficientNetB3 model, base and fine-tuning including augmentation.
7. **Model_SecondPhase_ReconstModel_hh** - Transition of EfficientNetB3 weights saved from the Model_SecondPhase_EFB3_hh notebook, and placed into a new model for specific training. 
