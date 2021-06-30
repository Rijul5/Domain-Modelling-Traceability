# Domain-Modelling-Traceability



## Instructions to use the experiment data
Please click this [link](https://www.dropbox.com/s/ryw4nwoe0hspgcf/Experiment%20Data.xlsx?dl=0) to view the experiment data.

In the file, separate tabs have been created for each problem description. The first tab displays the summarized results of model extraction and traceability.



## Instructions to use the tool
As mentioned in the response letter, our tool is up and live now. It is available [here](http://modelling-bot.herokuapp.com/).

The tool is composed of two sub-systems - (1) backend and (2) frontend. These sub-systems are further composed of microservices that are responsible for various tasks such as model extraction using pre-trained ML and language models and construction of traceability knowledge graph. These microservices are currently deployed on the Heroku cloud where they communicate with each other based on users' requests. Due to the size limitation on the Heroku cloud, we currently deploy the small-scale spaCy [language model](https://spacy.io/models/en#en_core_web_md). 

Also, the tool should take a few seconds initially when our application's dyno on the Heroku cloud is asleep. After the first few hits, the application's response time will be quick.


