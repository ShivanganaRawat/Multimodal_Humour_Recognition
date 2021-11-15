# Multimodal Humour Recognition
This repository is maintained by [Shivangana Rawat](https://www.linkedin.com/in/shivangana-rawat-b12254124/) and [Pranoy Panda](https://sites.google.com/view/pranoy-panda/). This project is done as part of a course project at IITH. **The code will be released by the first week of December after the semester gets over**.

**Aim**: This project deals with using three modalities, Audio, Video and Text, for recognising a humorous scene. Specifically, we are focusing on the [M2H2 dataset](https://arxiv.org/abs/2108.01260) which has multimodal data for conversations happening in a Hindi comedy television show named "Shrimaan Shrimati Phir Se". Each utterance in the conversation between the speakers, across 13 episodes, is labelled as "humorous" or "not-humorous".   

**Work Done**: We have tried unimodal and multimodal features to capture the individual modality representations. The following flow chart shows the methods explored thus far:

<img src="/images/Flowchart.png" alt="flowchart" width="700"/>

The results we have got with our multimodal representation(without any strategic fusion of modality representation) is as follows:

<img src="/images/results.png" alt="results" width="500" >

Please note that we have unbalanced classes(65:35 ratio) in our dataset, and both classes are equally important. So, in our task F1 is the important metric. And, it can be seen above that the multimodal model performs the best w.r.t. F1 score.

**Ongoing work**:

1. Including sequential modelling into our methodology: </br>
(a) LSTM </br>
(b) Attention mechanism </br>

2. Exploring modality fusion techniques such as MISA(Modality-Invariant and-Specific Representations for Multimodal Sentiment Analysis, AAAI 2020) for exploiting relationship between different modalities for better humor recognition.
