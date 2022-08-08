# Automation of Gene Signature Generation

## Problem Statement
Gene expression signature in a cell that occurs due to some biological process. This is helpful for us in determining the effectiveness of a drug. In this project, we want to classify our samples into two states:  control and perturbation. Control would be to know that our experiment has worked. However manual curation of these gene signatures is a very extensive task and thus there is a need to automate this process.

## Dataset

Since the manual curation of gene expressions is a very extensive task, we do not have access to a large amount of labelled data. The dataset we have consists of 20k samples but labels are only present for 600 of them. Our dataset is divided into seperate files for labelled and unlabelled dataset. 

## Solution

To overcome the problem of a small amount of labelled data present, I used a technique called Semi Supervised Learning. In this technique, I initially trained my model on the small labelled dataset I had and then predicted labels and confidence score of the unlabelled dataset. After which i set a confident score threshold and created a larger labelled dataset and trained my model on it.
