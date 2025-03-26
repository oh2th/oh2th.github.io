# FMB003 data

## FMB Supported Parameters So Far

As collected and combined from VW ID.3 (2023) and Fiat Ducato.

| ID   | Parameter                                  | Unit            | Notes |
|------|--------------------------------------------|-----------------|-------|
| 12   | Fuel Used GPS                              | ml              |       |
| 13   | Fuel Rate GPS                              | cl/100 km       |       |
| 15   | Eco Score                                  | factor 0.01     |       |
| 16   | Total Odometer by FMB GPS                  | m               |       |
| 17   | X-axis Acceleration                        | mG              |       |
| 18   | Y-axis Acceleration                        | mG              |       |
| 19   | Z-axis Acceleration                        | mG              |       |
| 21   | GSM Signal Strength                        | 0-5             | 0	=< -111 or not known/not detectable, 1	< -101, 2	< -93, 3	< -83, 4	< -73, 5	>= -73 |
| 24   | GNSS Speed                                 | km/h            |       |
| 30   | Number of DTC - Detected Error Codes       | count           |       |
| 31   | Engine Load                                | %               |       |
| 32   | Coolant Temperature                        | °C              |       |
| 36   | Engine RPM                                 | RPM             |       |
| 37   | Vehicle Speed                              | km/h            |       |
| 51   | Control Module Voltage                     | mV              |       |
| 57   | Hybrid Battery Pack Remaining Life         | %               |       |
| 66   | External Voltage as Measured by FMB        | mV              |       |
| 67   | FMB Internal Battery Voltage               | mV              |       |
| 68   | FMB Internal Battery Current               | mA              |       |
| 69   | GNSS Status                                | 0-3             | 0 = OFF, 1 = ON with fix, 2 = ON without fix, 3 = Sleep |
| 80   | Data Mode                                  | 0-5             | 0 = Home On Stop, 1 = Home On Moving, 2 = Roaming On Stop, 3 = Roaming On Moving, 4 = Unknown On Stop, 5 = Unknown On Moving |
| 113  | Battery Level                              | %               | Not confirmed which battery |
| 181  | GNSS PDOP                                  | -               | Divide by 10 to get decimal value |
| 182  | GNSS HDOP                                  | -               | Divide by 10 to get decimal value |
| 199  | Trip Odometer                              | m               |       |
| 200  | Sleep Mode                                 | 0-4             | 0 = No Sleep, 1 = GPS Sleep, 2 = Deep Sleep, 3 = Online Sleep, 4 = Ultra Sleep |
| 205  | GSM Cell ID                                | -               |       |
| 206  | GSM Area Code                              | -               |       |
| 239  | Ignition                                   | 0/1             | 0 = Off, 1 = On |
| 240  | Movement                                   | 0/1             | 0 = Off, 1 = On |
| 241  | Active GSM Operator                        | MNC + MNI       | Example: 24491 = Telia FI |
| 256  | VIN (Vehicle Identification Number)        | -               | Example: WVWZZZ... |
| 303  | Instant Movement                           | 0/1             |       |
| 383  | AXL Calibration Status                     | 0-3             | 0 = No Calibration, 3 = Fully Calibrated |
| 387  | GPS Location                               | -               | Format: `+Lat+Lng+Speed/` |
| 389  | Vehicle Odometer Value                     | km              |       |
| 410  | OEM Battery Charge State                   | 0/1             | 0 = Not Charging, 1 = Charging |
| 411  | OEM Battery Charge Level                   | %               |       |
| 412	 | Unknown                                    | °C              |       |
| 449  | Ignition On Counter                        | count           |       |
| 543  | Hybrid System Voltage                      | V               |       |
| 544  | Hybrid System Current                      | A               |       |
| 755  | Range Remaining                            | km              |       |
| 1152 | OEM Battery Temperature                    | °C              |       |

https://wiki.teltonika-gps.com/view/FMB003_Teltonika_Data_Sending_Parameters_ID

## Sample data collected from an ID.3

