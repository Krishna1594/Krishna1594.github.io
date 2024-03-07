---
name: Commodities & Pesticides Data Project 
tools: [MySQL, Tableau, Dashboards, Data Analysis, Article Writing]
image: [https://i.postimg.cc/j54RN0H9/dashboard-final.png]
description: An analysis on ~11000 food commodity samples collected by USDA approved agencies to monitor the residue of pesticides concentration before the commoditiy reaches consumers. Analysed over 2 million test results of the samples, tracking key parameters such as origin, pesticide tolerance levels etc.
---

![Preview](https://i.postimg.cc/SKtvvZys/9807.jpg)

# Commodities & Pesticides Data Project

I met lot of farmers in my country in my life. I think I had to hear the farmer's point of view in using any pesticide in agriculture. I asked, "Why do you think it is important to use pesticide?". I was expecting some technical answer such as "peticide kills insects or algea that harm our crops", But he said with a sense of responsibility and concern in his eyes, "If I don't use pesticides, the amount of food I produce will not be enough to feed all my citizens". That was a moral and accountable answer. It is true that population is increasing, at least in India. So basically, they pesticides help farmers grow more food on less land by protecting crops from insects or pests, diseases and weeds as well as raising productivity per hectare. 

We didn't talk about health concerns and that's where government and organizations come into picture. We as consumers undermine the damages of using pesticides, we should be aware nonetheless. I am talking about damages to health and balanced diet. Organizations like USDA ensures that it is safe for consumers to consume a food product/commodity but at the same time, ensure a good practice of usage of pesticides by farmers. Such organizations have a significant responsibility providing knowledge to farmers in terms of increasing technology and safe practices in agriculture and creating awareness among consumers about the product. 

I think one of the reasons that USDA made this data available to public is to make sure consumers know what they are eating and ensure safe dietary exposure to consumers.

## The Data
The data is publicly available [here](https://www.ams.usda.gov/datasets/pdp/pdpdata). I used the latest datset (2022) for this analysis. The 2022 PDP dataset contains data dictionary, reference tables, samples data and results data. It hosts a comprehensive dataset and I decided to make an amazing database with this data.

### Database
The file size says it all. I immediately recognized I won't be able to work on this data on MS excel since this tool has 1,048,000 row limit but, the datsaet has like ~3 million rows. I chose MySQL workbench. I can connect tables, access data from multiple tables and bring data to life.

#### Importing Data
The main data is in text file and reference tables hold various information regarding the dataset. I separated each sheet in the reference date excel file into multiple excel files so that I will be able to upload into my database. Before I could do anything, I had to provide access/permissions to my server;

<script src="https://gist.github.com/Krishna1594/ea5f26be3019b4bf9e0f3ad1596c3029.js"></script>



### Stored Procedure for calculating KPIs

### EER Diagram of the Database

## Analysis and Visualization

