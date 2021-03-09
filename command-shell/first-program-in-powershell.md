# Hello World program in PowerShell 

1. Create a new file 'hello.ps1'
2. Open the file with 'notepad hello.ps1'
3. Type the following script in the file:
```sh
$strString = "Hello, World!"
write-host $strString
```
4. Save the file and open it in PowerShell
5. Run the file by typing ```.\hello.ps1```
6. If no error appeared - 'Hello, World!' message should appear on the screen
7. If error message appeared, probably, the ExecutionPolicy is set to Restricted. To check this, type 'Get-ExecutionPolicy' in the PowerShell. Message 'Restricted' should appear.
8. Run the command 'Set-ExecutionPolicy unrestricted' in PowerShell
9. Run the file ```.\hello.ps1``` again
10. Message 'Hello, World!' should appear on the screen