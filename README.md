# ui-auto-testing

## Install JDK(version >= 8.0) & Configure JAVA_HOME and PATH variable

## Download & Install node.js

## Download & install python
https://www.python.org/downloads/

## Download & install android studio & Configure ANDROID_HOME and PATH variable
https://developer.android.com/studio
install android SDK, 
SDK Tools
    Build Tools
    NDK
    Command-line Tools
    CMake
    Android Auto API Simulators
    Android Simulator
    Platform Tools
    Tools
    Google Web Driver
```
export ANDROID_HOME=/Users/liuchengqiang/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME:$ANDROID_HOME/platforms:$ANDROID_HOME/tools:$ANDROID_HOME/cmdline-tools:$ANDROID_HOME/platform-tools:$ANDROID_HOME/bundle-tool
```

## Download & install Xcode and do the following configuration
Xcode–>Preferences–>Locations–>Command Line Tools 
select the version

## Install appium & appium-doctor
```
mkdir -p $ANDROID_HOME/bundle-tool
wget https://github.com/google/bundletool/releases/download/1.10.0/bundletool-all-1.10.0.jar
mv bundletool-all-1.10.0.jar bundletool.jar

brew install carthage
brew install lyft/formulae/set-simulator-location
npm install -g ios-deploy
brew install ffmpeg
npm install -g mjpeg-consumer
brew install gstreamer gst-plugins-base gst-plugins-good gst-plugins-bad gst-plugins-ugly gst-libav
brew tap wix/brew
brew install applesimutils
brew tap facebook/fb
brew install idb-companion
pip install fb-idb
brew install cmake
brew install opencv
export OPENCV4NODEJS_DISABLE_AUTOBUILD=1
export OPENCV_LIB_DIR=/opt/homebrew/Cellar/opencv/4.5.5_2/lib
npm i -g opencv4nodejs

npm install -g appium appium-doctor
appium-doctor --android
appium-doctor --ios
```

## Download Senlenum 4 and start it
https://www.selenium.dev/downloads/
```
~~java -jar selenium-server-4.1.4.jar standalone~~
```

## Install user level pipenv
```
pip install pipenv
```

## Install the latest version robot framework
```
pip install robotframework
```

## Run the test case
go to project folder and run the following command
```
pipenv run robot --argumentfile src/config/arguments.robot product/tests/pc
```