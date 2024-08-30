# Image-classifier
This project aims to build a deep learning model for image classification using a Convolutional Neural Network (CNN) implemented with Keras. The model will be trained to recognize and classify images into predefined categories, leveraging the power of deep learning to achieve high accuracy.
# Usage
First, collect training and validation data and deploy it like this(for multiclass classification),

./data/
  train/
    pizza/
      pizza1.jpg
      pizza2.jpg
      ...
    poodle/
      poodle1.jpg
      poodle2.jpg
      ...
    rose/
      rose1.jpg
      rose2.jpg
      ...
  validation/
    pizza/
      pizza1.jpg
      pizza2.jpg
      ...
    poodle/
      poodle1.jpg
      poodle2.jpg
      ...
    rose/
      rose1.jpg
      rose2.jpg
      ...
and then run train script.

python src/train-multiclass.py
Train script makes model and weights file to ./output/.

To test another images, run

python src/predict-multiclass.py
After training, you'll have tensorboard log in ./tf-log/ So you can see the result

tensorboard --logdir=./tf-log
