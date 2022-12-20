# Wing Landmark Detection Model
Wing Landmark Detection model with image segmentation and detection. Used UNet model architecture to train the model.

# Sample outputs of pipeline
<img width="435" alt="Screenshot 2022-12-20 at 12 12 49" src="https://user-images.githubusercontent.com/78916039/208629561-ae761233-4d44-4729-af75-fa1f2e2db0fd.png">![download (4)](https://user-images.githubusercontent.com/78916039/208629540-0e84a25d-b7dc-405e-8b7b-93cd0fd865e9.png)



# Model Architecture and Pipeline

![fnins-14-568614-g001](https://user-images.githubusercontent.com/78916039/201339602-d70eb5bf-c28a-4f5a-87e4-25434e36ca0b.jpg)

U-Net was used to handle the segmentation tasks. Annotated wing image coordinates are used to create landmark point masks. After that, those masks were used in training the model. 

<img width="422" alt="Screenshot 2022-11-11 at 15 28 25" src="https://user-images.githubusercontent.com/78916039/201340675-762f426b-9b82-4991-8489-fc1e31dce950.png"><img width="468" alt="Screenshot 2022-11-11 at 15 28 39" src="https://user-images.githubusercontent.com/78916039/201340683-599f5ad3-8f64-46a4-bed6-ee209efc5350.png">

After segmentation, Blob detection method is used to extract coordinates of the landmarks.

<img width="431" alt="Screenshot 2022-11-11 at 15 30 10" src="https://user-images.githubusercontent.com/78916039/201341006-a5decead-418b-4595-903f-3d5889dc07d4.png"><img width="432" alt="Screenshot 2022-11-11 at 15 30 25" src="https://user-images.githubusercontent.com/78916039/201341027-7845a438-3bb1-492b-8629-c6000a9e3da7.png">
