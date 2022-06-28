# Selecting a New Tennis Racquet

![federer racquet](https://user-images.githubusercontent.com/100224330/176103361-d486528e-14cd-4673-afb1-2bbbed0ff635.jpg)

## Motivation

I love playing tennis and I am long overdue for a new racquet. I haven't bought a new racquet in 9 years and would like to search for a new one that fits my game a little better. I find my current racquet to be slightly too heavy and not spin-friendly enough, so I will be looking for something with easier access to power and topspin, ideally within the strung weight range of 11-11.5 ounces. Instead of just clicking through page by page on the internet for each racquet, I thought I'd combine my passions for data and tennis together for a fun and informative exercise that can help narrow in on which racquets to consider. With the help of a Tableau dashboard, I will try to identify a handful of racquet to demo and then select one to purchase.


## Data Acquisition

To acquire the data needed for the Tableau dashboard, I will be scraping from Tennis Warehouse, an online store selling tennis gear, apparel, and accessories. Below are the categories of racquet data that I will be scraping:
  - **Racquet names and prices**
    - [Link to sample Tennis Warehouse racquet page](https://www.tennis-warehouse.com/Wilson_Blade_98_16x19_v8/descpageRCWILSON-16BV8R.html)
  - **Racquet specs**
    - Racquet specs can include strung weight, string pattern, head size, power level, etc. This will be important for me to have so that I can filter the overall space down to the racquets that meet my desired specs. For example I will need a racquet that meets the following specs:
      - 11-11.5 oz strung weight
      - Open string pattern
      - 100 square inch head size
      - Medium stiffness
      - Low/medium power level
  - **Pro players using/endorsing the racquet**
    - Knowing which pro players use the racquet helps me understand which game styles the racquet might be suitable for
  - **Racquet review scores**
    - Most of the top racquets are reviewed by a team of Tennis Warehouse playtesters and are given an overall score, as well as scores for how the racquet performs on various categories, such as groundstrokes, power, topspin, etc. Some of these categories are more important to me than others, so I can play around with sorting the racquet list by the most important categories to me.
    - [Link to sample Tennis Warehouse Review](https://www.tennis-warehouse.com/learning_center/racquet_reviews/16BV8Rreview.html)
    
After scraping the required data, there is some data cleaning I need to perform. Much of the data cleaning efforts go toward cleaning string values to remove unwanted characters, converting strings to numeric types, and reshaping the dataframes from long to wide.

## Visualization in Tableau

[Link to Tableau Dashboard](https://public.tableau.com/app/profile/r.prabhu/viz/SearchingforMyNextTennisRacquet/RacquetOverview)

The fun, interactive part comes in Tableau. I set up the dashboard to have questions that ask the user to answer some questions about their desired racquet specs using some parameters that essentially act as filters. If you don't have a preference for a certain spec, you can just select Unsure.

![image](https://user-images.githubusercontent.com/100224330/176096872-9c01eb57-f311-411c-a734-21974523d48f.png)

Once I selected my desired specs, this is the view that I see in the dashboard. I can see how many racquets there are by brand, what % has been reviewed, the list of racquets meeting my specs, and a visual of how the racquets compare between balance and swingweight. If I want to see which players use a certain racquet, I can select a racquet from the list or a select a point in the scatter plot (see 2nd screenshot below).

![image](https://user-images.githubusercontent.com/100224330/176097179-a5a7488a-6ec2-480d-ac31-19e3925ff9b0.png)

![image](https://user-images.githubusercontent.com/100224330/176097619-a2b140eb-6cd7-485b-8b3f-86861a0e82fd.png)

<br>

## Next Steps

While it's tough to get down to a shortlist to demo, I am leaning towards trying out the **Prince Twistpower X100 Tour**, the **Yonex EZONE 100 2022**, and the **Babolat Pure Aero**. The latter two racquets had the highest overall review scores within my filtered list, while the Babolat scored highest for topspin, something this flatter hitter is trying to add more of to his game. Before this exercise, I had largely written off Prince and Yonex racquets in favor of Head and Babolat, my two most recently used brands, but after seeing them at the top of the list and doing my research into both, I was pleasantly surprised and will be giving them a very strong look. Here's to a fresh racquet helping me improve my game!
