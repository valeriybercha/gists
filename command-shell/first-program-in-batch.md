# Hello World program with Batch scripting

1. Create a new file ```hello.bat```
2. Open the file with ```notepad hello.bat```
3. Type the following script in the file:
```sh
@echo off
title First Program 
:: Display Hello World message
set hello=Hello, World!
echo %hello%
pause
```
4. Save the file and open it in CMD
5. Run the file in cmd by typing ```hello.bat```
6. Message 'Hello, World!' should appear on the screen