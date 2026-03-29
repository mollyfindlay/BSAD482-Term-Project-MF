## Wrangling Process 

# Government of Canada (2026). Monthly Climate Summaries. Canada.ca
There are many pages within this excel sheet, making it a legthy task to clean. Using tableau prep, the pages were joined together to create one dataset. Cleaning and Unioning 11 pages of data led to some repetiviness in some columns which then hasd to be deleated. Using the legened from the Government of Canada website, the acronyms for each column title were changed to more understandable title names (Ex. Tm = Mean Temperature). 

# Statistics Canada, (2026). Electric power generation, monthly generation by type of electricity
Firstly, Dates were edited in Excel using the "replace" function to add the year to the date rows. Once this was done, each date was formated as "mm/dd/yyyy". The data was provided in horozontal format which was not compatable with Tableau Prep, so this miust be changed so the values will show when creating visualizations. To fix this, the data was pivoted so information headers (such as "Date" and "Types of Electricity Generation") would apear as column titles. After this, multiple columns were deleated as they contained null values as certain forms of electric power generation are not present in Newfoundland and Labrador (Ex. Solar Power). 

# Newfoundland Hydro (2026). Publications, Annual Reports 2017-2024
This data was primarily sorted by hand, as all the information came from separate pdf documents. All missing null values from the data were removed. This strategy was chosen because there were minimal null values in the sheet, making it a quick fix.

# Statistics Canada, (2024). Household energy consumption, Canada and provinces
This set of data was wrangled both by hand in Excel and through Tableau Prep as there were many aspects that needed to be changed to be able to create visualizations in Tableau. First, unnessesary rows were compleatly removed in Excel. THis includes columns related to natrual gas and heating oil, as they were not needed in the visualizations. Secondly, the data was pivoted through Tableau Prep to further organize for the creation of visualizations. This step allowed for the usage of Tableau. All null values were removed from the data, and calumns were given thr proper classifications (EX. Changing the format of year to 'Date'). 


# Government of Newfoundland and Labrador, (2025). Historical GHG Emissions Summary Newfoundland and Labrador, 1990-2023
For this wrangeling process, the data had to be moved into an editable format. When first downloaded, the data was in PDF format, making it difficult to manipulate and use in Tableau. Extracting this data had to be done by hand, copying and pasting values into a blank excel spreadsheet. Once this was complete, appropriate headers were given to organize the data further. No manipulation had to be done in Tableau Prep as the only information taken from this report were the final totals. 



