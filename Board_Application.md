# fNIRS 보드 지원서 (Board Application) - 디벨롭 버전(V2)

### 1. Title of your idea
**OpenNIRScap V2: Wireless, Edge-AI Powered Multi-modal BCI for Social Assistance Robots** 

### 2. Which scenario will your solution address?
**Robotics - Social Assistance Robot**

### 3. What are you going to build?
We will build an advanced, fully-wireless functional Near-Infrared Spectroscopy (fNIRS) cap. Building upon the original OpenNIRScap design, V2 will introduce an upgraded microcontroller (such as an ESP32 or specialized Arduino board) for BLE/Wi-Fi streaming, an integrated IMU (Inertial Measurement Unit) to cancel out head motion artifacts, and flexible PCBs (FPCBs) for superior scalp conformity. This cap will act as a high-precision, low-latency BCI wearable enabling users with motor disabilities to control a social assistance robot.

### 4. How does your solution work? What are the main features?
The system utilizes near-infrared light (660 nm & 990 nm) to measure neural activity by tracking blood oxygenation changes.
**Main upgraded features include:** 
- **Fully Wireless Operation:** Tether-free data acquisition via Bluetooth/Wi-Fi to a host device or cloud.
- **Multi-Modal Sensor Fusion:** An onboard IMU dynamically tracks and subtracts motion-induced noise from the fNIRS signals to ensure medical-grade accuracy even when the user moves.
- **Flexible PCB (FPCB) Modules:** Replacing rigid boards with FPCBs ensures perfect ergonomic fit across different head shapes, directly improving optical signal quality.

### 5. Will your project focus on sustainable solutions? How?
Yes. We will use a highly efficient edge-computing microcontroller to eliminate the energy consumption required to constantly stream raw data to a heavy external PC. Furthermore, by releasing the flexible node designs and housing as open-source hardware, we allow users to repair or replace only individual faulty nodes through 3D printing and component swapping, drastically extending product lifespan and minimizing e-waste.

### 6. Briefly explain your user experience. How intuitive and user-friendly is your solution? Can it be easily integrated into existing systems or workflows?
The transition to a fully wireless, FPCB-based cap completely removes cable tangles, allowing the user to simply wear it like a lightweight beanie. Without being tethered to a computer, users experience maximum freedom. Caregivers and engineers can seamlessly integrate the cap into existing Robot Operating System (ROS) workflows because the device can output clean, finalized motion-intent commands directly over the local network. 

### 7. Consider the scalability of your project. How can it be expanded to serve a larger audience or be applied in different contexts?
The modular wireless architecture allows the network to scale infinitely—users can snap on more sensors for a full-brain scan or reduce them to a simple headband for daily focus tracking. Because the added IMU actively filters out motion noise, this project can scale beyond static wheelchair use into highly active scenarios, such as "Gaming - Mixed-Reality" applications, sports performance tracking, or ambulatory stroke rehabilitation.

### 8. How will you use App Lab in your project?
We will utilize App Lab to deploy a real-time, cross-platform mobile dashboard. Data processed by the cap will be pushed to the Arduino Cloud/App Lab. This allows caregivers and family members to remotely monitor the user's cognitive workload, stress levels, and the social robot's current task status via their smartphones, ensuring safety and continuous care from anywhere in the world.

### 9. How will you integrate AI in your project?
Instead of relying on a centralized PC, we will integrate **TinyML (Edge AI)** directly into the cap's microcontroller. We will train lightweight neural networks to locally process the complex, multi-modal fNIRS and IMU data. This means the cap itself will classify human intentions, cognitive fatigue, and emotional states instantaneously at the edge. By removing the data transmission bottleneck, this TinyML approach ensures virtually zero latency when sending thought-commands to the social assistance robot.
