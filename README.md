# Quickstart: Data Exploration and Analysis with Python

<blockquote>
    <center>
        <img alt="ds-community-logo" src="images/logo.png" title="Catalent Data Science Community Logo"/>
        <br>
        For use by members of Catalent's
        <a href="https://catalent.sharepoint.com/sites/EnterpriseDataScience" title="Catalent Data Science Hub">
            Data Science Community of Practice
        </a>
        <br>
    </center>
</blockquote>

<center>
    <a href="https://mybinder.org/v2/gh/catalent-data-science-community/python-quickstart/main">
        <img alt="launch-binder-badge" src="https://img.shields.io/badge/launch-binder-F5A252.svg?logo=data:image/png;base64,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" title="Jupyter Lab in Binder"/>
    </a>
</center>

## Getting Started

Click on the badge above to launch a [Jupyter Lab](https://blog.jupyter.org/jupyterlab-is-ready-for-users-5a6f039b8906) instance in [Binder](https://mybinder.readthedocs.io/en/latest/index.html), and open the file in the **notebooks** folder named after the desired procedure.
<blockquote>
    <ul>
        <li>
            For example, open 'exploratory_data_analysis.py' to work through a notebook of <em>Exploratory Data Analysis</em><br><img alt="jupyter-lab-example" src="images/jupyter-lab-example.png" title="Notebooks Folder in Jupyter Lab"/></li>
        <li>
            After launching a Jupyter Lab instance, it is possible to switch to the "classic" <a href="https://jupyter-notebook.readthedocs.io/en/latest/">Jupyter Notebook</a> mode by manually changing the last portion of the URL from '/lab' to '/tree' and navigating to the modified address
        </li>
</blockquote>
<br>

## Contents

![data-science-roles](images/ds-process.png)  
This repository provides an introduction to ***Exploratory Data Analysis*** and ***Data Cleaning*** in Python, and contains the following four (4) directories:  

- **binder**  
Contains .txt file with packages required to build a python environment for this repository using [Binder](https://mybinder.readthedocs.io/en/latest/index.html)

- **data**  
Contains .csv files with anonymized results from the questionnaires and surveys polled during our Kick Off sessions, as well as a sample dataset of the items sold in the [Cocoon Pharmacy site](https://www.cocooncenter.co.uk/c/cares-body.html) and their reviews [(from Kaggle).](https://www.kaggle.com/datasets/kholoudowais/cocooncenter-pharmacy)  

- **images**  
Contains .png files of graphics referenced in markdown across this repository

- **notebooks**  
Contains .ipynb files of *Exploratory Data Analysis* and *Data Cleaning* done on the contents of the **data** folder

## Contributors

*Miguel Montano*  
[![GitHub Badge](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/miguelmcps)

*Dev Shah*  
[![GitHub Badge](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/devshah096)

## License

This project is licensed under [GPL-3.0](LICENSE)
