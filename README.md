# Medical_Image_Classification

For this project, the team aims to replicate an earlier work by Hussain et al. on comparing different augmentation techniques applied on a medical imaging dataset (DDSM) by their testing accuracy and ROC curves. Specifically, the team focuses on four augmentation techniques: Gaussian blur, Gaussian noise, Random rotations, Color jittering. The team shows that some augmentation techniques are able to extract medical image statistics more effectively than others, which will lead to better predictive performance in the corresponding models. 


# Steps to Obtain DDSM dataset
1. Navigate to https://www.kaggle.com/skooch/ddsm-mammography
2. Under the data explorer, navigate to "training10_0".
3. Download "training10_0.tfrecords". It is roughly a 1.0 GB file.


# Steps to Execute Code
1. Git clone the repository.
2. Move all notebooks in the Code folder in git repository, to Google Colab or another container with GPU access for faster runtime.
3. Notebooks labelled "01" to "05" reference the 5 models created (baseline, gaussian blur, gaussian noise, random rotations, and color jittering). Open the desired notebook in Google Colab or another container of your choice. 
4. Move the "training10_0.tfrecords" file into your google drive or container comprising of the notebooks. 
5. Update the filepath to your "training10_0.tfrecords" file in the code, so the notebook can successfully load the dataset.
6. Once the filepath has been updated, select "Restart Kernal and Run All Cells" or the equivalent of it in your chosen container settings.
7. The model validation section towards the end of the notebook will allow you to assess model performance corresponding to that data augmentation technique.


# Compare All Model Outputs (Side-by-Side)
1. Having already cloned the git repository by folling the above steps, open the "Model_Results.ipynb" notebook in your local laptop's jupyter instance (You do not need GPU availability for model comparision). This file exists inside the Code directory.
2. Select "Restart Kernal and Run ALl Cells" or the equivalent of it in your chosen container settings.
3. This will allow you to assess all model's ROC curve, PR curve, Accuracy, Precision, Recall, F1, Balanced Accuracy, AUC, and Average Precision Scores.
