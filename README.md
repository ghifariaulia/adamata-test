# adamata-test

## My approach
The TrashNet dataset has an imbalanced class distribution, with the "trash" class having significantly fewer images compared to other classes. To address this issue, I performed oversampling on the "trash" class to match its size with the other classes.
Next, I performed training using a transfer learning approach with the MobileNetV2 model. The reason I chose this model is that it is relatively lightweight and offers good accuracy.

Transfer learning is advantageous because it significantly cuts down the overall training time since the model has already been trained on a large dataset and only fine-tuning is needed. It also improves performance as pre-trained models have learned rich feature representations from extensive training on large datasets. Additionally, transfer learning is more resource-efficient, making it ideal when computational resources and data are limited. Furthermore, for tasks with limited data, transfer learning helps mitigate the risk of overfitting by utilizing the knowledge from the pre-trained model. These benefits make transfer learning an effective approach for achieving high performance in a shorter time.
