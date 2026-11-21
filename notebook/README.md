# Notebook

Download the datasets
https://drive.google.com/drive/folders/1hPuhiOkjPaorl-10XZH2yxdbd9gcR_NO?usp=drive_link 
Rename the folder to "data" and put in this folder

and run the pipeline expected output
First Cell
== roboflow_quality ==
train {'Clear': 25, 'Foam': 354, 'Highly_Turbid': 90, 'Medium_Turbid': 148, 'Unlabeled': 8}
valid {'Clear': 4, 'Foam': 88, 'Highly_Turbid': 27, 'Medium_Turbid': 40, 'Unlabeled': 2}
test {'Clear': 1, 'Foam': 263, 'Highly_Turbid': 17, 'Medium_Turbid': 96, 'Unlabeled': 1}

== roboflow_turbidity ==
train: ../train/images
val: ../valid/images
test: ../test/images

nc: 2
names: ['clean', 'turbid']

roboflow:
  workspace: dataregenerator
  project: turbidity
  version: 4
  license: CC BY 4.0
  url: https://universe.roboflow.com/dataregenerator/turbidity/dataset/4
boxes per class id: {'1': 2194, '0': 374}

== mendeley_polluted ==
clean 300
images 1236
masks 1236

Second Cell
train {'Clean': 593, 'Cloudy': 2124, 'Foam': 354, 'Polluted': 984}
valid {'Clean': 111, 'Cloudy': 485, 'Foam': 351, 'Polluted': 252}