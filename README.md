Predictive Modeling of Data Exhaust in Voice Assistant Network Traffic Data

For this analysis, we used PCAPs published in teh paper namely "Amazon Alexa Traffic Traces" dataset (2022) by Barcel et al.
Barceló-Armada, Rubén, Ismael Castell-Uroz, and Pere Barlet-Ros. "Amazon Alexa traffic traces." Computer Networks 205 (2022): 108782.

For the next step, we used CICFlowMeter. 
Lashkari, Arash Habibi, et al. "Characterization of tor traffic using time based features." International conference on information systems security and privacy. Vol. 2. SciTePress, 2017.

CICFlowMeter is a network traffic flow generator distributed by CIC to generate 84 network traffic features. It reads pcap file and generate a graphical report of the features extracted and also provides csv file of the report. It is an open source application written in Java and can be downloaded from Github.
So, we created the dataset which is all the NTD of an Amzon Alexa Echo Dot, and then we labled all the datapoints based on the name of the commander and the correspanding content of the command. 
Then, we started our analysis and the Classification. Among all the mthods, we git the best reults from RF. Then, creating a new dataset from all the missclassified datapoints, we assume that by applying a clustering method, one cluster should be considered as Data exhaust as they are not being generated either by the commander or based on the user's command.
