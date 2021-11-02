# Metagenomics bioinformatics (Virtual) - 2021

Learn about the tools, processes and analysis approaches used in the field of metagenomics.

This course will cover the use of publicly available resources to manage, share, analyse and interpret metagenomics data; including marker gene, whole gene shotgun (WGS) and assembly-based approaches.

The virtually-delivered content will involve participants learning via pre-recorded lectures and live presentations, followed by live Q&As with the trainers. Practical experience will be developed in group activities and in computational exercises run in Docker containers on our virtual training infrastructure.

For more information about please refer to [Metagenomics bioinformatics (Virtual) - 2021](https://www.ebi.ac.uk/training/events/metagenomics-bioinformatics-virtual-2021/)

## Preparing the interactive notebooks

We will have to install the dependencies to run the notebooks. To do so, we will use [miniconda](https://docs.conda.io/en/latest/miniconda.html).

Open a Terminal.

```shell
(base) conda create -n mgnify-ebi-2021 python=3.9
(base) conda activate mgnify-ebi-2021

(mgnify-ebi-2021) pip install -r requirements.txt
(mgnify-ebi-2021) ipython kernel install --name "mgnify-ebi-2021" --user
(mgnify-ebi-2021) jupyter-lab course.jupyterlab-workspace
```

Jupyter should be using the "mgnify-ebi-2021" kernel, so that the packages are available.
To check, look at the top right of the Jupyter Lab window:
![selecting kernel in jupyter](notebooks/assets/jupyter-kernel-selection.png)
