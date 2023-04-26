# Capstone for Nashville Software School Data Analytics Program
<p align="left">Completion date: April 28, 2023</p>

# <p align="center">Redlining In Tennessee</p>

## Table of Contents
1.	History
2.  Motivation
3.	Data Question
4.	Methodology
5.	Technologies
6.	Data Sources

## History
Redlining is the illegal and discriminatory practice of the denial of services like (i.e. mortgage loans) based on race. The term “redlining” originates from the New Deal policy put into effect by President Roosevelt in 1933. Off the heels from the Great Depression, there was a housing shortage. The federal government sponsored a program that was designed to increase segregation amoung American’s Real Estate. In 1934 the Federal Housing Administration was created to spearhead this initiative along with the Home Owner’s Corporation which classified mapped areas by color: 
#### •	Green (Best) 
#### •	Blue (Still Desirable)  
#### •	Yellow (Declining)
#### •	 Red (Hazardous) 
Homes in the red were not insured by the Federal Government. Federal Housing Administration also was subsidizing builders who were mass-producing entire subdivisions for whites — with the requirement that none of the homes be sold to African-Americans. Restrictive covenants were placed on the deeds which included provisions used to discriminate against all manner of racial and ethnic groups, most commonly African Americans but also Asians, Latinos, and Jews. 			

Racially restrictive covenants came into being as a private method of maintaining racial separation. However, in 1948, Federal Courts ruled in Shelley v. Kraemer racially restrictive covenants unconstitutional; individuals could enter into such contracts, but courts could not enforce them. In 1968, President Lyndon Johnson signed into effect the Fair Housing Act which prohibits discrimination regarding the sale, rental, and financing of housing based of race, religion, national origin, sex, handicap, and family status. Racially restrictive covenants on deeds were deemed illegal, however, such language can still be found on deeds today. 				

As a result of redlining, whites moved to the suburbs, leaving non-whites in the downtown urban areas of the city. In 1954, a federal policy known as urban renewal was established by the Housing Act, which created new requirements for cities to develop actionable revitalization plans. Federal funding is provided to cities to improve the attractiveness and property values of specific geographic areas rather than improving the lives of the residents. This term is called “sum clearing,” which is widespread displacement and dispersal of historical communities with deep social ties. Urban renewal projects use eminent domain to acquire private homes that were usually deemed sub-standard. Oftentimes the homeowners were promised they would be compensated for their property and helped with relocation, however, in many cases, homeowners didn’t see any assistance. They became renters without receiving a fair market value for their seized properties. Residents who lost their homes were forced to live in outlying areas putting them further away from jobs, transportation, and social spaces.
## Motivation 
By trade, I have spent close to 2 decades within Mortgage Underwriting. I have seen cases of disparate impact on borrowers due to policies and procedures utlitized by mortgage originators in effort to "hedge risks". I am also an African American homeowner and a lover of history. We see as a nation the impact that discrimination on certain ethinic groups can have upon the entire society. My motivation and quest is to determine if the concept of redlining (in its various forms) are still occuring today. 
## Data Question
The old saying goes “history always repeats itself.” Could it be that redlining is occurring again in Nashville and Memphis, TN under the guise of gentrification?
## Methodology
### Gathering the Data
I started in search of a definition for redlining to refresh my understanding and the scope of this issue. I looked to multiple peer review articles and journals regarding redlining in the U.S. and specifically the state of Tennessee along with its implications throughout the years. By law, financial institutions must maintain, report, and publicly disclose loan-level information about mortgages. HMDA is the Home Mortgage Disclosure Act which was enacted in 1975 by Congress and is implemented by Regulation C. I was able to pull HMDA datasets for the state of Tennessee through their website. 

I decided to investigate Nashville and Memphis because these are the two largest cities in Tennessee, also both cities have a very historical presence. Laws and policies from these cities have shaped how we live today. I was able to pull data from the U.S. Census Bureau and Data U.S. regarding Nashville (Davidson County) and Memphis (Shelby County). 					
### Cleaning the Data
I decided to stick with definitive responses when looking at the derived race. For derived race I excluded data for “Free From Text Only”, “Joint”, and “Race Unavailable,” as I am unable to determine the race of these borrowers. 						

Alhtough the data for declined applications is small relative to the amount of applications that were approved, the purposes of this analysis is to dive into the reasons for the denials. For the denial reasons, I exclude “NA” because this is an approved application. 

I was able to pull a map from the 1930s drawn by the Home Owner’s Loan Corporation that revealed that Downtown Memphis-38103, South Memphis-38106, Orange Mound-38114,	Binghampton-38112, Frayser-38127, North Memphis-38107, Parkway Village-38118 were deemed "hazardous". For Nashville East Nashville-37206 and 37216, North Nashville-37208 and 37207, South Nashville-37211 and 37204, Germantown-37208, Edgehill-37212, Hadley Park-37208 we deemed “hazardous.” 

I was able to pull a Building Permit Issued dataset from Nashville.gov. Although I did not dive deep into this topic, it is still one of interest worth conducting a meaningful analysis. The data covers a 3 year period, therefore, I believe in order to determine any trends or points of interest more data is needed (a 10 year period at minimum).  
### Analyzing the Data
From the HMDA dataset the data is for the year 2021 and it is includes data gathered from The majority of the mortgages are conventional. 
The top 40 banks and financial institutions took 345,273 (61.17%) applications in 2021, but the remaining institutions took 219,138 (38.83%) applications in 2021. I considered banks and financial institutions that were considered major players in the mortgage industry. 
### Visualizing the Data
As part of the exploration analysis stage, I used Matplotlib and Seaborn in Python. I used Tableau to complete the analysis. 
## Technologies
1.	Python  for  pandas, numpy, seaborn, matplotlib
2.  Tableau for visualizations
## Data Sources
•	Rothstein, R. (2018). The color of law: A forgotten history of how our government segregated America. New York: Liveright Publishing Corporation, a division of W.W. Norton & Company.

•	Public Use Database-Federal Home Loan Bank System: Public Use Databases | Federal Housing Finance Agency (fhfa.gov).  

•	Federal Reserve Bank of St. Louis- 30-Year Fixed Rate Mortgage Average in the United States: https://fred.stlouisfed.org/series/MORTGAGE30US

•	https://ffiec.cfpb.gov/data-browser/data/2021?category=states&items=TN

•	https://worldpopulationreview.com/states/tennessee/counties

•	https://nowandthen.ashp.cuny.edu/2010/02/segregation-in-deed/

•	https://www.hud.gov/program_offices/fair_housing_equal_opp/aboutfheo/history

•	https://nowandthen.ashp.cuny.edu/2010/02/segregation-in-deed/

•	https://www.planetizen.com/definition/urban-renewal#:~:text=The%20federal%20policy%20known%20as,to%20develop%20actionable%20revitalization%20plans.

•	https://datausa.io/profile/geo/shelby-county-tn?compare=davidson-county-tn

•	https://www.lei-lookup.com/record/?keyword=549300FNXYY540N23N64

•	https://www.zillow.com/research/data/

•	https://www.highgroundnews.com/features/SeeingRedlining.aspx

•	https://data.nashville.gov/Licenses-Permits/Building-Permits-Issued/3h5w-q8b7

•	https://www.washingtonpost.com/business/2020/10/23/redlining-black-wealth/




