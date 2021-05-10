# Leaf-Classifier

```diff
! CODE UPDATED FOR MATLAB v2021b

```
## Introduction
Disease detection in the field of agriculture is an important field of study
in India. We find that 17.6% of the GDP is
accounted for by Agriculture, Forestry and fishing. As such it becomes
an important field to study since classifying diseased leafs using image
analytics makes it significantly cheaper to treat.

To do this, a four step approach is applied, beginning with the acquisition of
the image to its segmentation, feature extractions as well as classification
which is the end result of the project.
## Methodology
The approach to solve the problem is systematic, image segmentation is done
with K-means clustering method and features are computed from disease
affected cluster. The features that are extracted are fed to the ANN (Artificial
Neural network) are essentially the Contrast, Correlation, Energy, Homogeneity,
Mean, Standard Deviation and Variance. To classify the images, a support
vector machine classifier was used.
A color transformation was used to convert the leaves into HSV type format.
The acquired images are processed into the program and are
segmented using Kmeans, segmentation is the process of dividing the images
into different parts, in essence clusters and is done using clustering
algorithms, For Image processing and its clustering the Kmeans algorithm is
used. Kmeans clustering identifies according to the number of clusters, the
different clusters, each of these clusters have similar characteristics that is
each cluster has parts of the image. This essentially means that one of the
cluster would contain the diseased part of the leaf. We can further train the
program to run with a command that asks what cluster to use to classify the
disease and identify it.

## Feature Extraction
Feature extraction is the process of extracting essential statistical values and
numerics that are associated with the image.
Once the cluster is entered, the image is converted into gray scale and gray
level co-occurrence matrices are created. The program uses the said matrices
to extract features.
The derived features, Contrast, Correlation, Energy, Homogeneity, Mean,
Standard Deviation and variance, are given as an input to the classifier.
## Classification
Any classifier works on a Machine learning mode. In this case, a Neural
Network was applied. The Extracted features are fed into the neural network
that learns from the data and uses it to classify further inputs. It provides with
the performance plot, Confusion matrix, error and histogram plot after the
training of the network. Figure 3 contains a diagram of the neural network that
is used, it is a basic push pull neural network.

## Conclusion

Leaf disease detection is done using neural network classifier. The
segmentation is done using k-means clustering. Various features like Contrast,
Correlation, Energy, Homogeneity, Mean, Standard Deviation and Variance are
extracted for cotton and tomato diseases. The diseased leaves considered for
simulation are bacterial leaf spot, target spot septoria leaf spot and leaf mold
disease. Features are computed from disease affected clusters 1 and 3. The
features are fed to the classifier for recognising and classifying the diseases.
Out of twenty cotton samples nine samples are classified correctly as bacterial
leaf spot and one sample is misclassified as target spot. Eight samples are
classified as target spot and two samples are misclassified as bacterial leaf
spot. Out of twenty tomato samples 10 samples are classified as septoria leaf
spot disease and 10 samples are classified as leaf mold disease. Accuracies
for four diseases bacterial leaf spot, target spot septoria leaf spot and leaf
mold are 90%, 80% and 100% respectively and its average classification
accuracy is 100%.
