570 Final Project - Parth R. Doshi

Note: The implementation of the project is done on Google Collabotory, with a runtime type of A100 GPU. The following README includes details of how to run the experiments, what code was originally written by the student, what code was modified from which specific file and how the dataset was obtained.

The implementation is broken into two parts: a preliminary implementation, and an extended implementation.

a. PRELIMINARY EXPERIMENTS

The preliminary experiments are divided up into 3 parts. 

Experiment 1 : cells 2,3,4 should be executed. 
Experiment 2 : cells 2,3,5,6,7 must be executed.
Experiment 3 : cells 2,3,8,9,10 must be executed.

b. EXTENDED IMPLEMENTATION 

To run the extended implementation follow the sequence of steps below.

    1. To load the datasets and initialise the helper functions used run cell 11. This code has been modified from the existing tutorial for RT-1 dataset acquisition found on the link below.

    2. To choose the dataset path in the dropdowm on the right run cell 12.

    3. Run cell 13 to obtain results for the extended implementation. All this code has been written by the student after taking inspiration from the original code provided by Google's RT-1 researchers and InstructPix2Pix.

Additional Comments:

1. To customize inputs and change the image to edit, change the url in cell 13, to that of the desired image. This code is written by the student completely. 

2. To select your own input image uncomment cell 14 and rerun the model. This code has been written completely by the student.

3. The implementation of the training function is a modification of the train.yaml file of the InstructPix2Pix github repository (https://github.com/timothybrooks/instruct-pix2pix/blob/main/configs/train.yaml). It has been modified by cahnge the target and path (data: params: train: target:) parameter. 

4. More about the dataset used: The dataset is obtained from Google's Research website with the project titled RT-1 from the link below: 
https://console.cloud.google.com/storage/browser/gresearch/rt-1-data-release;tab=objects?pli=1&prefix=&forceOnObjectsSortingFiltering=false

The dataset consists of real-world robotic experiences that consists of over 130k episodes, which contain over 700 tasks, and was collected with a fleet of 13 robots over 17 months.

The current set of skills includes picking, placing, opening and closing drawers, getting items in and out drawers, placing elongated items up-right, knocking them over, pulling napkins and opening jars. The list of instructions was designed to show multiple skills with many objects to test aspects of RT-1 such as generalization to new instructions and ability to perform many skills. The entire process of adding tasks and data is described in detail in the paper for RT-1.

REFERENCES:

1. InstructPix2Pix Hugging Face Model: https://huggingface.co/spaces/timbrooks/instruct-pix2pix
2. IntructPix2Pix GitHub Link: https://github.com/timothybrooks/instruct-pix2pix
3. RT-1 GitHub Link: https://robotics-transformer1.github.io/



