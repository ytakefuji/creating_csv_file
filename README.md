# creating_csv_file for data science
<pre>
pandas DataFrame library can be used for creating a csv file.

The first goal is to creat a csv template for scoring individual policies:
           country  deaths  population  score
0      South Korea       0           0      0
1            India       1           1      1
2           Brazil       2           2      2
3           France       3           3      3
4      New Zealand       4           4      4
5           Taiwan       5           5      5
6           Sweden       6           6      6
7            Japan       7           7      7
8    United States       8           8      8
9           Canada       9           9      9
10  United Kingdom      10          10     10
11          Israel      11          11     11
</pre>

csv files can be created by pandas DataFrame. 
The csv file contains 4 columns including country, deaths, population, and score.
<pre>

import pandas as pd
dd=pd.DataFrame(
 { "country": d,
  "deaths": range(len(d)),
  "population": range(len(d)),
  "score": range(len(d)),
 })
 
 d is a list of country names.
 
 In order to make d (a list of countries), countries file is needed.
 
 d=open('countries').read().strip()
 print(d)
 
 South Korea,India,Brazil,France,New Zealand,Taiwan,Sweden,Japan,United States,Canada,United Kingdom,Israel
</pre>

# Generate a pop.csv file with the populations of all countries.
<pre>
Hint:
Scrape populations from the site on the internet.

</pre>

# Generate a deaths.csv file with the total deaths of all countries.
<pre>
Hint:
Check  python-novice repository.
Scrape total deaths information from the site on the internet.

</pre>

# Use pop.csv and deaths.csv for filling values of pandas DataFrame.

Hint:

# Calculate score of the countries.

Hint:
scoring individual policies can be calculated by dividing the total number of deaths by a population.

score=total deaths/population (million)

# Create a score.csv file

Hint:

see python-novice.
 
 
