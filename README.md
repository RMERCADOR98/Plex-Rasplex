![Banner](https://drive.google.com/uc?export=view&id=1mj7AOSJV2LlBd4YbfKGKPjYO8RTfCK-t "Banner")

Being the first project i´ve ever made with a Raspberry Pi, i was challenged to learn how to use this "mini computer" as a plex media player.

I´m going to share all the steps i made in order to use a Raspberry into a portable device to connect anywhere i want.

* [Plex](#plex)
* [RasPlex](#rasplex)
* [Raspberry](#raspberry)

# Plex 

Plex is a **Media Player** that allows you to stream your Multimedia content, either movies, songs, photos ...

It´s an excellent app because you can see your content anywhere as long as you have your Plex Server Running directly where your files are stored! Nowadays you can access them with your Phone, Tablet, PC or even in a Raspberry Pi, which turns any "old" TV into a Smart TV.

### 1. Create a Plex account

Go to [Plex][1] and Sign Up with whatever´s handy to you (Email,Facebook...).

### 2. Download and Install Plex Media Server

Go to [Plex Media Server][2] and download it for your chosen Operating System. 

Then follow the steps of the installation.

![PlexInstall](https://drive.google.com/uc?export=view&id=1y4oajmuvy5bAiMLld4okZ8Mlnbs1LxcD "Plex Install")

### 3. Open the server

Once installed, open Plex Media Server which is going to take you a web page that in the reality is your server running in your computer, the first part of your link it´s your IP address (http://127.0.0.1:5000/, for example).

### 4. Create a new library

On the left menu, Click a "More >" button

![PlexInstall](https://drive.google.com/uc?export=view&id=1Q62KW4ND2EDpjlp8FONHIXKDVE0AiLRw "Plex Install")

Then, it will appear your libraries, which will be connected to your computer.  
To add a Library, you need to click on "+" button next to your computer name and a pop up will appear.

![PlexInstall](https://drive.google.com/uc?export=view&id=19e5wETBySYqw7cViweAT0FtGGTo5r_1N "Plex Install")

Once the Pop Up appear, you will need to chose the type of library you need (because each library type only reads some formats). Give it a name and an idiom, then, chose the a directory in your computer that you want to be connected.

![PlexInstall](https://drive.google.com/uc?export=view&id=1fYbqCb9BqoKhyXODzkC080Ni_bPQXOkL "Plex Install")





# RasPlex 

Rasplex is what makes possible transform the Raspberry Pi into a plex client, which means that we can access our plex server (that will be our computer) and see our content that we have stored.

### 1. Download and Install Rasplex

Go to [Rasplex][3] and download Rasplex according to your operating system. 

After you done the download, follow the steps during installation.

### 2. Raspberry Pi Model

Once you have opened the program, you will need to chose your raspberry model, therefore, you only need to know this:

* Raspberry Pi -> Raspberry Pi models 0 to 1
* Raspberry Pi2 -> All Raspberry Pi models above 1

### 3. Rasplex Version

If you have a Raspberry Pi until version 3, great! You can chose the latest version of Rasplex and follow to the next step! 

Although... 

If you have a Raspberry Pi 3B+ or superior, you need to chose another version, because newer versions don´t support newer Raspberries. 

The solution i found, was going to their list of [repositories][4] on GitHub and after reading and searching, i found that the version [1.8.0.0][5] works just fine! (I have used a Raspberry Pi 3B+)

If you get stuck on the famous "Rainbow Screen", you might need to check a few things:
 * Your SD card needs to be at least **class 10** and have **4GB**
 * The Power Supply needs to be at least **2A at 5V** ( i recommend using the power Supply that comes with the kit, in case you buy one ), it might change the voltage depending on your Raspberry version 
 * Be sure you selected the right **Rasplex version** or **Raspberry Model** on the Rasplex settings according to the Raspberry Model

 
### 4. Download the image
 
 If you selected the last version of Rasplex, you can Click the "Download" button and select the path you want to download. 
 
 If you need to chose another version you downloaded from GitHub or anywhere else, you can click on "Select Image", chose it , and continue to the next step. 
 
### 5. Select your SD card
 
 In the dropdown menu, it will appear the SD cards you have connected, chose the one you want to target and continue.
 
 In case of don´t show any, check if it is well connected to the computer or the adapter (as well as the cables, in this case)
 
 
### 6. Write SD card
 
 With your image already selected,click on "Write SD card" now it´s going to insert it into your SD Card, for the Raspberry Pi understand it. 
 
 **Only take off the SD card when the writing is finished!** (check the down left corner).
 
 
# Raspberry 

### 1. Insert SD card and plug cables

It´s important to have everything connected to the board before turning it on, just to be sure that everything goes right and you don´t have any errors. 

* Plug the HDMI cable to the monitor or TV
* Plug your Ethernet cable (if your board as it, you can use the WiFi too, just be aware that Ethernet is more stable)
* Plug your keyboard or your remote controller (be aware that the controller needs to be directly connected to the board by some kind of connector and not to the TV)
* Insert the SD card

And finally you can plug it in! 

### 2. Boot

If it went good for you, Great! You can follow the next step!

If you got stuck in the "Rainbow Screen", don´t freak out, it happened to me as well! :)

* **Small Square** -> If it appears a small square in the corner of your screen, you might not have enough power in your power supply

* **Big Square** -> This means that the board as enough power and can read the SD card but the image is not the correct one, check the [Rasplex](#rasplex) section again

### 3. Chose the Network 

Connect to your Network via WiFi using the Router password or simply just connect to the network via Ethernet. 

### 4. Accept the remote access

Just accept the automatic configuration if you don´t want to go deeper into connections.

### 6. Screen Calibration

For the most cases it´s okay the way it is and you can just proceed to the next step , although, if your screen looks funky, try to adjust the settings you like.

### 7. Log in into your Plex account 

To Sign in you can either:

* **Use the Pin**, going to the link Rasplex gives you and right the Pin on the screen on that Link
 
* **Connect Manually**, just putting your email and password will allow the permission to access the server.


### 8. Ready to go! 
 
 After your connection is confirmed, you will be directed to the Rasplex Menu, and travel between your libraries! 


[1]: https://www.plex.tv
[2]: https://www.plex.tv/media-server-downloads/#plex-media-server
[3]: http://www.rasplex.com/get-started/rasplex-installers.html
[4]: https://github.com/RasPlex/RasPlex/releases
[5]: https://github.com/RasPlex/RasPlex/releases/tag/PRE-1.8.0b%2B
