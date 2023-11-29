# Fruit-Detection-and-its-Three-Stage-Maturity-Grading
This project has used a high-quality dataset with 9997 images comprising 15 fruit classes. Moreover, based on the significant applications that Convolutional Neural Networks have had till now, it proposes an analysis of deep learning algorithms for fruit detection and three-stage maturity grading considering the unripe, riped, and rotten stages of the given fruits: red apple, papaya, pear, cherry, and orange and achieves 90.24 percent accuracy. The results obtained will help in the development of fast and accurate detection of fruits and their quality.
### Methodology - 
We have used Fruits-360 dataset by extracting images from recording videos of fruits. The images from the Fruits-360 dataset were not annotated or segregated according to the ripeness or maturity but instead according to the type of fruit. The dataset did not contain the images for all the 3 stages of every fruit so we captured and added them to the existing dataset. The videos were captured under proper illumination and plain white background. After recording, the video frames were extracted from the videos. We have used the OpenCV python library to extract frames from the video. After extracting the videos, we removed the background, reduced the noise from the images, and then cropped the image to focus on the fruit for better feature extractions. The preprocessing of images is depicted in Fig 1. The training dataset contains a total of 9997 images of 5 different types of fruits which include orange, pear, cherry, apple, and papaya. There are a total of 15 classes as we have divided each fruit into 3 categories:
1. Unripe.
2. Ripe.
3. Rot.
### Model Configuration - 
The neural network structures that we are using consist of 3 convolutional layers intertwined with 2 max pooling layers. The output layer succeeds the last max-pooling layer which consists of one dropout layer, one flatten layer, and four dense layers to reduce the dimensions and execute the maturity stage grading for the fruit. Using the Dropout layer, the number of neurons in this hidden layer was minimized to reduce overfitting. We have used a total of 4 dense layers after implementing the flattening layers. The first dense layer, consisting of 5000 neurons, takes flattened image input from the preceding max-pooling layer. Successively, two more dense layers are implemented with 1024 and 512 neurons respectively. In the end, to predict each category of the fruits, a dense layer with 15 neurons was utilized as the output layer. In Table 1 we present the model configuration.
### Results - 
The project is maily focusing on reducing human effort and making their life easier The applied CNN architecture is a very mighty technique for deep learning approaches that successfully recognizes the fruits and performs fruit classification based on three different stages, that is unripe, ripe and rot. We have successfully trained this model using 15 classes. This model had given 90.24 percent accuracy in fruit ripening recognition and its classification.
