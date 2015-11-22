Uses apple's squarecam example to detect faces. 

Modifications done: 
Facial features such as height and width are extracted from detected faces, changing width or height is compared between frames to predict if the person is moving closer or farther from camera. This is an attempt to get estimates of moving person by using only face detection. 

Outstanding Problems: Data received is repreentative of the motion of the person but noisy. Rolling average or Kalaman filter needed to smoothen out data toget better predictions. 

Dependencies for getting SqaureCam example to run: 
### SquareCam ###

===========================================================================
DESCRIPTION:

SquareCam demonstrates improvements to the AVCaptureStillImageOutput class in iOS 5, highlighting the following features:
- KVO observation of the @"capturingStillImage" property to know when to perform an animation
- Use of setVideoScaleAndCropFactor: to achieve a "digital zoom" effect on captured images
- Switching between front and back cameras while showing a real-time preview
- Integrating with CoreImage's new CIFaceDetector to find faces in a real-time VideoDataOutput, as well as in a captured still image.
     Found faces are indicated with a red square.
- Overlaid square is rotated appropriately for the 4 supported device rotations.
===========================================================================
BUILD REQUIREMENTS:

Xcode 4.2 or later; iPhone iOS SDK 5.0 or later.

===========================================================================
RUNTIME REQUIREMENTS:

iOS 5.0 or later. This app will not deliver any camera output on the iOS simulator.

===========================================================================
APIs USED:

ALAssetsLibrary - to write to the photos library
AVFoundation
AVCaptureConnection
AVCaptureDevice
AVCaptureDeviceInput
AVCaptureSession
AVCaptureStillImageOutput
AVCaptureVideoDataOutput
AVCaptureVideoPreviewLayer
CoreImage
CIFaceDetector
===========================================================================
Link : https://developer.apple.com/library/ios/samplecode/SquareCam/Introduction/Intro.html