| Key  | Description                                      | Sample Value |
|------|--------------------------------------------------|--------------|
| 12   | Fuel Used GPS (0.001 l)                         | 351          |
| 13   | Fuel Rate GPS (0.01 l/100km)                    | 107          |
| 15   | Eco Score (factor 0.01)                         | 1000         |
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
| 80   | Data Mode                                       | 0 (Home On Stop) |
| 113  | Battery Level % (Unknown which battery)         | 100          |
| 181  | GNSS PDOP (Position Dilution of Precision)       | 14, 15, 15, 14, 16, 17, 17, 15, 17 |
| 182  | GNSS HDOP (Horizontal Dilution of Precision)     | 7, 6, 6, 7, 7, 8, 8, 8, 8          |
| 199  | Trip Odometer (m)                               | 16314        |
| 200  | Sleep Mode (0: No Sleep, 1: GPS Sleep, 2: Deep Sleep, 3: Online Sleep, 4: Ultra Sleep) | 0 (No Sleep)  |
| 205  | GSM Cell ID                                     | 32042        |
| 206  | GSM Area Code                                   | 4119         |
| 239  | Ignition (0 = Off, 1 = On)                       | 1            |
| 240  | Movement (0 = Off, 1 = On)                       | 1            |
| 241  | Active GSM Operator MNC, MNI                     | 24491        |
| 256  | VIN (Vehicle Identification Number)              | WVWZZZ.... |
| 303  | Instant Movement                                | 0            |
| 383  | AXL Calibration Status (1 = Calibrated)        | 1            |
| 387  | GNSS Position (Latitude + Longitude + Speed)    | `+601970.5000+0245902.9667+000.021/` |
| 389  | Vehicle Odometer Value (km)                      | 23689        |
| 410  | OEM Battery Charge State (0 = Not Charging, 1 = Charging) | 1            |
| 411  | OEM Battery Charge Level (%)                     | 87           |
| 412  | Unknown            | 16, 17       |
| 449  | Ignition On Counter                             | 4844         |
| 543  | Hybrid System Voltage (V)                        | 1023         |
| 544  | Hybrid System Current (A)                        | -858, -1021, -1008, -942, -342, -30, -84, -78, -49 |
| 755  | Range Remaining (km)                             | 243          |
| 1152 | OEM Battery Temperature (°C)                     | 22           |
| ts   | Timestamp                                        | 1742907783000, ... |
| pr   | Unknown                                          | 0            |
| latlng | Latitude, Longitude                            | 60.202057, 24.596032, ... |
| alt  | Altitude (m)                                     | 21, 22, 22, 22, 22, 20, 22, 23, 27 |
| ang  | Angle (°)                                        | 96, 109, 130, 149, 155, 155, 162, 173, 184 |
| sat  | Satellites in Use                                | 14, 14, 14, 14, 14, 13, 13, 14, 13 |
| sp   | Speed (km/h)                                     | 28, 27, 27, 28, 40, 50, 50, 49, 49 |
| evt  | Event                                            | 0            |

## Sample data collected from Fiat Ducato

| Key  | Description                                      | Sample Value |
|------|--------------------------------------------------|--------------|
| 16   | Total Odometer by FMB GPS                        | 9870         |
| 21   | GSM Signal (0-5)                                 | 3            |
| 66   | External Voltage as measured by FMB              | 13076        |
| 67   | FMB Internal Battery (mV)                        | 3990         |
| 68   | FMB Internal Battery (mA)                        | 0            |
| 69   | GNSS Status (1 = GNSS ON with fix)               | 1            |
| 113  | Battery Level % (Unknown which battery)          | 100          |
| 181  | GNSS PDOP                                        | 25           |
| 182  | GNSS HDOP                                        | 10           |
| 199  | Trip Odometer by FMB GPS                         | 273          |
| 200  | Unknown                                          | 0            |
| 239  | Ignition (0 = Off)                               | 0            |
| 240  | Movement (1 = On)                                | 1            |
| 241  | Active GSM Operator (MNC 244, MNI 91 = Telia FI) | 24491        |
| 387  | GNSS Position (Latitude + Longitude + Speed)     | `+601970.3000+0245902.4000+000.022/` |
| 443  | Unknown                                          |              |
| 449  | Ignition On Counter                              | 615          |
| ts   | Timestamp (ms)                                   | 1742967958000 |
| pr   | Unknown                                          | 0            |
| latlng | Latitude & Longitude (Parsed)                  | 60.197030, 24.590240 |
| alt  | Altitude (m)                                     | 22           |
| ang  | Angle (Course)                                   | 351          |
| sat  | Satellite Count                                  | 12           |
| sp   | Speed (km/h)                                     | 0            |
| evt  | Unknown (Possibly Event Type)                    | 240          |

