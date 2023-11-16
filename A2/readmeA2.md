**Since I drew advanced charts that take up a lot of memory in this project, most of the charts may appear blank in the current project (even including clustering results), so please be sure to follow the steps below to view my project. Thank you so much!**

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
