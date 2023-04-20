# propensity_groups_using_voter_models_trainV---company_project
Creates customer propensity groups using several voter algorithms

Creating customer propensity groups according to their sale probabilities was an important tool for our models. Using these bins in our modeling processes increased the gain percentage significantly, and also increased the consistency of these models. It is an ad-hoc project, periodically ought to be triggered, these updated scores ought to be used on production other than old scores. 

There are 2 types of scripts for this project, one is for training the models and the other one is for making inferences on lookup values of customers, in order to use it on production.

Model is based on binary classification mainly, it uses several classification algorithms, ranks them, selects the top N performers among them and uses their predictions to create customer propensity groups. 

Tried to construct most of the features inside script parametrically, set at configuration section. Several preprocessing sections are applied, an embedded feature selection section is available inside the pipe, also a GridSearchCV section is embedded during training of the algorithms. 

All model results, selected best models, settings, bin values etc. are saved into dynamic model folders automatically. And for the inference part, we can reach to them via same folder with a simple setting. 

*There are also 2 more variations for this pipeline. One is using Stacking algorithm at the end, creating a final prediction from meta predictor ML algorithms. 2nd one is using an ANN pipeline to create customer bins. These scripts will be added too.

** Since it was a company project, and working due to time constraints, some development steps were skipped. This script will need a functional structure, some of the cells need to convert into functions, and need to be called from source files. 

*** Since it is an ad-hoc, and non-frequent script, it doesn't need an MLOPS structure. It can be handled manually, or with simple cron jobs. For further requirements, it will need to be converted according to MLOps requirements. 


