# template_shinydashboard

Starter template for creating a shinydashboard

### File and Folder Structure

Use deploy.R script to deploy the app

Only files and folders that need to be deployed with the Shiny app go in the "shiny_app/" folder.

##### Project root level folders:

  - "data_prep/" - for data preparation.  Most projects need data to be prepped from some raw format to a format ready for the app.  This folder is most heavily used in the early days of the project as we are exploring the data and cleaning up initial data issues.
      - "provided/" - raw data provided by the client goes here.  This data is not tracked on GitHub
      - "prepped/" - cleaned versions of the data in "provided" goes here.  This data is also not tracked on GitHub.
  - "docs/" - additional documentation goes here
  - "analysis/" - additional analysis e.g. EDA goes here.  Also if you are training models that may or may not end up in your Shiny app, do that here.
  - You can make other folders as is appropriate for your project
  
##### "shiny_app/" level folders:

  - "www/" - contains all front end assets (i.e. css, js, and images)
  - "data/" - contains any flat files that need to be deployed with the app
  - "funs/" - contains functions specific to the project calculations.  e.g. if the Shiny app calculates insurance rates, any functions to calculate the rate would go here.
  - "helpers/" - contains functions for building UI and other generic Shiny utility.  E.g. a function to generate the UI for a custom widget would go here. 
  - "modules/" Shiny modules go here
