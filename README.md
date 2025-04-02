# Ultrasonic distance detection sensor 
1. Project Description
1.1 Operating Principle

The proximity sensor project is based on the HC-SR04 ultrasonic module, which measures distances up to 2 meters. The system’s primary goal is to detect objects and signal their presence via LEDs and an audible buzzer.

1.2 Detailed Operation

The HC-SR04 emits an ultrasonic pulse and measures the time taken for the reflected sound wave to return. Based on this time, the distance to the object is calculated. If an object is within 0–10 cm, the system activates:

-  10–8 cm: 1 LED lights up, buzzer emits sound at frequency f.

- 8–6 cm: 2 LEDs light up, buzzer emits sound at 2f.

- 6–4 cm: 3 LEDs light up, buzzer emits sound at 3f.

- 4–2 cm: 4 LEDs light up, buzzer emits sound at 4f.

- <2 cm: All 5 LEDs light up, buzzer emits sound at 5f.

1.3 Modules Used

- GPIO: Controls LEDs, HC-SR04 sensor, and buzzer.

- PWM: Adjusts buzzer frequency based on distance.

- Timer: Measures ultrasonic pulse return time to calculate distance.

1.4 Applications

The system serves as a warning device (e.g., parking sensor or presence detector). Its 5-tier feedback (LEDs + buzzer) provides intuitive distance awareness.
