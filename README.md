# Python backdoor V1

<p>This project is a cross-platform (Windows/Linux/android) open source, backdoor and uses reverse http request to make connections between host and slave. It's made using Python 3</p>

# Installation

### Prerequisities
<ul>
<li>Should have python version 3.9.* and above</li>
<li>Contact me on this mail to ask access for this backdoor : <a href="mailto:jayantkhanna3105@gmail.com">jayantkhanna3105@gmail.com</a></li>
<li>Visit this website to get in touch with me through multiple more ways <a href="https://jayantkhanna.herokuapp.com/">jayantkhanna.herokuapp.com</a></li>
</ul>

### Install
```
    git clone "<Git link will be provided after permission is taken>"
```
Then run following commands:

```
    cd backdoor
    pip install pipwin
    pipwin install pyaudio
    pip install -r requirements.txt
```
Software is now installed 

### Usage

Get your local Ip address:

#### For windows
```
ipconfig
```
#### For LINUX
```
ifconfig
```
Copy your ip address and paste them in following files : master.py and slave.pyw <br>

In master.py line 8
```
    host = "your ip"
```

In slave.py line 6 and 33
```
    host = "your ip"
```

Enter slave folder and find slave.pyw file you need to make a exe(windows)/apk(android) to send to remote host via social engineering methods <br>
To convert to exe a module is already provided if you have followed above steps follow these steps
```
    pyinstaller --onefile slave.pyw
```
If you have not installed all modules as told above run following commands:
```
    pip install pyinstaller
    pyinstaller --onefile slave.pyw
```
Make sure you are inside slave folder else you might recieve following error :
```
    102 INFO: UPX is not available.
    script 'path/to/your/download/slave.pyw' not found
```
Make sure master.py is running before remote host tries to connect using slave.pyw 

```
    python master.py
```
If all goes well when remote host double clicks executable file (some name.exe) you should recieve following on your terminal:
```
    python master.py

    waiting for connection
    ('your ip address', <port>) has connected
    command >>
```
# Features
<ul>
<li>Get directory where backdoor is installed</li>
<li>Send, download and remove files and folders from remote system</li>
<li>Always up untill user chooses to end backdoor on remote host</li>
<li>Get OS details</li>
<li>Open remote host's camera remotely</li>
<li>Open remote host's microphone remotely *</li>
<li>Screen share remote host's screen remotely *</li>
<li>Shutdown remote host's computer remotely *</li>
<li>Inbuilt keylogger *</li>
<li>Encrypt/Decrypt files/folder *</li>
</ul>
<p>Features with '*' are not yet present will be added soon</p>

# Plans for future Versions:
<ul>
<li>Even if slave.pyw is run first still master will be able to connect </li>
<li>Work after every restart</li>
<li>Complete control of remote hosts desktop</li>
<li>Migration of task to GUI task on remote host to prevent killing form task manager</li>
<li>Hooking browser with beef</li>
<li>Get saved passwords from remote host</li>
<li>Get remote host Geolocation</li>
<li>Make a web-based GUI for ease of understanding</li>
</ul>

# Disclaimer
<p>This program is for educational purposes only. I take no responsibility or liability for own personal use. You are not allowed to edit this software in any form</p>

# Terms and condition for use
You are not allowed to use or modify this code for any illegal purpose that includes but is not limited to, Modifying code to make Ransomeware, Hacking user for any personal gain, Hacking someone without their knowledge, Targeting an Organization. In case of any such event your information (which is being recorded) will be provided to respected authorities

