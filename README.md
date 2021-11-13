# Employment and Wage Data Project

**Setting** 

One of my good friends informed me that he would be unable to come to town to watch a movie because he would be busy all weekend inputting data into a project for his dissertation. I jokingly asked if he would like some help, and he took me up on my offer. We hopped on a Zoom call late that night to go over the project and what he would need done. He initially indicated 1) that we would have to manually input this data and 2) that he needed approximately 2,000 pieces of data. He suggested that we split the task up between us to tackle it given the scope of how much data we'd have to look up and enter.

However, during our discussion, it became evident to me that there was a better way to approach the problem by collecting/aggregating the data and using Microsoft Excel to lookup the data he wanted, so I informed him that I could gather the data and create what he wanted without manual entries, which are prone to human error, and that I could do it in about four hours. After our discussion late Friday night, I was on a mission to get him a finished product before he woke up the next day so that he did not have to worry all weekend. 

Not only did I exceed his expectations, but I provided a flexible and adaptable model he could use to view additional information, which he ultimately needed. We ended up watching a movie that Sunday thanks to my work.

**The Ask**

I was tasked with gathering the weekly employment ("WKEMP") figures and the average weekly wage ("AVGWG") (from the fourth quarter data) for two years prior to the base case year and two years after the base case year for 493 counties among 8 different states with base case years from 2005 through 2019. I was provided with an Excel sheet with two tabs - "Original Sheet" and "Subsidy Pivot".  The "Original Sheet" tab had all of the base case year data filled in for both WKEMP and AVGWG with only a handful of each of the data points I needed to obtain.

**My Approach**

1. The BLS site from which he needed data provides CSV file downloads for all counties in a particular state per year. As such, my first step was to grab all CSV files from the 8 states for all 18 possible years needed (from 2003 through 2020 as that was the last full year of data available).

2. I then aggregated those files into separate tabs within my Excel file with each state having its own tab ("AL", "GA", "KY", "MS", "NC", "SC", "TN", "VA"), which was crucial for later on when I wanted to reference those sheets.

3. After aggregating the data, I performed multiple tests to confirm that I copied and pasted the bulk data over correctly. These tests confirmed that I did have the correct data and can be found in the "Data Integrity Testing" tab. 

4. Once I confirmed the integrity of the data, I was ready to look up the data with VLOOKUPs in the "Main Data" tab.  However, I also had to clean up the county names my friend had inputted because they started with the state abbreviations, so I used a simple REPLACE formula to remove the first two letters. I also had to create unique identifiers for the datasets and the "Main Data" tabs because I was looking up information based on multiple values (i.e., county AND year).  As such, I just concatenated those two values to arrive at the Unique Identifier. 

5. I ultimately created the attached "Main Data" sheet, which enabled my friend to view more than just two years before and two years after the base case years. This was critical as the next step in his project was calculating a compound annual growth rate ("CAGR") for which he needed to reference different years. The model also looked up the correct data for the base case years without worrying about human error in transcribing those pieces of data.

6. Once I completed the Excel model, I included an "Error Check" tab to illustrate how manual entry is prone to errors. I compared the data he had originally provided me and what I pulled from the data sets. This showed 25 errors, 23 of which were in entries for base case years - i.e., years I was not tasked with inputting!

After completing the above in a few hours, my friend was extremely grateful, and I am glad I was able to help him solve a problem by producing something that he could be confident in using.

Take a look at the model and what I did!
