# An-accessible-applications-based-on-EEG-Android-

> A DeepBCI-based brain-computer interface project featuring EEG acquisition and automated Android control.  
> **Totally in Python.**

---

## Program Overview

Collecting brain signals with DeepBCI EEG equipment to implement interaction with Android.

---

## Hardwares

1. **DeepBCI EEG Development Board**
2. **Android equipment**

---

## Technical Description

### 1. DeepBCI
DeepBCI is an accessible, high precision bio-signal acquisition platform which is also an open source community.  
In this system, it serves as an front-end to collect the physiological brain signals, the ADS1299-based circuit system provides a high-performance electrode impedance measurement, noise filtering, and biopotential signal amplification.

* **GitHub Homepage**: [https://github.com/DeepBCI/Deep-BCI](https://github.com/DeepBCI/Deep-BCI)

### 2. Airtest
It is a mature and stable cross-platform UI automation framework which is designed mainly for automated testing, performance profiling, and test scripting across mobile apps.  
In this system, it serves as the scripts to control an android tablet equipment with readable codes and good performance, you can do such as connecting adb serve, touching, swiping, pinching (zoom in or zoom out), inputing something, screenshot and the simulating navigation keys.

* **GitHub Homepage**: [https://github.com/AirtestProject/Airtest](https://github.com/AirtestProject/Airtest)

---

## Why Choosing These Two Frameworks? What's their advantages?

### 1. DeepBCI
* Mature, Stable, Easy to secondary develop based on community experiences.

### 2. Airtest
* **Comparing to Auto.js**: Auto.js is only available to JavaScript, not available to Python, having an inconvenient influence such as there will be an additional communication required (websocket/mqtt etc..) when using across platforms in this program. And it has already stopped maintenance.
* **Comparing to openatx uiautomator2**: Airtest has stock OCR and image display and analysis, you don't need to worry about the compatibility to open-cv, no need to install more libraries at the same time.

---

## Start Quickly

### 1. Set up the environment

1. Install Anaconda, open Anaconda prompt, and input:
   ```bash
   conda create -n YourEnvName python=3.10
   ```
2. Navigate to where you unzip this program, make sure it is the main branch, and input:
   ```bash
   pip install -r requirements.txt
   ```

### 2. Hardware operation


### 3. Connect your Android device
*(Taking Xiaomi Pad 5 and HyperOS 1.0.3 version numbers as an example)*

1. Click OS version for 7 times to enter developer mode. Then find **"USB Debugging"**, **"USB installation"**, and **"WLAN Debugging"**, turn on them both.
2. Enter **"WLAN Debugging"**, remember IP address and port which you will input in the input box in this script.

### 4. Run the program
```bash
python main.py
```
