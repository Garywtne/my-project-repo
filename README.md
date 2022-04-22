# Which factors contribute to accident risk?

![Title Image](readme_images/title.jpg)

This is a team based project that explored a traffic accident data set.


##  Contents

* [Dataset](#dataset-header)
* [Project Outline](#project-header)
* [Example Plots](#example-header)
* [Findings Reports and Presentation](#reports-header)
* [Dependencies and Setup Required](#dependencies-header)
* [How to View / Run the code](#how-header)
* [Jupyter Notebooks File Guide](#which-header)
* [Repository Structure](#structure-header)
* [Team](#team-header)



## <a id="dataset-header"></a>Dataset

We used the [UK Road Safety: Traffic Accidents and Vehicles](https://www.kaggle.com/tsiaras/uk-road-safety-accidents-and-vehicles)\
Detailed dataset of road accidents and involved vehicles in the UK (2005-2017).\
Available from [Kaggle.com](https://www.kaggle.com)

There are 2 CSV files in this data set. 

* Accident_Information.csv
* Vehicle_Information.csv

Both files should be placed in the Resources/ Directory:

![KaggleData](readme_images/kaggle_data.PNG)

Both CSV files were merged into a single dataframe. The resulting data file was extremely large so a decision was made to focus on Years 2010-2016. This data was filtered and placed into a New CSV [all.CSV](#all-header) which is the main data used for all the investigation, analysis and plots.


**Data Limitations**\
It must be noted that the data was limited in scope. Therefore, despite some interesting findings, the plots extracted from the data although **"true"**, do not **"tell the entire story".**


## <a id="project-header"></a>Project Outline

We decided our client question would be **"which factors contribute to accident risk?"** and used this question to formulate some hypotheses and used these to target the data relevant to our hypotheses and attempt to turn that raw data in to **meaningful information**.

* **Hypothesis 1: Greater volume of traffic increases the number of accidents**
* **Hypothesis 2: Urban areas have a greater number of accidents than rural areas**
* **Hypothesis 3: The time or day of the week does not affect the number of accidents**
* **Hypothesis 4: Speed limits do not influence the number of accidents**
* **Hypothesis 5: Biological factors like gender and age do not influence the number of accidents**
* **Hypothesis 6: Location on the road or vehicle manoeuvre does not influence the number of accidents**
* **Hypothesis 7: Poor weather conditions influence the number of accidents**

For each hypotheses we created a number of [visualisations](#example-header) to display the data in an easier to analyse format which helped us understand the information required.

## <a id="example-header"></a>Example Plots
Here are 2 examples plots we created from the data.\
The plots can be found in the [/Images](/Images) folder after running the code in the Notebook files that are in the root directory.

<img src="readme_images/accidents_england.png" width="50%" height="50%"></img>
![seaborn_chart](readme_images/VM.png)


## <a id="reports-header"></a>Findings Reports and Presentation

The findings of this project can be found in the [/Presentation](Presentation/) directory.

There are 3 files:

* 01_Project_scope_notes.pdf
* 02_Presentation.pdf
* 02_Traffic Accidents Report.pdf

## <a id="dependencies-header"></a>Dependencies and Setup Required

In order to run the files you will need to install the following packages.

* gmaps `pip install gmaps`
* pandas `pip install pandas`
* seaborn `pip install seaborn`
* matplotlib `pip install matplotlib`
* scipy `pip install scipy`
* jupyter notebook `pip install notebook`

**Other Required Files:**

**Add the below 2 files into your local cloned repository!** 

* <a id="all-header"></a>**File 1:** [all.csv - Click to Download](https://drive.google.com/file/d/1ES10z-PFW_QcRHwZx63NA42c2y1LmVPS/view?usp=sharing) (accidents from 2010-2016) - File was not included in the repository due to the large file size.

The all.CSV must be placed in the "/Resources" directory.
![Resources_folder](readme_images/resources_folder.png)

**Gmaps API Key requirement**

For gmaps you will also need an API key from the [Google Maps Platform](https://developers.google.com/maps). Please visit the Google maps platform to set up an API key if you do not already have one.

1. **File 2:** [config.py - Click to Download](https://drive.google.com/file/d/1dQNAoCH0c7C_d5NYVAebVbOevwE1jWqN/view?usp=sharing)

2. Open the file in a text editor or VS code and change "YOUR API KEY HERE" to your API key from the Google Maps API.
![api](readme_images/api_key.png)

3. The config.py file should be stored in your local repository root folder.
![config](readme_images/config.png)


## <a id="how-header"></a>How to View / Run the Code

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)

The work was completed primarily using Jupyter Notebooks and the modules listed in the Dependencies section.

1. Clone the repository

2. Complete steps in the [Dependencies and Setup Required](#dependencies-header) section above.

3. Open any of the Jupyter Notebook files (.ipynb) in the root directory and run the cells in order.

The Jupyter notebook files have comments in the code and Markdown cells beneath each step explaining what was done in the cell above.

For a short description of what each notebook contains, please see the [Jupyter Notebooks File Guide](#which-header) section below.


## <a id="which-header"></a>Jupyter Notebooks File Guide

* 01_data_retrieval_step_1.ipynb - Initial data processing and filtering
* 01_data_retrieval_step_2.ipynb - Initial data processing and filtering
* 01_data_retrieval_step_3.ipynb - Initial data processing and filtering
* 02_traffic_vol_vs_accidents.ipynb - Volume of Traffic  vs Number of Accidents
* 03_When_accidents_happen.ipynb - Days of the week, Time of day, Gender, Age, vs Accidents
* 04_Where - Heatmaps.ipynb - Google heatmaps of accidents across the UK and accidents in Birmingham
* 05_RoadSafety.ipynb - Number of Casualties vs Speed limit and Number of Casualties vs Time of day
* 06_Speed Limit Project - FINAL.ipynb - Number of accidents vs speed limit and Number of Accidents vs Vehicle Manouvre.
* 07_Accidents By Road Class and Road Type - Number of Accidents by Severity for Road Class and Road Type
* 08_weather.ipynb - Number of Accidents vs Weather Condition

## <a id="structure-header"></a>Repository Structure

* Notebook code files in the root directory [root/](/)
* Presentation and report files in the Presentation directory [Presentation/](Presentation/)
* Image and Plots in the Images directory [Images](Images/)
* Dataset files in the Resources directory [Resources](Resources/)



## <a id="team-header"></a>Credits / Collaborators / Team

* [Gary Whitney](https://github.com/Garywtne)
* [Jessica Uppal](https://github.com/JessicaUppal)
* [Serdar Bayramov](https://github.com/serdar-bayramov)
* [Arshad Sheikh](https://github.com/ashsams18)
* [Abdurrahman Raja](https://github.com/Abzraja)
