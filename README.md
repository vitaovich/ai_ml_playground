# ai_ml_playground

## install miniconda
- make sure to install the correct architecture of your system
    - m series mac: aarch64

    ```bash
    mkdir -p ~/miniconda3
        wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-aarch64.sh -O ~/miniconda3/miniconda.sh
        bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
        rm -rf ~/miniconda3/miniconda.sh

        ~/miniconda3/bin/conda init bash
        ~/miniconda3/bin/conda init zsh
    ```

## conda environment
- add conda forge channel for packages
    ```bash
    conda config --add channels conda-forge
    ```
- create
    ```bash
    conda env create --file ./HandsOnMLLearning/environment.yml
    ```

- update
    ```bash
    conda env update --file ./HandsOnMLLearning/environment.yml --prune
    ```