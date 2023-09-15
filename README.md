# ProjectTypeClassification Finetuning DistilBert
Classify Project type with fine tuning a transformer model (DistilBert)

## 🤔 What is this?
**Description:**  How to know the type of IT projects/contracts (Services) that have been carrying out in the Portuguese Public Administration?.
In addition to project values, what type of projects have been developed and by whom? What is the competition and what type of services do they focus on? Strategic Digital Transformation Consulting; in Project Management/PMO; in Requirements Gathering/Analysis or Architecture; in Project Implementation; in Support/Maintenance; in Change Management; or in SaaS?

It involves the research and design of Artificial Intelligence algorithms, in this project we will be fine tuning a transformer model (DistilBert) for the **Multiclass text classification** problem.
Given a Project description the model will classify into one of the project categories out of the given list.


## 📚 Data

Data with the projects (to train the model and to apply the model) are in data dir.
 
We are using Project Descriptions from   Portuguese Public Administration site of Contract  aggregator dataset available at [base.gov Repository](https://https://www.base.gov.pt/base4).

Please bear in mind that this data has already been cleaned and processed: `ContratosAP_v5.2_TrainPred.xlsx`.

Dataframe `DadosTreinoVal` has `751` rows of data to train and test.  Where each row has the following data-point:
	
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


Due to the power of GPU needed i advise you to use colab with `ClassifyContratType_TransformersFineTunEx_v2_colab.ipynb`(in classification dir)

copy data (in data dir) `ContratosAP_v5.2_TrainPred.xlsx` to sample_data.


Run


## 📖 Documentation

Please see the description in .ipynb about this project.




##  🚀 Results (Applied AI vs Transformers)

Having in consideration that we have few data (751 projects) to fine tune the 8 project categories, we´ve understood that distilbert focus on the categories with more data, so we only managed to obtain about 50% acurracy (for instance with Support Linear Classifier - SVC - Applied AI, with the same data to train we manage to obtain 84% acurracy).
