# Android Media Recorder

This app is based on [Google Android Media Recorder sample](https://github.com/googlesamples/android-MediaRecorder).

The purpose of the app is to record videos and send them to the IVS lab server.

## Prerequisites

- Android SDK 27
- Android Build Tools v27.0.2
- Android Support Repository

## Getting started

This app uses the Gradle build system. To build this project, import the project in Android Studio, build and run the app on an Android device.

## Videos

### Storage

The recorded videos are stored in your device external storage public directory, in a `CameraSample` folder created at runtime.

### Upload

The videos are sent to http://www.ivs.auckland.ac.nz/quick_stereo/upload/videos/ public directory.

## Media recorder package files

- `MainActivity` is in charge of displaying a welcome message and recording videos.
- `SendVideo` activity sends the video to the IVS lab server, through `Upload` class
- `Upload` builds and sends the HTTP upload request to the server.
