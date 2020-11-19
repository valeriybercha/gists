# Install and setup Charles Web Proxy for Android

Pre-requisites:
- Charles Proxy should be already installed on your computer.

Steps to perform:
1. Open Charles Proxy on the computer.
2. Click on 'Help' and select 'Local IP Adress'. Save the IP address for the network shown in the window
(e.g. ``` 192.168.8.100 ```).
3. Click on 'Proxy' and select 'Proxy Settings'. Be sure that 'HTTP Proxy' port is set to '8888'.
4. Now, we have to connect the mobile device to Charles Proxy. Open the WiFi settings on the smartphone and make sure that you are connected to the same network as your computer.
5. Open 'Advanced options' in the Wifi settings and change proxy setting to manual and fill the following fields: 'Proxy hostname' with the IP address saved earlier (step 2) and 'Proxy port' with ``` 8888 ```.
6. Save the proxy stettings.
7. In a few seconds a new window will appear in Charles proxy on the computer with a request to allow a connection.
Make sure to 'Allow' the connection.
8. Installing Charles Root Certificate. On the Android device using any browser navigate to [http://chls.pro/ssl](http://chls.pro/ssl) or
[http://www.charlesproxy.com/getssl](http://www.charlesproxy.com/getssl).
1. Authenticate and provide anu certificate name (e.g. 'charles').
2.  Make sure 'VPN and apps' is selected and tal 'OK'.
3.  From Charles proxy on the computer click on 'Proxy' and turn off 'Windows Proxy'. Your computer now will not collect ant browser logss, just from your mobile device.
4.  Now you can test wether you can collect browser logs from a mobile device. First, clear all the records made in the Charles proxy before by click-ing on the 'broom icon' and make sure that recording logs are turned on.
5.  On the mobile device, open an application in the browser. Charles proxy should start collecting logs.
6.  When finished, click on 'File' > 'Save session' and save the log into '.chls' format.
