# Wing Landmark Detection Model
Wing Landmark Detection model with image segmentation and detection. Used UNet model architecture to train the model.

# Sample outputs of pipeline
![WhatsApp Image 2022-09-26 at 15 48 33 (1)](https://user-images.githubusercontent.com/78916039/201337278-633a9167-65d1-4a28-a653-a63900f7fb32.jpeg)

# Model Architecture and Pipeline

![fnins-14-568614-g001](https://user-images.githubusercontent.com/78916039/201339602-d70eb5bf-c28a-4f5a-87e4-25434e36ca0b.jpg)

U-Net was used to handle the segmentation tasks. Annotated wing image coordinates are used to create landmark point masks. After that, those masks were used in training the model. 

<img width="422" alt="Screenshot 2022-11-11 at 15 28 25" src="https://user-images.githubusercontent.com/78916039/201340675-762f426b-9b82-4991-8489-fc1e31dce950.png"><img width="468" alt="Screenshot 2022-11-11 at 15 28 39" src="https://user-images.githubusercontent.com/78916039/201340683-599f5ad3-8f64-46a4-bed6-ee209efc5350.png">
