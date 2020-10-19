# Waves
Buoy data recording

## Folder Structure
In the root folder of your CSV's directory include a file called `buoys.csv` as described in the 'Buoy Information' table below.

### CSV Folder Structure
`/buoy_id/YEAR/MONTH/DAY/FILENAME.csv`

| Item | Definition |
| ---- | ---------- |
| `buoy_id` | Unique identifier for this buoy in it's current location |
| `YEAR` | Full digit year I.e. `2021` |
| `MONTH` | Two digit month with leading zero when necessary I.e. `05` |
| `DAY` | Two digit day with leading zero when necessary I.e. `09` |
| `FILENAME` | UTC Timestamp for when CSV was generated adjusted to GMT with csv extention I.e. `2020-10-19T05:13:22Z.csv` |

## CSV Definition

### Buoy Information
| Tag        | Data Type           | Definition  |
| ------------- | -------------:| -----:|
| `buoy_id` | varchar(255) **(Required)** | Unique identifier for this buoy in it's current location |
| `type` | varchar(255) **(Required)** | Buoy manufacturer |
| `enabled` | tinyint(1) **(Required)** | `0` not visible, `1` visible, `2` map only, `3` chart only  |
| `order` | mediumint(9) **(Required)** | Order in list |
| `data` | text **(Required)** | Additional data |
| `start_date` |  datetime **(Required)** | Deployed date |
| `end_date` |  datetime | Completion date if ended |
| `first_updated` | varchar(255) | Filename for first CSV written |
| `last_updated` | varchar(255) | Filename for most recently written CSV |

### Wave Data
| Tag        | Data Type           | Definition  |
| ------------- |:-------------:| -----:|
| `buoy_id` | | | 
| `wave_height_significant` | | | 
| `wave_height_max` | | | 
| `wave_height_avg` | | | 
| `wave_steepness` | | | 
| `period_peak` | | | 
| `period_mean` | | | 
| `period_significant` | | | 
| `direction_peak` | | | 
| `direction_mean` | | | 
| `directional_spread_peak` | | | 
| `directional_spread_mean` | | | 
| `crest_peak` | | | 
| `number_of_zero_crossings` | | | 
| `t_avg` | | | 
| `t_max` | | | 
| `tp5` | | | 
| `te` | | | 
| `t10` | | | 
| `h10` | | | 
| `hm0` | | | 
| `latitude` | | | 
| `longitude` | | | 
| `data` | | | 
| `timestamp` | | | 
| `temperature` | | | 
| `wind_speed` | | | 
| `wind_direction` | | |
