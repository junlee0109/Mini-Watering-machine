# Mini-Watering-machine


# 🌱 Mini Watering Machine (스마트 화분 자동 급수 시스템)

## 📌 프로젝트 개요 (Project Overview)
이 프로젝트는 **아두이노 UNO**와 다양한 센서를 활용한 **스마트 화분 자동 급수 시스템**입니다.  
토양 수분 센서를 이용해 흙의 건조 상태를 감지하고, 자동으로 워터 펌프를 구동하여 화분에 물을 공급합니다.  
또한 **HC-06 블루투스 모듈**을 통해 스마트폰과 연동하여 수분 상태 확인, 강제 급수 명령을 내릴 수 있습니다.  
LCD 화면에는 현재 수분 값과 동작 상태가 표시됩니다.  

This project is a **Smart Plant Watering System** built with **Arduino UNO** and various sensors.  
It monitors soil moisture using a **capacitive soil sensor** and automatically activates a **water pump** when the soil is too dry.  
Through the **HC-06 Bluetooth module**, the system can connect to a smartphone for monitoring soil data and manual watering control.  
An LCD screen displays the current soil moisture level and operation status.  

---

## ⚙️ 주요 기능 (Features)
- 🌱 **자동 급수 (Automatic Watering)** : 토양 수분 값이 일정 임계치 이하일 때 자동으로 펌프 동작  
- 📲 **스마트폰 제어 (Smartphone Control)** : 블루투스를 통한 강제 급수 기능  
- 💧 **실시간 수분 모니터링 (Real-time Monitoring)** : LCD에 현재 수분 값 표시  
- ⏱ **최근 급수 시간 확인 (Last Watering Log)** : 마지막 급수 시각 확인 가능  
- 🔔 **부저 알림 (Buzzer Alert)** : 펌프 동작 시 알림음 발생  

---

## 🔧 사용 부품 (Components Used)
- Arduino UNO (또는 Nano)  
- Soil Moisture Sensor (정전식 / Capacitive)  
- I2C LCD 16x2  
- HC-06 Bluetooth Module  
- 1-Channel Relay Module (5V)  
- 5V DC Water Pump + 1N4001 Diode (flyback protection)  
- Active Buzzer  
- Jumper wires, Breadboard  

---

## 🖥 회로 설명 (Circuit Description)
- Soil Sensor AO → Arduino A0  
- LCD SDA/SCL → A4/A5  
- HC-06 TX → D2, RX ← D3  
- Relay IN → D8 → Pump control  
- Buzzer → D6  

---

## 🚀 실행 방법 (How to Run)
### 한국어
1. 아두이노 IDE에서 코드를 업로드합니다.  
2. HC-06을 스마트폰과 블루투스로 페어링합니다 (기본 비밀번호: 1234).  
3. LCD에 현재 수분 값과 상태가 표시됩니다.  
4. 토양이 마르면 자동으로 펌프가 동작합니다.  

### English
1. Upload the code using Arduino IDE.  
2. Pair HC-06 with your smartphone (default password: 1234).  
3. Check the current soil moisture and system status on the LCD.  
4. Pump will automatically activate when soil is dry.  

---

## 📜 라이선스 (License)
이 프로젝트는 교육 및 개인 학습 목적에 자유롭게 사용할 수 있습니다.  
This project is open for educational and personal learning purposes.  
