MASTER DISSERTATION «APPLICATIONS OF MACHINE LEARNING IN MICROBIOME DATA»

**Introduction**

The data used in this postgraduate thesis were from the Earth Microbiome Project by Thompson et al., 2017. Specifically, the EMP-wide sample metadata was used, available at the following link: http://ftp.microbio.me/emp/release1/. Additionally, the results derived from the bioinformatics analysis conducted by the researchers can be found at the link: https://zenodo.org/records/890000.

Initially, a bioinformatics analysis was conducted for practice purposes on 5 random samples from the EMP-wide sample metadata on the Galaxy Europe bioinformatics analysis platform using the QIIME 2 tool, which is recommended for microbiome data analysis.

However, the purpose of this thesis was to create a prediction model that would classify the data based on the empo (empo_1, empo_2 & empo_3) representing different categorizations or properties of the samples according to the Earth Microbiome Project Ontology. The construction of such a model is of vital importance as the volume of the data is vast, and it is not easy to classify new data that emerges and pertains to the microbiome present in the environment. For the construction of the models, various algorithms were tested, such as Random Forest, Logistic Regression, due to their simplicity and their ability to handle large volumes of data. Additionally, Gradient Boosting and XGBoost were tested due to the high accuracy they offer.
