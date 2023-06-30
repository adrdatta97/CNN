# Convolutional Neural Network 

<h3> "I dream of painting and then I paint my dream." - Vincent Van Gogh" </h3>

Discovering the fascinating realm of deep learning algorithms to unleash the power of computer vision techniques, particularly convolutional neural networks (CNN), to tackle intricate image classification tasks, uncovering effective strategies like transfer learning, fine-tuning, and augmented data, amplifying recognition performance. 


<p align="center">
  <img src="https://github.com/adrdatta97/CNN/assets/117360902/7cee0d47-03d8-4c74-9883-75f4821c71b7" alt="Image" width="300" />
</p>


The project aimed to investigate the utilization of Convolutional Neural Networks (CNNs) for artist identification based on artwork. Various studies and approaches were explored to address the challenge of limited data availability. The application of transfer learning, brushwork analysis, statistical models, and multi-layer feature fusion was examined. Promising results were observed in the classification of artists using CNNs, providing a strong foundation for further research and the development of models. The key finding is that CNNs can be effectively utilized for artist identification, opening up opportunities for future advancements in this field.

1. The CNN model is designed to recognize artists based on the patterns of their artwork by extracting and learning features from the input images.
2. It consists of multiple layers, including convolution layers with different numbers of filters to extract features and max pooling layers to reduce spatial dimensions and retain useful information.
3. The model uses a combination of convolutional, pooling, and fully connected layers to progressively extract complex features from the input images and make predictions about the artist.
4. The softmax activation function is employed in the output layer to convert the network's outputs into a probability distribution across the projected output classes, enabling multiclass classification.
5. The model is trained using the softmax loss (categorical cross-entropy loss) and optimized with the Adam optimizer, which adjusts the learning rate based on gradients and squared values to improve training performance.



<p align="center">
  <img src="https://github.com/adrdatta97/CNN/assets/117360902/21479603-cc64-4756-850b-8cf662df9dbd" alt="Image" width="900" />
</p>

~ ~ Several convolution neural net architecture were tested in this project ~ ~

<b>Custom Model: </b> The custom CNN model is designed with data augmentation techniques to address imbalanced data. It consists of input, data augmentation, convolutional, max pooling, dense, and output layers. However, the model's performance is below average with an test set accuracy of 54.89%, indicating the need for a more complex architecture. 

<b> VGG16: </b> VGG16 is a pre-trained model developed by the University of Oxford. It has been trained on a large dataset of 14 million images belonging to 10,000 classes. Due to its outstanding performance in the ILSVRC-2014 challenge, it is utilized in this project with slight modifications to match the 50 classes in the dataset. The model performed moderately with the test set accuracy of 63% (with augmentation) and 64% (without augmentatation)

<b> ResNet50: </b> ResNet50 addresses the issue of vanishing gradients in deep neural networks. By incorporating residual connections, it enables the creation of very deep networks. The architecture of ResNet50 is similar to VGG16, consisting of input, convolutional, dense, and output layers. However, in this project the performance yielded a result of 16.3% test set accuracy. 

<b> ConvNeXt:</b> ConvNeXt models, developed by Facebook research engineers, are an improved version of convolutional ResNet models. They outperform Vision Transformers (ViT) in computer vision tasks. ConvNeXt follows a similar architecture to the previous models, with the addition of dense and output layers specific to the artwork recognition task. The test set accuracy of the ConvNext model was 74.4%. 

<h3>Conclusion : </h3>
The findings highlight the potential of deep learning for art classification, with implications for art cataloging and authentication. Further research can explore additional architectures and augmentation methods in this field.

<h3> Acknowledgements : </h3>
The data was scraped from artchallenge.ru at the beginning of Februray 2023.













