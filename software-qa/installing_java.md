# Java installation process

Four step tutorial for installing Java on your machine (for Windows OS users)

1) Download the 'Java Development Kit' (Java JDK) - [https://www.oracle.com/java/technologies/javase-downloads.html](https://www.oracle.com/java/technologies/javase-downloads.html) or click on the latest 'Java JDK' version kit - [https://www.oracle.com/java/technologies/javase-jdk15-downloads.html](https://www.oracle.com/java/technologies/javase-jdk15-downloads.html)
2) Download the '.exe' file for the needed OS - JDK ('jdk-15.0.1_windows-x64_bin.exe' for Windows x64 in my case)
3) Open the downloaded '.exe' file and installing 'Java JDK'. By default the kit will be installed in the 'Program Files' directory. The path should look like this ``` C:\Program Files\Java\jdk-15.0.1 ```
4) To verify if Java was successfully installed on your machine run the following command in 'Command Prompt (cmd)': ``` java -version ```. It shoud display the installed version and build for the 'Java Development kit'

### Set the JAVA_HOME Variable

1) Copy to the clipboard the path for the Java JDK installation: ``` C:\Program Files\Java\jdk-15.0.1 ```
2) Right click on 'My computer' -> 'Settings' -> 'Environment Variables'
3) Click on 'Environment Variables' button
4) Under 'System Variables', click 'New'
5) In 'Variable Name' field type: 'JAVA_HOME'
6) In 'Variable Value' paste the path the Java JDK installation: ``` C:\Program Files\Java\jdk-15.0.1 ```