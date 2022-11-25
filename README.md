# CVNN_AmbulanceFacilityToolTrafficLights
The repository is aiming at finding a way to help Ambulances during trajectories over tights roads commanded by traffic lights

GENERAL INFORMATIONS:

AUDIO DATASET SOURCE LINK: https://www.kaggle.com/datasets/tabarkarajab/ambulance-dataset


Workspace organization:

    The workspace is divided in 2 Macro folders:

        -- CVNN_AmbulanceFacilityToolTrafficLights
        -- Dataset
    
    The first one is the folder containing all the code to be executed (which is also a git repository to be uploaded). The second one is the dataset containing the datasets (for both, audio and video). The orgininal dataset is then split into train/test/validation sets. These one are then preprocessed by data-augmenting the original dataset. The augmented dataset is then saved in another folder.


When performing an experiment, the code responsible to launch the training/inference face are:

    -- TRAIN: *NOME DA DECIDERE*
    -- TEST: *NOME DA DECIDERE*

These files are launched by terminal with a parser whose responsible to provide a configuration file in .yaml format.

The .yaml file contains informations about the dataset adopted for the training (also val and test phases) and also the target folders for the parameters of the models. The .yaml file also is responsible to choose the preloaded network. We talk about preloaded networks since we download form pytorch some of the most famous networks available on the marker (f.i. ResNet_X -- MobileNetV2/V3 -- ...)