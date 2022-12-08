# User Throughput Time Series Forecasting
                                                 
![image](https://user-images.githubusercontent.com/55108824/206439900-562b74c3-3827-4448-ab2b-d29d4212cc92.png)

# Understanding Data

The Data set has Average UE Downlink Throughput for 1 Market for the last 227 days. The average throughput means in a particular market how much is the average dl throughput an user is getting. The Market consists of thousands of Cellular nodes serving millions of users. The average throughput here is an average of those millions of users represented by Peak_UE_In_Connected_Mode in the data set. The other columns in the data are the KPIs that can impact the average throughput.

Telecom operator aim towards maintaining a minimum Throughput KPIs making sure on an average user gets x mbps of throughput. Time Series Forecasting can help in detecting if the throughput may go below that set threshold and operator can take appropiate action to resolve the situation.

**DATA** 

Data set has 9 Columns which are listed below.

DAY : Represents the DAY of the year when the KPIs were collected

MARKET : Market Name tells the name of the market the KPIs belong to.

UE_DL_Throughput_Mbps : DL Throughput is the average Download throughput perceived by users in that market. In a market there will be million of users served by thousasnds of Cellular Nodes

Peak_#_UE_In_Connected_Mode : Peak UE connected shows the number os users in that market who are using the cellular network

Downlink_Data_Volume_MB_Test : Gives the total volume downloaded by all the users

PRB_Util_DL_GT_90%: Tells the %of time when the Resource Block utilization was greater than 90%. More the resource usage the user throughput will reduce because of lack of resources.

PDCCH_Util_% : tell the % of PDCCH utilization

Weighted_Avg_PRB_Util_DL : Gives resource block utilization

CQI_Legacy_AllRanks: gives the Channel Quality indicator the users are seeing. Higher the CQI means users are in good radio quality and will enjoy better DL Throughput.


**METHODOLOGY**

![image](https://user-images.githubusercontent.com/55108824/206452016-df3e8622-a992-4386-9bdc-a4b6a752d27a.png)


**MODELING**

![image](https://user-images.githubusercontent.com/55108824/206452194-21af50ff-ce68-4252-a1c2-776a742c598e.png)

**ARIMA**

![image](https://user-images.githubusercontent.com/55108824/206525286-12347396-3244-43d9-845c-c8dc939a9657.png)

![image](https://user-images.githubusercontent.com/55108824/206525352-71132a0b-c09c-49c1-8bff-d874dc5ee1bb.png)

![image](https://user-images.githubusercontent.com/55108824/206525407-a96e855b-6cd0-4884-a89e-108d54d61c4c.png)

![image](https://user-images.githubusercontent.com/55108824/206525524-3e73fc93-d1f1-4943-b791-b770e62060da.png)


**XGBOOST**

![image](https://user-images.githubusercontent.com/55108824/206525716-9ff01200-cc8c-447f-9271-5742fc803510.png)

![image](https://user-images.githubusercontent.com/55108824/206525803-93ff0fc1-6e5d-4fae-9d04-f599017e25b4.png)

**LSTM**

![image](https://user-images.githubusercontent.com/55108824/206525880-71417392-f94f-4b1f-9277-a4bbff4a6863.png)

![image](https://user-images.githubusercontent.com/55108824/206526143-c92cbe5b-7edf-41f1-9585-93c165ad0705.png)


**CONCLUSION**

![image](https://user-images.githubusercontent.com/55108824/206525014-b917b533-b2ce-40eb-8a91-c13aec016ec8.png)



