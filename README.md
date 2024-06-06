# CLIP_ZeroShot_AntsBees

In this notebook, we use [CLIP](https://openai.com/index/clip/) to classify the popular hymenoptera dataset (see for example this [tutorial](https://pytorch.org/tutorials/beginner/transfer_learning_tutorial.html)).

**CLIP** is a neural network developed by researchers at OpenAI that is trained using aigned images and text from the internet. This model represents a dramatic shift from training on gold-standard labeled datasets to training on prevalent amounts of images from the web which are "naturally" annotated by text captions.

The model utilizes a vision and text transformer to encode the images and texts and is trained by maximizing the cosine similarity (dot product) between images and texts that are likely to be paired together. For more details, please see the link to Open AI's research above. 

Here we simply import the trained model and use it for inference on the hymenoptera to classify pictures of "ants" versus pictures of "bees." This is an example of **zero-shot classification**, which is essentially where one attempts to classify a dataset using a model that was not explicitly trained to do so. 
