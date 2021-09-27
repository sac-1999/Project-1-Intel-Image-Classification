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
      
      model.load_weights(checkpoint_filepath)


## EfficientNetB0.ipynb :

* loaded the dataset by using fetch_dataset.py file and then creted a model (EfficientNetB0) by using keras transfer learning (include_top = False). 
* Achieved almost 90% accuracy with 89% F1-Score


#### CLASSIFICATION REPORT

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
    
    
    
#### Confusion Matrix:
            
            [[390   0   0   0   3  44]
             [  0 471   0   2   1   0]
             [  3   1 428  94  24   3]
             [  0   0  66 452   5   2]
             [  3   1   7   4 490   5]
             [ 31   1   0   2   2 465]]



## Xception.ipynb :

* loaded the dataset by using fetch_dataset.py file and then creted a model (Xception) by using keras transfer learning (include_top = False). 
* Achieved almost 91.10 % accuracy with 90% F1-Score.

#### CLASSIFICATION REPORT:


              precision    recall  f1-score   support

           0      0.920     0.892     0.906       437
           1      0.994     0.994     0.994       474
           2      0.863     0.821     0.842       553
           3      0.848     0.851     0.850       525
           4      0.940     0.990     0.965       510
           5      0.910     0.930     0.920       501

      accuracy                          0.911      3000
      macro avg     0.913     0.913     0.913      3000  
      weighted avg  0.910     0.911     0.910      3000
      
      
#### Confusion Matrix: 


            [[390   0   0   1   5  41]
             [  0 471   1   1   1   0]
             [  1   2 454  76  18   2]
             [  0   1  68 447   7   2]
             [  0   0   3   1 505   1]
             [ 33   0   0   1   1 466]]




             




