# Flight-Analysis-using-Pyspark

I will explore and analyze the ‘airline-delay-and-cancellation-data-2009-2018’  dataset, using the appropriate technologies and methodologies, to expand and  further understanding the data.

NB#

Data was extracted and placed onto linux based system and then Hadoop (HFDS): HDFS, or Hadoop Distributed File System, is a distributed file system that runs on commodity 
hardware. 

Analysis completed on Pyspark - PySpark is a Python interface to Apache Spark. It includes the PySpark shell for interactively examining data in a distributed environment, as well as the ability to develop Spark applications using Python APIs. Most Spark technologies, such as Spark SQL, DataFrame, Streaming, MLlib 
(Machine Learning), and Spark Core, are supported by PySpark.


DATASET

Data taken from Harvard Dataverse: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/HG7NV7
The dataset consists of flight and departure details for all commercial flights within the United 
States, from 2009 to 2018

The data used consists of Airline on-time data. Every two years, at the Joint Statistical Meetings, 
the Graphics Section and the Computing Section collaborate every two years during the Joint 
Statistical Meetings to host a special Poster Session named The Data Exposition, but more 
generally known as The Data Expo. 

NOTEBOOKS

Notebook 1: Exploratory Data Anlysis to gain and understanding of the data – using DataFrame and SQL functionality

Notebook 2: Machine Learning using Random Forrest  & Machine Learning using Logistic regression Model

The Random Forrest Classification gave me 79% accuracy, and test error 20%. I believe with time I could have increased this number, or possibly looked at a different classification tool such as binary – which I think would have been cleaner and more concise. I used the model to predict Distance and Airtime based on Carrier – with the features being our categorical columns Origin, Destination and Carrier.

The Logistical Regression Model scored a little better – focusing on a more binary prediction on Cancellations based on state. I thought about removing this model asit didn’t quite turn out as I planned but left it there simply to show the process.

In relation to both models, I used this the same encoding and Indexing process as taken from the databricks official website, and then the same vector assembler to combine all the feature columns into a single vector. The pipeline methodology was the same also, the output was then used to feed the algorithm.

