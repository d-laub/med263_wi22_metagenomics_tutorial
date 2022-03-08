# Installation Instructions

Install QIIME 2 as a conda environment named `qiime2-2022.2`. Choose the instructions that match your operating system.

- **Mac**
    
    ```bash
    wget https://data.qiime2.org/distro/core/qiime2-2022.2-py38-osx-conda.yml
    conda env create -n qiime2-2022.2 --file qiime2-2022.2-py38-osx-conda.yml
    # OPTIONAL CLEANUP
    rm qiime2-2022.2-py38-osx-conda.yml
    ```
    
- **Linux**
    
    ```bash
    wget https://data.qiime2.org/distro/core/qiime2-2022.2-py38-linux-conda.yml
    conda env create -n qiime2-2022.2 --file qiime2-2022.2-py38-linux-conda.yml
    # OPTIONAL CLEANUP
    rm qiime2-2022.2-py38-linux-conda.yml
    ```
    
- **Windows (WSL)**
    
    You should skip any step that you have done prior.
    
    1. [Install WSL](https://docs.microsoft.com/en-us/windows/wsl/install)
    2. [Install `miniconda`](https://docs.conda.io/en/latest/miniconda.html)
    3. Install Qiime2
    
    ```bash
    wget https://data.qiime2.org/distro/core/qiime2-2022.2-py38-linux-conda.yml
    conda create -n qiime2-2022.2
    conda env update -n qiime2-2022.2 -f qiime2-2022.2-py38-linux-conda.yml
    # OPTIONAL CLEANUP
    rm qiime2-2022.2-py38-linux-conda.yml
    ```
    
    Note: If you run into issues installing Qiime2 (as we did), try reinstalling conda (backup your environments first!) and installing Qiime2 again.
    

After installing QIIME 2 confirm that the installation was successful by activating your new environment and checking that `qiime` runs.

```bash
conda activate qiime2-2022.2
qiime --help
```

Then, clone the GitHub repository for the tutorial.

```bash
git clone https://github.com/d-laub/med263_wi22_metagenomics_tutorial.git
```