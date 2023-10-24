# Useable techs: Unity with Vuforia for AR

## What is Vuforia?
* AR Software Development Kit (SDK)
* Created for mobile devices
* Enables creation of AR applications
* Uses: Computer Vision Technology, Image tracking and 3D object tracking

## Unity and Vuforia demo project
In [THIS](https://www.youtube.com/watch?v=9XikHnTiukk&list=PLX2vGYjWbI0Thl0pOCbKWrbbiw7RWiRG7&index=1) video series created by Unity themselves they give a clear demonstration how Unity and Vuforia can be used to create an AR experience. Though this experience is far from what we need but it includes a couple of concepts we also need to use like Image Tracking. Therefore it serves as a basis in getting to know Unity's environment and using Vuforia.

### Key components

#### Image target behavior
What is the image that the Vuforia system will be looking for?
* Type: Predefined (e.g. from an Unity Store asset), User defined (upload own images to Vuforia website) or Cloud Recognition
* Default trackable event handler: A script that defines how the object will respond when it begins tracking or when it loses tracking. This can then be used to hook in functions.
* Turn off behavior: Only shows objects when the tracking is being done

