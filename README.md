## Raw dataset for weather
-- Rainfall.csv, RH.csv, Tavg.csv, Sun shine csv files are the raw dataset of rainfall, relative humidity, average temperature, sunshine respectively for all weather stations from January 2022- December 2024. 

## Raw dataset for dengue
-- Dengue3.csv file contains the raw dataset of dengue cases from January 2022- December 2024. There are 8 missing values of affected_in_Dhaka and daily_affected_cases of entire country respectively and 10 missing values of affected_in_Chittagong and affected_in_Khulna respectively.


## Primarily processed dataset for weather variables

-- d_Dhaka.csv, d_chitagong.csv, d_khulna.csv contains the primarily processed weather data of Dhaka, Chittagong, Khulna which is generated from raw dataset by manually copying the values of weather variables of each month for each station in corresponding region. In d_chittagong.csv file, there are 31 null values in Sunshine of Hatiya station of Chittagong, 1 null values of sunshine in a station of Khulna division, 122 null values of humidity in a station of Chittagong.


## processed dataset for dengue and weather of Dhaka, Chittagong and Khulna regions

-- Dhaka.csv, Chitagong.csv, Khulna.csv contains the processed dengue and weather data of Dhaka, Chittagong, Khulna which are generated using the “Weather Impact (Regional analyses). ipynb” code file where null values of dengue are filled using forward-backward filling algorithm and null values of weather are filled using liner interpolation algorithm. Just in case of 122 missing values in a station of Chittagong, we have consider remaining 11 stations for those days. Then, each weather variable values are averaged for the respective stations in each region. To get the processed data, d_Dhaka.csv, d_chitagong.csv, d_khulna.csv, Dengue_3.csv files are used.

 ## feature importance with standard variaion of Dhaka, Chittagong and Khulna regions
-- Importance (Dhaka).csv, Importance (Chittagong).csv, Importance (Khulna).csv file contains the feature’s(weather) relative importance with standard deviation on dengue cases in the respective regions and code are available in “Weather Impact (Regional analyses). ipynb”  code  file.

## Network_Properties(National_scale)

-- The network properties and surrogate analysis of the corresponding properties are generated using Dengue3.csv file and the code is available in "Network_Properties(National_Scale).ipynb" file.

## Network_Properties(Regional_scale)
-- The network properties and surrogate analysis of the corresponding properties of Dhaka and Khulna division are generated using Dhaka.csv file and Khulna.csv file and the code is available in "Network_Properties(Regional_Scale).ipynb" file.


## Visibolity graph
-- The code is available at "Visibility_Graph.ipynb" file.
