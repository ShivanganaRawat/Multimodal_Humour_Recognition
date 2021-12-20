# Multimodal Multiparty Humour Recognition
This repository is maintained by [Shivangana Rawat](https://www.linkedin.com/in/shivangana-rawat-b12254124/) and [Pranoy Panda](https://sites.google.com/view/pranoy-panda/). This project is done as part of a course project at IITH. 

**Aim**: This project deals with using three modalities, Audio, Video and Text, for recognising a humorous scene. Specifically, we are focusing on the [M2H2 dataset](https://arxiv.org/abs/2108.01260) which has multimodal data for conversations happening in a Hindi comedy television show named "Shrimaan Shrimati Phir Se". Each utterance in the conversation between the speakers, across 13 episodes, is labelled as "humorous" or "not-humorous".   

**Work Done**: We have tried unimodal and multimodal features to capture the individual modality representations. The following flow chart shows the methods explored thus far:

<img src="/images/flowchart.png" alt="flowchart" width="700"/>

The results we have got with our multimodal representation(with and without strategic fusion of modality representation) is as follows:

<img src="/images/result.png" alt="results" width="500" >

Please note that we have unbalanced classes(65:35 ratio) in our dataset, and both classes are equally important. So, in our task F1 is the important metric. And, it can be seen above that the multimodal model performs the best w.r.t. F1 score.

**Information about the code**
1. The folder ```/feature_representations``` contains notebooks which we used for extracting features from text, audio and video
2. The folder ```humor_recognition_models``` contains our three final models that 

    (a) Simple concatenation of feature representations of each modality: ```/humor_recognition_models/Multimodal_Humour_Recognition(simple_concatenation).ipynb```
    
    (b) MISA for humor recognition based on utterance only: ```/humor_recognition_models/MISA_for_humor_recognition(Utterance_based)```
    
    (c) MISA with sequence modelling: ```/humor_recognition_models/Sequence_modeling_with_MISA```
