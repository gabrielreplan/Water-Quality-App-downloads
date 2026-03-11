Water Quality Monitoring App 🌊
An Android application designed to interface with an ESP32-based water quality monitoring system. This app allows users to configure WiFi credentials and Blynk tokens on the ESP32 via a local Access Point (AP) and visualize water data.

Features 🚀
WiFi Provisioning: Easily connect your ESP32 to your home network without hardcoding credentials.

Blynk Integration: Configure Blynk Template IDs and Auth Tokens directly from the app.

Real-time Monitoring: (Mention if you use MPAndroidChart or Lottie for visuals based on your dependencies).

Material 3 Design: Modern UI using Bottom Sheets and CardViews.

Hardware Required 🛠
Microcontroller: ESP32 (configured with an AP named ESP_WaterQuality).

Sensors: Compatible with pH, TDS, and Turbidity sensors.

Connectivity: 2.4GHz WiFi.

How to Use 📱
Power on the ESP32: Ensure it is in Configuration Mode (broadcasting the ESP_WaterQuality SSID).

Connect Phone: Connect your smartphone's WiFi to the ESP_WaterQuality network.

Open App: Launch the Water Quality App and navigate to WiFi Setup.

Configure:

Enter your Home WiFi SSID and Password.

Enter your Blynk Auth Token and Template details.

Save: Click "Save Credentials." The app sends an HTTP POST request to http://192.168.4.1/save.

Restart: The ESP32 will reboot and connect to your home network.

Download & Installation 📦
You can find the latest ready-to-install version in the Releases section.

Download the app-release.apk.

Enable Install from Unknown Sources on your Android device.

Install and run.

Tech Stack 💻
Language: Java / Kotlin

Networking: OkHttp3 (for ESP32 communication)

UI Components: Google Material Design, Lottie Animations, MPAndroidChart.

Permissions: Requires ACCESS_FINE_LOCATION and NEARBY_WIFI_DEVICES to scan for the ESP32 AP.
