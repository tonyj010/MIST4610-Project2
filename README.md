# Team 9 - U.S. Chronic Disease Indicators Analysis

# Team Information
Hailey Brakke (https://github.com/haileybrakke/MIST4610-project2)

Will Federer (https://github.com/willfederer10/MIST4610-project2)

Summer Sayedzada (put link here)

Tony Jimenez (https://github.com/tonyj010/MIST4610.git)


Ja’Khiyan Dowdy (https://github.com/jakhiyan0219-hub/MIST4610-Project2.git)

# Our Dataset

The dataset used for this analysis is the **U.S. Chronic Disease Indicators dataset**, obtained from Data.gov and originally compiled by the Centers for Disease Control and Prevention (CDC). This dataset provides comprehensive, state-level data on a wide range of chronic health conditions and risk factors across the United States. The dataset has 34 columns and over 300,000 rows. Data can be analyzed across several dimensions, including time (year), geography (state), health condition (indicator), and demographics. 

**Key Columns and Data Types:**      
Year (Numerical): The year data was collected   
Location (String): The U.S. state where data was collected   
Question (String): Describes the specific health indicator being measured  
Data Value (Numerical): The number associated with the specific health indicator   
Data Value Unit (String): Specifies the unit of measurement    
Stratification Category (String): Collects demographic information   
Stratification (String): Collects more specific demographic breakdowns within the category   
Geolocation (Geographic values): Specifies the exact location data was collected   

We are basing our analysis on **geographic variation and demographic disparities in colorectal cancer screening across U.S. states.** The team chose to analyze colorectal cancer for two reasons: 

1. Amount and depth of colorectal cancer data in the dataset. The dataset includes data on screening rates and mortality rates by location, year, data value type, and stratification group, which makes it possible to study both statewide patterns and disparities across groups.
2. Colorectal cancer prevalence within the United States. Recently, colon cancer has been the subject of many news articles due to the increase in number of cases, especially in young people. As of 2026, about 1 in 25 men and 1 in 26 women will develop colorectal cancer (Cancer Research Institute).


# Question 1

**How do colorectal cancer screening rates vary across U.S. states, and which regions consistently show the lowest screening rates?**     
**Importance:** This question is important because geographic variation in screening rates can reveal differences in access to preventive healthcare, public health outreach, insurance coverage, healthcare infrastructure, and awareness across different parts of the country. Colorectal cancer screenings are immensely important for the mortality of a patient, reducing death by up to 73% (American Cancer Society). Understanding which areas have low screening rates is important to realize where to focus education efforts on colorectal cancer screenings.

# Question 2

**How do colorectal cancer screening rates differ by race/ethnicity across U.S. states, and where are the largest disparities?**   
**Importance:** This question is critical because racial and ethnic disparities in screening rates reflect the difference in healthcare access, quality of care, and societal determinants of health. While screening can reduce colorectal cancer mortality by up to 73%, these benefits are not distributed equally, which is shown by the difference in the screening rates.

# Manipulations Applied to Dataset

For both questions, we used Excel’s Transform feature to narrow the original U.S. Chronic Disease Indicators dataset to only the records needed for colorectal cancer screening analysis. We filtered the data to the Cancer topic, selected “Colorectal cancer screening among adults aged 45–75 years,” kept only Age-adjusted Prevalence and Overall values, limited the data to 2020 and 2022, and removed non-state locations so the dataset matched our focus on U.S. states. We also created a new Region column that grouped states into the Northeast, Midwest, South, and West. Finally, we kept only the columns needed for analysis and visualization, resulting in a clean dataset ready for Tableau. For Question 1, we decreased to nine, keeping only relevant information about the time data was collected, the area, the question, and the results. For Question 2, we also decreased the number of columns, but kept the necessary columns to analyse Race/Ethnicity. These manipulations resulted in a clean dataset ready for Tableau.


# Question 1 Analysis
<img width="1226" height="907" alt="Screenshot 2026-05-04 at 12 00 07 PM" src="https://github.com/user-attachments/assets/eb92eb0c-64e6-4453-9f24-73e8107390b2" />      

<img width="1222" height="903" alt="Screenshot 2026-05-04 at 12 00 33 PM" src="https://github.com/user-attachments/assets/77048b14-13ca-423f-8b57-568faffadb4b" />

**Interpretation:**       
The results show that colorectal cancer screening rates vary substantially across U.S. states and regions rather than being evenly distributed nationwide. The state-level map suggests a clear geographic pattern: many states in the Northeast have relatively higher screening rates, while several states in the West and Southwest appear among the lowest. The regional comparisons reinforce this conclusion. The Northeast had the highest average colorectal cancer screening rate in both years, with an average of 65.76% in 2020 and 58.34% in 2022. In contrast, the West had the lowest average screening rate in both years, at 57.83% in 2020 and 53.74% in 2022. There was not significant changes in screening rates between 2020 and 2022. This is also reflected in the 10 States with Lowest Screening Rates graph, where the majority of states appear in the lowest group across both years.      

Overall, screening rates were higher in 2020 than in 2022. This is surprising because many medical procedures were disrupted due to Covid-19 in 2020, and the USPSTF officially expanded routine colorectal cancer screening from ages 50–75 to ages 45–75 in May 2021. Two possible reasons for screening rates being higher in 2020 is that people were especially concerned for their health given the pandemic, or it could reflect incomplete or skewed data in the dataset.     

The Northeast region's consistently higher rates is also an interesting finding from this analysis. This is likely due the region's better access to care and insurance coverage. KFF notes that uninsured adults are much less likely to have a usual source of care and much more likely to skip care because of cost. Since preventive screening usually depends on having regular access to primary care, insurance, and follow-up care, places with better coverage and stronger healthcare access would reasonably be expected to have higher screening participation. Also, the South and West regions might have lower rates due to access barriers such as substantial rural areas with long travel distances and fewer colonoscopy providers. The CDC notes that colorectal screening can be especially difficult in rural communities because colonoscopies require specialist access, preparation time, and transportation support.     

Overall, our analysis reflects that the West is the region that needs the most education and support to improve their screening rates. Another interesting analysis would be to compare the 2022 screening rates to 2025 screening rates, which would hopefully reflect overall rates given the increased prevalance of colorectal cancer in the United States.

# Question 2 Analysis
<img width="1231" height="801" alt="Screenshot 2026-05-04 at 5 11 01 AM" src="https://github.com/user-attachments/assets/3a529df4-f083-49f3-865e-d6b8882be45f" />

<img width="1229" height="778" alt="Screenshot 2026-05-04 at 5 12 31 AM" src="https://github.com/user-attachments/assets/8d49ac46-19ca-4024-8b4a-00cbfb30a18e" />

**Interpretation:**
The results show that the colorectal cancer screening rates across regions are fairly consistent by when categorized by race, as the White, non-hispanic group reached a peak of 63.81% making the Northeast the leader in screening rates. This is an indicator that there is a stronger healthcare infrastructure in the Northeast than the rest of the United States. In the South region, there is more disparity in the equity gap, as the highest screened group (Black, non-Hispanic at 61.92%) and the lowest screened grou (Hawaiian or Pacific Islander at 42.55%) had the most significant gap in the country. The results also show the West region having the lowest ceiling at 58.02%, which is an indicator that the west region has a systematic lack of access.

The screening equity gaps chart highlights consistent trends across all four regions. The Hispanic, Asian, and American Indian/Alaska Native populations are consistently among the lower end of the screenign spectrum. This indicates that these groups have the lack of healthcare access and possibly a language barrier access as well causing them to have a lower screening rate. The higher screening rate among the white and black populations  in certain regions suggest that these groups have better acess to primary healthcare and lwoer risk for colorectal Cancer, yet the lower rates for other minority groups indicate that they are at higher risk for later cancer diagnosis. 

The interactive map shows the in detail variations by state while being seperated in regions. As a whole, the South region has the lowest screening rate for American Indian/Alaska Native, however in Texas they have the highest screening rate which is over 60%. Viewing the data by state allows it to be better detailed and allow the viewer to now what specific health initiatives must be targeted in those communites specifically rather than on a regional basis.

Overall, our analysis reflects that a "one size fits all" approach to the public health of colorectal cancer will not close the equity gap. The West and South regions require the most support, but the efforts must be broken down into the specific groups for each state. To improve overall national health focused on colorectral cancer, the length of the dumbbell line in the equity gap chart should be focused on to ensure that a person's race or state doesn't dictate their likelihood of receiving the prevantative care needed.
