# ProjectTypeClassification
Classify Project type with NLP and ML

## 🤔 What is this?
**Description:**  How to know the type of IT projects/contracts (Services) that have been carrying out in the Portuguese Public Administration?.
In addition to project values, what type of projects have been developed and by whom? What is the competition and what type of services do they focus on? Strategic Digital Transformation Consulting; in Project Management/PMO; in Requirements Gathering/Analysis or Architecture; in Project Implementation; in Support/Maintenance; in Change Management; or in SaaS?
It involves the research and design of Artificial Intelligence algorithms, namely Natural Language Processing (NLP) and Machine Learning (ML) that allow the extraction of relevant information, which convert textual data into vector spaces in order to be inputs into data models. ML that will classify each IT service project.


## 📚 Data

Data with the projects (to train the model and to apply the model) are in data dir.
 
We are using Project Descriptions from   Portuguese Public Administration site of Contract  aggregator dataset available at [base.gov Repository](https://https://www.base.gov.pt/base4).

Please bear in mind that this data has already been cleaned and processed: `ContratosAP_v10.0_All TrainPred`.

Dataframe "DadosTreinoVal" has `751` rows of data to train and test.  Where each row has the following data-point:
	
    - Objeto do Contrato: Contract Object
    		 
    - Contrato (Tipo): Type of Contract
    		 
   
Type of Contract to be able to classify IT project descriptions from Public Portuguese Administration into the following categories:		 
		 
     
     - Digital Transformation (0)
		 
     - Project Management/PMO (1)
		 
     - Requirements Definition/Analysis/Architecture (2)
		 
     - Implementation (3)
		 
     - Support/Maintenance (4)
		 
     - Change Management (5)
		 
     - Licenses (6)
		 
     - SaaS (7)


##  🚀 Quick Install

`pip install -r requirements.txt` #install environment.

copy data (in data dir) "ContratosAP_v10.0_All TrainPred" to c:\DadosAP.

run python or jupiter notebook file (in classification dir).


## 📖 Documentation

Please see docs dir for full documentation.

See document that explains the project (in Portuguese - from slide 24 to 43).
