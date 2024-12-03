
# Workshop Environment Setup Guide

This guide provides step-by-step instructions to set up a Python environment for the workshop using Miniconda and Jupyter Notebook. Follow each step carefully to ensure everything is installed and configured correctly.

---

## Steps to Set Up the Environment

1. **Check if Python is Installed:**
   - Open a terminal or Command Prompt.
   - Type the following command to check if Python is installed:
     ```bash
     python --version
     ```
     or
     ```bash
     python3 --version
     ```
   - If Python is installed and the version is **3.10 or higher**, skip to Step 3 (Install Miniconda).
   - If Python is **not installed** or the version is lower than 3.10, proceed to install Python.

2. **Install Python (if required):**
   - Download Python from the official website: [https://www.python.org/downloads/](https://www.python.org/downloads/)
   - Follow the installation instructions, ensuring to check the **"Add Python to PATH"** option during setup.

2. Install Miniconda:
   - Visit [https://www.anaconda.com/download/success](https://www.anaconda.com/download/success).
   - ***Scroll down*** to the **Miniconda Installer** section and download the appropriate version for your operating system(Windows,Mac or Linux).
   - Install Miniconda by following the on-screen instructions.

3. Verify Miniconda Installation:
   - Open Miniconda.
   - Type the following command to verify the installation:
     ```bash
     conda --version
     ```
   - If this shows the Conda version, proceed to the next step. If not, make sure you implemented above steps correctly.

4. Create and Activate the Workshop Environment:
   - Run the following command to create a new Conda environment:
     ```bash
     conda create -n workshop_env python=3.10
     ```
   - Activate the environment:
     ```bash
     conda activate workshop_env
     ```
   - Ensure you see `(workshop_env)` at the beginning of your terminal prompt.

5. Install Required Python Libraries:
   - Make sure you are in the `(workshop_env)` environment.
   - Run the following command to install the required libraries:
     ```bash
     pip install numpy pandas matplotlib scikit-learn jupyter
     ```

6. Configure VSCode:
   - Download and install [Visual Studio Code (VSCode)](https://code.visualstudio.com/). (Unless already installed)
   - Install the following VSCode extensions:
     - **Python**
     - **Code Runner**
   - Open a folder in VSCode where you'd like to work.
   - Create a file named `test.ipynb`. (it is essential you add the ".ipynb" yourself)
   - Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac) to open the command palette.
   - Search for and select **"Python: Select Interpreter"**.
   - Select the interpreter with the name of your environment (`workshop_env`).
   - Run a cell in the notebook. When prompted to install the Jupyter kernel, click **Install**.

7. Test Your Setup:
   - In your `test.ipynb` file, copy and paste the following Python commands:
     ```python
     import numpy as np
     import pandas as pd
     import matplotlib
     import matplotlib.pyplot as plt
     print(np.__version__, pd.__version__, matplotlib.__version__, sep='\n')
     ```
   - If no errors occur your setup is complete and ready for the workshop!

---

### **Additional Notes**  
- Ensure that you are working within the `(workshop_env)` environment for all workshop-related tasks.
- If you encounter any issues, refer to the official documentation for Python, Conda, or VSCode, or reach out for support during the workshop.

---
