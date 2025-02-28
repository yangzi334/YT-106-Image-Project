This paper is called: Comparative Analysis of CNN and Vision transformer Models for Small Image Classification.
The goal of this research is to explore the effectiveness of different deep learning models in distinguishing visually similar images. In this paper, the author use ‘muffin and chihuahua’ dataset from an open-source repository to train and compare multiple CNN (Convolutional Neural Network) models and a Vit (Vision Transformer) model.
In this paper, CNN models include an initialized ‘the original CNN model from scratch’, a ‘CNN model from scratch with hyperparameter adjustments’, a ‘fine-tuned CNN’ model’, and a ‘fine-tuned Vision Transformer’ model. And data augmentation is applied during training using real-time transformations to increase image variability.
Model performance is assessed using confusion matrix, precision, recall, and F1-score. This paper includes five sections: including original dataset introduction, preprocessing dataset, CNN models and Vit model building and training, CNN models and Vit model evaluation and precision, Models comparison. 
For the section 1: it introduces the raw data muffin and chihuahua, there are 5917 images totally, including 4733 training images, and 1184 testing images.


![image](https://github.com/user-attachments/assets/adc71038-7912-41bb-8437-c8454e57597b)

For section 2: it describes how to preprocess the dataset with augmentation transformation method to adjust the images. For all details, please read the python code file: ‘Final_project preprocessing’ Jupiter notebook.

Before using augmentation transformation: 

![image](https://github.com/user-attachments/assets/706e1b8c-3871-4de5-a572-ea77e7fce558)

After using augmentation transformation:

![image](https://github.com/user-attachments/assets/b7b370eb-e6cd-4ced-80ba-4e23a03e39e8)

The 32 images after augmentation in a mark grid: 

![image](https://github.com/user-attachments/assets/ef5bee97-5073-4c6d-9dbd-bef43ab30c91)

For the section 3: 
In this section, we build three CNN models including the initial CNN from scratch, CNN from scratch with hyperparameter adjustment, CNN fine-tuned model, and a Vit transformer fine-tuned model. 
For the section 3, please read all details in the python code file: Final_CNN model and training.ipynb and Final_Vit model and training.ipynb Jupyter notebook. 
We design CNN model with two layers, after design CNN model architecture, then we define the loss and optimizer functions, Then we start to design the training process. 
The CNN model from scratch architecture

![image](https://github.com/user-attachments/assets/5d526947-c9c7-42bb-b95d-e1e712408a67)

After the training process, we plot two figures including the loss at the end of each epoch for training data and validation data: for all the detailed analysis, please read the final paper and the python code . 

3.1: the original CNN model from scratch 

![image](https://github.com/user-attachments/assets/a48e08f5-4936-48f8-9d2a-7aa9410ff5c9)

![image](https://github.com/user-attachments/assets/9ddbcee3-5e9d-48e3-997f-18bdf0c85897)

3.2: the CNN model from scratch with hyperparameter adjustment 

![image](https://github.com/user-attachments/assets/a0202a11-8c81-4aa2-98c5-dbeaeed1cd87)

![image](https://github.com/user-attachments/assets/b2f6e875-abbc-49d9-be5e-249c19643b36)

3.3: CNN fine-tuned model, for the predefined model, we use mobileNetV2 model. 

![image](https://github.com/user-attachments/assets/5b94b84a-94f5-4ee2-ba14-df858e9f495f)

![image](https://github.com/user-attachments/assets/52d1164f-f60a-4138-a392-99cc7814e6d1)

3.4: Vision transformer (Vit) fine-tuned model, we use Vit-B/16 transformer model. 

![image](https://github.com/user-attachments/assets/90f973f0-0529-4791-88c8-e2b1f6315503)

![image](https://github.com/user-attachments/assets/6dba26c7-a5e8-4ee0-a9eb-b064225e345d)

Section 4: CNN models and Vit model evaluation and precision, please read all details and analysis in the final paper and “Final_CNN evaluation and prediction.ipynb” and “Final_Vit evaluation and prediction.ipynb”.
confusion matrix, precision, recall, and F1-score shown below for each model:
4.1: original CNN model from the scratch

![image](https://github.com/user-attachments/assets/cb4ee23b-1f22-48ac-948c-2dd8b0b7ce45)

4.2: the CNN model with hyperparameter adjustment from the scratch

![image](https://github.com/user-attachments/assets/8e18171a-a951-4b1b-9dd4-8f6161915fab)

4.3: the CNN fine-tuned model 

![image](https://github.com/user-attachments/assets/d493a99d-3348-4c89-8717-47444db4f711)

4.4: the Vision transformer fine-tuned model (note: since the Vit fine-tuned model is too big to upload in the github, so please run the code yourself and you will see all those updated parameters)

![image](https://github.com/user-attachments/assets/a8915d56-417d-46be-ae9c-32061c6e20cc)

Section 5:  Models comparison 
In this section, we will compare the models with two ways, including comparing within CNN models and comparing between CNN fine-tuned and Vision transformer fine-tuned models. 
Comparison within CNN models: from section 4, we can see CNN fine-tuned model has a dramatic improvement in performance. 
Comparison between Fine-tuned CNN and fine-tuned Vit models: Vit outperforms the fined-tuned CNN with marginally better precision and recall, indicating it generalizes better and makes fewer classification error. 


















