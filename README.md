# Domain-Modelling-Traceability



## Instructions to use the experiment data
Please click this [link](https://www.dropbox.com/s/ryw4nwoe0hspgcf/Experiment%20Data.xlsx?dl=0) to view the experiment data.

In the file, separate tabs have been created for each problem description. The first tab displays the summarized results of model extraction and traceability.



## Instructions to use the tool
Our tool is composed of two sub-systems - (1) backend and (2) frontend. These sub-systems are further composed of microservices that are responsible for various tasks such as model extraction using pre-trained ML and language models and construction of traceability knowledge graph. These microservices are currently deployed on the Heroku cloud where they communicate with each other based on users' requests. Due to the size limitation on the Heroku cloud, we currently deploy the small-scale spaCy [language model](https://spacy.io/models/en#en_core_web_md). 

As mentioned in the response letter, our tool is up and live now. It is available [here](http://modelling-bot.herokuapp.com/). However, due to memory run-time issues during deployment, only limited features are working. Therefore, to give an overview of our tool, we have also prepared a [video](https://www.dropbox.com/s/96y5a7t9eyz57au/modelling-bot-demo.mp4?dl=0) while running our tool locally. In this video, we demonstrate how we extract domain models for given problem descriptions and trace the modelling decisions of extracted model elements. The modelling decisions are presented in the form of highlighted sentences and words. In addition, a rationale explanation is provided in some cases inside the chat widget. In this [video](https://www.dropbox.com/s/96y5a7t9eyz57au/modelling-bot-demo.mp4?dl=0), we use a sample problem description as mentioned below:

**Problem Description** - _Students can be part-time students or full-time students. Each student is identified by an ID and an email. Different multiple projects can be assigned to a student. Each project has a title and a deadline._

Also, the tool should take a few seconds initially when our application's dyno on the Heroku cloud is asleep. After the first few hits, the application's response time will be quick.


