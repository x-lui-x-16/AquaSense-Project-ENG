# AquaSense: Autonomous Drip Irrigation System with Moisture Sensors for Optimizing Crop Water Usage

This repository documents the development of AquaSense, an innovative system designed to autonomously regulate drip irrigation in crops. The solution is based on the use of moisture sensors that, by continuously measuring the state of the soil in an area of 100 cm x 100 cm, allow to adjust the water supply precisely, promoting efficiency and sustainability in agriculture.

[Spanish Version](https://github.com/x-lui-x-16/AquaSense-Proyecto-ESP)


## Table of Contents
- Engineered Materials
- Construction Instructions
- Table of Contents
- Introduction to the system
- Objectives, Objectives
- Beneficiaries and Impact
- Methodology
- Explanation of the Code
- System Components and Management
- Expected Results
- Budgeting
- Conclusion
- Bibliography


## Engineering Materials
- Arduino Mega 2560: Processor that reads the data from the humidity sensors and controls the electrovalve or pump.
- Humidity Sensors (9 units): Strategically arranged to measure humidity in different zones of the cultivation area.
- Solenoid Valve / Water Pump: Regulates water flow to the irrigation system.
- Relay: Allows the safe control of the solenoid valve or pump, avoiding overloads in the Arduino.
- Plastic Pipes and Dripper: Distribute the water uniformly in the irrigation area.
- Power Supply: It can be a battery or a power adapter, which ensures the continuous operation of the entire system.
- Protoboard and Connector Cables: Facilitate temporary connections and circuit testing.
- Water Container: Source from which water is drawn for irrigation.


## Construction Instructions
### Hardware Assembly:
- Connect the humidity sensors to the Arduino using the breadboard and wires.
- Integrate the solenoid valve or water pump using a relay to control the water flow.
- Distribute the pipes and drippers along the growing area (100 cm x 100 cm).

### Electronic Circuit Configuration:
- Ensure that each sensor is assigned to a digital pin to receive readings.
- Configure the relay to allow the Arduino to safely activate or deactivate the solenoid valve.

### Mounting the Irrigation System:
- Attach the plastic tubing to the solenoid valve or pump, distributing it evenly across the growing area.
- Place the drippers in each section, ensuring an even distribution of water.

### Testing and Calibration:
- Calibrate each sensor by comparing readings in dry and wet soil.
- Perform controlled tests to verify relay response and water flow.


## Repository Contents
[Code](src/): Source code for programming the Arduino.

[Schematics](schematics/): Electrical diagrams and schematics of the system.

[Project Images](p-photos/): Photographs of the assembly, testing and operation of the prototype.


## Introduction
Agriculture is essential for food security and the economy, especially in regions where water is a limited resource. Traditionally, many growers use inefficient irrigation methods, resulting in excessive water use. AquaSense was developed to automate drip irrigation using moisture sensors, allowing precise control of water delivered directly to the roots. This solution not only optimizes water consumption, but also improves crop health, contributing to a more sustainable and resilient agriculture in the face of climate change.


## Objectives
### General Objective
To design and implement an autonomous drip irrigation system that, based on the continuous measurement of soil moisture, regulates the water supply in an area of 100 cm x 100 cm, optimizing the use of water resources.

### Specific Objectives
Moisture Measurement: Use nine strategically distributed moisture sensors to obtain a representative average of the soil condition.
Automated Control: Program the Arduino so that, based on the readings, it activates the solenoid valve or water pump only when necessary.
Efficiency Comparison: Evaluate the water savings and efficiency of the system compared to traditional irrigation methods.
Crop Growth Impact: Analyze the effect of controlled irrigation on plant development and health.


## Beneficiaries and Impact
### Beneficiaries
- Farmers and Small Producers: Reducing costs and labor by automating irrigation.
- Rural Communities: Optimizing water use in areas with limited water resources.
- Educational and Research Institutions: Platform for teaching and experimentation in precision agriculture.
- Governments and Development Agencies: Tool to promote sustainable agricultural practices and improve food security.

### Project Impact
- Environmental: Decrease in water consumption and protection of aquifers.
- Economic: Reduced operating costs and increased crop productivity.
- Social: Promotion of responsible agricultural practices and environmental education.
- Innovative: Scalable and adaptable platform that can be integrated with renewable energy and other emerging technologies.


## Methodology
The development of AquaSense has been structured in several phases:
### Sensor Design and Distribution:
- Strategic placement of nine sensors in the 100 cm x 100 cm area to obtain accurate measurements.

### Electronic Circuit Configuration:
- Connection of sensors and relay to the Arduino, ensuring protection and correct interpretation of signals.

### Programming of the Arduino:
- Periodic reading of sensors.
- Average humidity calculation.
- Activation of the solenoid valve or pump if the average is below the set threshold.
- Automatic deactivation once the optimum level is reached.

### Irrigation System Assembly and Testing:
- Piping and dripper integration.
- Calibration and verification under controlled conditions.

### Field Implementation and Monitoring:
- Installation in the crop area and performance monitoring.
- Data logging for comparative analysis with traditional methods.

### Efficiency Evaluation:
- Analysis of water consumption, irrigation frequency and effects on plant growth.


## Code Explanation
[The source code](src/) (located in the /src folder) is developed in C++ for the Arduino and performs the following functions:

- Initialization: Pin configuration for sensors, relay and other components.
- Data Reading: Periodic capture of signals from the humidity sensors.
- Processing: Calculation of the average humidity of the area.
- Control: Automatic activation and deactivation of the solenoid valve or pump according to the defined threshold.
- Error Handling: Calibration and verification routines to ensure system reliability.


## System Components and Management
### System Components
- Moisture Sensors: For continuous measurement of soil condition.
- Solenoid Valve/Pump and Relay: To control water flow in a safe and automated way.
- Irrigation Infrastructure: Pipes and drippers for uniform water distribution.
- Power Supply: Adaptable to renewable energy solutions (e.g. solar panels) for operation in remote areas.

### System Management
- Real-Time Monitoring: Moisture data is recorded and can be viewed for future adjustments.
- Irrigation Automation: The system automatically responds to soil conditions, avoiding water waste.
- Scalability and Flexibility: Modular design allows the system to be adapted to different crop areas and specific needs.


## Expected Results
- Reduced Water Consumption: Projected savings of 30-50% compared to conventional methods.
- Improved Crop Health: Optimal irrigation for plant growth and vitality.
- Data Collection for Optimization: Generation of records that will facilitate decision making in agricultural management.
- Autonomous Operation: Minimization of manual intervention and greater efficiency in irrigation management.


## Budget
(Space reserved  to enter the details of the budget and costs associated with the implementation of the system).


## Conclusion
AquaSense represents a breakthrough in the application of automation technologies in agriculture, offering a comprehensive solution for drip irrigation that responds to the real needs of the soil. The implementation of this system not only promotes the efficient use of water, but also contributes to environmental sustainability and the strengthening of food security. Its scalable and adaptable design makes it an accessible tool for small farmers and research projects, opening the door to future innovations in the field of precision agriculture.


## Bibliography
FAO. (2021). Sustainable use of water in agriculture. [https://www.fao.org](https://www.fao.org)

IDIAP. (2022). Sustainable practices in agriculture in Panama. [https://www.idiap.gob.pa](https://www.idiap.gob.pa)

Netafim. (2020). Drip irrigation technology. [https://www.netafim.com](https://www.netafim.com)

Ministry of Agricultural Development (2023). Irrigation initiatives in Panama. [https://www.mida.gob.pa](https://www.mida.gob.pa)

Arduino.cc. (2023). Arduino Mega 2560 Rev3. [https://www.arduino.cc/en/Guide/ArduinoMega2560](https://www.arduino.cc/en/Guide/ArduinoMega2560)

Adafruit. (2019). Soil Moisture Sensor Guide. [https://learn.adafruit.com/adafruit-stem](https://learn.adafruit.com/adafruit-stem)

SparkFun Electronics. (2023). Soil Moisture Sensor Hookup Guide. [https://learn.sparkfun.com/tutorials/soil-moisture-sensor-hookup-guide](https://learn.sparkfun.com/tutorials/soil-moisture-sensor-hookup-guide)

Banzi, M., & Shiloh, M. (2015). Getting Started with Arduino (3rd ed.). Maker Media.

Torres, L., & Valencia, J. (2019). Irrigation technology: innovation for the efficient use of water in agriculture. Ediciones Uniminuto.

Jordán, R., & González, F. (2020). Technology and sustainable agriculture: Automatic irrigation systems with Arduino. Ediciones Agrícolas.

Vázquez, E., & Ramos, P. (2019). Automation in agriculture with microcontrollers and sensors. Editorial Académica Española.

Journal of Irrigation and Drainage Engineering. “Drip Irrigation Systems for Efficient Water Use and Crop Yield.”

