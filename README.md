# Project-1-Intel-Image-Classification

## Step - 1:
Upload data to following path in google drive 
* train_dir = pathlib.Path('/content/drive/MyDrive/Kaggle/seg_train/seg_train')
* pred_dir =  pathlib.Path('/content/drive/MyDrive/Kaggle/seg_pred/seg_pred')
* val_dir =  pathlib.Path('/content/drive/MyDrive/Kaggle/seg_test/seg_test')


              precision    recall  f1-score   support

           0      0.913     0.892     0.903       437
           1      0.994     0.994     0.994       474
           2      0.854     0.774     0.812       553
           3      0.816     0.861     0.838       525
           4      0.933     0.961     0.947       510
           5      0.896     0.928     0.912       501


    accuracy                           0.899      3000
    macro avg      0.901     0.902     0.901      3000
    weighted avg   0.899     0.899     0.898      3000

