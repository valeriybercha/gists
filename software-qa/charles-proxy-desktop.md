# Install and setup Charles Web Debugging Proxy for Windows

Steps to perform:
1. Download and install 'Charles Proxy' from here - [https://www.charlesproxy.com/download/](https://www.charlesproxy.com/download/)
2. Open Charles Proxy.
3. First, we need to install the 'Charles Root Certificate'. Click on 'Help' select 'SSL Proxying' and then click on 'Install Charles Root Certificate'.
4. A certificate window will open, click on the 'Install Certificate' button and then click on 'Next'.
5. Choose 'Place all certificates in the following store' and click on 'Browse'.
6. Select the 'Trusted Root Certification Authorities' folder and click on 'OK'.
7. Click on 'Next' and finally click on 'Finish'.
8. Close Charles software and restart your computer.
9. Open Charles again and click on 'Proxy' and ensure 'Windows Proxy' is enabled.
10. Now, we'll have to setup SSL Proxy settings. Click on 'Proxy' and select 'SSL Proxy Settings', check 'Enable SSL Proxying', and click on the 'Add button' under 'Include'.
11. In the 'Edit Location' popup, type ``` * ``` for 'Host' or leave it empty and type ``` 443 ``` for 'Port'.
12. Click on 'OK' button.

