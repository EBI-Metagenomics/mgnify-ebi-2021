Opening the Jupyter notebook
----------------------------

|action| Open a new Terminal. There should be a Terminal application icon in the lefthand menubar.

|action| Type these commands to enter the repository:

.. code-block:: bash

    cd ~/mgnify-ebi-2021

    conda activate mgnify-ebi-2021

|info| That should have worked, but if you got an error you’ll need to create the environment:

.. code-block:: bash

    conda create --n mgnify-ebi-2021 python=3.9

    conda activate mgnify-ebi-2021

    pip install -r requirements.txt

|action| To open the notebooks, run:

.. code-block:: bash

    jupyter-lab course.jupyterlab-workspace
