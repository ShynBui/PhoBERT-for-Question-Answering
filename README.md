# Table of Contents

1. [How to Install and Run the Project](#How-to-Install-and-Run-the-Project)
2. [System requirements] ()
3. [Data for train]()
4. [How to Use the Project](#How-to-Use-the-Project)
5. [Data for test](#Data-for-test)
    - [Data 1](#Data-1)
    - [Data 2](#Data-2)
6. [File structure](#File-structure)
7. [Dependencies, basic commands and libraries)](#Dependencies,-basic-commands-and-libraries)
8. [Contribute](#Contribute)

   
# PhoBERT-for-Question-Answering
The project is a deep learning model based on PhoBERT architecture to find the answer to a Reading comprehension problem with Question answering task. The ultimate goal of this work is to create a solution that helps solve problems to answer Vietnamese Reading comprehension problems without any reasoning or knowledge. The model focuses on solving Reading comprehension questions of the easy and medium form (Factoid), suitable for students in grades six and seven. The model will help solve the self-explanatory question from a given text.

# How to Install and Run the Project
# Option 1: 
        Install Jupyter Notebook on your computer.
        Download the Demo.ipynb file from the GitHub repository.
        Open the Demo.ipynb file in Jupyter Notebook.
        Run command boxes to perform actions in files.
# Option 2:
        Open Google Colab.
        Download the Demo.ipynb file from the GitHub repository.
        Open the Demo.ipynb file in Google Colab.
        Run command boxes to perform actions in files.

# System requirements
## Training hyperparameters<br>
The following hyperparameters were used during training: <br>.
learning_rate: 2e-05 <br>.
train_batch_size: 8 <br>.
eval_batch_size: 8 <br>.
seed: 42 <br>.
optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08<br>.
lr_scheduler_type: linear <br>.
num_epochs: 3 <br>.

## Framework versions<br>
Transformers 4.34.1 <br>
Pytorch 2.1.0+cu118 <br>
Datasets 2.14.5 <br>
Tokenizers 0.14.1<br>

# Data for train
The data used in this project is SquAD (translate into Vietnamese) and self combine by OU-Teams
# Result
# How to Use the Project
While you open the interface with gradio (When you run all command boxes).<br>
You will have six tables to enter data. Respectively: 
+ Context (A given passage to model reading comprehension)
+ Question (Question regarding given data)
+ Four answers (A, B, C, D)<br>
After filling in those six tables, please click the submit button below.
The model will give you the correct answer in the "output" box.

# Data for test
## Data 1
**Context:** <br>The same " xx " system is used for other parts of the testing sites in NV. The Original Rectangular Base from 6 to 10 miles is now part of the so-called " room ", which is the rectangular base from 23 to 25.3 miles of prohibited air space. The area is connected to the nts indoor road network, and the road road leading south to mi and west to flat. The North-East of the lake leads to a well-maintained, well-maintained lake c road that runs through the Humboldt Hills. Previously it was leading to mines in the Jerome Basin, but it has improved since its closure. The Zigzag road passes through security checkpoints, but the prohibited area around the base extends more to the east. After exit from the prohibited area, lake c road descends east to the valley of the tikaboo valley, passing through the entrances to the dirt roads of several cattle farms, before they meet with main road 375, on the " off-Earth highway ", to the south of the Rachel. <br>
**Question:**<br> Where does the lake road lead to the lake?<br>
**Answer A:** <br>South East<br>
**Answer B:** <br>North and South East<br>
**Answer C:** <br>North with  South East<br>
**Answer D:** <br>North East<br>
**True answer: <br>D.North East**<br>

## Data 2
**Context:** <br>Lake C was used for artillery shelling and artillery training during world War II, but was then abandoned until April 1955, when it was selected by the team of the Luke as a perfect location to test the u-2 spy plane. The bottom of the lake provided the perfect tape that can do annoying aircraft tests, the height of the mountains of the valley of the grant valley and the ocean protects the test site from the eyes of prying and external intervention.<br>
**Question:** <br>What made the test bar for the plane?<br>
**Answer A:** <br>Moutant bottom<br>
**Answer B:** <br>Lake top<br>
**Answer C:** <br>Lake bottom<br>
**Answer D:** <br>Lake right<br>
**True answer:<br> C. Lake bottom**<br>

# File structure
QuestionAnswering_MultipleChoice_BERT/<br>
├── Demo.ipynb<br>
└── README.md

# Dependencies, basic commands and libraries
List of dependencies, basic commands and libraries required to run the .ipynb file.

- pipeline: Deploy the model
- SentenceTransformer: Encodes text sentences into numeric vectors of height
- cosine_similarity: Calculate the similarity between two texts
- gradio: Create interactive user interfaces for the model

# Contribute
If you want to contribute to our project, follow these steps:

- Fork the project.
- Create a new branch on your fork.
- Make your changes on the new branch.
- Create a pull request to merge your changes into the main repository.

# Author 
This project was created by ShynBui.
