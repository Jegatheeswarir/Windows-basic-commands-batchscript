# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 
# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Jegatheeswarir/Windows-basic-commands-batchscript/assets/144871077/e954f052-0218-49a0-bd2c-bfe8c26d4e9f)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/Jegatheeswarir/Windows-basic-commands-batchscript/assets/144871077/519cd8e5-3ef8-44f3-8981-c57ae28926ec)


![image](https://github.com/Jegatheeswarir/Windows-basic-commands-batchscript/assets/144871077/6f36ffa3-3caa-464e-904e-ea1fb503c71f)




## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Jegatheeswarir/Windows-basic-commands-batchscript/assets/144871077/6b8e3db2-fa41-4e49-bd0b-69a05fad650b)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.

```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/Jegatheeswarir/Windows-basic-commands-batchscript/assets/144871077/3ca37b65-c310-4acb-a098-33a0afa1113a)

![image](https://github.com/Jegatheeswarir/Windows-basic-commands-batchscript/assets/144871077/d913439e-055c-4bf3-8e90-984d222ba640)

## COMMAND AND OUTPUT

```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/Jegatheeswarir/Windows-basic-commands-batchscript/assets/144871077/934f226e-70ea-420b-ab23-c5e031194d18)








## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```






## OUTPUT

![image](https://github.com/Jegatheeswarir/Windows-basic-commands-batchscript/assets/144871077/19d3cb68-f3e2-4f6c-9bfb-271f0fe1b05c)




# RESULT:
The commands/batch files are executed successfully.

