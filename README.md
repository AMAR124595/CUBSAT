# CUBSAT
The cubesat is a nano satellite that helps us to monitor parameters on space ,it will monitor the Weather , Cosmic radiation , Earth’s magnetic field etc.....
# ABSTRACT
A CubeSat is a small satellite with a form factor of 10 cm (3.9 in) cubes, weighing no more than 2 kg (4.4 lb) per unit. These miniaturized satellites often use commercial off-the-shelf components for their electronics and structure. CubeSats are deployed into orbit from the International Space Station or launched as secondary payloads. They serve purposes such as Earth observation, amateur radio, and technology demonstrations. The CubeSat standard has encouraged engineering collaboration, student training, and scientific research.
# AIM
To Monitor the Weather ,Cosmic Radiation ,Earth Magnetic field etc....
# CONTROLERS & SENSORS 
- Arduino mega 2560 pro
- Arduino nano
- Bme 280
- Mpu 6050
- Mq 7
- Hmc5883l Magnetometer
- Photodiode
- IR Sensor
- Thermoelectric coolers
- Ntc thermistor
- Brushless  motor
- UV sensors
- Heat sink
- NRF24L01
# Block diagram
![Screenshot (2)](https://github.com/user-attachments/assets/25ef32cd-26b0-473a-b9ec-cd7ae87b9339)
# Working Principle of CubeSat System
The CubeSat is a small satellite designed for space missions that typically operates at altitudes between 350 and 700 kilometers above Earth's surface. It is equipped with a range of sensors to monitor various environmental parameters in space. The sensors collect data, which is then processed by an Arduino Mega 2560 Pro microcontroller. Processed data is transmitted via an NRF24L01 wireless module for communication.
## Components and Their Functions
### Sensors
#### BME280: Measures temperature, humidity, and barometric pressure.
* Temperature: Measures the ambient temperature in space.
* Humidity: Measures the relative humidity in the surrounding environment (if applicable).
* Pressure: Measures the atmospheric pressure (useful for understanding atmospheric layers and trends).

#### MPU-6050: Measures acceleration and angular velocity.
* Accelerometer: Measures the CubeSat’s acceleration along three axes, helping to determine its orientation and movement.
* Gyroscope: Measures the rate of rotation around three axes, which aids in attitude control and stabilization.

#### MQ-7: Measures carbon monoxide (CO) concentration.
* Carbon Monoxide Detection: Provides data on CO levels, which can be important for understanding space vehicle interactions and environmental conditions.

#### MC5883L Magnetometer: Measures the Earth's magnetic field.
* Magnetic Field Strength: Measures the strength and direction of the magnetic field in space, aiding in orientation and navigation.

#### Photodiode/UV Sensors: Measures light intensity and UV radiation.
* Light Intensity: Measures the intensity of visible light, helping to understand the light environment in space.
* UV Radiation: Measures ultraviolet radiation levels, which can be important for understanding solar radiation effects.

#### Solar Wind Sensor: Measures the intensity of solar wind.
* Solar Wind Intensity: Converts solar wind's intensity into a voltage signal, providing data on space weather conditions.

### Processing Unit

#### Arduino Mega 2560 Pro: Acts as the central processing unit.
* Data Acquisition: Collects raw data from all sensors.
* Data Processing: Processes the raw sensor data to extract meaningful information, such as calculating average values or detecting anomalies.
* Data Formatting: Prepares the processed data for transmission by formatting it into a suitable protocol.
   
### Communication Module

#### NRF24L01: A wireless module used for data transmission.
* Data Transmission: Sends the processed data to a ground station or another satellite system for further analysis and monitoring.
* Frequency and Range: Operates on a specific frequency band, ensuring data is transmitted over the required distance.
  
## Data Flow

1. Sensor Data Collection:  Each sensor continuously or periodically measures its respective parameter. The sensors output their readings in analog or digital form, depending on the sensor type.

2. Data Processing: The Arduino Mega 2560 Pro receives the sensor readings. It processes this data using algorithms to convert raw sensor outputs into meaningful information. For 
   instance, it may convert analog voltages into temperature readings or compute acceleration from raw accelerometer data.

3. Data Formatting and Transmission: After processing, the Arduino formats the data into a structured format compatible with the NRF24L01 module. The NRF24L01 then transmits this data to 
   a ground station or another receiving system using radio frequency communication.

4. Data Reception and Analysis: The transmitted data is received by a ground station or receiving system, where it is further analyzed. This analysis can provide insights into the space 
   environment, CubeSat performance, and other scientific measurements.
# PCB layout 
![Screenshot (3)](https://github.com/user-attachments/assets/fbe66fc5-371b-466a-b98e-a694c2a8db02)
![Screenshot (4)](https://github.com/user-attachments/assets/eee872cc-e681-441e-a185-39dfcdf480ff)
![Screenshot (5)](https://github.com/user-attachments/assets/7d79b169-9124-43ba-8858-a3476a574a9e)
![Screenshot (6)](https://github.com/user-attachments/assets/5d62efcb-ab8c-4b75-a27d-51d4da3a8d72)
![Screenshot (7)](https://github.com/user-attachments/assets/f0acf332-c2de-4f82-96d0-d5339ed0accd)
# Demonstration 
![cubsat](https://github.com/user-attachments/assets/5af2ff7c-d40e-4b03-a735-59d7ed6a187b)
![reading](https://github.com/user-attachments/assets/0e60b8c0-ffc2-4c91-898a-9c0d48ee8047)
# Linkedin
https://www.linkedin.com/posts/amar-gangadhar-6b25a5267_cubesat-spacetech-satellite-activity-7234093794793533440-_h4-?utm_source=share&utm_medium=member_desktop
# Summary
The CubeSat system operates by utilizing a suite of sensors to gather data on various environmental parameters in space. This data is processed by the Arduino Mega 2560 Pro and transmitted via the NRF24L01 module. The collected information helps in monitoring space conditions, aiding scientific research, and ensuring the proper functioning of the satellite.







