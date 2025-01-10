---
title: "Poodle"
fulltitle: "Projecting Observations On a Deep Learned Embedding"
excerpt: 'Pipeline for the projection of new samples onto a shared product space'
imgname: Poodle_img.jpg
author: 'TD Maarseveen'
githuburl: 'https://github.com/levrex/Poodle'
collection: tools
permalink: /tools/Poodle
---

Poodle
<b><u>Projecting</u></b> <b><u>Observations</u></b> <b><u>On</u></b> a <b><u>Deep</u></b> <b><u>Learned</u></b> <b><u>Embedding</u></b>

Clustering techniques that use deep learned embeddings often outperform conventional clustering techniques such as k-means [1]. However, when it comes to projecting new samples onto the learned embedding there is a lack of guidelines & tools. We built POODLE to facilitate the projection of new samples onto this product space. Samples are clustered one-by-one according to their orientation in the latent space.

Deep learning technique
We used the autoencoder architecture of MAUI as an example. However, one could also adopt a different deep learning architecture or even a factor analysis technique (like MOFA). Currently, this github repo does not provide examples for other techniques.

Robust to difference in dimensionality
Poodle is flexible for situations where certain data is absent in the clinic, as one may build a shared product space and only project patients on the variables present in both sets. However, ensure that the key features are still included. The more you diverge from the initial set of features, the more you'll loose the cluster essence.