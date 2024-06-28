# openaihackathoneyjune24-groupA

**Problem statement**
Develop a generative AI model that can assist healthcare professionals and patients in the early detection and diagnosis of various types of cancer by analyzing reported symptoms and medical history. The model should be capable of processing natural language input to identify patterns and correlations between symptoms and specific cancer types. It should provide a probabilistic assessment of potential cancer risks based on the input data, thereby facilitating timely medical intervention and personalized care plans.

**Collecting Data:**
We collected open data from https://www.kaggle.com/datasets/falgunipatel19/biomedical-text-publication-classification.
For Biomedical text document classification, abstract and full papers(whose length less than or equal to 6 pages) available and used. This dataset focused on long research paper whose page size more than 6 pages. Dataset includes cancer documents to be classified into 3 categories like 'Thyroid_Cancer','Colon_Cancer','Lung_Cancer'.
Total publications=7569. it has 3 class labels in dataset.
number of samples in each categories:
colon cancer=2579, lung cancer=2180, thyroid cancer=2810
We have divided the data sets into multiple sets. So that the dats is easy to index.


**Building RAG with your own Data**
We have used azure open ai playground to deploy gpt-35-turbo-16k model and datasource with upload options into the storage account. We have give the system a message of "You are an AI assistant that helps people find information related different types of cancers"
![image](https://github.com/arunps27/openaihackathoneyjune24-groupA/assets/73843760/76e5e5f0-c2b7-4d52-a2ef-c5e9e04db3e5)
![image](https://github.com/arunps27/openaihackathoneyjune24-groupA/assets/73843760/72e54219-cdce-4d2a-a374-0e15ec894842)


**Deploying the Model and Consuming in client application**

We used webapp deploy option available in playground with B1 tier, which was then deployed to https://group1hotelsuggestions.azurewebsites.net/

**Examples:**

We have tried following examples and system started responding with right results with citation.

1. Define colon cancer
![image](https://github.com/arunps27/openaihackathoneyjune24-groupA/assets/73843760/92704286-13ed-4f83-b6e1-433c1f5880d6)

2. what is lung cancer
![image](https://github.com/arunps27/openaihackathoneyjune24-groupA/assets/73843760/00970dac-8008-4b1f-a6ce-0d1b49e7ffc4)

3. Common Symptoms of lung cancer
   ![image](https://github.com/arunps27/openaihackathoneyjune24-groupA/assets/73843760/4333f60a-88a1-4031-9ad9-a154989d19fd)

