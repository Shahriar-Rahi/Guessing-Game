Guessing Game - RAHI


  

 

Abstract
Guessing game is a simple & easy game where you have to guess the correct number in different game mode & difficulties. This report details the development of a Guessing game application that is written in Java, designed in XML and developed to work in Android systems. I’ve used Android Studio as development environment.





Acknowledgments

While implementing the application I took references from many open source resources across the web. To find solution of different problems I were in while working in the project I’ve used: 
http://stackoverflow.com/

The app was developed for android platform by using the official documentation and tutorials from Android Developers. For help I’ve used:
https://developer.android.com/training

And as always for any kind of problem I had a quick visit to:

https://www.google.com/

 
Contents

1. Introduction
	1.1 Guessing Game and Its Rules
	1.2 Aims and Objectives

2. Software & Tools
	2.1 JDK
	2.2 SDK
	2.3 Eclipse
	2.4 Android Studio

3. Design
	3.1 Code Structure
3.2 Game Source
	3.3 GUI
		3.3.1 startscreen.xml
		3.3.2 main.xml
		3.3.3 app_menu.xml ,  arrary.xml & preferences.xml 

4. Implementation
	4.1 Version Control & Gradle Building
	4.2 StartScreen.java
	4.3 GuessingGame.java
	4.4 Preferences.java
	4.5 HelpDialog.java and DeveloperInfo.java
	4.6 Intent

5. Discussion & Conclusion
	5.1 Obstacles
	5.2 Achievement
	5.3 Future Plan
	5.4 Last few Words
 
1. Introduction


1.1	Guessing Game and Its Rules:

Guessing Game is an easy game where you have to guess the correct number. This game is a great source of fun too & addictive also (For people of age 10+). There are two modes: Time and Tries.

Time mode gives you 1/2/3 minute(s) to come to as high level as possible. For level 1 the range of hidden number is 0-10. For each level up, the range for the random number is increased by 10 times.

Tries mode gives you a number in a range according the chosen difficulty: Easy 0-10, Normal, 0-100, Hard 0-1000, Harder 0-10000, Hardest 0-100000, The goal is to find the number in as few tries as possible.


1.2	Aims and Objectives:

The first objective of this game is to generate a random number according to the chosen difficulty of the game.

Then the game takes input from the player and checks the given number with the hidden (randomly generated number). If the input is correct then the game will go to the next level otherwise the player will be informed about the given number whether the number is Greater than or lesser than the correct number. All those things are done in GuessingGame.java activity.
 
2. Software & Tools

2.1 JDK: JDK is Java Development Kit used for developing, debugging and monitoring Java applications. Java Platform lets us develop and deploy Java applications on desktops, android platform and servers, as well as in today's demanding embedded environments. Java offers the rich user interface, performance, versatility, portability, and security that today's applications require. In my project JRE version 8 is used for Java.   


2.2 SDK: A software development kit (SDK or devkit) is typically a set of software development tools that allows the creation of applications for a certain software package, software framework, hardware platform, computer system, video game console, operating system, or similar development platform. Later on I’ll discuss about which SDK I’ve used to complete my project.
 
2.3 Eclipse:  Eclipse is famous for our Java Integrated Development Environment (IDE).  I’ve used Eclipse to check my raw code in Java before working on Android Java in platforms like Android Studio.
 
 

2.4 Android Studio :  It’s the official Android IDE from Google & best way to build Android apps. I’ve spent most of the time working on this project in the Android Studio 2.3.   It comes with different Emulators which is really fun to work with.
 
                     3. Design


3.1 Code Structure:  

 
            
			Fig: Code Structure




3. 2 Game Source: The source code for the game is divided into packages with appropriate names.
 

3.3 GUI:
3.3.1 startscreen.xml:

  
3.3.2 main.xml:
 

3.3.3 app_menu.xml, arrary.xml & preferences.xml:
     
4.Implementation
4.1 Version Control & Gradle Building:
The application is built using Android Studio 2.3, an IDE for Android development that Google developed in cooperation with JetBrains, based on the IntelliJ Platform and the existing functionality of IntelliJ IDEA Community Edition.
The source codes are written in Java programming language. JRE version 8 is used for Java. The build system used for the app is Gradle which is a JVM based build system.

The SDK Version used for building the android app is Android SDK 25 that will support the API level 25 (Nougat) while the minimum API required is API level 4, so the app is compatible for any android device having API and above.
 

4.2 StartScreen.java: In this class, In the upper right corner there are a menu option to show menu in game. This menu is created in this class by onOptionsItemSelected(MenuItem item)  method. Many of new Intent is created in this class.
 

4.3 GuessingGame.java:
I’ve worked with 3 buttons activity here and activity of 1 drop menu. Where Start Game button is used to start game, Settings button show modes & difficulties and EXIT button ends the game. This is the main Class of this game. Generating number, checking number, mode & difficulty switching, activity of keyboard, result generation & showing etc. All the main activity of game is handle in this Class by creating and calling various methods. Such as public void checkNumber(View view) this method is created to check the number which is given by the player. 

4.4 Preferences.java:
This class is used to run the xml file preferences.xml

 


4.5 HelpDialog.java and DeveloperInfo.java:
These two class is used to run the xml file help.xml & devinfo.xml  


4.6 Intent: An Intent is an object that provides runtime binding between separate components, such as two activities. The Intent represents an app’s "intent to do something." You can use intents for a wide variety of tasks
 
Here the starActivity() method starts an instance of the GuessingGame specified by the Intent.




5. Discussion & Conclusion
5.1 Obstacles:
1. Working with Android Studio & Java was completely a new experience for me. Had to learn first to complete the project.
2. I adopt these things by video tutorials, text tutorials, internet and learning materials given by the tools themselves. It's a matter of time, patience and hard work.
3. It was very much tough to work with Intents at first but after implementing I’ve captured the whole concept of it.
4. Creating the time was a little bit challenging for me, but at last all happened as I wanted.
5.Building Gradle for the first time was a headache.
After all the thing is that a game project is not a project for one people, a team work would’ve been great!

5.2 Achievement:

1. Now I know much more about Java for android, core Java, JDK, SDK, Gradle, Android Studio, Eclipse, XML, Intent etc.
2. Now I got the ability to design a project & implement in a fixed period of time which will help me in future projects.
3. The main thing is that as a software engineer, skill and expertise to create a software & product report is now better than before. 
4. Growing creative thinking and imagination capability.
5. Experiencing the feeling of making the first ever software of my life which is an Android Game.

5.3 Future Plan:
•	Level, mode & difficulty Extension
•	Improve Graphical Representation
•	Introduce new game features
•	Take user response and work as they suggest
•	Introduce other Guessing options like word guessing as the current game is only based on number guessing.
•	Introduce multiplayer mode

5.4 Last few Words:
I’ve learned a lot through this project. This project has sharpened my concept of android Java, core Java, XML, SDK, JDK, the software-hardware interface etc. 
I’ve learned a lot about different documentation. The piece of software(game) I’ve developed is intended to serve the gamers of the world. This project not only helped me to bring my skills into a product but also encouraged me to make more quality software & games in near future. 
There were times that I almost lost hope but recovered through constant concentration and hard work. If anyone has any kind of suggestion, improvements, more efficient development idea please feel free to communicate with me.


