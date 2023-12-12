# Useable techs: Unity with Vuforia for AR

## What is Vuforia?
* AR Software Development Kit (SDK)
* Created for mobile devices
* Enables creation of AR applications
* Uses: Computer Vision Technology, Image tracking and 3D object tracking

## Unity and Vuforia demo project
In [THIS](https://www.youtube.com/watch?v=9XikHnTiukk&list=PLX2vGYjWbI0Thl0pOCbKWrbbiw7RWiRG7&index=1) video series created by Unity themselves they give a clear demonstration how Unity and Vuforia can be used to create an AR experience. Though this experience is far from what we need but it includes a couple of concepts we also need to use like Image Tracking. Therefore it serves as a basis in getting to know Unity's environment and using Vuforia.

### Key takeaways from this video series
#### Image target behavior
What is the image that the Vuforia system will be looking for?
* Type: Predefined (e.g. from an Unity Store asset), User defined (upload own images to Vuforia website) or Cloud Recognition
* Default trackable event handler: A script that defines how the object will respond when it begins tracking or when it loses tracking. This can then be used to hook in functions.
* Turn off behavior: Only shows objects when the tracking is being done

## Vuforia Engine: How to Create Image Targets
In [THIS](https://www.youtube.com/watch?v=Z4bBMpa4xWo) video created by Vuforia they give a clear explanation and demonstration of how to create image targets using Unity and Vuforia.

### Key takeaways from this video: 
#### Recommendations for image targets
1. At least 12 cm wide
2. A Flat, not glossy image
3. For rounded image targets use Vuforia Cylinder Targets

#### What will you need? 
1. Unity
2. Vuforia SDK

#### Unity: Vuforia Engine configuration
* Needed right here is a licence key -> obtainable for free on the Vuforia developer portal only for development

#### Method 1: Vuforia: Image tracking via development portal
1. Add database
    * Name 
    * Type: Cloud (paid service), device, VuMark
2. Upload image to database -> Add Target
    * Type: **Single image**, Cuboid, Cylinder or 3D Object
    * File: Choose the image .png, .jpg (max 2mb)
    * **Width property**: Physical width of the image in meters (C-units), VERY VERY IMPORTANT not the image size but the actual real world size of the image (e.g. printed out on a a4 page, the width property is the a4 page width)
3. Download database
    * Development platform: Unity Editor

#### Method 1: Use the image target database in Unity
1. Vuforia Engine -> Image Target
    * Image Target Behavior: Set to from database -> import database -> choose database -> choose image
2. Add the asset/model (fbx format) -> drag and drop into assets folder -> drag and drop asset into the imageTarget that is in the Unity scene -> Asset will become child asset of imageTarget
3. Use the Unity play mode to test the project

#### Method 2: Unity: Instant Image Targets
Avoids having to go into the Unity Developer Portal at all, expect for the licence key and allows you to create the image target in Unity itself. 
1. Add into the Unity Scene: Vuforia Engine -> ImageTarget 
2. Image Target Behavior: 
    * Type: From image -> add the image into the Unity Project
    * Texture Type: Sprite (2D or UI)
    * **Width property**: Physical width of the image in meters (C-units), VERY VERY IMPORTANT not the image size but the actual real world size of the image (e.g. printed out on a a4 page, the width property is the a4 page width)
3. Download database
    * Drag and Drop image into the texture object

#### Method 2: Use the image and asset
1. Add the asset/model (fbx format) -> drag and drop into assets folder -> drag and drop asset into the imageTarget that is in the Unity scene -> Asset will become child asset of imageTarget
2. Use the Unity play mode to test the project

*created by Marnik Maes*






