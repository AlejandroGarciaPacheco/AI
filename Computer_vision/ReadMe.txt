Two of my worse performing models were left out of the function MaskDetection(). They are SVM/MLP with SIFT
All models can be tested for both datasets

PATH_TO_DATASET AND PATH_TO_PERSONAL_DATASET are the paths. these can be inserted in the line 
'X_test, y_test = import_selected_data(path chosen) - this allows the program to set the selected the path to be tested in the models.
in the test_dataset = CustomDataset(GOOGLE_DRIVE_PATH_TEST_LABELS, GOOGLE_DRIVE_PATH_TEST_IMAGES, transform=transform_test) - this path is to load the provided dataset
for the personalDataset is 
test_dataset = CustomDataset(PATH_TO_PERSONAL_DATASET + '/labels', PATH_TO_PERSONAL_DATASET + '/images', transform=transform_test)
in the MaskDectection, the path for the dataset also has to be changed accordingly.