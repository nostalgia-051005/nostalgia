# fNIRS 보드 지원서 (Board Application)

### 1. Title of your idea
**OpenNIRScap: Open-Source Wearable fNIRS Brain-Interface for Social Assistance Robots** 

### 2. Which scenario will your solution address?
**Robotics - Social Assistance Robot**

### 3. What are you going to build?
We will build an accessible, ergonomic functional Near-Infrared Spectroscopy (fNIRS) cap and system. This system will include 24 custom sensor modules and dual-wavelength LEDs, integrated with a low-power microcontroller (STM32/Arduino) to acquire real-time brain blood oxygenation data. This cap will act as a Brain-Computer Interface (BCI) wearable to control or communicate with a social assistance robot.

### 4. How does your solution work? What are the main features?
The system utilizes near-infrared light (660 nm & 990 nm) to measure changes in blood oxygenation in the brain, reflecting neural activity (modified Beer-Lambert Law). 
**Main features include:** 
- Synthesized control of 24 detectors and 8 emitters via a central microcontroller unit (ECU).
- Ergonomic mechanical cap design for comfortable, long-term wear.
- Real-time communication and an interactive Python-based GUI for data visualization and robot command mapping.

### 5. Will your project focus on sustainable solutions? How?
Yes. Traditional fNIRS systems are extremely expensive, bulky, and energy-consuming. Our project focuses on sustainability by utilizing a low-power microcontroller (e.g., STM32L476RET6 or supported Arduino boards) to minimize energy consumption. Furthermore, the open-source hardware approach allows users to repair, upgrade, and 3D-print parts individually, significantly extending the product’s lifecycle and reducing e-waste.

### 6. Briefly explain your user experience. How intuitive and user-friendly is your solution? Can it be easily integrated into existing systems or workflows?
The user simply wears the ergonomic cap like a standard hat, avoiding the messy conductive gels required by traditional EEG caps. The raw brain data is instantly translated into intuitive graphs via the interactive GUI and mapped to simple output commands (e.g., Yes/No, Move forward) for the social robot. Its Python-based backend natively supports seamless integration into existing ROS (Robot Operating System) workflows or healthcare monitoring setups.

### 7. Consider the scalability of your project. How can it be expanded to serve a larger audience or be applied in different contexts?
The modular and open-source nature makes it highly scalable. The number of nodes can be adjusted to fit different head sizes (from children to adults) or targeted brain regions. Beyond social robots, the framework can be easily expanded to the "Gaming - Mixed-Reality" scenario for mind-controlled gaming, or integrated with wireless modules (Wi-Fi/BLE) for remote tele-medicine and personal health tracking.

### 8. How will you use App Lab in your project?
We will use App Lab to create a mobile-friendly dashboard. The brain activity data and the social robot's status will be sent to the App Lab interface via Wi-Fi/Bluetooth. This allows caregivers or researchers to remotely monitor the user's cognitive state and the robot's responses in real-time from any smart device.

### 9. How will you integrate AI in your project?
The raw fNIRS data contains complex blood flow patterns that vary per individual. We will integrate Machine Learning (AI) classification models to process this raw sequential data. By training the AI on user-specific brain patterns, the system will accurately decode the user's focus, fatigue levels, or specific motion intentions, translating human thoughts into precise, autonomous actions for the social assistance robot.
