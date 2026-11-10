# econ3916_midtermproject

## 1. Research Question

Did the implementation of New York City's congestion pricing policy on January 5, 2025, reduce daily vehicle traffic volumes through the Hugh L. Carey Tunnel and Queens Midtown Tunnel?

My hypothesis is that congestion pricing is associated with a reduction in traffic volumes through these two tunnels.

## 2. Data Source

**Dataset:** MTA Bridges and Tunnels Hourly Crossings: Beginning 2019

**Source:** New York State Open Data

**URL:** [https://data.ny.gov/Transportation/MTA-Bridges-and-Tunnels-Hourly-Crossings-Beginning/ebfx-2m7v](https://data.ny.gov/Transportation/MTA-Bridges-and-Tunnels-Hourly-Crossings-Beginning/ebfx-2m7v/about_data)

The analysis uses six months of data before and after January 5, 2025. The original MTA data was aggregated into daily traffic counts for two tunnels and four vehicle classes: cars, buses, trucks, and motorcycles.

The cleaned dataset contains 2,920 observations, with no missing values.

## 3. How to Run the Notebook

1. Download the Jupyter notebook and cleaned Excel dataset from this repository
2. Open the notebook in Google Colab
3. Upload the Excel dataset to the Colab session
4. Run all cells in order
   
## 4. Headline Finding

One of the main limitations of the analysis is that the regression results can help to establish correlation, not causality. Additionally, my dataset only includes the Hugh L. Carey Tunnel and the Queens Midtown Tunnel. It does not include other tunnels that are a part of New York City’s congestion pricing initiative, such as the Lincoln Tunnel and the Holland Tunnel. My results are limited in their scope and cannot be generalized to all changes to traffic entering Manhattan. 

After removing 216 influential observations using the Cook’s distance method, the sensitivity analysis estimated that the coefficient on congestion pricing changed from -307.41 to 31.49. The regression analysis that included all of the observations may be sensitive to these extreme values and can influence the outcome of the regression. These observations cannot be removed from the analysis, as they may be representative of real fluctuations in traffic volumes. 

My analysis finds that average daily traffic decreased by 3.23 percent after congestion pricing was implemented. The base regression produced a coefficient of -307.10, which is not statistically significant at the 5% level. After including vehicle class, day of the week, and facility, the coefficient was -307.41 and was statistically significant. The sensitivity analysis concluded that influential observation could have had an impact on the regression. I cannot confidently conclude that congestion pricing caused a reduction in traffic volume. 
With additional bandwidth, I would expand the analysis to other tunnels impacted by congestion pricing. It would be interesting to see if roads not impacted by congestion pricing saw higher traffic volumes because drivers were taking alternative routes. Other potential omitted variables could be traffic volume by season or economic conditions in NYC. I think this could help provide a more reliable estimate of the policy’s impact.
