# Data Driven Insights into Exoplanet Characteristics and Discovery Trends

## Problem Statement

The discovery and study of exoplanets—planets that exist outside our solar system—have grown immensely in recent years. With thousands of exoplanets identified, understanding their unique characteristics and the methods used to discover them is key to advancing our knowledge of planetary systems beyond Earth. To contribute to this understanding, the objective of this project is to systematically collect detailed information on exoplanets from NASA’s Exoplanet Catalog, available on [this website](https://science.nasa.gov/exoplanets/exoplanet-catalog). 

This catalog provides a wealth of information on various exoplanet properties, such as their distance from Earth (measured in parsecs), mass, stellar magnitude, radius, orbital period, and eccentricity, among others. It also includes data on the methods by which these exoplanets were discovered, the types of stars they orbit, and when they were identified.

Once the exoplanet data is collected through web scraping techniques, the goal is to analyze and visualize this dataset to uncover patterns, correlations, and trends. Specifically, this project seeks to explore questions such as:
- How are the characteristics of exoplanets—such as mass, radius, and orbital period—related to one another?
- Are there observable trends in the methods used to discover exoplanets over time?
- What types of exoplanets are most frequently discovered, and how are they distributed across different types of star systems?

To address these questions, I utilized Tableau, a powerful data visualization tool, to create an interactive dashboard that allows users to visually explore the dataset and gain data-driven insights. Through the dashboard, viewers can investigate exoplanet demographics, filter data based on various parameters, and identify key trends. This visualization highlights how exoplanet discoveries have evolved over time and how certain characteristics—such as planet size or orbital period—may be correlated with the discovery method or stellar magnitude.

In conclusion, this project aims not only to gather and clean the raw data on exoplanets but also to transform it into meaningful visual insights that offer a clearer understanding of exoplanet characteristics and discovery trends. The final Tableau Dashboard, available for public access, provides an interactive way to engage with the data and uncover significant findings. You can explore the dashboard at this [link](https://public.tableau.com/app/profile/farhan.noor.dehan/viz/Data-DrivenInsightsintoExoplanetCharacteristicsandDiscoveryTrends/Data-DrivenInsightsintoExoplanetCharacteristicsandDiscoveryTrends).

## Findings and Observations from the [Dashboard](https://public.tableau.com/app/profile/farhan.noor.dehan/viz/Data-DrivenInsightsintoExoplanetCharacteristicsandDiscoveryTrends/Data-DrivenInsightsintoExoplanetCharacteristicsandDiscoveryTrends)

Several key insights emerged from the analysis:

1. **Exoplanet Types**: Neptune-like planets make up the largest portion of identified exoplanets, while terrestrial planets are the least common. Gas giants have the highest mass and radius, requiring the longest orbital periods, followed by Neptune-like planets and super-Earths. Terrestrial planets, in contrast, have the smallest masses and orbital periods.

2. **Mass vs. Radius**: Gas giants exhibit the largest mass relative to their radius compared to other exoplanet types, highlighting their immense size and density.

3. **Discovery Methods and Characteristics**: Exoplanets discovered via radial velocity tend to have the longest orbital periods, with some spanning nearly 5,250 years and boasting radii exceeding 2,500 Jupiters. On the other hand, planets found using the transit method often have the largest orbital radii, some exceeding 7,200 Jupiters, but shorter orbital periods of about 669 Jupiters. As orbital radius increases, the preferred detection methods shift, ranging from transit timing to techniques like astrometry, eclipse timing variations, imaging, microlensing, and finally radial velocity and transit.

4. **Trends Over Time**: In the early 2000s, the majority of discoveries were gas giants. However, from 2013 to 2017, there was a surge in the discovery of Neptune-like planets, super-Earths, and an average number of gas giants and transient planets. Following 2020, discoveries again leaned toward Neptune-like planets, followed by gas giants, though the frequency was lower compared to the 2013-2017 peak, yet still higher than in earlier years.

5. **Evolution of Discovery Methods**: From 1991 to 1994, pulsar timing was the primary method of discovering exoplanets. However, after that period, other techniques gained prominence, with the transit method leading the way. Between 2013 and 2017, the transit method uncovered the highest number of exoplanets by a significant margin, surpassing other methods like radial velocity, microlensing, and others. Radial velocity followed as the second most effective method, with microlensing and additional techniques trailing behind.


## Build From Sources and Run the Selenium Scraper
1. Clone the repo
```bash
git clone https://github.com/Dehan001/Data-Driven-Insights-into-Exoplanet-Characteristics-and-Discovery-Trends
```
2. Intialize and active virtual environment
```bash
virtualenv --no-site-packages venv
source venv/bin/activate
```
3.  Install dependencies
```bash
pip install -r requirements.txt
```
4. Download Chromedriver from https://googlechromelabs.github.io/chrome-for-testing/

5. Run the scraper
```bash
python exoplanet_scraper/exoplanet_scraper_main.py --chromedriver_path <path_to_chromedriver>
```
6. You will get a file named `nasa_exoplanets.csv` containing all the required fields. Alternatively, check our scraped data here: [nasa_exoplanets.csv](https://github.com/Dehan001/Data-Driven-Insights-into-Exoplanet-Characteristics-and-Discovery-Trends/blob/main/Dataset/nasa_exoplanets.csv)



