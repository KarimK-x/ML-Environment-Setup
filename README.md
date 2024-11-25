
# Workshop Environment Setup Guide

This guide provides step-by-step instructions to set up a Python environment for the workshop using Miniconda and Jupyter Notebook. Follow each step carefully to ensure everything is installed and configured correctly.

---

## Steps to Set Up the Environment

1. Install Python:
   - Download Python from the official website: [https://www.python.org/downloads/](https://www.python.org/downloads/)

2. Install Miniconda:
   - Visit [https://www.anaconda.com/download/success](https://www.anaconda.com/download/success).
   - Scroll down to the **Miniconda Installer** section and download the appropriate version for your operating system.
   - Install Miniconda by following the on-screen instructions.

3. Verify Miniconda Installation:
   - Open Miniconda (or any terminal with Miniconda added to the PATH).
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
     pip install numpy pandas matplotlib scikit-learn keras jupyter
     ```

6. (Optional) Configure VSCode:
   - Download and install [Visual Studio Code (VSCode)](https://code.visualstudio.com/).
   - Install the following VSCode extensions:
     - **Python**
     - **Code Runner**
   - Open a folder in VSCode where you'd like to work.
   - Create a file named `test.ipynb`.
   - Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac) to open the command palette.
   - Search for and select **"Python: Select Interpreter"**.
   - Select the interpreter with the name of your environment (`workshop_env`).
   - Run a cell in the notebook. When prompted to install the Jupyter kernel, click **Install**.

7. Test Your Setup:
   - In your `test.ipynb` file, try running the following Python commands:
     ```python
     import numpy as np
     import pandas as pd
     import matplotlib.pyplot as plt
     ```
   - If no errors occur, your setup is complete and ready for the workshop!

---

### **Additional Notes**  
- Ensure that you are working within the `(workshop_env)` environment for all workshop-related tasks.
- If you encounter any issues, refer to the official documentation for Python, Conda, or VSCode, or reach out for support during the workshop.

---
