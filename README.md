# Weapon Detections

## Project Description
The project is about how we can use images to detect weapons do a data classification into 3 categories, which includes normal, threat, or carrying weapon,.

<b>Normal</b> means that no weapons are detected in the image. <b>Threat</b> means that weapons are detected in the image but the holder / actor is not in any threatening stance. For example, a police keeping a gun in the holster. <b>Carrying</b> means that a weapon is detected in the images and the actor / holder is in threatening stance. For example, a robber holding a gain aiming at a hostages.

The project consists of the preprocessing steps done to the training images as well as the LeNet-5 model used to classify the images. In addition to that, there is also a grad-cam steps to analyze the results of the model further.

## About the Data

The data is gathered from various sources, including raw footage and internet sources (Youtube) in a form of a videos. Each videos gathered are first categorized into the 3 difference class. Images are then generated from each frames of the videos collected.

Collected images were than carefully cleaned. These are the few steps and considerations during data cleaning steps:

1. For images that initially falls under the category between **Threat** and **Carrying**, if no apparent weapon are to be seen in the image we would remove that from the dataset.
2. Remove blurry / highly pixelated images.
3. Remove any mistakenly classified images, such as images that contains weapon found under **Normal** dataset.

## Experimentation Result
For more details about this project, please refer to the pdf [Poster.pdf](Poster.pdf).
