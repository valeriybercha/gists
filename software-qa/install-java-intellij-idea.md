# Install and setup Intellij Idea for Windows

Pre-requisites:
- Java JDK should be already [installed on your computer](https://gist.github.com/valeriybercha/5ba0e91c83bf1d1143527d7f29dec30d)

Steps to perform:
1. Download and install the 'Community' (free) version of Intellij Idea from the official website - 
[https://www.jetbrains.com/idea/download/#section=windows](https://www.jetbrains.com/idea/download/#section=windows)
2. Open the Intellij Idea application.
3. Click on 'New Project' link to create a new project.
4. In the opened window, be sure to check 'Java' as project in the left side of the window. Also be sure that in 'Project SDK' field Java version is selected. Click on 'Next'.
5. Next click on 'Create project from template' checkbox and click 'Next'.
6. In the following window you should complete 'Project name': 'helloWorld' (e.g.); 'Project location': you can leave it by default and 'Base package': yuo can leave it by default. Click on 'Finish'.
7. Project structure is displayed in the left corner. All the files are placed in the 'src' folder. In the main window project code is displayed in
the 'Main' class.
8. Write down the followin code:

```sh
package com.company;

public class Main {

    public static void main(String[] args) {
	// write your code here
        System.out.println("Hello, World! My first program in Java");
    }
}
```

9. Click on 'Run' icon in the upper-right corner of the application. 'Hello, World! My first program in Java' message will be displayed in the result window at the botton of the application.