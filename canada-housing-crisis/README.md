# Canadian Housing Crisis Analysis

I am glad you are here. Here is a brief breakdown of the project's scope. It is still under construction and MVP 1 is completed. There will be multiple analysis for the housing crisis in Canada which will follow the industry standard MVP style

# Table of Contents

## MVP1

This analysis utilizes two datasets downloaded from Government of Canada's open data portal, related to the housing crisis in Canada. Please download the following datasets and place them in the appropriate directory:
1. **Immigrant Population Data**: The dataset containing information on the number of immigrants in various regions of Canada is also sourced from [immigrant-status-and-period-of-immigration-e](https://open.canada.ca/data/en/dataset/9adddd8a-e15b-497c-86af-641457a78bea/resource/255012de-7f8a-4f5e-b62a-bc438dc89543)
2. **House Prices Data**: The dataset containing information on house prices across different regions in Canada is sourced from [New housing price index, monthly](https://open.canada.ca/data/en/dataset/324befd1-893b-42e6-bece-6d30af3dd9f1)

- [Analysis](#mvp1-analysis)

## DATA: 
The immigration data contains 3 time bins i.e 'Before 1996', '1996 to 2005' and '2006 to 2011' -  To analyze the trends, the data needs to be normalized. Housing data conatins information on per month basis so the immigration data has be to converted into similar format. The first bin i.e. 'Before 1996' does not have a start date; I followed up with the official about the start date and they responded the start date is not avaialble. Quote: "For the start year for Before 1996, this is every person in Canada aged 15 years or over and who was still living during that Census in 2011 and immigrated before 1996. So it would go back a long time, some people could have been in their 100s when they filled this and came to Canada a very long time ago when they were children." You can reach out to the official at groupederecherchesurlespol-polresearchgroup@pch.gc.ca

- Since the data can not be normalized for the first time bin in immigration dataset i.e 'Before 1996', I have extracted the number of Immigrants in Canada uptil December 1995. The analysis period will be from December 1995 till 2011. 
- I have normalized the other two time bins by dividing the total number of immigrants by the number of months.
- For 1996 - 2005, there are 10 years x 12 months/year => 120 months
- For 2006 - 2011, there are 6 years x 12 months/year => 72 months
- Now we have house prices and number of immigrants on monthly basis for Canada
- Since I know how many immigrants were in Canada as of December 1995 and number of immigrants on monthly basis. I performed cummulative sum to get the total number of immigrants for each month uptill 2011. 
- After preprocessing and cleaning, the data is merged for analysis

  
- [Results](#mvp1-results)



- [Future Work](#mvp1-future-work)

## MVP2
- [Overview](#mvp2-overview)
- [Analysis](#mvp2-analysis)
- [Results](#mvp2-results)
- [Future Work](#mvp2-future-work)

## MVP3
- [Overview](#mvp3-overview)
- [Analysis](#mvp3-analysis)
- [Results](#mvp3-results)
- [Future Work](#mvp3-future-work)
