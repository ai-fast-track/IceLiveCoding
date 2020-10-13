# Live Coding on Tuesday 13th 2020

**When:** Tuesday October 13th 2020 at 2:00 p.m. (GMT-4)

**Where:** http://tinyurl.com/IceData

**Calendar:** http://tinyurl.com/ICE-BYOD-2



## Program

### Part 1: Dataset 1

- Indoor Objects dataset: http://tinyurl.com/ICE-Indoor-Objects
- Notebook : https://github.com/airctic/icedata/blob/master/notebooks/dev/indoor_objects.ipynb 

> **Goal:** This notebook shows how to create a new parser for a custom XML annotation file. The XML file contains all images annotation in one single file. In a sense, it is similar to the COCO annotation format where all the image annotation are stored in the same JSON file as opposed to VOC annotation where each file has its XML annotation file.

## Part 2: Dataset 2

- Plant diseases dataset: http://tinyurl.com/ICE-PlantDoc
- Notebook : https://github.com/airctic/icedata/blob/master/notebooks/dev/plantdoc.ipynb 

The PlantDoc Dataset provides both the VOC annoatation and a CSV annotation. 

> **Goal**: This notebook shows how to parse the PlantDoc dataset using 2 different methods:
- Using the Icevision default VOC parser
- Creating a new parser using the csv annotation file

### Part 3: Demonstrating the new Data Validity Checking API

Virtually, every dataset has some invalid data. Parsing as well training such datasets is time consuming because of the error raised during both those steps. 

In order to overcome those obstacles and to accelerate both parsing and end-to-end training processes, we are introducing some new IceVision features that will automatically check the validity of the dataset as well auto-correcting them whenever is possible.

### Part 4: Some announcements

We will announce some upcoming events as well as some new features that we intend to work on during the upcoming weeks.

## Announcements

### Hackathon: Bring Your Own Dataset (BYOD)

**When:** Tuesday October 20th 2020 from 9AM to 4PM (GMT-4)

**Where:** http://tinyurl.com/IceData 

[Links to datasets]( https://github.com/Tessellate-Imaging/Monk_Object_Detection/tree/master/application_model_zoo#training-and-inference-examples-with-pretrained-models)

**Setting**
- Users could bring their own datasets to parse and to train.

- They could team-up with other Airctic members or invite their friends/colleagues

- We will be there to help you and to guide you

- If you wish, it would be great if you could help other users

- We will organize the hackathon into several chat/video rooms

    * Main Room

    * Several Rooms where users could gather and work together

    * Help Room: at any moment, users can step in this room to ask for help. Whenever Lucas and Farid are available will join this room to help. Any other Airctic member is encoutaged to join to volunteer helping.

### Adding new features

We will soon start working on creating an API that will enable us to create down-scaled datasets that can be train more quickly thanks to their reduced size.

Example: We have the [TACO dataset](https://github.com/pedropro/TACO). It size est greater than 3GB. We would like to reduce all the image sizes to, say, 640 (while prserving the ratio), and save the new down-scaled dataset as a COCO dataset.
