# W-GAN for Celebrity Face Generation

## Overview
This project utilizes a Wasserstein Generative Adversarial Network (W-GAN) to generate high-quality, artificial face images. The model is trained on a large dataset of celebrity faces, allowing it to learn the complex distributions of facial features, expressions, and lighting. The key innovation of the W-GAN architecture is its use of the Earth Mover's (EM) distance, which provides a more stable training process compared to traditional GANs and helps to prevent mode collapse.

## Why W-GAN?
Generating realistic human faces is a challenging task due to the high-dimensional and varied nature of the data. Traditional GANs often struggle with training instability and can suffer from mode collapse, where the generator produces a limited range of outputs.

The W-GAN addresses these issues by:
- Improving Training Stability: The Wasserstein distance provides a smooth and continuous gradient, which makes training more predictable and reliable.
- Preventing Mode Collapse: The EM distance allows the generator to better explore the entire diversity of the training dataset, resulting in a wider variety of high-quality generated images.

I have added well enough comments and introduction in the .ipynb file itself so that the workflow is quite easy to Grasp. Below are my screenshots of outputs and the Graph of my GAN-Model.
- Plotted out the Faces from the dataset and the generated images in a form of a graph. Look closely how the face changes after removal of noise during the training 

<img width="432" height="807" alt="Screenshot 2025-09-19 at 3 18 31 AM" src="https://github.com/user-attachments/assets/ac0657a6-739b-44e3-b541-70fd744c7d87" />

Here is my Training Loop Graph Representation of the Project  
- Every Graph progress I have added the Generator Loss and Critic Loss
- The generated image gets more finer and detailed after a lot of epochs 
- the epochs batch has been divided earlier.
<img width="654" height="476" alt="Screenshot 2025-09-19 at 3 20 52 AM" src="https://github.com/user-attachments/assets/5d1f36de-8497-4c93-b54d-0216d9b9e6d1" />
