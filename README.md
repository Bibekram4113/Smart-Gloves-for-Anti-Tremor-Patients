# Smart Gloves for Anti-Tremor & Paralyzed Patients  

A wearable **IoT-enabled biomedical glove** designed to assist patients with **neurological disorders** such as **Parkinson’s disease, stroke, or spinal cord injury**.  
The glove integrates **flex sensors, accelerometer, gyroscope, and EMG sensors** with **machine learning** and **cloud computing** to detect tremors, provide adaptive corrective feedback, and enable **remote neuro-rehabilitation**.  

---

## 🎯 Features  
- 🖐️ **Tremor Detection** using flex sensors, accelerometer, and gyroscope  
- 🤖 **Machine Learning Models** to classify tremor severity & predict movement intent  
- 🔄 **Closed-Loop Vibration Damping** to actively reduce tremor amplitude  
- ☁️ **Cloud-Based Monitoring** (IoT, Firebase/AWS/Azure) for remote rehabilitation tracking  
- 📡 **Wireless Connectivity** via **Bluetooth & Wi-Fi** (MQTT protocol)  
- 🧩 **Assistive Communication** – converts hand gestures into text/speech for patients with limited mobility  

## 🛠️ Hardware & Components  
- **Microcontroller**: Arduino / ESP32  
- **Sensors**:  
  - Flex Sensors – finger bending detection  
  - MPU6050 – accelerometer & gyroscope for tremor detection  
  - EMG Sensors – muscle activity signals  
  - Temperature & force sensors (optional)  
- **Actuators**: Mini vibration motors for corrective haptic feedback  
- **Power**: Rechargeable Li-ion battery  
- **Connectivity**: Bluetooth Low Energy (BLE), Wi-Fi  


**📂 Methodology**
Data Acquisition – Flex + IMU + EMG sensors capture tremor & movement data.

Signal Processing – Microcontroller filters noise and extracts features.

Machine Learning – Classifies tremor vs normal movement, predicts motion intent.

Feedback Control – Activates vibration motors to counteract tremors.

Cloud Integration – Logs rehabilitation data, enabling remote doctor monitoring.

Assistive Communication – Converts gestures into commands or speech output.

**▶️ Usage**
Assemble hardware with glove (sensors + actuators + microcontroller).

Upload firmware from /code/smart_glove.ino.

Pair glove with PC/mobile via Bluetooth or Wi-Fi.

Run the ML model (/ml_model/train.py) for tremor classification.

Monitor rehabilitation data via IoT dashboard.

**📊 Results**
Successfully detected tremors and reduced amplitude using closed-loop feedback.

Enabled gesture-based communication for patients with limited mobility.

Real-time monitoring achieved via IoT with <200 ms latency.
**
🔐 Security & Safety**
Encrypted data transfer using MQTT + TLS/SSL

HIPAA-compliant cloud storage for patient data

Biocompatible glove materials to minimize skin irritation

Electrical safety tested for wearable use

**🔮 Future Work**
Integrate AI-powered adaptive therapy for more precise tremor suppression

Add Brain-Computer Interface (BCI) integration for direct neural control

Optimize battery life & wearability with smart fabrics & flexible circuits

5G & Edge Computing for ultra-fast, real-time rehab monitoring

🩺 Biomedical Applications
Rehabilitation therapy for stroke & Parkinson’s patients

Assistive communication via gesture-to-speech

Remote monitoring & personalized therapy recommendations

Enhancing neuroplasticity with biofeedback

