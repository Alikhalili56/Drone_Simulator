# **Immersive Drone Flight Simulation**

## **Project Overview**

This project aims to create an immersive drone flight simulation in Unity using Cesium for rendering real-world geospatial data. The application connects to Google Cloud Maps data via an API key, allowing real-time access to dynamic satellite imagery, terrain elevation, and 3D building models. Users can control a drone and explore global locations, experiencing an authentic simulation with real-world data.

## **Features**
- **Real-time 3D geospatial rendering** with **Cesium for Unity**.
- Fly to any location on Earth using **latitude, longitude, and height**.
- Adjustable drone controls (movement speed, rotation, altitude).
- Multiple camera views:
  - **Third-Person**
  - **Bird’s-Eye**
  - **Top-Down**
    
- **Create and Use your own Google Cloud API key to access dynamic real-world data from Google Maps.**

## **Installation**

### **1. Install Unity**
- Download and install **[Unity Hub](https://unity.com/download)**.
- Use **Unity Hub** to install **Unity 6000.0.34f1 LTS**.

### **2. Install Cesium for Unity**
- follow this guide: https://cesium.com/learn/unity/unity-quickstart/

### **3. Install TextMeshPro (TMPro)**
To ensure proper rendering of text in the application, you will need to install **TextMeshPro**:
1. Open **Unity Editor**.
2. In the **Window** menu, go to **Package Manager**.
3. Search for **TextMeshPro** and click **Install**.


### **4. Set Up Google Cloud API**
1. **Sign up** for **Google Cloud** at [console.cloud.google.com](https://console.cloud.google.com/).
2. **Create a new project**.
3. Enable **Google Maps API** and generate an **API Key**.
4. Navigate to Unity>Cesium>Token and Add the **API Key** in **Specify a token** field.

<img width="768" alt="Screenshot 2025-02-17 at 14 42 30" src="https://github.com/user-attachments/assets/e4cd682e-174e-4c71-a09a-7d9a4f6e3d2b" />

A comprehensive guide: (https://www.youtube.com/watch?v=sHrXO_5-YJg).

### **5. Build the Application**
1. In Unity navigate to File>Build Profiles
2. Choose your Preferred Platform like Windows or MacOS
3.Select your scenes : scene 0 should be **Menu** and scene 1 should be **Game**
4.Click on Build, choose a location on your system and wait a few seconds for Unity to finish the build.


**OR** you can add your token after building the application for prefered OS in the **Main Menu** of the application (located in the settings).
<img width="568" alt="Screenshot 2025-02-17 at 14 51 16" src="https://github.com/user-attachments/assets/284924a7-3e4c-42c1-970d-3cd08179152e" />

# **User Manual: Immersive Drone Flight Simulation**

## **Getting Started**

### **Step 1: Setting Up Your Google Cloud API Key**
To ensure the simulation works properly, you need to integrate the Google Maps API by obtaining an API key from Google Cloud.

1. Sign up or log in to Google Cloud at [Google Cloud Console](https://console.cloud.google.com/).
2. Create a new project.
3. Go to **APIs & Services** and enable the **Google Maps API**.
4. Navigate to **Credentials**, and create an **API Key**.
5. Copy the generated API Key.
**(You may use your Api for free for 90 days, Free of charge up to $300)**


### **Step 2: Enter the API Key in the Application**
1. Launch the application.
2. Open the **Main Menu**.
3. Locate the **API Key field**.
4. Paste your **Google Cloud API Key** into the field.
5. Click **Save** to apply the key.

## **Main Features**

### **1. Select a Location**
You can choose any location in the world by entering **latitude**, **longitude**, and **height** coordinates:

1. In the **Main Menu**, find the **Coordinate Input Box**.
2. Enter the coordinates in the following format:
   - **Latitude, Longitude, Height**
     - **Latitude**: A decimal value between **-90** and **90**, where positive values represent locations in the **Northern Hemisphere** and negative values represent locations in the **Southern Hemisphere**.
     - **Longitude**: A decimal value between **-180** and **180**, where positive values represent locations in the **Eastern Hemisphere** and negative values represent locations in the **Western Hemisphere**.
     - **Height**: A numerical value representing the **altitude** in meters (e.g., **100 meters**).
   
   Example:  
   `45.464220, 9.189060, 100` location of the Duomo of Milan
   <img width="136" alt="Screenshot 2025-02-17 at 15 10 07" src="https://github.com/user-attachments/assets/99eddcc5-532a-47db-ac69-e137e246eabe" />


4. Click **Apply** to load the map of the selected area. (Please note that it may take a few seconds depending on your internet connection, so be patient!)

<img width="1552" alt="Screenshot 2025-02-17 at 15 11 50" src="https://github.com/user-attachments/assets/0794028f-afe0-417a-a701-86fd98209c68" />
<img width="1606" alt="Screenshot 2025-02-17 at 15 15 44" src="https://github.com/user-attachments/assets/53b07965-3fc8-4f1b-8f44-a1a5783a3066" />
### **2. Drone Control**
Once your location is loaded, you can control the drone using your Keyboard(Keyboard control guide is available) and explore the Area.


#### **Keyboard Control Guide**:
- Find a complete guide to the keyboard controls under the **Help** menu, for easy reference.
  <img width="947" alt="Screenshot 2025-02-17 at 15 20 28" src="https://github.com/user-attachments/assets/95cfe5d3-7ca6-4b21-84d8-68bf10ee562e" />


## **Troubleshooting**

### **Common Issues:**
#### **Application Crashes or Fails to Load Location**:
- **Solution**: Ensure you’ve added a valid Google Maps API Key in the **Main Menu**.
- **Solution**: Ensure to insert the Geographical coordinates in a valid format.
- **Solution**: Check your internet connection to ensure real-time data is loaded properly.

#### **Lag or Slow Performance**:
- **Solution**: Before Building your application in unity Navigate to Game Scene on Navigate to CesiumGeorefrence>Cesium3DTielset Heirachy then on inspector increase the calue of **Maximum Screen Space Error**.
- **Solution**: Ensure no other resource-heavy programs are running in the background.

## **FAQs**

**Q: How do I fly to a new location?**  
A: Simply enter the new latitude, longitude, and height in the **Coordinate Input Box**, and click **Go**. The map will automatically load your new destination.

**Q: What if I don’t have an API key?**  
A: You’ll need to sign up for **Google Cloud**, enable the **Google Maps API**, and generate an **API Key** to use the application fully. Without the key, the geospatial data won’t load correctly.

**Q: Can I use this for educational purposes?**  
A: Absolutely! This application is designed for students, researchers, and anyone interested in exploring real-world geospatial data in an interactive manner.






