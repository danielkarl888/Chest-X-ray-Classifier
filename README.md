# Test Notebook Instructions

## Prerequisites

Before running the test notebook, please follow these steps to download the necessary files and set up your environment.

### Step 1: Download Files

Download the model weights and KNN's joblib file from [this Google Drive link](https://drive.google.com/drive/folders/1gPmMeEmym7qc35gnU7JhfCrAPpwHjBZI).

### Step 2: Move Files to Your Drive

After downloading, move the files to your Google Drive.

### Step 3: Update Path Variables

Change the path variables in the notebook to match the location of the downloaded files in your Drive.

For example, update the paths as follows:

```python
BINARY_MODEL_WEIGHTS_PATH = Path("/content/drive/MyDrive/chest_xray/binary_model_VGG19_finetuned_weights_final.h5")
MULTICLASS_MODEL_WEIGHTS_PATH = Path("/content/drive/MyDrive/chest_xray/multiclass_model_ResNet101.keras")
ANOMALY_MODEL_WEIGHTS_PATH = Path("/content/drive/MyDrive/chest_xray/encoder_decoder_weights_final.h5")

BINARY_KNN_PATH = Path("/content/drive/MyDrive/chest_xray/binary_knn_classifier.joblib")
MULTI_KNN_PATH = Path("/content/drive/MyDrive/chest_xray/multi_knn_classifier.joblib")
