# Project-1-Intel-Image-Classification

## Step - 1:
* Download Intel Image Dataset from kaggle https://www.kaggle.com/puneet6060/intel-image-classification and load into drive.
* Upload data to following path in google drive.      

      train_dir = pathlib.Path('/content/drive/MyDrive/Kaggle/seg_train/seg_train')
      pred_dir =  pathlib.Path('/content/drive/MyDrive/Kaggle/seg_pred/seg_pred')
      val_dir =  pathlib.Path('/content/drive/MyDrive/Kaggle/seg_test/seg_test')



## Step - 2:
        
* Upload this project in drive .

## Step - 3:

* If you want to train your own model then please Manually open colab notebooks enable GPU and run each cell accordingly.
* If you want to only predict for a set of images then also manually go to colab notebooks and run model architecture cell and load already uploaded model check points.
      
      





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

