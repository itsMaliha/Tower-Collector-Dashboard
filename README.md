![Capture](https://user-images.githubusercontent.com/70474312/177979794-919ad842-7399-4986-8ca2-ffa19e04e6f2.PNG)
Here is an interactive dashboard that lets you analyze your cellular logs data from the app Tower Collector! The dashboard focuses on mainly signal strength as the metric of evaluation however the data collected from this application is super rich and can be used for a variety of purposes.

<h2>Open Cell Id</h2>
Before we move on to what Tower Collector actually does, its important to talk a bit about Open Cell Id. It is an initiative presented by Unwired Labs and is a collaborative community project that collects GPS positions of cell towers and their corresponding location area identity. More than 49,000 contributors are registered with OpenCellID, contributing more than 1 million new measurements every day on average to the OpenCellID database. As of August 21, 2017 the database contained 35.5 million unique cells and 2.1 billion unique measurements. OpenCellID publishes an aggregate data set of cell locations licensed under a Creative Commons Attribution-ShareAlike 4.0 International License with the intention of promoting free use and redistribution of the data.

Data on Cell IDs and their locations can be used to provide location information to mobile devices. Using Cell ID locations to find device location is more power efficient and often faster than using satellite-based navigation systems, although it is less precise because of the lack of known Cell IDs.The database is also used to determine the strength of available wireless connections and which mobile phone service providers have coverage in specific geographic locations.

Take a look at this OpenCellId heatmap from 2013.
![image](https://user-images.githubusercontent.com/70474312/177980763-35d1d228-ccf6-4b8f-82f2-e9a4454f9181.png)

<h2>Tower Collector</h2>
Among other applications, Tower Collector is also an app used to contribute to Open Cell Id. It also allows you to keep track of your data based on numerous features such as mcc, mnc, cell id, device etc.

Here is a small snippet of some features gathered from the application.
![image](https://user-images.githubusercontent.com/70474312/177981411-e5061ec3-0190-49fa-ba4f-5225e395e469.png)

<h3>Data Processing</h3>
Before moving to the actual visualization, we need to process our data. 
<h4>mcc and mnc</h4>
Here the mcc gives the mobile country code and since all of my data was from Pakistan I did not decode this feature however the mnc - Mobile Network Code represented the arious networks I was in contact with. Initially it is represented by numbers if you look at the snippet above. To address that I created a column using Power BI's conditional column and decoded the data to the different networks in question. 
