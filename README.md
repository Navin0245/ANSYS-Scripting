# ANSYS-Scripting
Python scripts for automating ANSYS tasks, including mesh generation, parametric studies, and result extraction. Efficiently manage simulations, automate processes, and save results. Easy to customize, organized, and adaptable for diverse engineering needs.

This script is designed to automate the process of exporting high-quality images from ANSYS Mechanical. It allows users to capture various graphical representations, including material views, geometry, mesh, analysis results, figures, and boundary conditions. By saving these images automatically, users can efficiently document their simulation results without manually capturing each view.

 Key Features:
1. Automated Image Export:
   - The script captures and exports images of material displays, geometry views, mesh structures, analysis results, figures, and boundary conditions.
   - All images are saved in **PNG** format with high resolution (1200x2000 pixels).

2. Easy Folder Configuration:
   - Users can specify the export directory at Line 12 of the script:
     ```python
     export_folder = r'C:\Desktop\Images'
     ```
   - **Important**: Make sure to keep the `r` before the string to handle the file path correctly. This ensures that special characters (like `\`) are processed as literal characters.

3. Automated Folder Creation:
   - If the specified export folder does not already exist, the script will create it, ensuring that the images are saved without any errors.

 How to Use:
1. Update the Export Folder:
   - Modify Line 12 to specify where you want the images to be saved. For example:
     ```python
     export_folder = r'D:\SimulationResults\Images'
     ```
   - Ensure there are no conflicting files with the same name in the folder, as the script will overwrite existing files.

2. Run the Script:
   - The script will automatically:
     - Set up the necessary views in ANSYS.
     - Capture and save images of materials, geometry, mesh, and results.
     - Export high-quality images to the specified folder, named according to the items in the model tree.

3. Verify Saved Images:
   - Navigate to the export folder to review the saved images. Each image file corresponds to the respective view or result captured from the ANSYS Mechanical session.

This script simplifies the process of documentation by automating image capture, making it ideal for users who need consistent, high-quality graphical outputs from ANSYS analyses.
