# WIR-Earthquake-Shakes-Twitter-Users-Event-Detection-by-Social-Sensors

Inspired by the [paper](https://dl.acm.org/citation.cfm?doid=1772690.1772777), we designed a tweet-based earthquake detection system applying some modifications and simplification. 

After having prepared the training data through some preprocessing technique and having selected the types of features to extract from tweets we devised a binary classifier using Support Vector Machine (SVM) - as the authors suggested - and, in addition, we also used K-Nearest Neighbors (kNN) in order to make some interesting comparisons.

Subsequently, the trained classifier has been used for designing the spatio-temporal model. At this point, we made some simplifications with respect to the assigned paper. For the temporal model we implemented a burst detection technique which uses the posting time of each crisis-related tweet to obtain an approximation of the correct strike time of an earthquake. For the spatial model, instead, we exploited geo-tagged crisisrelated tweets in order to determine approximately the epicenter of an earthquake through latitude and longitude information, when available.

Since the authors of the paper did not share any dataset, we have decided to use the well-known [CrisisNLP](https://crisisnlp.qcri.org/lrec2016/lrec2016.html) dataset.

For more information take a look at the pdf file *paper_journal.pdf*.
