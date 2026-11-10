# ESP32 Automatic College Bell System

An ESP32 that rings a buzzer automatically at scheduled times and publishes each event over MQTT.

## Features
- Syncs time over WiFi using NTP (IST, UTC+5:30)
- Rings the buzzer for 5 seconds at each scheduled time
- Publishes the event name to the MQTT topic `college/bell`
- Rings each event only once per day

## Schedule
| Time  | Event         |
|-------|---------------|
| 10:30 | Morning Break |
| 10:45 | Break End     |
| 13:00 | Lunch Start   |
| 13:40 | Lunch End     |
| 16:00 | College End   |

## Hardware
- ESP32 DevKit C
- Buzzer (GPIO 18 and GND)

## Libraries
- WiFi
- PubSubClient

## Run
Open the project on [Wokwi](https://wokwi.com/projects/480312310091592705) and press Play.
