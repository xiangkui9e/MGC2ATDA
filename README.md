```markdown
# MGC2ATDA

## Getting Started

This repository provides the setup instructions and required dependencies to get started with the **MGC2ATDA** project. The following steps will guide you through creating the appropriate environment and installing all necessary libraries.

## Installation

### 1. Setup Conda Environment

To begin, you need to create a Conda environment and activate it:

```bash
conda create -n MGC2ATDA python=3.10 -y
conda activate MGC2ATDA
```

### 2. Install Required Packages

Once the environment is activated, install the required Python packages using the following `pip` commands:

```bash
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

Prepare Datasets(Random 50 times)

run run_gen_fold.sh in data

To train models for cross-validation, please follow the following steps:

Run run_main.sh and run_result_compare.sh in MGC2ATDA.
For other methods mentioned in the paper, run run_main.sh and run_result_compare.sh in ETGPDA, iPiDA-GCN, iPiDA-SWGCN, iPiDA-GBNN, piRDA folder.
