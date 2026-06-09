### Overview
This workflow has been developed in Python.

All package requirements can be found in the **package_requirement.txt** file, as well as the **gred_env.yml** file.

All required input files can be found under the **input** folder. A separate README file can be found inside the folder describing the purpose and source of each of the files. All files must be uploaded to the same workspace as the main script before attempting to run it.

Namibia is used as an illustrative case study, but the script can be modified to model other countries/study regions.

Output maps and figures from the Namibian case study can be found in the four **output** folders, corresponding to different steps in the workflow. Again, a separate README file can be found inside each of the folders describing the format and contents of each of the files.

### How to run the script: Option 1
After downloading the main script and package_requirements file, the user is advised to follow these steps when running the script for the first time:
1. Download and install Microsoft Visual Studio Code; [download link](https://code.visualstudio.com/download).
2. Click on **File** in the upper left Menu Bar and select **Open Folder**.
3. From the pop up window that appears, browse to the folder containing the main script, the requirements text file, and all other necessary input files. Click **Select Folder**. All the folder contents should now appear in the **Explorer** side bar on the left.
4. Double click on the main script (Python notebook) titled **high-res-elec-demand.ipynb** to open it.
5. Press **Ctrl+Shift+P** to open the Command Palette.
6. Search for **Python: Create Environment** and select that command.
7. Select **Conda** from the drop-down list of environment types.
8. From the drop-down list of Python versions, select **Python 3.12**.
9. A pop-up notification should appear showing the progress of environment creation. Once the environment is created, it should appear in your folder in the **Explorer** side bar.
10. Finally, run the first cell in the script, which installs all required packages. You can then proceed with the rest of the script normally.

For subsequent runs using Microsoft Visual Studio Code, the user should use the same environment installed according to the above steps. This can be done via clicking on **Select Kernel** at the upper right corner of the open notebook and navigating to the right environment. When in doubt, the user can re-create the environment using the aforementioned steps.

### How to run the script: Option 2
1. Download and install one of Anaconda's versions according to your operating system; [download link](https://www.anaconda.com/download).
2. Download this repository directly to your local directory, or clone it using git.
```
> conda install git
> git clone https://github.com/mai-elsayed23/high-res-elec-demand.git
```
3. Open Anaconda Prompt and switch to the local directory where you saved the repository, using:
```
> cd ..[insert path]..\high-res-elec-demand
```
4. Create a new environment that has all the packages required to run the entire workflow, using:
```
> conda env create --name GRED --file gred_env.yml
```
5. After the new virtual environment has been created, activate it using:
```
> conda activate GRED
```
6. Start a Jupyter notebook session by typing:
```
..\high-res-elec-demand>jupyter notebook
```
7. A new session should start in a browser window, where you can navigate to each of the four scripts that make up this workflow.

For subsequent runs using Anaconda Prompt, follow steps 3 >> 5 >> 6. Whenever the kernel is restarted, make sure to re-run the first cell in the script that imports all the required packages installed in the virtual environment.
