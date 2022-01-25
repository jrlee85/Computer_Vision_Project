# Computer_Vision_Project

**Using deep learning to classify animals at the family level in camera trap images**

I produced this work for the Final Project of my Data Science MSc.

ABSTRACT

Camera traps are a vital source of information for ecologists, biologists and conservationists. They can capture millions of images of animals in their natural habitat without human intervention. However, analysing the images produced by camera traps is a time-consuming operation. Recently, a number of studies have attempted to perform automated image analysis using convolutional neural networks. While results have been positive (up to 97% accuracy in image classification in some cases), there remains a problem of generalisation. Models perform well when faced with images produced by camera traps that they have previously been trained on. However, performance suffers once the models attempt to classify images from new locations. This is a result of overfitting. 

To attempt to address this issue, this study has developed a sequence of classifiers. The first classifies animals by their family/subfamily taxonomic level, rather than by their species. This allows the classifier to be exposed to a wider range of locations during training, with the aim of reducing overfitting. The next classifier is then designed to classify only animals from a certain subfamily/family. This classifier returns the species of the animal. Three of these species-level classifiers were developed for this project, classifying images from the families Canidae, Felinae and Sciuridae. Alongside these models, one benchmark model was also developed, designed to take images from all families and return the species label.

While the species-level models showed improved results when compared directly against the benchmark model (91%, 88% and 91% accuracy for Canidae, Felinae and Sciuridae respectively, versus 74% accuracy for the benchmark model), when the extra step of first classifying the images by family was taken into account, the results were actually worse than the benchmark results (a 77% accuracy for the family-level model effectively reduced the species-level accuracies to just 70%, 68% and 70% respectively). 
Furthermore, the out-of-sample results were mixed, with 66% and 53% accuracy for the Canidae models, but just 1% accuracy for the Sciuridae model. 
These results suggest that the approach of developing family-specific classifiers does not help with the issue of generalisability, although the study does acknowledge that the results obtained were somewhat limited by the computational power available, and that future work may be able to improve upon these results. 
