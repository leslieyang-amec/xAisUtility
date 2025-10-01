# AIS Configuration Tool

## macOS

Due to macOS security reasion, there are two steps need to do before execute the application.

### 1. Allow applications from anywhere

(1) Type following command in the terminal to disable Gatekeeper.

```text
sudo spctl --master-disable
```

(2) Change allow applications from anywhere

System Setting > Privacy & Security > Security

Select "Anywhere" from the "Allow applications from" dropdown menu for the option to fully appear and take effect.

![Alt text](./pic/macOS_AllowAppFrom.png)

### 2. Remove quaratine

It needs to remove the quarantine attribute manually from the download file before executing it.
 
(1) Download .dmg.zip
https://github.com/leslieyang-amec/xAisUtility/releases/download/v3.73/AIS_Configuration_Tool_3.73.dmg.zip

(2) Decompress the .zip file.

(3) Double clicks on the .dmg file

(4) Drag out the AIS_Configuration_Tool.app file from the .dmg

(5) Execute follow command

```text
xattr -r -d com.apple.quarantine /the/path/to/the/app/AIS_Configuration_Tool.app
xattr /the/path/to/the/app/AIS_Configuration_Tool.app
```
