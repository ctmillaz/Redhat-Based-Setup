# Redhat-Based-Setup

# Setup Linux Operating System
### Create and open sudo user file
```nano /etc/sudoers.d/<user>```
### Add this to sudoer.d file
```<user> ALL=(ALL) NOPASSWD: ALL```

### Install almalinux os, vmware, and extra updates
```sudo dnf install open-vm-tools open-vm-tools-desktop```

### Verify you have added Virtualbox Guest Additions or VirtualBox Guest Addons

### Install Dash to Panel from Store
### Install Gnome Tweaks and Dash to Dock
```sudo dnf upgrade```

```sudo dnf update```

```sudo dnf install epel-release```


### Install/Update kernel headers
```sudo dnf install gcc make perl kernel-devel kernel-headers bzip2 dkms```
```sudo dnf update kernel-*```

# Install git 
```sudo yum install git -y```
### Make git directory
``` mkdir /home/$USER/git```

# Instal Chrome
```yum install -y google-chrome-stable.x86_64```

# Install Virtual Stuiod Code
```sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc```

```sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'```

```dnf check-update```

```sudo yum install code```

# Install python 
### Install python38 or current version of python
```sudo yum install python3.8```
### Update python3 version to reflect the version of python you want to use
```sudo update-alternatives --config python3```
### Updated pip or install
```pip install --upgrade pip```

```curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py```

### Get pip3
```python3.8 get-pip.py```

## Reboot after updates and installations are complete for them to take affect
```sudo reboot```