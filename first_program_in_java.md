# Create the first 'Hello, World' program in Java

### Pre-requisites:
- Java should be already installed on your machine. To verify if 'Java JDK' is installed on your computer, simply run the ``` $ java -version ``` command
in 'Command Prompt (cmd)' (for Windows users). The installed Java version and build should be displayed. If not make sure to [install 
'Java Development Kit' first](https://gist.github.com/valeriybercha/5ba0e91c83bf1d1143527d7f29dec30d).

### Creating a 'Hello, World' program in Java

1. Create a project folder on your computer - ``` C:\Java ```.
2. Open the text editor (e.g. 'Notepad++') and create a new file.
3. Type in the file the following code:

```sh
public class helloWorld { 
      
    public static void main (String args[]){
          
        System.out.println("Hello, World! My first program in Java");
    }
}
```

4. Save the file as 'helloWorld.java' ('.java' is the extension for Java files) and save it in the previously created project directory (``` C:\Java ```).
5. Open the 'Command Prompt (cmd)' and type the following command ```$ cd C:\Java ``` to navigate to the project directory where the 'helloWorld.java' was created.
1. Now we'll have to compile the code first. In terminal type the following command - ``` $ "C:\Program Files\Java\jdk-15.0.1\bin\javac" helloWorld.java ```.
Press 'Enter'. If no error appeared the Java code is compiled correctly. Note that the path for the 'javac' compilator should be placed in 
quotation marks ("") if 'JAVA_HOME' variable is [not set in the 'Environment Variables'](https://gist.github.com/valeriybercha/5ba0e91c83bf1d1143527d7f29dec30d). If 'JAVA_HOME' is set, simply type ``` $ javac helloWorld.java ``` command. The result will be the same.
7. Run the program with the command ``` $ "C:\Program Files\Java\jdk-15.0.1\bin\java" helloWorld ```. The message ``` "Hello, World! My first program in Java" ``` should be displayed. Note again that the pass for java execution file should be placed in quotation markas ("") and the file name can be specified without '.java' extension.