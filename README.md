# flutter_docker
 A docker container for flutter development.

 Contains latest flutter version + latest Android SDK.
 
 You can use this docker container for Remote Development in VSCode.

 # How to

 1. Run the docker deamon
 2. Run your local Android emulator
 3. Run the following command from the Android platform-tools folder: ```adb tcpip 5555```.
 4. Open VSCode and Open Remote Folder and select flutter_docker folder. This will build the docker image and start it up.
 5. Go to the docker container cmd and run ```adb connect 192.168.9.101:5555``` (the ip of the device can be found when running on your local machine: ```adb devices```)
 6. In the docker container: ```flutter run```