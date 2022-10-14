# Chrome_Browser-chrome_remote_Ubuntu_20.04

## Install Google Chrome Browser on Ubuntu 20.04

You can install Google Chrome browser by downloading the Debian binary package or by simply installing the Chrome sources lists and then installing the Chrome browser from these sources lists.

### Update System Package Cache

Before you can proceed, update your package cache.

```
sudo apt update
```

### Install Google Chrome using DEB Binary Package

Download Google Chrome DEB binary package from Google Chrome page.

```
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb -P /tmp
```

Then install it using APT so as to deal with required dependencies automatically.

```
sudo apt install /tmp/google-chrome-stable_current_amd64.deb
```
Run the code below to see the version of chrome installed 
```
google-chrome --version
```

### Sign in Google Account

Before you can begin to setup Chrome Remote Desktop on Ubuntu 20.04 login to your Google account on your browser using your gmail account.

### Install Chrome Remote Desktop Extension

Next, you navigate to Chrome extensions page and search for Chrome remote desktop.

Click Add to Chrome to install the extension.

After the installation, you should be able to see the Chrome remote desktop icon just beside your search address bar on the right.
### Install Chrome Remote Desktop Package

Next, install Chrome remote desktop package which provides the required host components;

```
wget https://dl.google.com/linux/direct/chrome-remote-desktop_current_amd64.deb -P /tmp
sudo apt install /tmp/chrome-remote-desktop_current_amd64.deb

```

You can as well navigate to the download folder, /tmp, in this case, and run the command;

```
cd /tmp
sudo apt install ./chrome-remote-desktop_current_amd64.deb
```

Enable Remote Desktop Connections

To allow remote access to your Ubuntu 20.04 via Chrome remote desktop tool, you need to enable this by opening the Chrome remote desktop extension or just using the remote desktop access address, https://remotedesktop.google.com/access and clicking TURN ON as shown in the screenshot below;


If you do not see the TURN ON button, simply create the Chrome remote desktop configuration directory on your home directory;

```
mkdir ~/.config/chrome-remote-desktop
```
Once you create the directory, reload the access URL above.

Next, enter the name of your system;
Click Next to set the remote connection PIN. Ensure that the PIN is at least 6 digits.
Once you set the PIN, click START to run Chrome Remote Desktop.

If prompted for authentication to run Chrome remote desktop, authenticate and proceed.
Chrome Remote Desktop is now up and running on your Ubuntu 20.04.
