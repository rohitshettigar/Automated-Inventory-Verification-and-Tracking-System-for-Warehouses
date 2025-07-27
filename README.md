#  Automated Inventory Verification and Tracking System for Warehouses

---

##  Abstract

Manual warehouse inventory tracking is error-prone and inefficient. This project presents an **Automated Inventory Verification and Tracking System** using **IoT, cloud connectivity (Firebase), and mobile application support**. It automatically verifies incoming products using RFID, assigns storage slots, and provides real-time tracking via a custom Android app. The system reduces human error, improves speed, and enhances warehouse scalability through ESP32 microcontroller-based automation.

---

##  Acknowledgment

We would like to express our heartfelt gratitude to the faculty and department of Electronics and Communication Engineering, N.M.A.M. Institute of Technology, Nitte, for their valuable guidance and support throughout the course of this project.

---

##  Objectives

- Automate product verification using **RFID technology**
- Assign and display **slot numbers** for verified products
- Provide **real-time inventory updates** using **Firebase**
- Control **servo-operated gates** based on IR detection
- Enable **remote monitoring** via an Android app
- Minimize human error in product handling
- Build a **scalable system** for future expansion

---

##  Methodology

The system works as follows:

1. A product is placed on the conveyor and detected by the first **IR sensor**
2. The **RFID reader** scans the product's NFC tag
3. The product ID is verified against a **Firebase** cloud database
4. If valid, a slot number is assigned and displayed on a **16x2 LCD**
5. A second IR sensor detects the product at the gate
6. A **servo motor** opens the gate to direct the product to its slot
7. The product is tracked via a **mobile app** built using Kotlin and XML

---

##  Hardware and Software Requirements

###  Hardware
- ESP32-WROOM-DA (Wi-Fi enabled microcontroller)
- RC522 RFID Reader + NFC Tags
- IR Sensors ×2
- SG90 Servo Motor
- 16x2 LCD Display (I2C)
- Breadboard, jumper wires
- USB power bank
- Wooden frame + conveyor base

###  Software
- Arduino IDE with:
  - WiFi.h
  - Firebase_ESP_Client.h
  - MFRC522.h
  - LiquidCrystal_I2C.h
  - Servo.h
- Firebase Console
- Android Studio (for Kotlin-based app)


---

##  Results and Discussion

- Products with valid RFID tags are correctly identified and sorted
- Firebase ensures **real-time updates** to product status and storage
- Servo and IR sensors enable accurate gate control
- LCD shows assigned slot number clearly
- Mobile app provides remote access and visibility

 **Mobile App Features:**
- Displays index page, inventory details, search functionality, and results

 **Screenshots:**
![Index Page](outputs/index_page.png)  
![Inventory Details](outputs/inventory_details.png)  
![Search Box](outputs/search_box.png)  
![Search Results](outputs/search_results.png)

---

##  Conclusion

The proposed system successfully automates warehouse operations by using a combination of **RFID verification**, **cloud integration**, and **servo-controlled sorting**. Real-time data synchronization with Firebase ensures accurate inventory management, while the mobile app makes monitoring accessible from anywhere.

Future enhancements can include:
- Multi-lane support
- Motorized conveyor automation
- Obstacle detection with additional sensors

This scalable system can significantly benefit warehouses, logistics centers, and industrial storage environments.

---



