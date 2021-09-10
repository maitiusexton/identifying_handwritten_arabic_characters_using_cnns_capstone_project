# Project 6: Identifying Handwritten Arabic Characters Usings Convolutional Neural Networks (CNNs)

## Problem Statement
***How accurately can we identify handwritten Arabic characters from the Handwritten Arabic Characters data set using CNNs?***

### Background
OCR (Optical Character Recognition) technology has countless applications to problems in a variety of industries. These include data entry, information extraction translation, and more. Most of these technologies are based on languages which use Latin scripts. While it is true that the Latin script is the most widely used writing system in the world, this still leaves out millions of people who primarily use other scripts. Arabic is the 5th most spoken language in the world and several other languages (Farsi, Kurdish, Urdu, Uyghur, Pashto, and several more) use an Arabic-based alphabet. These reasons create a clear motivation for the creation of OCR software that can read Arabic.

### Data that was analyzed
train_images and test_images were both pulled from [this](https://www.kaggle.com/mloey1/ahcd1) data set. The original download included .csv files for the images, but the only files used in this modelling was the 17,000 32x32 .png images of each character (600 of each of the 28 main letters of the arabic alphabet

### Data Dictionary
The data was simply a large collection of .png images each labelled with a number to indicate which character they were. Below is provided the dictionary used in the data to distinguish the letters (common hijaa'ii order/الترتيب الهجائي is used). 


|Class Label  | Arabic Character | Letter Name |
|------------:|-----------------:|:------------|
|          01 |                 أ|alef         | 
|          02 |                 ب|beh          |
|          03 |                 ت|teh          |
|          04 |                 ث|theh         |
|          05 |                 ج|jeem         |
|          06 |                 ح|hah          |
|          07 |                 خ|khah         |
|          08 |                 د|dal          |
|          09 |                 ذ|thal         |
|          10 |                 ر|reh          |
|          11 |                 ز|zain         |
|          12 |                 س|seen         |
|          13 |                 ش|sheen        |
|          14 |                 ص|sad          |
|          15 |                 ض|dad          |
|          16 |                 ط|tah          |
|          17 |                 ظ|zah          |
|          18 |                 ع|ain          |
|          19 |                 غ|ghain        |
|          20 |                 ف|feh          |
|          21 |                 ق|qaf          |
|          22 |                 ك|kaf          |
|          23 |                 ل|lam          |
|          24 |                 م|meem         |
|          25 |                 ن|noon         |
|          26 |                 ﻫ|heh          |
|          27 |                 و|waw          |
|          28 |                 ي|yeh          |

## Conclusions and Future Research
Our strongest model was 94.17% accurate when predicting unseen data. The Categorical Cross Entropy Loss Function had a score of 0.2306.

Ideally, this method of extracting data could be extended up to larger data sets consisting of lines/paragraphs of handwritten text, such as the [KHATT data set](http://khatt.ideas2serve.net/) or several others. Its final iteration would be to apply this to full images and be able to detect where Arabic text is present in a picture or video and possibly even provide translations. A much bigger but very worthwhile project.
