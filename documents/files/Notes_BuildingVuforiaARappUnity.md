# Proof of Concept Documentation: Augmented Reality Application with Vuforia in Unity

## Introduction

This documentation guides you through the process of creating a Proof of Concept for an Augmented Reality (AR) application using Vuforia and Unity. Follow the steps below to efficiently develop and build an AR application for mobile platforms.

### Requirements

- Unity
- Vuforia Engine
- iOS development environment (Xcode) (if you plan to build for iOS)

## Step 1: Installation and Configuration

1. Download and install Unity from the official Unity website: [Unity Hub](https://unity.com/unity/features/hub).
2. Open Unity Hub and create a new project with the appropriate settings for your platform.
3. Import the Vuforia Engine Package into Unity. This can be done via the Unity Package Manager.

## Step 2: Integration of Vuforia in Unity

1. Add an AR Camera to your scene.
2. Select the AR Camera and open the Vuforia Engine Configuration.
3. Add the App License Key obtained from the Vuforia Developer Portal.

## Step 3: Configuration of Vuforia Developer Portal

1. Go to the [Vuforia Developer Portal](https://developer.vuforia.com/).
2. Create a new project and add a database via the Target Manager.
3. Add all necessary images as targets to the database (note: the width is the physical width of the image in meters).
4. Download the database and drag it into the 'Assets' folder in Unity.

## Step 4: Create Image Targets in Unity

1. Add an Image Target to your scene.
2. Select the Image Target and choose the type 'Select from Database'.
3. Select the specific Image Target from the downloaded database.

## Step 5: Place Objects on the Image Target
I have designed custom objects using Fusion 360 and integrated them into the app.

1. Drag the desired object from the 'Assets' onto the Image Target in the scene.
2. Position and scale the object so that it is clearly visible on the Image Target.

## Step 6: Build Settings and Deploy

1. Go to the Build Settings in Unity.
2. Select the desired platform (e.g., iOS).
3. Build the project and open it in the corresponding development environment (e.g., Xcode for iOS).
4. Configure signing with your own account/team and bundle identifier. (For Xcode)

## Issues Encountered:

### Issue: No access to the iPhone camera

#### Solution: Unity Player Settings

1. Check the Unity Player Settings.
2. Ensure the correct "Camera Usage Description" is set in the Player Settings.
3. Go to Edit > Project Settings > Player > iOS > Other Settings.
4. Fill in the "Camera Usage Description" field with a clear and informative description.

## Conclusion

With the right settings in Unity and Vuforia, developing an AR application is a plug-and-play process. Make sure all steps are followed carefully, and you should have a working Proof of Concept. Don't forget to regularly consult the official documentation of Unity and Vuforia for any updates and additional information.
