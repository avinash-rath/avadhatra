# avadhatra
Our shoe project.

In this hectic everyday life, it is hard to keep track of our fitness status. As hard work and smart work go
simultaneously, our fast pacing lives demand more from the technocrats. Here comes the role of the
revolutionary shoe "Avadhatra". This nimble creation is well-equipped with an accelerometer, gyroscope,
pulse rate sensor which update the user of their health status on a Native app
where the data is transferred via Wifi. This data is then stored on a cloud server from where the user
can access the data anytime anywhere. These shoes are capable of alerting the user’s emergency contacts when they are in any
imminent danger of life by non-natural causes by reading their frantic and erratic movements
(which are not generally done in a day-to-day life, the device learns it from the user’s day-to-day
activities) and converting it into digital data which is sent to the mobile application via Bluetooth.  


The files uploaded in the repo are only the code written by us (library implementation also included). The imports are at the top of the code in each file. However, the installation of the libraries such as pubspec.yaml file etc. are not shown. The repo also does not include any kind of build files. Only the code written has been submitted for evaluation.

# Files Description
1. The App's files are placed in app_data folder.
2. The arduino code is found in the repository itself.
3. The app is built on flutter SDK. The code execution starts from main.dart. The Splash screen will be the first page the user     experiences.
4. Many Routes from the HomePage are created that can be found in the main.dart file.
5. Main page has an SoS button at the bottom end as a floatingActionButton, that is used to get the location of the device, right now it shows only the location as an alertDialog.
6. Buddy and Account information with forms and new routes were added. Here the account info is about the person using the shoe, and the buddies refer to the emergency contacts of the users, to which the SMS text will be sent(Alert Message).

# Requirements

#HARDWARE:
• Arduino-uno
• Pulse rate sensor
• Accelerometer sensor(GY-521)
• Wifi module(ESP8266)

#SOFTWARE:
• Firebase
• Flutter

# Functions
1. The pulse Rate sensor interfaced with arduino is keeping a track of the pulse rate of the user and the data is sent to the firebase through Wifi.
2. The accelerometer is counting the number of steps and sending the data in real time to the firebase through Wifi.
3. The collected data is stored in the firebase cloud and is regularly displayed on the App.
4. It also keeps a track of the location of the user using SoS.
5.  In case of emergency a security alert message will be sent to the buddy contacts provided by the user along with the current location.
