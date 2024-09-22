# Data Driven Insights into Exoplanet Characteristics and Discovery Trends

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
python exoplanet_scrapper/exoplanet_scrapper_main.py --chromedriver_path <path_to_chromedriver>
```
6. You will get a file named `nasa_exoplanets.csv` containing all the required fields. Alternatively, check our scraped data here: [nasa_exoplanets.csv](https://github.com/Dehan001/Data-Driven-Insights-into-Exoplanet-Characteristics-and-Discovery-Trends/blob/main/Dataset/nasa_exoplanets.csv)


## Analytics 
Tableau Public View : https://public.tableau.com/app/profile/farhan.noor.dehan/viz/Data-DrivenInsightsintoExoplanetCharacteristicsandDiscoveryTrends/Data-DrivenInsightsintoExoplanetCharacteristicsandDiscoveryTrends
