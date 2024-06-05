How to run the test notebook:

please download the weights and the knn's joblib file from here:
https://drive.google.com/drive/folders/1gPmMeEmym7qc35gnU7JhfCrAPpwHjBZI

after downloading, move it to your drive.

please change the paths vars accordingly to their name.

for example, 

BINARY_MODEL_WEIGHTS_PATH = Path("/content/drive/MyDrive/chest_xray/binary_model_VGG19_finetuned_weights_final.h5")
MULTICLASS_MODEL_WEIGHTS_PATH = Path("/content/drive/MyDrive/chest_xray/multiclass_model_ResNet101.keras")
ANOMALY_MODEL_WEIGHTS_PATH = Path("/content/drive/MyDrive/chest_xray/encoder_decoder_weights_final.h5")

BINARY_KNN_PATH = Path("/content/drive/MyDrive/chest_xray/binary_knn_classifier.joblib")
MULTI_KNN_PATH = Path("/content/drive/MyDrive/chest_xray/multi_knn_classifier.joblib")

Now you can run the cells. pay attention that you can upload image
in the cells of files.upload() command.

