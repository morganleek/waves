# Waves
Buoy data recording

# Folder Structure
In the root folder of your CSV's directory include a file called buoys.csv

# CSV Definition

## Buoy Information
| Tag        | Data Type           | Definition  |
| ------------- |:-------------:| -----:|
| `buoy_id` | varchar(255) **(Required)** | Unique identifier for this buoy in it's current location |
| `type` | varchar(255) **(Required)** | Buoy manufacturer |
| `enabled` | tinyint(1) **(Required)** | `0` not visible, `1` visible, `2` map only, `3` chart only  |
| `order` | mediumint(9) **(Required)** | Order in list |
| `data` | text **(Required)** | Additional data |
| `start_date` |  datetime **(Required)** | Deployed date |
| `end_date` |  datetime | Completion date if ended |
| `last_updated` | datetime **(Required)** | Date when most recent CSV was written for this buoy |

## Wave Data
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
