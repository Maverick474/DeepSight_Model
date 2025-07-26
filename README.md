# Model Creation
The user can preprocess the dataset, train a pytorch model of your own, predict on new unseen data using your model.

### [Google Colab](https://colab.research.google.com/) is recommended when training the model

## Dataset
- Deepfake Detection Challenge (DFDC)
- Celeb DF
- FaceForensics ++

## Model Preprocessing
- Load the dataset
- The video is splitted into frames
- Face is cropped from each frame
- Cropped face is saved

## Model Training 
- Preprocessed video is loaded along with the labels with csv file
- Create a pytorch model using transfer learning with RestNext50 LSTM and Attention layer
- Data is splitted into train and test
- Train the model
- Test the model
- Save the model as .pt file

## Predict
- The saved pytorch model is loaded
- Predict the output based in trained weights.

## Benchmarks

| DFDC   | Celeb-DF | FF++  |
|--------|----------|-------|
| 89.4 % |  89.3 %  | 89.1 % |




