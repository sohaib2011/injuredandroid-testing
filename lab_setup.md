# Lab Setup: Injured Android Testing

## Required Tools
- **JADX GUI** – For decompiling APKs and analyzing code
- **ADB (Android Debug Bridge)** – For interacting with the Android device/emulator
- **Apktool** – For reverse engineering Android applications
- **Android Studio** – For running an emulator and debugging

## Getting Injured Android
**Note:** Injured Android is **not available on Google Play Store** and must be downloaded from GitHub.

1. Go to the official GitHub repository:  
   [https://github.com/B3nac/InjuredAndroid](https://github.com/B3nac/InjuredAndroid)
2. Click on **"Releases"** on the right side of the page.
3. Download the latest **APK file**.

We want to download the APK onto our Android emulator to thoroughly conduct a penetration test of the application. Here, we will analyze its behavior, intercept the traffic, and test for vulnerabilities.

---

## Step-by-Step Setup

1. Install `InjuredAndroid.apk` and ensure you are in the correct directory to run the following command:  
   **adb install <application.apk>**
   
    <img src="https://github.com/user-attachments/assets/845a2801-0fc6-4e15-bdcb-4669c0e35d9c" width="150">
    
   <img src="https://github.com/user-attachments/assets/e0377c1e-8711-4c39-9d24-c73da04c0d6f" width="400" height="50">
   
   As shown in the images above, the application has been successfully installed inside the emulator.  


### Now, for further flags and tasks, we need to run the emulator and interact with it through ADB shell.

5. Start an emulator so we can interact with it in the ADB shell:  
   
   <img src="https://github.com/user-attachments/assets/f0b22ec3-b76b-4047-9f88-ebd707901897" width="400">

6. To ensure that we can interact with the emulator through the terminal, run:  
   **adb shell**
   
   <img src="https://github.com/user-attachments/assets/437f9cd2-954c-4458-8470-e3efda2dcdc9" width=400>

   We have now successfully connected to the shell on the emulator and now have direct access to interact with the device. 
