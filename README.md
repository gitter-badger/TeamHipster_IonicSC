# CS115 - Team Hipster - Ionic SC 
##Group repository for CS115 group

Everybody in this group is writing code for all aspects of the project, but more formally our roles are: 

Project/Product Manager & Developer: Kangdi Ni

Lead Implementation Developers: John Ta & Andrew Lien

Lead UI/UX Developers: Kent Diao, Taylor Stratton, Bryant Tran


##Summary of the App 

This is a hybrid web application written entirely in javascript for the CMPS 115 - Intro to Software Engineering class at the University of California, Santa Cruz. Our team is using the Ionic Framework as the front-end user interface, and are attempting to write the entire web scraper and parser on the client side for the purpose of the class. Future implementations will be moving the app onto a dedicated server where we will write server sided code that will parse UCSc’s public class page and the app will use the server’s information, instead of UCSC’s 

Our application uses AngularJS’ ‘$http’ requests for the GET and POST request, and we’re using crossorigin.me as a cors proxy for the GET request, in order to get around the CORs issue. So far, POST request is not working for the average user, but once the application gets ported to their respective app stores (iOS and Android), users should be able to search for their classes successfully. 

If you’re a visitor on this repository, and it’s the Fall quarter, you may see a lot of broken, and dirty code. Our aim is to have a fully functional and well designed app by the tenth week, so bear with us and our development process! 

##screenshots 

![Alt text](screenshots/snip1.png?raw=true “Screenshot 1“)

![Alt text](screenshots/snip2.png?raw=true “Screenshot 2“)
![Alt text](screenshots/snip3.png?raw=true “Screenshot 3“)

![Alt text](screenshots/snip4.png?raw=true “Screenshot 4“)

![Alt text](screenshots/snip5.png?raw=true “Screenshot 5“)
![Alt text](screenshots/snip6.png?raw=true “Screenshot 6“)



##Notes to team members (From Andy): 

### Where to start

All of our stuff will be modified under IonicSC/www/ the css, img, js, lib, and templates will have our relevent stuff. Don't worry about the other files. 

### How to start

To set up the dev environment, if you are on the mac, make sure you have Xcode, Android SDK (android studio down is OK), JDK 7, VirtualBox, and Genymotion. This option is not needed for the initial development phases.

What is essential is to have node.js installed on your machine. 

To install cordova: 
` sudo npm install -g cordova `

And to install Ionic: 
` sudo npm install -g ionic `

To install Bower:
` sudo npm install -g bower `

To test app, go to the IonicSC/ root folder and use the

` ionic serve `

command to view the web application. 

Use

` ionic serve --lab `

to view the android and ios version running side by side. 

To add for ios and android platform, the process is as follows:

` ionic platform ios `

` ionic platform android `

To build:

` ionic build ios `

` ionic build android `

To test:

` ionic emulate ios `

` ionic run android //for Genymotion `

`  ionic emulate android //for the slower android emulator in the SDK  `

If you're getting

` Error executing "adb devices": ADB server didn't ACK 

   * failed to start daemon * `

Go to Settings in Genymotion > ADB tab > Use custom Android SDK tools and select the path of your Android SDK installation. 

For the adventerous team members and want to test on your device: 

` ionic run ios `

` ionic run android `


