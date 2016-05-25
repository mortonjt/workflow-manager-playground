# workflow-manager-playground

To get started first install conda as follows

```bash
wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh
chmod a+x Miniconda3-latest-Linux-x86_64.sh
./Miniconda3-latest-Linux-x86_64.sh
source ~/.bashrc
```

Then install a new environment.  To install a snakemake compatible environment, use the following code
```bash
conda config --add channels http://conda.anaconda.org
conda create -n snakemake-tutorial -c zechxu --file requirements.txt
snakemake -np mapped_orfs/seq.cluster001.m8
```
