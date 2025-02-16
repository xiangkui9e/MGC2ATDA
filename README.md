# MGC2ATDA

## Overview

The **MGC2ATDA** project provides tools and methodologies for [Prediction of the Association between Transfer RNA and Diseases: A Deep Learning Approach Combining Multi-View Graph Convolution and Attention Mechanisms]. This repository contains the necessary setup instructions and dependencies to get started on your journey with MGC2ATDA.

## Getting Started

Follow the steps below to create the appropriate environment, install required libraries, and prepare datasets for analysis.

### Prerequisites

Ensure you have [Anaconda](https://www.anaconda.com/products/distribution) installed on your system.

## Installation

### Step 1: Set up the Conda Environment

To begin, create and activate a new Conda environment for the project:

 
conda create -n MGC2ATDA python=3.10 -y conda activate MGC2ATDA
### Step 2: Install Required Packages

With your environment activated, install the necessary Python packages using the following `pip` commands:

```
pip install numpy==1.25.0
pip install scipy==1.11.1
pip install pandas==1.5.3
pip install openpyxl==3.0.10
pip install scikit-learn==1.2.2
pip install biopython==1.83
pip install obonet==1.0.0
pip install gensim==4.3.1
pip install tqdm==4.65.0
pip install jupyterlab==3.6.3
pip install matplotlib==3.8.2
pip install torch==2.1.2 torchvision==0.16.2 torchaudio==2.1.2 --index-url https://download.pytorch.org/whl/cu118
pip install https://data.pyg.org/whl/torch-2.1.0%2Bcu118/torch_cluster-1.6.2%2Bpt21cu118-cp310-cp310-win_amd64.whl
pip install https://data.pyg.org/whl/torch-2.1.0%2Bcu118/torch_scatter-2.1.2%2Bpt21cu118-cp310-cp310-win_amd64.whl
pip install https://data.pyg.org/whl/torch-2.1.0%2Bcu118/torch_sparse-0.6.18%2Bpt21cu118-cp310-cp310-win_amd64.whl
pip install https://data.pyg.org/whl/torch-2.1.0%2Bcu118/torch_spline_conv-1.2.2%2Bpt21cu118-cp310-cp310-win_amd64.whl
pip install torch-geometric

```
### Step 3: Prepare Datasets

To prepare datasets for analysis, run the following command:

 
bash run_gen_fold.sh
### Step 4: Train Models for Cross-Validation

To train models using cross-validation, run the main training and result comparison scripts in the MGC2ATDA:

 
bash run_main.sh bash run_result_compare.sh
### Step 5: Additional Methods

For training and evaluating additional methods discussed in the associated paper, run the respective scripts in the following folders:

- **ETGPDA**
- **iPiDA-GCN**
- **iPiDA-SWGCN**
- **iPiDA-GBNN**
- **piRDA**

Run the commands for each method:

 
bash run_main.sh bash run_result_compare.sh
