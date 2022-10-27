# Predicting Financial Risk Models with Neural Networks
This tool uses deep neural networks to create binary classifications models and predictions to analyze funding risks



# Risk Classificaton - Supervised Machile Learning
This application pedicts risk through Supervised Learning's imbalanced-learn library. 
It uses a dataset of historical lending activiy from a peer-to-peer lending services company to build a model that can identify the credit worthiness of borrowers. 


<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#purpose">Purpose</a>
      <ul>
        <li><a href="#inputs">Inputs</a></li>
        <li><a href="#outputs">Outputs</a></li>
      </ul>
    </li>
    <li>
      <a href="#modeling_techniques">Modeling Techniques</a>
      <ul>
        <li><a href="#pandas">Pandas</a></li>
        <li><a href="#sklearn">sklearn</a></li>
        <li><a href="#standardscaler">Standard Scaler</a></li>
        <li><a href="#binary-crosscentropy">Binary Crosscentropy</a></li>
        <li><a href="#adam-optimizer">Adam Optimizer</a></li>
        <li><a href="#accuracy-evaluation">Accuracy Evaluation</a></li>
      </ul>
    </li>
    <li><a href="#version-release">Version Release</a></li>
    <li><a href="#how-to-run">How to run</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contributors">Contributors</a></li>
    <li><a href="#license">License</a></li>
        <ul>
        <li><a href="#permissions">Permissions</a></li>
        <li><a href="#disclaimer">Disclaimer</a></li>
        </ul>
    </li>
    <li><a href="#aknowledgements">Aknowledgements</a></li>
</details>

---

<!--Purpose -->
## Purpose
This tool employs Supervised Machine Learning to model and identify creditworthiness of borrowers.


### Inputs
The application reads a data set of 34000 organizations that have recieved funding over the years. The CSV file contains a variety of information about each business including weather or not it became successful. 
We'll use this data to predict weather a business will be successful. The financial institution will use this to decide upon lending to the business.

    applicants_data.csv
 
### Process:
1. Read historical business data in the CSV file.
2. Process data for Neural Network Modeling.
3. Compile and Evaluate a Binary Classification Model using a Nerural Network. 
4. Optimize the Neural Network Model using Tensorflow and Keras.
5. Define 2 deep neural network models from the original network model and 2 optimization attempts.
6. Obtain each model's Predictive Accuracy metrics. 
7. Predictive accuracy metrics will be saved as outputs that summarize each optimization attempt and model.

### Outputs:
1. HDF5 file named AlphabetSoup.h5 
File includes the initial model's data
2. AlphabetSoup_Model_1.h5
First attempt to evaluate the model using test data to determine the model's loss and accuracy.
3. AlphabetSoup_Model_2.h5
Second attempt to evaluate the model using test data to determine the model's loss and accuracy.


    
---
<!--Technologies -->
## Technologies
### Python:

    Phyton Version: **3.7.13**

## Libraries and Dependencies

### Pandas
[pandas](https://pandas.pydata.org/)

### Sklearn
[sklearn](https://scikit-learn.org/stable/)

### Standard Scaler
[standardscaler](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.balanced_accuracy_score.html)

### Binary Crossentropy
[binary-crosscentropy](https://scikit-learn.org/stable/auto_examples/model_selection/plot_confusion_matrix.html) 

### Adam optimizer
[adam-optimizer](https://datascience.stackexchange.com/questions/64441/how-to-interpret-classification-report-of-scikit-learn)

### Accuracy Evaluation Metric
[accuracy-evaluation](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html)


---
<!--How to run -->
## How to run
1. Clone the repository on a folder that will easy to open
2. File can run on a Jupyter notebook or Google Colab
3. Open the file with Jupiter using the Anaconda Navigator
4. Navigate open the folder where the files were cloned to
5. Open the file on JupyterLab
ANACONDA - Navigator
![jupyterlab](./images/anaconda_nav.png)
6. Make sure to import and install the required libaries and dependencies: 

        Install the required Supervised Learning libraries
            conda activate dev
            conda install -c conda-forge imbalanced-learn

        Import the required libraries and dependencies
            import numpy as np
            import pandas as pd
            from pathlib import Path
            from sklearn.metrics import balanced_accuracy_score
            from sklearn.metrics import confusion_matrix
            from imblearn.metrics import classification_report_imbalanced
            from sklearn.model_selection import train_test_split
            from sklearn.linear_model import LogisticRegression

---
<!--Version Release -->
## Version Release

### Version 1.0


---
<!--Usage -->
## Usage


### Data: Lending data
![lending_data](./images/lending_data.png)

### Classification Report
![classification_report](./images/classification_report.png)

### Balanced Accuracy Score and Confusion Matrix:

![balanced_confused](./images/balanced_and_confusion.png)

### Classification Reports: Original and Oversampled

![oversampled](./images/classification_report1.png)






---
<!--Contributors -->
## Contributors

Jeremy Vargas

    Managing Director
    Resonant Solutions LLC
    email:    jeremyvargas@resonantsolutions.org
    linkedin: https://www.linkedin.com/in/jeremyvargas/

UW FinTech Bootcamp
- Startup code provided by institution

---
<!--License -->
## License
Tool is available under an MIT License.

Copyright (c) 2022 - Resonant Solutions, LLC

### Permissions
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
### Disclaimer
The Software is provided “as is”, without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software or the use or other dealings in the Software.

---
<!--Aknowledgements -->
## Aknowledgements
* [Markdown Guide](https://www.markdownguide.org/basic-syntax/#reference-style-links)


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->