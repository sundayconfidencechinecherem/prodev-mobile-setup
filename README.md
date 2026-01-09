# Mobile Development Environment Setup

## Overview
This project documents the setup of a mobile development environment using the Expo Framework for React Native. The setup focuses on using Expo Go to test applications on physical devices, providing a cost-effective alternative to device emulators.


### Required Tools
- **Node.js LTS** (v18.x or higher recommended)
- **VS Code** (or any preferred IDE)
- **Compatible Operating System**: macOS, Linux, or Windows
- **Physical Device**: Android or iOS smartphone/tablet

## Installation Steps

### 1. Expo Go Installation

#### For Android Devices:
1. Visit the [Expo Go homepage](https://expo.dev/go)
2. Select the latest SDK version
3. Click "Install for Android"
4. Download from Google Play Store
5. Open Expo Go app after installation
6. Create an account or log in

#### For iOS Devices:
1. Visit the [Expo Go homepage](https://expo.dev/go)
2. Select the latest SDK version
3. Click "Install for iOS"
4. Download from Apple App Store
5. Open Expo Go app after installation
6. Create an account or log in

## Setup Verification

### Check Your Environment
Verify your setup by running the following commands in your terminal:

```bash
node --version
npm --version
```

### Test Expo Installation
```bash
npx create-expo-app test-app
cd test-app
npx expo start
```

## Challenges Faced & Solutions

####  **Expo Go Connection Issues**
- **Problem**: Unable to connect to development server
- **Solution**: Ensure both computer and device are on the same network


## Project Structure

```
mobile-development-setup/
├── README.md          
This is a documentation file and all you need to know about this project.
(Future project files will be added here)
```


 **Start Development Server**:
```bash
npx expo start
```

3. **Connect Physical Device**:
   - Scan QR code with Expo Go app (Android)
   - Scan QR code with Camera app (iOS)
   - OR manually enter the connection URL

4. **Verify Connection**:
   - Device should load the default Expo app
   - You should see "Open up App.js to start working on your app!"


#
*Last Updated: [9/12/2026]*
#
*Environment Verified: Node.js v[22.20.0], Expo Go v[54.0.31]*
##
Author: Sunday Confidence Chinecherem*