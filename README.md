# Slide Deck Images (SDI) Dataset

This is the official repository for the *Slide Deck Images (SDI) Dataset* 

The dataset can be downloaded here:
[SDI Dataset Download](coming soon)

Our Arxiv Paper can be found here: 
[Slide Deck Images Dataset: Retrive and Create Educational Slides](coming soon)


Annotation link [Local LAN](http://10.2.16.142:8000)

 [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]
 
[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

# Overview

This repo is divided into the following sections:

* `dataset` -- this directory contains more information on the dataset structure 

# The dataset
The slide images of SDI dataset are harvested from the [slideplayer web](https://slideplayer.com/) with a popular computer science and  engineering course namely Data structures. The topics we used to search the slide images are the followings: 
* Arrays and Structures
* Stacks and Queues
* Lists
* Trees
* Graphs
* Sorting
* Hashing
* Heap Structures
* Search Structures
* Algorithms
* Stacks and Queues
* Binary trees.
 
 We collected $1700$ slide deck with around $54K$ slide images after cleaning the collected slide image and removing duplicate slides,

# Experiments
## Document figure retrival using sketch images

| Model | S2I-1 | S2I-5 | S2I-10 |S2I-50 |S2I-100 | 
| --- |  --- | --- |--- | --- | --- |
| RN50 |14.58 | 23.63 | 28.06 | 42.77 |52.73 |
| RN101 |16.15 | 25.33 | 30.47 | 46.09 |54.95 |
| RN50x4 |14.32 | 23.83 | 27.86 | 43.82 |54.56 |
| RN50x16 |15.95 | 25.91 | 31.51 | 46.42 |55.21 |
| RN50x64 |14.65 | 22.66 | 27.67 | 45.90 |55.86 |
| ViT-B/32 |17.71 | 27.67 | 31.12 | 46.16 |55.73 |
| ViT-B/16 |17.12 | 25.98 | 30.47 | 44.60 |55.01 |
| ViT-L/14 |19.60 | 30.66 | 35.87 | 51.11 |58.40 |
| ViT-L/14@336px |20.05 | 28.78 | 33.79 | 50.13 |58.59 |
