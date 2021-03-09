# Install Apps with adb on Ubuntu 

Step to add apps or send apps from local server to Laptop and install app to tablet

#### Access to local server 

1. Connect to server local or local LAN like : test

2. Access to the site local like : http://example.cat:8080/

3. Download apps : apps_release.apk

#### Manual configuration

5. Put apps on Download or Desktop directory.
6. Connect your andoid device in to laptop.
7. Open the terminal on ubuntu.
8. Using `adb` to enable USB debugging on your Android Device.

   If not have adb on OS ubuntu you need to install it.

9. Install adb in to OS ubuntu `sudo apt install android-tools-adb android-tools-fastboot`
10. After install adb you can run adb devices in terminal `add devices` to see your list of devices.
11. Install `adb install -r -g ~/Downloads/app-release.apk` 
   ```
   ➜  ~ adb install -r -g ~/Downloads/app-release.apk
   3803 KB/s (1515143 bytes in 0.389s)
   	pkg: /data/local/tmp/app-release.apk
   Success
   ➜  ~
   ```
   Note : If you install get an error like :

   ```
   ~ adb install -r -g ~/Downloads/app-release.apk
   3744 KB/s (1515143 bytes in 0.395s)
   	pkg: /data/local/tmp/app-release.apk
   Failure [INSTALL_FAILED_UPDATE_INCOMPATIBLE]
   ```

   ​

12. Test apps using : `adb logcat | grep -i eskola `

```
➜  ~ adb logcat | grep -i eskola                  
08-03 13:04:40.602  8756  8756 I eskola-notify: Start fetch job
08-03 13:04:40.612  8756 10506 E eskola-notify: Could not connect/fetch POLL_URL: https://education-staging.catalpa.build/mattermost_messagecount/351823080178288
08-03 13:04:50.632  8756  8756 I eskola-notify: Start fetch job
08-03 13:04:50.642  8756 10660 E eskola-notify: Could not connect/fetch POLL_URL: https://education-staging.catalpa.build/mattermost_messagecount/351823080178288
08-03 13:05:00.662  8756  8756 I eskola-notify: Start fetch job
08-03 13:05:00.662  8756  8804 E eskola-notify: Could not connect/fetch POLL_URL: https://education-staging.catalpa.build/mattermost_messagecount/351823080178288
08-03 13:05:10.672  8756  8756 I eskola-notify: Start fetch job
08-03 13:05:10.672  8756  8884 E eskola-notify: Could not connect/fetch POLL_URL: https://education-staging.catalpa.build/mattermost_messagecount/351823080178288
08-03 13:05:20.692  8756  8756 I eskola-notify: Start fetch job
08-03 13:05:20.692  8756  8987 E eskola-notify: Could not connect/fetch POLL_URL: https://education-staging.catalpa.build/mattermost_messagecount/351823080178288
```

