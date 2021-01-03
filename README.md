# SG-Weather-Server
Rewrite <a href="https://github.com/maxng07/SG_Weather_GO"> SG-Weather-Go </a> into Web API Server that serve Singapore Weather, Air Temperature, PSI and Rainfall data via API. You can either query the server directly using API to obtain the output or use a WebPage (provided here as sample). The API Server fetch and extracts data from Govtech API (https://data.gov.sg) before serving it. Data output similar to SG_Weather_GO.

## Usage
Download the zipped file in Release, extract it into a common folder, change the WebServer config (IP address and TCP port) and start the server.

Access the data either using the browser which will serve a default webpage or query data directly using API. The web page is formatted with CSS for mobile and works fine using browser on mobile.

### API
API for Weather Forecast
http://sg-weather.kams.com.hk:8080/api/weather/?text=city

http://sg-weather.kams.com.hk:8080/api/weather/?text=all

API for PSI Readings
http://sg-weather.kams.com.hk:8080/api/psi/

API for Air Temperature
http://sg-weather.kams.com.hk:8080/api/temp/

API for Rainfall Readings at Rain Gauge
http://sg-weather.kams.com.hk:8080/api/rainfall/

The API Server supports concurrency and multi-thread.

Data are not cache and fetch direct from Govtech data.gov.sg

