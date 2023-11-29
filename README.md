<h1>Pet Facial Expression Classification with Vision Transformer</h1>

<h3>Introduction</h3>

In this project, we focus on the task of identifying animal facial expressions through the analysis of animal facial images. Utilizing a dual approach, we have developed both a manually crafted Vision Transformer (ViT) and employed a pretrained Vision Transformer model. This innovative methodology is designed to decipher the nuanced expressions found in various animal species, leveraging the advanced capabilities of Vision Transformers. ViTs, known for their effectiveness in understanding global image contexts, are particularly suited for this task. By comparing and contrasting the performance of a manually tailored model against a pretrained alternative, we aim to explore the intricacies of animal facial expressions, a relatively uncharted territory in the realm of machine learning and computer vision. This project not only pushes the boundaries of existing image recognition technologies but also opens new avenues for understanding animal behavior and communication.

<h3>Data</h3>
https://www.kaggle.com/datasets/anshtanwar/pets-facial-expression-dataset
This dataset contains 1000 face images of various pets, such as dogs, cats, rabbits, hamsters, sheep, horses, and birds. The images capture the diversity of expressions these animals can display, such as happiness, sadness, anger etc.
It contains over 200 images for each class: Angry, Sad, Happy, and Other, with augments.

<h3>Data Flow in the Vision Transformer Architecture</h3>
<img width="430" alt="Screen Shot 2023-11-29 at 11 46 10 AM" src="https://github.com/mandali8686/pet-facial/assets/100242191/8ee5321e-55f8-4363-9a5a-071af22c6013">


<img width="552" alt="Screen Shot 2023-11-29 at 10 11 26 AM" src="https://github.com/mandali8686/pet-facial/assets/100242191/7b53c5f9-5184-4e52-94e4-8d4bb7268933">
<h3>Colab Code</h3>
https://colab.research.google.com/drive/11KmsZ15QM9kDKn0g8iGO-kgoOD2l5mVv#scrollTo=sz_RJvAXP5hi
https://colab.research.google.com/drive/1zYN-LvMGxgr6sXv3EMEUCAzDKUmJwnz_#scrollTo=PZF1kjW1WeLu

<h3>Code Demonstration</h3>
<href>https://huggingface.co/mandali8686/pet-expression/tree/main</href>

<h3>Result Comparison</h3>

<h4>Manual Vision Tranformer</h4>
<img width="719" alt="Screen Shot 2023-11-29 at 10 18 18 AM" src="https://github.com/mandali8686/pet-facial/assets/100242191/73a04dc9-5218-4722-8584-db34b9a0056d">
<img width="771" alt="Screen Shot 2023-11-29 at 11 05 15 AM" src="https://github.com/mandali8686/pet-facial/assets/100242191/3a3a3bf2-6d82-4af6-820f-0cf05bcbd7f6">


<h4>Pretrained Vision Transformer</h4>
<img width="717" alt="Screen Shot 2023-11-29 at 10 19 42 AM" src="https://github.com/mandali8686/pet-facial/assets/100242191/69fdc493-4674-435c-96cb-61ba3e419cd1">
<img width="763" alt="Screen Shot 2023-11-29 at 11 04 49 AM" src="https://github.com/mandali8686/pet-facial/assets/100242191/39e8d44b-68a5-4540-8fee-7e5a3ecc884f">


<h3>Prediction Comparison</h3>
<h4>Prediction with manual Vision Transformer</h4>
<img width="419" alt="Screen Shot 2023-11-29 at 10 50 28 AM" src="https://github.com/mandali8686/pet-facial/assets/100242191/e4eae3e2-d8f9-41f3-bfeb-a7fb85ea306f">

<h4>Prediction with pretrained Vision Transformer</h4>

<img width="403" alt="Screen Shot 2023-11-29 at 10 51 48 AM" src="https://github.com/mandali8686/pet-facial/assets/100242191/60b6e8cb-3cea-4bdd-89c9-36416b8b0317">

<h3>Limitation and Critical Analysis</h3>
Upon close examination of our project employing a fine-tuned Vision Transformer, it becomes evident that the model may encounter issues with generalization, as indicated by a significantly higher test loss compared to the training loss. This disparity suggests that while the model performs well on familiar data, its ability to adapt to new, unseen data is limited. Additionally, the training dataset, albeit augmented, is relatively small, which could contribute to the model's constrained learning capacity. This limitation is particularly relevant considering the diversity of animals in the study. Each species exhibits unique facial expressions, adding layers of complexity to the task. The challenge is thus twofold: not only must the model learn to accurately interpret facial expressions, but it must also do so across a spectrum of different animal species, each with its own set of distinctive features and nuances. This complexity underscores the need for a more robust training regime and possibly a more diverse dataset to enhance the model's ability to generalize and accurately recognize a wider array of animal facial expressions.
<h3>Future Direction</h3>

A pivotal step in advancing our project on pet expression recognition involves expanding the dataset to encompass a broader and more diverse range of animal images. A larger dataset will not only enhance the model's ability to generalize across different breeds and species but also facilitate a more comprehensive understanding of nuanced pet expressions. 

Additionally, diversifying the range of emotion categories recognized by the model stands as a crucial objective. Currently, the model may be limited to identifying a handful of basic emotions. By incorporating a wider array of emotion categories, we can significantly enrich the model's interpretive capacity, enabling it to detect and differentiate between more subtle and complex emotional states in pets. This expansion is not merely quantitative but qualitative, as it will empower the model to provide deeper, more insightful analyses of pet behavior and welfare, ultimately leading to a more empathetic and informed interaction between pets and their human companions.

<h3>Reference</h3>

Pytorch Vision Transformer: https://pytorch.org/vision/main/models/vision_transformer.html
Pet Facial Dataset: https://www.kaggle.com/datasets/anshtanwar/pets-facial-expression-dataset
HuggingFace Model: https://huggingface.co/mandali8686/pet-expression
