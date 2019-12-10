## Installation
 
These steps guides you on how to install both pyIncore and Jupyter Notebooks on **All platforms** so you can develop your code.

1. From the Terminal (Mac/Linux) or Command Prompt (Windows) add [conda-forge](https://conda-forge.org/) package repository/channel to your environment:
    ```
    conda config -add channels conda-forge
    ```

2. To install pyIncore, navigate to the directory you want to use for running Jupyter Notebooks and run the following command (single line command):
    ```
    conda install -c https://inconda:CHANNEL_PWD_HERE@incore2.ncsa.illinois.edu/conda/pyincore/ pyincore
    ```
    Contact us at [incore-dev@lists.illinois.edu](mailto:incore-dev@lists.illinois.edu) for the **channel password** (CHANNEL_PWD_HERE is a placeholder for the real password). This command tells conda to install the ``pyincore`` package from the NCSA's conda ``incore`` channel.

    An alternative approach is to register NCSA's conda channel in the `.condarc` file which contains names and links of the channels.
    ```
    conda config --append channels https://inconda:CHANNEL_PWD_HERE@incore2.ncsa.illinois.edu/conda/pyincore/
    ```
   and then
     ```
    conda install pyincore
    ```
   Note, that the `.condarc` file is usually stored in your HOME directory. The typical location of a HOME directory is `C:\Users\<username>\` on Windows OS, `/Users/<username>` on Mac OS and `/home/<username>/` on Linux based machines.

The installation installs pyIncore and creates a `.incore` folder in your HOME directory to store cached files. 
The message *pyIncore credentials file has been created at <HOME directory>/.incore/.incorepw* appears 
in the terminal/prompt. The typical location of a HOME directory is `C:\Users\<username>` on Windows OS, `/Users/<username>` on MacOS 
and `/home/<username>` on Linux based machines.

To check that the package is installed run `conda list command`.

Replace `install` command above with `update` to update pyIncore to the latest version that is compatible with all other packages in the environment.