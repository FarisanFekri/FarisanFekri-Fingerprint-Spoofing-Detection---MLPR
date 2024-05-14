# Objective

The **goal** of the project is the development of a classifier to detect whether a fingerprint image represents an authentic fingerprint or a spoofed fingerprint. This will be done exploiting the most common Machine Learning tools. We will discuss how they perform for the problem we have chosen, explaining pros and cons.

## Overview of the problem

The **dataset** consists of embeddings extracted from fingerprint images. Each row corresponds to a different embedding and contains 10 features followed by the label (1 for authentic fingerprint, 0 for spoofed fingerprint). The features do not have any particular interpretation. The spoofed fingerprints are generated using one of 6 different spoofing approaches, but that information is not available. The training set consists of 2325 samples, 800 are authentic fingerprints and the remaining 1525 are spoofed. We can thus note that the dataset is imbalanced. The target application considers an application where prior probabilities of authentic and spoofed classes are the same, but labeling a spoofed fingerprint as authentic has a larger cost due to the security vulnerabilities that such errors would create.

