Assignment 2: Cohort characterisation and clustering
For assignment 1, you have identified a group of patients of interest (a patient cohort) and built a digital phenotype for a relevant clinical condition in critical care using MIMIC (profound hypotension).

Before embarking in a potentially laborious and challenging predictive modelling task (for example, employing a machine learning flavours such as deep learning or an interpretable learning approach), it might be valuable discovering simple patterns in the data that might segregate patients into subphenotypes (that might be related to different patient outcomes or increased risk). This can be achieved via Exploratory Data Analysis as well as Unsupervised Learning (in this case, clustering).

For this assignment, you will investigate the main characteristics of the cohort developed for assignment 1, identify clusters of patients and assess whether they have clinical meaning. As input, you will work on a profound hypotension patient cohort that we provide here: hypotension_patients.csv Download hypotension_patients.csv.

The main patient characteristics that you will use include: Demographics, Co-morbidity index (Charlson), Severity of illness scores (APSIII) as well as patient outcomes, including length of stay (LoS) and in-ICU mortality.

Describe via summary statistics the main properties of the profound hypotension cohort. (Up to 200 words. Also provide plots for visualising the distributions).
Perform k-means clustering to identify subgroups of patients. Use the elbow criteria to identify an adequate number of clusters. Justify your choice. Since selecting clusters based on elbow criteria is a heuristic, you may select two different values of k for further analysis. (Up to 300 words. Provide a plot to justify the number of clusters chosen).
What are the main property differences between the clusters you identified? Are they related to patient outcomes? Provide visualisation plots that demonstrate these differences. (Up to 300 words. Also provide plots for visualising the distributions between clusters).
Your code should be written in Python (>= 3.9). You can use any publically available libraries of your choice.

The provided cohort has the following columns:

“ID”: Patient de-identified number;
“anchor_age”: Age of the patient (years);
“gender”: F for female and M for male;
“dod”: Date of Death (if empty means survived - patient outcome variable);
“apsiii”: Severity of illness score;
“LoS”: Length of stay in ICU (days - patient outcome variable);
“charlson_comorbidity_index”: Co-morbidity index.
Submission Requirements
Your submission should consist of three files:

A README file that states your name, the assignment, a description of the problem being addressed by the code, and instructions on how to create the environment to run your submission (see #2 below).

A file that completely specifies the code environment you used (that is, the dependencies and version numbers for all the software you used in your solution. This could be either a requirements.txt (vanilla Python) or environment.yaml (for Anaconda).

A single Jupyter notebook with all the code, output, and explanatory text included.






**Since I drew advanced charts that take up a lot of memory in this project, most of the charts may appear blank in the current project (even including clustering results), so please be sure to follow the steps below to view my project.**

**Step 1:**
Create a new conda environment using *environment.yml* with the command:

`conda env create -f environment.yml -n env_muhan`

**Step 2:**
Activate the newly created environment:

`conda activate env_muhan`

**Step 3:**
Creating a New Kernel(*mykernel*) for Jupyter Notebook:

`python -m ipykernel install --user --name mykernel`

**Step 4:** 
Launch Jupyter Notebook:`jupyter notebook`

This will open a new tab in your web browser displaying the content of the current directory. Navigate to the project's notebook file and click to open it.

**Step 5:**
Change the Kernel (if necessary)
Make sure that the notebook is using the correct kernel (the newly created conda environment). If not, you can change the kernel by clicking on Kernel > Change kernel > selecting the *mykernel*.

**Step 6:** 
Run the Notebook:Now you are all set! You can run the notebook cells sequentially to view the results.



**Project Introduction**
This project is divided into two parts. The *first part* conducts a visual analysis of the main characteristics of the discovered hypotension patient cohort,then the *second part* preprocesses the data and uses the elbow method to determine the two best clustering points (k=4,k=5 respectively). Then use the optimal clustering points to perform k-means clustering, and eventually perform visual analysis on the clustering results.

**Package libraries** used in this project:`matplotlib,os,numpy,pandas,plotly,Scikit-learn,yellowbrick,lifelines,warnings`




**FINAL MARK**: 14/15
