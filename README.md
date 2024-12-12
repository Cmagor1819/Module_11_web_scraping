# Module_11_web_scraping

#Objective:
You’re now ready to take on a full web-scraping and data analysis project. You’ve learned to identify HTML elements on a page, identify their id and class attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. You’ve also learned to scrape various types of information. These include HTML tables and recurring elements, like multiple news articles on a webpage.

As you work on this Challenge, remember that you’re strengthening the same core skills that you’ve been developing until now: collecting data, organizing and storing data, analyzing data, and then visually communicating your insights.

This new assignment consists of two technical products. You will submit the following deliverables:

Deliverable 1: Scrape titles and preview text from Mars news articles.

Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

### Part 1:

This secion's purpose is to visit the Mars News website, analyze the data, scrape the data, and store the results.

### Part 2:

This section's purpose is to visit the Mars Weather Data website, scrape the webpage, store the data, analyze the data with multiple graphs for visualizations, and finally export the data to a CSV file.

### Storing the data:

This secion of part 2 is to create a list, loop through the scraped data to create a list of rows, and store that data back in the original empty list. We then create a DataFrame by using the list of rows and a lit of the column names. Finally, we confirm the data was created by assigning the column names to the DataFrame and display said DataFrame.

### Prep the data for analysis:

This section is taking the data we just stored, converting the data type of each column to the necessary types, and then display the datatypes again.

### Analyze the Data:

This section is analyzing the data to answer the questions: How many months exist on Mars?, How many Martian (and not Earth) days worth of data exist in the scraped dataset?, What are the coldest and the warmest months on Mars (at the location of Curiosity)?, Which months have the lowest and the highest atmospheric pressure on Mars?, and About how many terrestrial (Earth) days exist in a Martian year?. The answers have been calculated and provided in the code. We also use multiple graphs to answer these questions and visualize the answers/data.

We then have an analysis provided at the end of the code.

### Save the Data:

This final section is taking the data we gathered/have and exports it to a CSV file and saves it.

### I got/referenced the following lines of code from Xpert Learning Assistant/GitHub:

cols = soup.body.find('tr')
for name in cols:
    col_name.append(name.text)
col_name

total_sols = new_mars_df['sol'].nunique()

cold_and_hot_months = avg_month_df.sort_values()

first_terrest_day = new_mars_df['terrestrial_date'].agg('min')

plt.ylim(bottom=min(y), top=max(y) + 1)

