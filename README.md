# Name : BASKAR  J
# Reg no : 212223040025
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


## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/baskarsaraswathy/Windows-basic-commands-batchscript/assets/144871005/66be83b0-4044-4c7f-b5bf-38f9cfe7bc42)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/baskarsaraswathy/Windows-basic-commands-batchscript/assets/144871005/fccf8364-6dd7-4396-bc5e-f43b42a8ff0a)
![image](https://github.com/baskarsaraswathy/Windows-basic-commands-batchscript/assets/144871005/793e34af-fa69-4b6c-bcce-167bc8d3c9cf)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/baskarsaraswathy/Windows-basic-commands-batchscript/assets/144871005/4b74dc29-befc-416e-8286-04a31b5c1755)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/baskarsaraswathy/Windows-basic-commands-batchscript/assets/144871005/23d8f80d-2497-4cf2-bd1d-f6b7af312b0f)
![image](https://github.com/baskarsaraswathy/Windows-basic-commands-batchscript/assets/144871005/64f3cb6f-8c8c-4168-bb17-f6a5ac8fe9c9)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/baskarsaraswathy/Windows-basic-commands-batchscript/assets/144871005/43d81b74-fabc-41ee-be32-b905f7322310)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```




## OUTPUT

![image](https://github.com/baskarsaraswathy/Windows-basic-commands-batchscript/assets/144871005/3a4f96f3-07b1-4f51-afae-fe6709831448)




# RESULT:
The commands/batch files are executed successfully.

