# WhatsApp-Chat-Analysis
![Screenshot 2022-10-17 013058](https://user-images.githubusercontent.com/110452335/196062266-1fc1040d-2b9a-4cf1-8290-739464193cdd.png)

# 30 Days Analytics Learning WhatsApp Group Analysis
The last project I worked on during the 30 Days of Analytics Learning.

# Introduction
WhatsApp is one of the trendy social media platforms in the world today. Most social media users use WhatsApp since it is a more manageable communication platform and has attractive features. Also, the platform offers flexible and fast communication to individuals and groups, allowing sharing of different media. A WhatsApp group is where people are invited, and the invited people can chat. In the 30 Days Analytics Learning Group, Samuel Iheagwam created the group and invited the rest of the members.

# Project Overview
The project aims to identify the group's most active users, most active days, and frequently used words.

# Data Sourcing
I exported the group [chat data]( https://drive.google.com/file/d/1z8A4GaIZMu7WO4GNN1qi9qWrzFHgnzeF/view?usp=sharing) from the 30 days of Analytics Learning group, 
which was saved as a text file. The dataset was in one table that contained 1105 rows and two columns containing the group chat data. 

# Data Cleaning
## Microsoft Power BI
I cleaned the data using the power query editor and the Power BI desktop to visualize the insights from my Analysis.

# Data Cleaning Process
Data cleaning is a process that prepares data for Analysis by removing and modifying incorrect, irrelevant, incomplete, improperly formatted, and duplicated data.

## Cleaning Processes
After importing the data to Power BI as a text, I transformed it based on the entire dataset.

I Removed blank rows since the first and second columns had empty match rows. Then, I split the first column from Digit to Non-Digit and merge columns 1.2 and 1.3 (Month and Year).

Split column 2.2 by delimiter (custom -) and renamed column 2.2.1 as Time. I then split column 2.2.1 and renamed it as Members. From the members' column, I unchecked data that contained "Mr. Samuel removed…" and then removed the empty rows because any data from the chat would be due to active members (When I matched the blank rows with other data columns, they were also empty).  

I renamed Column 2.2.2 as messages, merged columns 2.23, 2.3, and 2.4, and renamed them Media. I then removed column 1.1.1.1.2, which was now empty.

I then merged the current first column (Day) and the second column (Month Year).

I added a new custom column from Date from the column tab and renamed it Day of Week. I then replaced the values (0-6) with (Sun to Sat), respectively.
## Power Query
The data was then loaded to the Power BI desktop for visualization.

## Power BI Desktop
I created the following DAX measures to help in visualization; Active members, Date1, Days, and Messages Sent.

# Analysis
I drew the following insights from the loaded data;
1.	Top 5 most active members in the group.
2.	Messages sent on each day of the week.
3.	Messages sent by Date.
4.	Frequently used words in the group.

[Interact with my Dashboard and report here]( https://drive.google.com/file/d/1l-BN9gYuNBitEm-GI2WNGYsDBvRyYtT5/view?usp=sharing)

# Conclusions
1.	The group had 13 active members for 19 days.
2. Group members were inactive on the 27th and 28th of August, 2022.
3.	Mr. Samuel and Divine were the most active users in the group.
4.	The most active day in the group is Monday.
5.	Apart from the articles and pronouns, the most frequently used words are "attached" and "File."
	

