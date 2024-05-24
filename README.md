# adamata-test

## My approach
The TrashNet dataset has an imbalanced class distribution, with the "trash" class having significantly fewer images compared to other classes. To address this issue, I performed oversampling on the "trash" class to match its size with the other classes.
Next, I performed training using a transfer learning approach with the MobileNetV2 model. The reason I chose this model is that it is relatively lightweight and offers good accuracy.

Transfer learning is advantageous because it significantly cuts down the overall training time since the model has already been trained on a large dataset and only fine-tuning is needed. It also improves performance as pre-trained models have learned rich feature representations from extensive training on large datasets. Additionally, transfer learning is more resource-efficient, making it ideal when computational resources and data are limited. Furthermore, for tasks with limited data, transfer learning helps mitigate the risk of overfitting by utilizing the knowledge from the pre-trained model. These benefits make transfer learning an effective approach for achieving high performance in a shorter time.

## How to reproduce the model
Open this [Kaggle notebook](https://www.kaggle.com/code/ghifari30/adamata). Make sure you sign in to your Kaggle account first, as you won't be able to use the GPU otherwise. After signing in, click "Copy & Edit" to open the notebook. To use the GPU, open the session options, select the accelerator, and then you're good to go.

Next, press "Run All." Once the training is complete, you can access the model in the /kaggle/working directory.

I don't use GitHub Actions because I don't employ any scripts for this model development; all of the work is done inside the notebook.
