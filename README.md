curl-android-ios
================
The goal of this project is to provide a pre-compiled version of libcurl to be
used in Android and iOS.

It uses cURL from the upstream repository and it's updated frequently.

For Android, it also uses OpenSSL from its upstream repository.

If you want to build the library, scripts are provided for both platforms.
Test projects are also provided for both iOS and Android.

# Building
* Clone this repo `git clone git@github.com:gcesarmza/curl-android-ios.git`
* Clone submodules `git submodule init && git submodule update`
* Make sure you have installed autoconf, automake and libtool or install them with `apt-get` or `brew`
* When building on Mac OS make sure you have Xcode Command Line Developer Tools installed
```
xcode-select --install
```

## Building for Android:
This project is not used anymore for Android - although the prebuilt libraries are still stored
within this project. A special docker container is used for building the more recent versions
of openssl and curl. Especially openssl has to be updated to 1.1.0 as in 1.0.2 it has some serious 
threading issues



## Building for iOS
```
cd curl-android-ios/curl-compile-scripts
./build_iOS.sh
```
