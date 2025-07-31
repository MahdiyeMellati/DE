# DE
Data Exhaust 

For this analysis, we used PCAPs published in teh paper namely "Amazon Alexa Traffic Traces" dataset (2022) by Barcel et al.
Barceló-Armada, Rubén, Ismael Castell-Uroz, and Pere Barlet-Ros. "Amazon Alexa traffic traces." Computer Networks 205 (2022): 108782.


Using CICFlowMeter. CICFlowMeter is a network traffic flow generator distributed by CIC to generate 84 network traffic features. It reads pcap file and generate a graphical report of the features extracted and also provides csv file of the report. It is an open source application written in Java and can be downloaded from Github.
So, we created the dataset which is all the NTD of an Amzon Alexa Echo Dot, and then we labled all the datapoints based on the name of the commander and the correspanding content of the command. 
Then, we started our analysis and the Classification. Among all the mthods, we git the best reults from RF. Then, creating a new dataset from all the missclassified datapoints, we assume that by applying a clustering method, one cluster should be considered as Data exhaust as they are not being generated either by the commander or based on the user's command.
