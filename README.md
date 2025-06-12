# Smart-Plant-Monitoring-System
The Smart Plant Monitoring System is designed using Arduino Uno R3 to measure soil moisture, temperature, and humidity and display the data on an OLED SSD1306 display. The system provides visual LED alerts and a buzzer alarm when conditions become critical, helping users maintain optimal plant health. 
 
📌 Features 
✅ Soil Moisture Sensor (A0): Measures the water level in the soil and prevents overwatering or drying. 
✅ DHT11 Sensor (Pin 2): Measures temperature and humidity for better environmental monitoring. 
✅ OLED SSD1306 Display (I2C - A4, A5): Shows real-time data for moisture, temperature, and humidity. 
✅ Tri-Color LED (Pins 3, 4, 5 - Common Anode): 
 
Green 🟢: Soil moisture is normal. 
 
Blue 🔵: Soil is drying (warning). 
 
Red 🔴: Soil is too dry, or temperature is too high/low (critical). 
✅ Buzzer (Pin 6): Alerts when conditions become critical (too dry or extreme temperature). 
✅ Standalone System (No WiFi Needed): Works independently without internet connectivity. 
 
📌 Working Principle 
1️⃣ Soil Moisture Sensor detects the amount of water in the soil and provides an analog value. 
2️⃣ DHT11 Sensor measures temperature and humidity and sends data to Arduino Uno. 
3️⃣ OLED SSD1306 displays real-time values for moisture, temperature, and humidity. 
4️⃣ Tri-Color LED changes color based on the moisture and temperature conditions. 
5️⃣ Buzzer sounds when soil is too dry or the temperature is out of safe limits. 
 
📌 System Alerts & Thresholds 
Condition	Moisture %	Temperature (°C)	LED Color	Buzzer 
Normal (Healthy)	>40%	20°C - 30°C	🟢 Green	OFF 
Warning (Slightly Dry)	30% - 40%	20°C - 30°C	🔵 Blue	OFF 
Critical (Very Dry / Extreme Temp)	<30%	>30°C or <20°C	🔴 Red	ON 
📌 Components & Wiring 
Component	Pins (Module Side)	Connect to Arduino Uno R3 
Soil Moisture Sensor	VCC, GND, A0	5V, GND, A0 
DHT11 Sensor	VCC, GND, Data	5V, GND, Pin 2 
OLED SSD1306	GND, VCC, SCL, SDA	GND, 5V, A5 (SCL), A4 (SDA) 
Tri-Color LED (Common Anode)	CO1, CO2, CO3, PC	Pin 3, Pin 4, Pin 5, 5V 
Buzzer	+, -	Pin 6, GND 
✅ Breadboard is used for multiple 5V and GND connections. 
✅ Tri-Color LED uses Common Anode → LOW for ON, HIGH for OFF. 
 
📌 Applications 
🌱 Smart Gardening & Irrigation – Helps automate watering decisions. 
🏡 Home & Indoor Plant Monitoring – Prevents overwatering or drying out plants. 
🚜 Agriculture & Farming – Assists farmers in maintaining crop health. 
🎓 Educational STEM Projects – Teaches about environmental monitoring with sensors. 
 
🚀 How to Use the Project 
1️⃣ Assemble all components as per the wiring table. 
2️⃣ Upload the provided Arduino code using the Arduino IDE. 
3️⃣ Observe real-time values on the OLED display. 
4️⃣ Check LED and buzzer alerts when moisture levels or temperature go beyond safe limits. 
5️⃣ Place the soil moisture sensor in different moisture conditions and test LED changes. 
 
🎯 Expected Outcome 
✅ OLED will display Moisture %, Temperature, and Humidity. 
✅ LED will change colors based on soil & temperature conditions. 
✅ Buzzer will alert when conditions become critical. 
✅ Arduino Uno R3 runs the system without internet connectivity. 
