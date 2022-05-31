# Israel Solar Radiation Forecast

Using [XML data][1] for ultraviolet (UV) radiation index for 15 cities around the country provided by [Israel Meteorological Service][2].

[1]: <https://ims.data.gov.il/sites/default/files/isr_rad.xml>
[2]: <https://ims.gov.il/en>

## Description
Python program to display hourly ultraviolet radiation index data for selected city.

## Usage

### Displaying Help Menu

`$ ./israel-uv --help`#

**Output:**  
```bash
Usage: ./israel_uv [OPTION]

Example:
./israel_uv -c haifa    # Display solar radiation forecast for the city of Haifa.

Options:
-l, --list              List avaiable cities.
-c, --city              Displays solar radiation forecast for selected city.
-h, --help              Display this help menu and quit.
```

### Listing Available Cities

`$ ./israel-uv --list`

**Output:**  
```bash
Select city from list and run using '--city' option.

CITIES
---------------
Tiberias
Nazareth
Lod
Eilat
Mizpe-Ramon
Beer-Sheva
En-Gedi
Jerusalem
Ashdod
Tel-Aviv---Yafo
Hadera
Bet-Shean
Afula
Haifa
Zefat
Qazrin

Data provided by:
Israel Meteorological Service
(https://ims.gov.il/en/UVIHourly)
```

### Displaying Hourly Forecast

`$ ./israel-uv -c jerusalem`

**Output:**  
```bash
Solar radiation forecast for Jerusalem, Israel:

TIME                    UV INDEX
----------------        --------------
2022-05-31 13:00        9 (Very High)
2022-05-31 14:00        8 (Very High)
2022-05-31 15:00        6 (High)
2022-05-31 16:00        4 (Medium)
2022-05-31 17:00        2 (Low)
2022-05-31 18:00        1 (Low)
2022-05-31 19:00        0 (Low)
2022-05-31 20:00        0 (Low)
2022-06-01 06:00        0 (Low)
2022-06-01 07:00        0 (Low)
2022-06-01 08:00        2 (Low)
2022-06-01 09:00        3 (Medium)

Data provided by:
Israel Meteorological Service
(https://ims.gov.il/en/UVIHourly)
```