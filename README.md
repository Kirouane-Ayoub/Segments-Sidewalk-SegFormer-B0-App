# Segments-Sidewalk-SegFormer-B0 App

## Model Details

+ **Model Name**: Segments-Sidewalk-SegFormer-B0
+ **Model Type**: Semantic Segmentation
+ **Base Model**: nvidia/segformer-b0-finetuned-ade-512-512
+ **Fine-Tuning Dataset**: Sidewalk-Semantic

## Model Description

The **Segments-Sidewalk-SegFormer-B0** model is a semantic segmentation model fine-tuned on the **sidewalk-semantic** dataset. It is based on the **SegFormer (b0-sized)** architecture and has been adapted for the task of segmenting sidewalk images into various classes, such as road surfaces, pedestrians, vehicles, and more.

## Model Architecture

The model architecture is based on SegFormer, which utilizes a **hierarchical Transformer Encoder and a lightweight all-MLP decoder head**. This architecture has been proven effective in semantic segmentation tasks, and fine-tuning the 'sidewalk-semantic' dataset allows it to learn to segment sidewalk images accurately.

## Intended Uses

The **Segments-Sidewalk-SegFormer-B0** model can be used for various applications in the context of sidewalk image analysis and understanding. 

**Some of the intended use cases include**

+ **Semantic Segmentation**: Use the model to perform pixel-level classification of sidewalk images, enabling the identification of different objects and features in the images, such as road surfaces, pedestrians, vehicles, and construction elements.
+ **Urban Planning**: The model can assist in urban planning tasks by providing detailed information about sidewalk infrastructure, and helping city planners make informed decisions.
+ **Autonomous Navigation**: Deploy the model in autonomous vehicles or robots to enhance their understanding of the sidewalk environment, aiding in safe navigation.

## App Description
The *Segments-Sidewalk-SegFormer-B0 App* is a user-friendly application built using the Gradio library that allows users to perform semantic segmentation on sidewalk images using the **Segments-Sidewalk-SegFormer-B0** model. With this app, users can upload sidewalk images, and the model will segment the images into various classes, providing a visual representation of objects and features present in the images.

## App Interface

+ **Input**: Users can upload sidewalk images through the app interface.
+ **Output**: The app displays the segmented image, highlighting different classes with distinct colors.

## Limitations

+ **Resolution Dependency**: The model's performance may be sensitive to the resolution of the input images. Fine-tuning was performed at a specific resolution, so using significantly different resolutions may require additional adjustments.
+ **Hardware Requirements**: Inference with deep learning models can be computationally intensive, requiring access to GPUs or other specialized hardware for real-time or efficient processing.


## Ethical Considerations

When using and deploying the **Segments-Sidewalk-SegFormer-B0** model, consider the following ethical considerations:

+ **Bias and Fairness**: Carefully evaluate the dataset for biases that may be present and address them to avoid unfair or discriminatory outcomes in predictions, especially when dealing with human-related classes (e.g., pedestrians).
+ **Privacy**: Be mindful of privacy concerns when processing sidewalk images, as they may contain personally identifiable information or capture private locations. Appropriate data anonymization and consent mechanisms should be in place.
+ **Transparency**: Clearly communicate the model's capabilities and limitations to end-users and stakeholders, ensuring they understand the model's potential errors and uncertainties.
+ **Regulatory Compliance**: Adhere to local and national regulations regarding the collection and processing of sidewalk images, especially if the data involves public spaces or private property.
+ **Accessibility**: Ensure that the model's outputs and applications are accessible to individuals with disabilities and do not exclude any user group.

## Usage 
```
pip install -r requirements.txt
python app.py 
```
![Screenshot at 2023-09-24 17-54-34](https://github.com/Kirouane-Ayoub/Segments-Sidewalk-SegFormer-B0-App/assets/99510125/8514158f-7fd2-45ae-b78f-a3d02368e49e)
