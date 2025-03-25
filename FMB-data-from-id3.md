# FMB003 data as seen from ID.3

## FMB supported parameters

https://wiki.teltonika-gps.com/view/FMB003_Teltonika_Data_Sending_Parameters_ID

## Sample data collected from an ID.3

| Key  | Description                                      | Sample Value |
|------|--------------------------------------------------|--------------|
| 16   | Total Odometer by FMB GPS (m)                    | 8235, 8243, 8254, 8267, 8313, 8415, 8527, 8582, 8636 |
| 21   | GSM Signal (RSSI)                                | 3 (RSSI: <-83) |
| 30   | Number of DTC - Detected Error Codes             | 0            |
| 31   | Engine Load (%)                                  | 23           |
| 32   | Coolant Temperature (°C)                         | -41          |
| 36   | Engine RPM                                       | 1500         |
| 37   | Vehicle Speed (km/h)                             | 78           |
| 51   | Control Module Voltage (mV)                      | 14412        |
| 57   | Hybrid Battery Pack Remaining Life (%)           | 77           |
| 66   | External Voltage (mV)                            | 14994, 15014, 15003, 15016, 15029, 15023, 15013, 14999, 14996 |
| 67   | FMB Internal Battery (mV)                        | 4024, 4024, 4025, 4024, 4024, 4024, 4024, 4024, 4077 |
| 68   | FMB Internal Battery (mA)                        | 100          |
| 69   | GNSS Status                                      | 1 (GNSS ON with fix) |
| 181  | GNSS PDOP (Position Dilution of Precision)       | 14, 15, 15, 14, 16, 17, 17, 15, 17 |
| 182  | GNSS HDOP (Horizontal Dilution of Precision)     | 7, 6, 6, 7, 7, 8, 8, 8, 8          |
| 200  | Sleep Mode (0: No Sleep, 1: GPS Sleep, 2: Deep Sleep, 3: Online Sleep, 4: Ultra Sleep) | 0 (No Sleep)  |
| 239  | Ignition (0 = Off, 1 = On)                       | 1            |
| 240  | Movement (0 = Off, 1 = On)                       | 1            |
| 241  | Active GSM Operator MNC, MNI                     | 24491        |
| 256  | VIN (Vehicle Identification Number)              | WVWZZZE1ZPP000660 |
| 389  | Vehicle Odometer Value (km)                      | 23689        |
| 410  | OEM Battery Charge State (0 = Not Charging, 1 = Charging) | 1            |
| 411  | OEM Battery Charge Level (%)                     | 87           |
| 412  | ?                                                | 16, 17       |
| 543  | Hybrid System Voltage (V)                        | 1023         |
| 544  | Hybrid System Current (A)                        | -858, -1021, -1008, -942, -342, -30, -84, -78, -49 |
| 755  | Range Remaining (km)                             | 243          |
| 1152 | OEM Battery Temperature (°C)                     | 22           |
| ts   | Timestamp                                        | 1742907783000, ... |
| pr   | ?                                                | 0            |
| latlng | Latitude, Longitude                            | 60.202057, 24.596032, ... |
| alt  | Altitude (m)                                     | 21, 22, 22, 22, 22, 20, 22, 23, 27 |
| ang  | Angle (°)                                        | 96, 109, 130, 149, 155, 155, 162, 173, 184 |
| sat  | Satellites in Use                                | 14, 14, 14, 14, 14, 13, 13, 14, 13 |
| sp   | Speed (km/h)                                     | 28, 27, 27, 28, 40, 50, 50, 49, 49 |
| evt  | Event                                            | 0            |

GNSS reference

- 0 - GNSS OFF
- 1 – GNSS ON with fix
- 2 - GNSS ON without fix
- 3 - GNSS sleep

RSSI refernce
- 0	=< -111 or not known/not detectable
- 1	< -101
- 2	< -93
- 3	< -83
- 4	< -73
- 5	>= -73
