# Termux-GUI
Install Graphical User Interface in Termux (XFCE)

![screenshot](https://user-images.githubusercontent.com/32305505/74161451-f92a2f80-4c44-11ea-8a84-bd1e9e406b42.png)

This script install xfce environment in Termux

## Installation
1) apt install python3
2) git clone https://github.com/Deadpool2000/Termux-GUI.git
3) cd Termux-GUI
4) python3 gui.py

## Download
VNC Viewer - [Download](https://play.google.com/store/apps/details?id=com.realvnc.viewer.android&hl=en_IN)

## How to start Termux-GUI

1) Run 'vncserver' command
2) Add new password for vnc
3) You will get IP Address like this -

   localhost:<session_number>
   e.g. localhost:1
   
3) After above step,type following command -

    DISPLAY=:1 startxfce4 &

Here,1 is a session number.
4) Install VNC Viewer on your phone
5) Add IP Address which you got at Step 3
    e.g. localhost:1
6) Add name
7) Click on Connect
8) Enter VNC password which you used at Step 2


**Important Note - If you want to exit from GUI,type following command before exit -
                    -> vncserver -kill :<session_number>
                    e.g. vncserver -kill :1
