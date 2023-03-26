# python-api-challenges

### Finding the perfect February getaway destination:
**Using citipy Python Library and OpenWeatherMap API to analyze weather patterns and their correlation to latitude.**

For this challenge, two separate scripts were created:

## 1. [WeatherPy.ipynb](https://github.com/wangavin/python-api-challenges/blob/main/starter_code/GW_WeatherPy.ipynb)

### A randomized list of cities was created
* First, a list of randomly chosen latitude/longitude coordinates was generated.
* This coordinate list was then used with the citipy Python Library to generate a list of cities nearest to the random coordinates.
* The OpenWeatherMap API was then accessed to provide a series of meteorological measures for each city.
* In order to begin analysis of the correlation between the meteorological measurements and latitude, four scatter plots were generated using MatPlotLib
* These scatter plots were saved as .png files in the output_data folder.
Latitude vs. Temperature (Fig.1)

![Screen Shot 2023-03-25 at 6 55 09 PM](https://user-images.githubusercontent.com/119981450/227746193-cf77b44e-81db-4269-84c6-f7e669d23f4e.png)

Latitude vs. Humidity (Fig.2)

![Screen Shot 2023-03-25 at 6 55 47 PM](https://user-images.githubusercontent.com/119981450/227746234-5101dcb1-da80-4ff8-8dde-cd4defe877b9.png)

Latitude vs. Cloudiness (Fig.3)

![Screen Shot 2023-03-25 at 6 56 59 PM](https://user-images.githubusercontent.com/119981450/227746258-1c1cc08c-0fd9-40de-ba2c-d7d021540282.png)


Latitude vs. Wind Speed (Fig.4)

![Screen Shot 2023-03-25 at 6 57 04 PM](https://user-images.githubusercontent.com/119981450/227746262-6d49aaa4-a368-494e-b982-7f92562633ec.png)


* Two linear regressions were then performed on each of the above scatter plots, one for cities in the northern hemisphere and one for cities in the southern hemisphere. The regression line was displayed over the scatter plot along with the regression equation.
* These 8 new scatter plots were manually saved to the output_data folder as Fig5.png through Fig12.png

**Northern Hemisphere Latitude vs. Temperature (Fig.5)	Southern Hemisphere Latitude vs. Temperature (Fig.6)**
![Screen Shot 2023-03-25 at 7 01 23 PM](https://user-images.githubusercontent.com/119981450/227746436-6835868b-2245-4bec-89ab-9d927f4e2ac8.png)
![Screen Shot 2023-03-25 at 7 01 36 PM](https://user-images.githubusercontent.com/119981450/227746438-910f01c6-ff43-45b9-912c-34608d57aa7f.png)

**Northern Hemisphere Latitude vs. Humidity (Fig.7)	Southern Hemisphere Latitude vs. Humidity (Fig.8)**
![Screen Shot 2023-03-25 at 7 04 02 PM](https://user-images.githubusercontent.com/119981450/227746509-e5062a18-2b0b-45e1-8faa-5cdbb195c872.png)
![Screen Shot 2023-03-25 at 7 04 08 PM](https://user-images.githubusercontent.com/119981450/227746511-5c96e9bf-fdfd-4ccb-809c-53a23462be25.png)

**Northern Hemisphere Latitude vs. Cloudiness (Fig.9)	Southern Hemisphere Latitude vs. Cloudiness (Fig.10)**
![Screen Shot 2023-03-25 at 7 04 57 PM](https://user-images.githubusercontent.com/119981450/227746538-72f358de-e5a6-412e-97b0-d1c64391ad9e.png)
![Screen Shot 2023-03-25 at 7 05 05 PM](https://user-images.githubusercontent.com/119981450/227746539-d65c20d8-0f0f-452b-9157-01e6005504a7.png)

**Northern Hemisphere Latitude vs. Wind Speed (Fig.11)	Southern Hemisphere Latitude vs. Wind Speed (Fig.12)**
![Screen Shot 2023-03-25 at 7 05 57 PM](https://user-images.githubusercontent.com/119981450/227746554-ed459fdc-dcfd-422e-a40a-4bdab26d6051.png)
![Screen Shot 2023-03-25 at 7 06 03 PM](https://user-images.githubusercontent.com/119981450/227746555-5b8b4d3c-b4c0-4a90-8920-6557472d1f08.png)


### 2. [VacationPy.ipynb](https://github.com/wangavin/python-api-challenges/blob/main/starter_code/GW_VacationPy.ipynb)
**Using hvplots.pandas the cities were plotted onto an OpenStreetMap tile:**

All Sample Cities from cities.csv output. (Fig.13)
![Screen Shot 2023-03-26 at 1 12 36 AM](https://user-images.githubusercontent.com/119981450/227756708-2eaca539-6a3d-48de-b974-db39880d1622.png)

**The list of cities was then filtered down based on a series of ideal meteorological values:**
* A max temperature lower than 27 degrees but higher than 21
* Wind speed less than 4.5 m/s
* Zero cloudiness

**Using hvplots.pandas the filtered cities were plotted onto an OpenStreetMap tile. Functionality was included that allows the user to mouseover each city to see the name of the nearest hotel and the country name:**

Ideal February Vacation Cities filtered from cities.csv output with Nearest Hotel Name. (Fig.14)
![Screen Shot 2023-03-26 at 1 13 09 AM](https://user-images.githubusercontent.com/119981450/227756800-7264fd40-eaa9-4074-92dc-11a5a9144190.png)

