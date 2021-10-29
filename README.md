# Metagenomics bioinformatics (Virtual) - 2021

Learn about the tools, processes and analysis approaches used in the field of metagenomics.

This course will cover the use of publicly available resources to manage, share, analyse and interpret metagenomics data; including marker gene, whole gene shotgun (WGS) and assembly-based approaches.

The virtually-delivered content will involve participants learning via pre-recorded lectures and live presentations, followed by live Q&As with the trainers. Practical experience will be developed in group activities and in computational exercises run in Docker containers on our virtual training infrastructure.

For more information about please refer to [Metagenomics bioinformatics (Virtual) - 2021](https://www.ebi.ac.uk/training/events/metagenomics-bioinformatics-virtual-2021/)

## Preparing the interactive notebooks
Open a Terminal.
```shell
pip install -r requirements.txt
ipython kernel install --name "mgnify-ebi-2021" --user
jupyter-lab course.jupyterlab-workspace
```

Jupyter should be using the "mgnify-ebi-2021" kernel, so that the packages are available.
To check, look at the top right of the Jupyter Lab window:
![selecting kernel in jupyter](notebooks/assets/jupyter-kernel-selection.png)
