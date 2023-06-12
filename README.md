# data_preprocessing
This repository contains the code for data preprocessing for the Capstone project.

## Data
Create a folder named `unprocessed_images` in the root directory of the project, and the raw GPR data should be copied to this folder. The data should be saved in the following way:
```
root directory
│   unprocessed_images
│   │   WLT_350_210926__001 P_2111131.JPG
|   │   WLT_350_210926__003 P_2111131.JPG
|   │   ...
```

## Annotation
The annotation tool we used is [CVAT](https://www.cvat.ai/).
### CVAT Annotation Platform
CVAT is a powerful annotation platform that facilitates the labeling and review process. It provides a variety of tools to visualize and annotate data effectively. It also supports a wide range of annotation formats, including bounding boxes, polygons, polylines, points, and cuboids for 3D annotations. In this project, we use bounding boxes to annotate the data.

CVAT is open-source platform that can be deployed on-premise or in the cloud. For this project, we use the cloud version of CVAT. The cloud version of CVAT is free to use, making it a great choice for small projects.

CVAT also allows users to collaborate on projects and share annotated data. However, from our experience, using two different accounts to annotate the same data is not a good idea. The platform is not quite stable and it is easy to lose your work. Therefore, we recommend that you use one account to annotate the data, and share the login information with your teammates. Also, you should communicate with your teammates and ensure that no more than one user logs in to the platform at the same time.

### Annotation File Output
The output of the annotation process in CVAT is a zip file. This zip file contains all the annotated data, making it easy to manage and share your labeled datasets.

### Instructions
1. Accessing CVAT: Visit the CVAT website at https://cvat.org/ and create an account if you don't have one already.

2. Creating a Project: Once logged in, create a new project by clicking on the "New Project" button. Setup the project name and the name of every annotation.

3. Creating a Task and Uploading Data: Create a new Task and upload the GPR images you want to annotate. You can upload multiple images at once. Once the images are uploaded, you can start annotating them.

4. Annotating Objects: Use the selected annotation tool to annotate objects in the uploaded images.

5. Reviewing Annotations: After completing the annotation task, review the annotations to verify their correctness and consistency. Make any necessary adjustments or corrections as needed.

6. Saving Annotations: Save your annotations within the CVAT platform to preserve your work.

7. Exporting Annotations: After saving, you can export the annotations as a zip file. Click on the "Menu" button and select "Export job dataset" to export the annotations as a zip file. Choose the "CVAT for images 1.1" format and click on the "Export" button to export the annotations as a zip file. You can customize the name of the zip file. The zip file will be downloaded to your computer.
