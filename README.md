# Chicago-Crime-Rate using FbProphet

This project analysis the Chicago Crime Rate from 2001 to 2017, and how the crime rate is influenced by month of year, location, etc. I have also used FBProphet to make prediction in the future. The dataset can be downloaded from: https://www.kaggle.com/currie32/crimes-in-chicago.

## About Dataset

Dataset contains the following columns:
1. ID: Unique identifier for the crime incident.
2. Case Number: Records Division Number assigned to the incident.
3. Date: Date when the incident occurred.
4. Block: Block address of the incident.
5. IUCR: The Illinois Unifrom Crime Reporting code.
6. Primary Type: The primary description of the crime according to IUCR code.
7. Description: Secondary description of the incident.
8. Location Description: Description of the location where the incident occurred.
9. Arrest: True or False if convict was arrested.
10. Domestic: True or False if incident was domestic related.
11. Beat: A beat is the smallest police geographic area – each beat has a dedicated police beat car.
12. District: District where the incident occurred.
13. Ward: The City Council district where the incident occurred.
14. Community Area: Chicago has 77 community areas.
15. FBI Code: Crime classification according to FBI's National Incident-Based Reporting System (NIBRS).
16. X Coordinate: The x coordinate of the incident.
17. Y Coordinate: The y coordinate of the incident.
18. Year: Year the incident occurred.
19. Updated On: Date and time the record was last updated.
20. Latitude: The latitude of the incident.
21. Longitude: The longitude of the incident.
22. Location: The location of the incident

Dataset contains a total of 7,941,282 entries for a span of 16 years.

## Data Analysis

### Crime Rate - Yearly

![image](https://user-images.githubusercontent.com/50113394/126898208-b4b52078-d6da-4f39-84d9-b72855c91013.png)
The Crime rate rose after 2005 but drastically decreased after 2010, and decreased continuously after that at a slow rate.

### Crime Rate - District

![image](https://user-images.githubusercontent.com/50113394/126898284-c579bacc-21b8-48a0-ae4b-322d5c219c74.png)
Highest crime rate in district 8, and lowest in district 20. (District 13, 21, 23 and 31 have zero crime rate, might be because of incomplete data)

![image](https://user-images.githubusercontent.com/50113394/126898355-f2e6d54e-2515-4a4c-b994-fcbc80f0004b.png)
The graph provides a district analysis of Chicago city.

### Arrests & Domestic Incidents

![image](https://user-images.githubusercontent.com/50113394/126898381-4743cbb0-a6cb-49e6-a7de-6bb78799ebad.png)

![image](https://user-images.githubusercontent.com/50113394/126898398-58209dd4-1d07-4dd3-ab13-38c4564f5104.png)

### Most Common Crimes

Most common type of crime is theft, followed by battery and criminal damage.
![image](https://user-images.githubusercontent.com/50113394/126898593-739c4e96-3cc7-4ea1-9734-66fbe0e793f3.png)


### Most Common Crime Locations

The most common crime location is the streets, which is almost twice than sidewalk. 
![image](https://user-images.githubusercontent.com/50113394/126898433-88e7dabc-a55f-4cb3-8eea-7948ad610ba5.png)

## FBProphet - Result Analysis

Prophet shows a decrease in crime rate in 2017, and show overall negative trend in number of crimes since 2010.
![image](https://user-images.githubusercontent.com/50113394/126898444-252682f7-31cb-4751-bae1-56f0b4812f80.png)

Prophet shows higher crime rate in the months from March to May and, lower in months from Novemver to January.
![image](https://user-images.githubusercontent.com/50113394/126898452-27d0b52a-ec31-4966-9627-f44186e01b10.png)
