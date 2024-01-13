# Face Expression Recognition Project - Facex_1

## Overview

This project delves into Data Science and Machine Learning, focusing on the potential of machine learning in classifying human emotions from facial expressions. While modest in scale, the project extensively explores various models, illuminating the nuances of emotion recognition technology.

// note - This project is first stand-alone project of mine. Facex_1 version will be kept as the 'raw' footprint of its further (potential) evolution.

## Dataset
https://www.kaggle.com/datasets/msambare/fer2013 \
https://www.kaggle.com/datasets/prilia/fer2013plus-cleaned-augm-balanced \
https://www.kaggle.com/datasets/shawon10/ckplus


### FER 2013 Dataset

The project is centered around the Facial Expression Recognition 2013 (FER 2013) dataset, a key resource in computer vision and emotion AI. This dataset contains 35,887 grayscale images, labeled with seven different emotions, offering a robust base for model training. 

### Additional Datasets

In addition to FER 2013, the project utilizes other datasets to evaluate and test the robustness of the models. This approach is aimed at understanding the models' generalizability and performance in diverse scenarios.

## Addressing Challenges

The project tackles inherent challenges in the FER 2013 dataset, such as class imbalance and noisy data. This involves applying the models to various datasets for a comprehensive understanding of emotion recognition complexities.

## Project Goals

The primary objective of the project is to create models for emotion classification. The focus is on gaining a deeper understanding of the factors influencing the performance, rather than achieving perfect accuracy. Key areas of exploration include:

- **Neural Network Capabilities:** Exploring the strengths and limitations of neural networks in emotion classification.
- **Model Performance Analysis:** Analyzing the performance of different models in classifying specific emotions versus their versatility in broader emotion recognition.

## Academic Relevance

While not a primary goal, the project's use of the FER 2013 dataset and the developed models have indirect relevance in academic research, contributing insights to the field of emotion AI.

// note - This project and its further stages will be later used in master thesis.

## Conclusion

This project is a comprehensive exploration into neural networks for emotion recognition, focusing on understanding the factors influencing model performance. It aims to provide significant insights into emotion AI, going beyond mere accuracy metrics.

# Final Model Comparison

## Custom CNN Model Performance

- **Strengths**:
  - Exhibited balanced performance across most classes.
  - Notable proficiency in recognizing 'happy' (83% precision) and 'surprise' (75% precision).

- **Weaknesses**:
  - Struggled with 'disgust' and 'fear', potentially due to their similarity to other expressions and ambiguous labeling in the dataset.

- **Overall**:
  - Achieved an accuracy of 60%, more effective in clear-cut expressions like 'happy', less so in nuanced expressions.

## EfficientNetB0 Model Performance

- **Issue**:
  - The model did not train correctly, only able to classify 'happy'. Possible misalignment with dataset specifics or training parameters.

- **Result**:
  - Due to skewed performance, EfficientNetB0 is excluded from the final comparison.

## VGG Model Performance

- **Strengths**:
  - Performed well in identifying 'happy' (80% precision) and 'surprise' (73% precision).
  - Showed a good ability to distinguish 'neutral' expressions.

- **Weaknesses**:
  - Less effective in distinguishing 'sad' from other similar expressions, impacted by label ambiguities.

- **Overall**:
  - With an overall accuracy of 64%, the VGG model showed balanced performance but faced challenges in subtle or ambiguous categories.

## Final Comparison between Custom CNN and VGG Models

- The **Custom CNN Model** displayed strong recognition of distinct expressions like 'happy' and 'surprise', but faced difficulties in differentiating similar emotions like 'sad' versus 'neutral'.
- The **VGG Model** showed slightly higher overall accuracy and balance, particularly adept at identifying 'happy', 'surprise', and 'neutral' emotions.
- Both models demonstrate the complexity in facial expression recognition, particularly with subtle differences and ambiguous labels in datasets like FER2013. **Despite these challenges, VGG slightly outperforms the Custom CNN in overall accuracy and balance.**
This format uses bullet points, bold text for emphasis, and headings to clearly separate 

VGG Training Graphs + Confusion Matrix + Model Predict on Testset(shuffled, to ensure all labels are predicted visually)
![__results___28_5](https://github.com/lukeanddata/facex_1/assets/101431694/fcc5b823-43ae-440d-b60e-723033b7c557)
![__results___30_5](https://github.com/lukeanddata/facex_1/assets/101431694/829023e9-9a41-4210-848a-23d6570a08f5)
![__results___52_1](https://github.com/lukeanddata/facex_1/assets/101431694/510b2c20-a719-4cef-bea7-1f8039df999b)




