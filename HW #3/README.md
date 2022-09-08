One of the most successful applications of deep learning in medical problems is Image Segmentation by using models such as U-Net, FPN and Masked RCNN.

We can use Image Segmentation for recognition of cancerous tissues in the lung, tumor tissue in the brain, etc.

In this question, we intend to use the implementation of U-Net model to distinguish brain tumor tissue in MRI images. The structure of UNET is shown below:
![unet](https://user-images.githubusercontent.com/88024963/189114656-b23ab2c4-a153-4883-b025-873aee5f4c1d.png)


Dataset is from kaggle:
https://www.kaggle.com/datasets/mateuszbuda/lgg-mri-segmentation?datasetId=181273&sortBy=voteCount

For evaluation of model's performance, we usd Jaccard and Dice metrics from the torchmetrics library.

In this part, we observed the effect of Data Augmentation and usage of Padding in Convolution.
In the end, we turned the "U-NET" model into a Residual model by adding some skip-connections and building some residual blocks.As shown below:
![resunet](https://user-images.githubusercontent.com/88024963/189115051-4b38b985-3b76-474f-9192-2dcfe93df6c2.png)


