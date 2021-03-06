## Description
ETL code for the project "Eat Safe on the Go" is written in Python 3 and it utilize packages: Pandas, Numpy, Matplotlib,
Jupyter Notebook, and scikit-learn.

## Package Installation
Please install Python 3 by following the instructions in https://realpython.com/installing-python/
To install all the required packages, please run commands after Python 3 is installed.
* pip install pandas==1.1.2
* pip install numpy==1.19.2
* pip install matplotlib==3.2.2
* pip install scikit-learn==0.20.3
* pip install notebook

If you are a user of Anaconda, all packages above may already be installed.

## Data & Code Download
Make a folder named 'cse6242' in your operating system, which will be used to store data and code. There are two methods
to download data and code.
1. Use Git or checkout with SVN using the web URL. https://github.com/ZXGERIC/cse6242-everywhere.git
2. Go to https://github.com/ZXGERIC/cse6242-everywhere and click Download Zip under Code.

Once download is complete, please make sure the following files are 'cse6242' folder.
* airbnb.zip
* restaurants.zip
* yelp.zip
* CSE6242_data_wrangling.ipynb

## Unzip Data Files
Unzip the following zip files to csv files, and place them in the folder 'cse6242'
* airbnb.zip -> airbnb.csv
* restaurants.zip -> restaurants.csv
* yelp.zip -> yelp.csv

##Code Execution
Three steps to run the code.
1. Change to cse6242 using cd command and run jupyter-notebook. Your browser will be automatically opened.
2. Open CSE6242_data_wrangling.ipynb in your browser.
3. Click 'Run All' in Cell menu.

Note that the ETL code has a set of logic of calculating distance between each Airbnb rental to each resturant (4 million haversine distances), getting nearest 100 resturants, and picking the top 10 restaurants with highest score, it may take up to 60 minutes to finish computing.  

##What to Expect After Code Finishes
After code finishes, 4 csv files will be generated, which will later used to render Geomap in Tableau.
1. airbnb_resto_1_to_many.csv
2. restaurants_history_clean.csv
3. restaurants_full_clean.csv
4. resto_yelp.csv
