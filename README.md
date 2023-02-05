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

## Todos
* qualitative results
* cycle gan based sketch generation

## Various text based slide image retrival and v.v. 

| Model | Text |T2I-1 | T2I-5 | T2I-10 |T2I-50 |T2I-100 | I2T-1 | I2T-5 | I2T-10 |I2T-50 |I2T-100 | 
| --- | --- | --- | --- |--- | --- | --- | --- | --- | --- | --- | --- |
| RN50 | glensOcr |55.14 | 77.06 | 82.94 | 92.16 |94.82 |57.14 | 77.61 | 82.72 |91.09 |93.59 |
| RN101 | glensOcr |54.38 | 77.03 | 82.88 | 92.37 |95.04 |52.63 | 73.76 | 79.79 |89.09 |91.90 |
| RN50x4 | glensOcr |61.44 | 83.24 | 88.37 | 95.84 |97.84 |60.75 | 80.90 | 85.40 |93.01 |95.02 |
| RN50x16 | glensOcr |60.95 | 84.27 | 89.60 | 96.86 |98.56 |60.56 | 82.51 | 87.53 |94.77 |96.47 |
| RN50x64 | glensOcr |64.75 | 86.24 | 90.94 | 97.05 |98.56 |58.43 | 80.50 | 86.03 |93.76 |96.01 |
| ViT-B/32 | glensOcr |38.20 | 60.88 | 68.66 | 83.40 |88.25 |38.64 | 61.39 | 69.05 |82.56 |87.12 |
| ViT-B/16 | glensOcr |50.82 | 73.96 | 80.34 | 91.09 |94.32 |48.30 | 70.62 | 77.18 |88.30 |91.65 |
| ViT-L/14 | glensOcr |54.04 | 76.99 | 83.76 | 93.39 |96.11 |46.22 | 69.75 | 76.73 |88.28 |92.08 |
| ViT-L/14@336px | glensOcr |58.19 | 80.79 | 86.47 | 95.33 |97.65 |49.67 | 73.78 | 80.28 |90.86 |94.08 |
| RN50 | summary60 |48.69 | 68.29 | 73.87 | 82.13 |84.86 |50.01 | 68.08 | 72.46 |80.04 |82.34 |
| RN101 | summary60 |47.61 | 67.85 | 73.59 | 82.16 |84.91 |45.36 | 64.36 | 69.59 |78.10 |80.96 |
| RN50x4 | summary60 |54.08 | 74.00 | 78.92 | 86.04 |87.82 |53.21 | 70.76 | 75.40 |82.47 |84.06 |
| RN50x16 | summary60 |53.70 | 74.77 | 80.01 | 86.99 |88.83 |52.39 | 72.44 | 77.62 |84.08 |85.64 |
| RN50x64 | summary60 |57.05 | 76.59 | 81.19 | 87.36 |89.01 |50.73 | 70.95 | 75.91 |83.39 |85.28 |
| ViT-B/32 | summary60 |32.70 | 52.45 | 59.14 | 72.90 |77.31 |33.19 | 52.89 | 59.62 |71.88 |75.69 |
| ViT-B/16 | summary60 |44.39 | 65.49 | 71.26 | 81.36 |84.30 |42.32 | 61.55 | 67.69 |77.76 |80.58 |
| ViT-L/14 | summary60 |47.07 | 68.13 | 74.24 | 83.51 |86.07 |41.20 | 61.17 | 67.23 |77.68 |81.18 |
| ViT-L/14@336px | summary60 |50.30 | 71.11 | 76.90 | 85.34 |87.74 |43.57 | 63.93 | 70.23 |80.26 |83.15 |
| RN50 | layoutSummary |16.01 | 34.74 | 43.45 | 63.64 |70.79 |20.77 | 40.47 | 49.18 |66.98 |73.44 |
| RN101 | layoutSummary |17.86 | 36.79 | 45.14 | 64.53 |71.67 |20.42 | 39.76 | 48.37 |66.66 |72.80 |
| RN50x4 | layoutSummary |18.61 | 37.47 | 46.50 | 66.32 |73.25 |18.14 | 36.13 | 44.72 |64.13 |70.99 |
| RN50x16 | layoutSummary |15.73 | 33.47 | 42.00 | 63.11 |71.12 |17.05 | 34.11 | 42.48 |61.99 |69.58 |
| RN50x64 | layoutSummary |13.89 | 30.44 | 38.96 | 59.98 |68.29 |15.05 | 30.68 | 38.49 |57.50 |64.83 |
| ViT-B/32 | layoutSummary |15.26 | 32.43 | 41.40 | 61.48 |68.46 |19.39 | 37.87 | 46.39 |65.12 |71.41 |
| ViT-B/16 | layoutSummary |12.77 | 28.56 | 37.14 | 57.87 |66.44 |14.94 | 31.56 | 39.80 |60.37 |67.97 |
| ViT-L/14 | layoutSummary |13.51 | 29.49 | 37.94 | 59.23 |67.93 |14.06 | 28.63 | 36.89 |56.28 |64.20 |
| ViT-L/14@336px | layoutSummary |13.90 | 31.09 | 39.71 | 61.58 |70.04 |14.61 | 30.34 | 38.24 |57.35 |65.24 |


ICFHR Notes

1) https://github.com/asciusb/21SyntheticStylesNom-Database
2) Synthetic generation 

https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9494351


