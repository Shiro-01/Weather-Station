# Weather-Station
This project involves building a weather station using Arduino and a BME280 sensor to measure temperature, humidity, and pressure. The sensor data is displayed on an LCD screen for local monitoring and sent to a cloud service using MQTT protocol for remote storage and analysis.

# Components Used:
Arduino (e.g., Arduino Uno or compatible board)
BME280 Sensor Module (for temperature, humidity, and pressure sensing)
16x2 LCD Display
ESP8266 Wi-Fi Module (for internet connectivity)
Jumper wires
Breadboard (optional for prototyping)

# Description:
The weather station is designed to provide real-time environmental data such as temperature, humidity, and pressure. The BME280 sensor collects this data, which is then displayed on the LCD screen for local monitoring. Additionally, the ESP8266 module facilitates Wi-Fi connectivity, enabling the Arduino to connect to a Wi-Fi network and communicate with a cloud service via MQTT protocol.

Upon successful connection to the Wi-Fi network and MQTT broker, the Arduino periodically publishes the sensor data to a specified MQTT topic. The data is formatted as JSON and includes temperature, humidity, and pressure readings. This data can be subscribed to and processed by any MQTT client, allowing for remote storage, analysis, or visualization.

The LCD screen provides a convenient way to view the current weather conditions locally. Users can monitor temperature, humidity, and pressure without the need for additional devices. Meanwhile, the cloud integration enables users to access weather data remotely, making it suitable for applications such as smart home systems, agriculture, or environmental monitoring.

Overall, this project demonstrates the integration of sensor data with cloud services, enabling real-time monitoring and analysis of environmental conditions from anywhere with an internet connection. It showcases the versatility of Arduino in IoT applications and provides a foundation for further experimentation and development in the field of weather monitoring and analysis.

# Important note: - 
This code assumes you have set up an MQTT broker (server) to handle the messages. Make sure to replace placeholders like "your_wifi_ssid", "your_wifi_password", "mqtt_server_address", "your_mqtt_username", and "your_mqtt_password" with your actual credentials and server details.
