# SeismicPatchNet_v1
Demonstration of automated searching a neural network architecture for cost-efficient seismic data classification


*** System requirements ***

* Python 3.7.4.1
* Tensorflow-gpu 1.14
* Nvidia CUDA 10
* Nvidia cuDNN v7.5.0 (Feb 21, 2019), for CUDA 10.0


*** Instructions for use ***

Functional programming scripts.


I. Run "1. synthetic_patch_models.py" to generate synthetic data as much as possible (e.g. more than 15000 samples) for architecture searching.

It is strongly recommended to run the script step by step. For example, comment:
# ========================================
#      Step 2:  summarize statistics of architectures' performance
# ========================================
before run:
# ========================================
#                    Step 1:  scan and delete/remove 
#                   failed/incomplete jobs/model folder
# ========================================


2. Run "2. random_search_SeismicPatchNet_v1p2.py" to start searching, which can be deployed on multiple GPUs by copies and specify a GPU ID as suggested in the script.


3. Run "3. random_search_Analysis.py" to sort the searching results and find the most qualified architecture.


More details were presented in our article.