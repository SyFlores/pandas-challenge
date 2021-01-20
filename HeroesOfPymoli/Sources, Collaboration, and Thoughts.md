### Sources
- 

### Collaborations
-

### Thoughts
What is Being Asked? Pseudocode.

- Player Count
  - WiBA
    - Display the # of players
  - Pc
    - We want to return the unique count of SN
      - Use a combination of .len and .unique
    - We want unique because players can and often will make multiple purchases
- Purchasing Analysis (Total)
  - WiBA
    - Obtain the # of unique items, average item price, # of purchases, and total revenue
    - Return as a dataframe and display
  - Pc
    - Run the four calculations separately and feed them into variables; Use those variables to build the dataframe
      - Use .len and .unique on Item ID or Item Name
      - Use .mean on Price
      - Use .len on Purchase ID
      - Use .sum on Price or multiply the previous two values
    - Build a small dataframe using the dictionary method
- Gender Demographics
  - WiBA
    - Return a 3x2 table with the 3 Gender values against Total Count and Percentage of Players
  - Pc
    - Use either .value_counts and then append the percentage after OR .groupby and perform .count and calculate the percentage using a sum and division
- Purchasing Analysis (Gender)
  - WiBA
    - Return a Gender breakdown giving Purchase Count, Average Purchase Price, and Total Purchase Value, and Average Total Purchase PER PERSON
  - Pc
    - Use .groupby on Gender to get the first three
    - For the PER PERSON average, we need to first sum on the user, then take those averages
- Age Demographics
  - WiBA
    - Make groups and labels for age groups
    - Return count and percentage for players in those groups
  - Pc
    - Use .cut to add as a column in the dataframe called Age Ranges
      - <10, 10-14, 15-19, 20-24, 25-29, 30-34, 35-39, 40+
    - Then apply the same logic used for the Gender Demographics section
- Purchasing Analysis (Age)
  - WiBA
    - Return an Age Ranges breakdown giving Purchase Count, Average Purchase Price, Total Purchase Value, and Average Total Purchase PER PERSON
  - Pc
    - Apply the same logic used for the Purchasing Analysis (Gender) section
- Top Spenders
  - WiBA
    - Return a SN breakdown giving Purchase Count, Average Purchase Price, and Total Purchase Value
    - Sort on Total Purchase Value descending
  - Pc
    - Use .groupby on SN to get the count on SN, mean on price, and total on price
    - Use .sort and set ascending = False
- Most Popular Items
  - WiBA
    - Return an Item ID and Item Name breakdown giving Purchase Count, Item Price, and Total Purchase Value
    - Sort on Purchase Count descending
  - Pc
    - Use .groupby on Item ID and Item Name, since they should be 1-1, this shouldn't cause any substantial issues. Might want to check this!
    - Use .sort and set ascending = False
- Most Profitable Items
  - WiBA
    - Sort previous result on Total Purchase Value descending
  - Pc
    - Use .sort and set ascending = False... but on a different column
