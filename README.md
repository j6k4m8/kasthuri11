# ocp_template
a blank template that can be cloned demonstrating ocp style.
note the milestones (which do not get copied when you clone).
also note that this can be public or private until we submit a manuscript.
this repo contains the following directory structure

- **Background**: to put all articles that we discuss, many of which will be referenced in our publication. Call each file <Last name of first author><last 2 digits of year>, eg, Smith15.
- **Code**: this will house all your code.
  - **Functions**: for various functions that you write. Essentially, any lines of code that you use multiple times it is worth making a function so that debugging becomes easier.
  - **Experiments**: these are scripts that set parameters for simulations or analyses, run them, and save the results (to the data directory)
  - **Plots**: for code to generate professional quality figures for eventual publication. This scripts should load data and statistics generated by code in 'Experiments' and saved in 'Data/Results' and makes some plots
  - **Dependencies**: for actually reproducible code, you need to include the correct version of any dependencies you used. Thus, any code that is not properly version controlled, best practice is to put the version we use here. For code that is properly version controlled, in the experiments, we just link to a specific commit.
  - **DataIngest**: code that (potentially downloads and) converts raw data into base data (see below)
  - **Tests**: unittests for all functions. Different languages have different packages:
- **Data**: storing all data (that is small enough to store in github. Organized into 3 subfolders
  - **Raw**: the raw data, downloaded from some website. If it is too large, in your opinion, for a github repo, you can just store a text file with a link to download the data from some public place.
  - **Base**: this is the raw data but after processing to make it suitable for your analysis. It gets into this form via scripts in the 'DataIngest' folder. This may include, for example, a script to download the data, convert it from csv to matlab, rename some of the variables, etc.
  - **Results**: this includes any data derivatives from running code that you wrote, including, especially, any data necessary to reproduce any results, including figures and tables and other numbers reported.
- **Draft**: will be the text & bib & style files for the manuscript
 

Code should follow the appropriate languages style guidelines.  In general, we default to Python.
  - [Python PEP 8](https://www.python.org/dev/peps/pep-0008)
  - [MATLAB](https://sites.google.com/site/matlabstyleguidelines/) 
  - [Google's R Style Guide](https://google-styleguide.googlecode.com/svn/trunk/Rguide.xml)

