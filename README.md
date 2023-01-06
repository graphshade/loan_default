# Loan Default Prediction

<img src="https://i.imgur.com/pWBEwXX.png" />

<h2>Problem statement</h2>
Over the years, So & So Lending Club has been experiencing increase in the dollar amount of loan defaults. The chart above shows the gravity of the problem the company face. As of 2013, the total loan portfolio amounted to $182 million and $30.4 million of that is in default. The situation is getting worse, and requires drastic measures to reverse the trend. 

In this project, I attempted to use machine learning to help So & So Lending Club predict the likelihood of a loan default, and also to identify the factors that driving loan default.

<h2>Languages and Libraries Used</h2>

- R programming language 
- [List of libraries](https://github.com/graphshade/Customer-segmentation---R-Shiny-App/blob/master/renv.lock)

<h2>Environment Used </h2>

- <b>Ubuntu 22.04.1 LTS</b>

<h2>Program walk-through:</h2>

<p align="left">

1. [Install R and RStudio](https://techvidvan.com/tutorials/install-r/)
 
2. Clone the project: Run this from the command line
 
 ```commandline
 git clone https://github.com/graphshade/customer_segmentation_shiny_app.git
 ```
 
3. Install Required Libraries Using Virtual Environment: 
   
   You may install the libraries directly on your computer however, using the virtual environment library `renv`. [Follow this guide to install renv](https://www.youtube.com/watch?v=yc7ZB4F_dc0)
   1. Open the app.R file in RStudio
   2. In the RStudio console run `renv::init()` to initiate the renv virtual environment and install the required libraries from the [renv.lock](https://github.com/graphshade/Customer-segmentation---R-Shiny-App/blob/master/renv.lock) file 

4. Run the app
 From the left corner of your RStudio, click on <kbd> <br> Run App
 
   When the app run properly, you'll see

   <img src="https://i.imgur.com/tLHZa7K.png" />

 5. Following the instructions from the left panel, you may upload the `sample_dataset.csv` file
 
 6. After uploading the dataset, you can use tha tabs in the right panel to view the results
 
    <b>Customer Segmentation Results Tab</b>
 
    <img src="https://i.imgur.com/GI53Iel.png" />
 
    <b>Cluster Visualization Tab</b>
 
    <img src="https://i.imgur.com/5CD2fij.png" />
 </p>
 
