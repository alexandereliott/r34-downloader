# rule34-paheal-downloader
A program to download all the images of a given tag from https://rule34.paheal.net [Warning - Not Safe For Work]

The website has a one request a second limit, thus users with fast internet connections won't max out their bandwidth.

![Screenshot of program](r34downloader.png?raw=true "Screenshot of program")

## Installation:

#### Install prerequistes
You need stack installed, along with the qt quick controls and qt quick controls2.

##### Debian based:
`sudo apt-get install haskell-stack qml-module-qtquick-controls qml-module-qtquick-controls2`

##### Arch based:
`sudo pacman -S stack qt5-quickcontrols qt5-quickcontrols2`

Commands should be similar for other distributions.

#### Clone the repository
`git clone https://github.com/ZedPea/rule34-paheal-downloader.git`

`cd rule34-paheal-downloader`

Alternatively, download the repo as a zip, unzip it, and move into the directory.

#### Compile
`stack install`

##### Windows
Get stack here and install it: https://www.stackage.org/stack/windows-i386-installer

You must download the 32 bit version, 64 bit won't work with hsqml.

Get the qt quick controls here: http://download.qt.io/official_releases/online_installers/qt-unified-windows-x86-online.exe

For the qt setup, skip the account creation, and deselect everything but MinGW under the most recent version of Qt. 
Note the version number.

Finish the install.

Download the repo as a zip, unzip it, and move into the directory, then open a terminal there.

Navigating to the directory in explorer, holding shift, and right clicking
"Open command window here" lets you easily get a terminal in the right spot.

`set PATH=%PATH%;C:\qt\5.9.1\mingw53_32\bin\`

It might not be 5.9.1, depends on what version you installed.

`stack install`

#### Run

Either add ~/.local/bin to your path and run the executable:

`r34Downloader`

Or, run

`stack exec r34Downloader`

This is the only option that will work on windows I believe.
