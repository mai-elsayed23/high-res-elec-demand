### Overview
This workflow has been developed in Python.

All package requirements can be found in the **package_requirement.txt** file.

All required input files can be found under the **inputs** folder in the main directory. A separate README file can be found inside each of the sub-folders describing the purpose and source of each of the files. All files must be uploaded to the same workspace as the main script before attempting to run it.

Namibia is used as an illustrative case study, but the script can be modified to model other countries/study regions.

Output maps and figures from the Namibian case study can be found under the **outputs_Namibia** folder in the main directory. Again, a separate README file can be found inside the folder describing the format and contents of each of the files.

### How to run the script
After downloading the main script and package_requirements file, the user is advised to follow these steps when running the script for the first time:
1. Download and install Microsoft Visual Studio Code; [download link](https://code.visualstudio.com/download).
2. Click on **File** in the upper left Menu Bar and select **Open Folder**.
3. From the pop up window that appears, browse to the folder containing the main script, the requirements text file, and all other necessary input files. Click **Select Folder**. All the folder contents should now appear in the **Explorer** side bar on the left.
4. Double click on the main script titled **high-res-elec-demand.ipynb** to open it.
5. Press **Ctrl+Shift+P** to open the Command Palette.
6. Search for **Python: Create Environment** and select that command.
7. Select **Conda** from the drop-down list of environment types.
8. From the drop-down list of Python versions, select **Python 3.10**.
9. A pop-up notification should appear showing the progress of environment creation. Once the environment is created, it should appear in your folder in the **Explorer** side bar.
10. Finally, run the first cell in the script, which installs all required packages. You can then proceed with the rest of the script normally.

For subsequent runs using Microsoft Visual Studio Code, the user should use the same environment installed according to the above steps. This can be done via clicking on **Select Kernel** at the upper right corner of the open notebook and navigating to the right environment. When in doubt, the user can re-create the environment using the aforementioned steps.
