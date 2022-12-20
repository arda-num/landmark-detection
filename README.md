# Wing Landmark Detection Model
Wing Landmark Detection model with image segmentation and detection. Used UNet model architecture to train the model.

<div style="display:flex">
<img style="margin:auto"width="435" src="https://user-images.githubusercontent.com/78916039/208629811-dc99a25b-89fd-42ed-8507-0ae0a8e90ef1.png">
<img width="435" alt="Screenshot 2022-12-20 at 12 20 47" src="https://user-images.githubusercontent.com/78916039/208630572-53206a0e-b991-485e-b51f-9f9f0e466eba.png">
</div>



# Model Architecture and Pipeline

![fnins-14-568614-g001](https://user-images.githubusercontent.com/78916039/201339602-d70eb5bf-c28a-4f5a-87e4-25434e36ca0b.jpg)

U-Net was used to handle the segmentation tasks. Annotated wing image coordinates are used to create landmark point masks. After that, those masks were used in training the model. 

<img width="422" alt="Screenshot 2022-11-11 at 15 28 25" src="https://user-images.githubusercontent.com/78916039/201340675-762f426b-9b82-4991-8489-fc1e31dce950.png"><img width="468" alt="Screenshot 2022-11-11 at 15 28 39" src="https://user-images.githubusercontent.com/78916039/201340683-599f5ad3-8f64-46a4-bed6-ee209efc5350.png">

After segmentation, Blob detection method is used to extract coordinates of the landmarks.

<img width="431" alt="Screenshot 2022-11-11 at 15 30 10" src="https://user-images.githubusercontent.com/78916039/201341006-a5decead-418b-4595-903f-3d5889dc07d4.png"><img width="432" alt="Screenshot 2022-11-11 at 15 30 25" src="https://user-images.githubusercontent.com/78916039/201341027-7845a438-3bb1-492b-8629-c6000a9e3da7.png">
