# Waves
Buoy data recording

## Folder Structure
In the root folder of your CSV's directory include a file called `buoys.csv` as described in the 'Buoy Information' table below.

### CSV Folder Structure
`/buoy_id/YEAR/MONTH/DAY/FILENAME.csv`

| Item | Description |
| ---- | ---------- |
| `buoy_id` | Unique identifier for this buoy in it's current location |
| `YEAR` | Full digit year I.e. `2021` |
| `MONTH` | Two digit month with leading zero when necessary I.e. `05` |
| `DAY` | Two digit day with leading zero when necessary I.e. `09` |
| `FILENAME` | UTC Timestamp for when CSV was generated adjusted to GMT with csv extention I.e. `2020-10-19T05:13:22Z.csv` |

## CSV Definition

### Buoy Information
| Tag | Type | Description |
| ------------- | ------------- | ----- |
| `buoy_id` | `string` | Unique identifier for this buoy **Required** |
| `label` | `string` | Label for pretty title for the buoy I.e. 'Port Headland Deap Sea' **Required** |
| `type` | `string` | Buoy manufacturer **Required** |
| `enabled` | `boolean` | `0` not visible, `1` visible, `2` map only, `3` chart only  **Required** |
| `order` | `integer` | Order in list **Required** |
| `data` | `string` | Additional data **Required** |
| `start_date` |  `datetime` | Deployed date **Required** |
| `end_date` |  `datetime` | Completion date if ended |
| `first_updated` | `string` | Filename for first CSV written |
| `last_updated` | `string` | Filename for most recently written CSV |

### Wave Data
| Tag | Type | Description |
| ------------- | ------------- | ----- |
| `buoy_id` | `string` | Unique identifier for this buoy **Required** | 
| `wave_height_significant` | `float` | Significant wave height | 
| `wave_height_max` | `float` | Max wave height | 
| `wave_height_avg` | `float` | Average wave height | 
| `wave_steepness` | `float` | Wave steepness | 
| `period_peak` | `float` | Peak period | 
| `period_mean` | `float` | Mean period | 
| `period_significant` | `float` | Significant Period | 
| `direction_peak` | `float` | Peak direction | 
| `direction_mean` | `float` | Mean direction | 
| `directional_spread_peak` | `float` | Peak directional spread | 
| `directional_spread_mean` | `float` | Mean directional spread | 
| `crest_peak` | `float` | Peak crest | 
| `number_of_zero_crossings` | `integer` | Number of zero crossings | 
| `t_avg` | `float` | | 
| `t_max` | `float` | | 
| `tp5` | `float` | | 
| `te` | `float` | | 
| `t10` | `float` | | 
| `h10` | `float` | | 
| `hm0` | `float` | | 
| `latitude` | `float` | Latitude, up to 6 decimal places | 
| `longitude` | `float` | Longitude, up to 6 decimal places | 
| `data` | `string` | Additional data | 
| `timestamp` | `datetime` | UTC date time in the format `yyyy-mm-dd hh:mm:ss` | 
| `temperature` | `float` | Temperature in celcius | 
| `wind_speed` | `float` | Wind speed in knots | 
| `wind_direction` | `float` | Wind direction in degrees |
