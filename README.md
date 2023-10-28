# Hacktonauts(Team 6)-Synthetic-DataGeneration-Challenge

Data is an indispensable resource with several varied applications across diverse sectors and industries. Its significance stems from its role in furnishing raw information and knowledge, thereby underpinning the foundations of informed decision-making and problem-solving. Whether in business operations, government policies, or personal contexts, data serves as the basis for evaluating options and devising strategies to address challenges and seize opportunities. It facilitates performance measurement, research, and analysis, making it indispensable for scientific investigations and market studies.


The task at hand is to develop a sophisticated algorithm capable of generating photorealistic images that represent the intricacies of urban driving scenes in India. These images should encapsulate the true-to-life complexities that drivers encounter on Indian roads, consisting of elements such as traffic congestion, unexpected road occurrences, and varying weather conditions. Our objective is to craft an algorithm that not only reproduces these aspects but also incorporates inherent control mechanisms, offering the ability to manipulate and fine-tune any or all of the mentioned factors while ensuring the photorealism of the output. In the pursuit of this goal, the resulting deliverable is anticipated to be a comprehensive dataset. Each image will be a meticulously crafted representation of an Indian driving scenario, taking into account the multitude of variables that define the ever-evolving and dynamic nature of road scenes in the Indian urban landscape. This undertaking represents a significant step towards generating synthetic data that closely mirrors the realities of driving on Indian roads, with a focus on realism, diversity, and contextual relevance.


# Dataset

The "Indian Roads Images Dataset and Model Repository",  facilitates a range of applications such as road condition analysis and more. The dataset and models in this project are designed to be accessible for public use and further development.
The dataset contains a diverse selection of Indian road images, suitable for a wide array of applications. These images serve as a valuable resource for tasks related to road analysis and more. The images consist of various changing parameters such as differing weather conditions, the condition of the road, the people and vehicles they occupy and so on. 


# Pre-trained Model

The pre-trained model weights are available for public use, enabling the generation of images with custom prompts. These prompts can include various parameters, such as density, time of day, and weather conditions, to control the image generation process. The base of the model proposed for the use of this algorithm is the stabilityai/stable-diffusion-2, as it is stable, and available to work with on Kaggle. However, due to memory and computational constraints, the primary exection of the V1 and V2 of this algorithm have been done using CompVis/stable-diffusion-v1-4.

# Image Refinement

In addition to model testing, an image refinement process is provided. This refiner, based on SDXL base 1.0, allows users to further enhance the generated images by applying additional prompts and adjustments to meet specific requirements. The refiner takes in the current image, and uses the control mechanisms to improve the initial image.

# Running the Project

To test the pre-trained model with custom prompts, follow these steps:

1. Clone or fork this repository to your local machine.
2. Install the necessary dependencies and libraries required to run the model.
3. Utilize the model by running the provided scripts and specifying your custom prompts.

Requirements

To run the project, ensure you have the following dependencies installed:

1. DiffusionPipeline from diffusers
2. torch
3. CUDA
4. Numpy
5. JSON
6. Image from PIL
7. libjpeg-dev (apt-get or Chocolatey install)
8. torchvision
9. clip-retrieval
10. transformers
12. matplotlib

Experiment with different prompts and settings to generate images that align with your specific needs.

# Contributors

 Nishtha Jain
 Diksha Chakravarty
 Aakash Rajaraman
 A. Ananya

This project is a valuable resource for the research community and those interested in working with Indian road images and image generation models.

The trained weights for the custom dataset trained on the Stable Diffusion pipeline are available to test at: https://huggingface.co/aakashrajaraman/output. This is the version 1.0, trained on just a small sample of data, and an abstract instance and class prompt set. 

For the future scope, the pipeline will use a latest version of Stable Diffusion, and additional hyperparameter tuning.
