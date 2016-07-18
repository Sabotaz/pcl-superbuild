CMake build scripts for cross compiling PCL and its dependencies for Android and iOS.

## Requirements

* Android NDK, Revision 8d
* Android SDK (unsure about specific version)

# Building for Android

    $ mkdir build && cd build
    $ cmake -DBUILD_IOS_DEVICE:BOOL="OFF" ../
    $ export ANDROID_NDK=${PATH_TO_ANDROID_NDK_R8}
    $ make

# Releases
Releases are downloadable in the release page.

Compiled with android-ndk-r8 for armeabi-v7a.

## Content:
 * boost-android (1.45)
 * eigen
 * flann-android
 * pcl-android (1.7.1)

## Missing:
 * VTK and VTK-dependent pcl modules
 * poisson (from pcl_surface)

