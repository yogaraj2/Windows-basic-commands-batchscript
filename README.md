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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
mkdir %userprofile%\Desktop\MyLab

![328464022-bae51f75-f6cf-48cf-b0e6-fbb3b6bdfa39](https://github.com/yogaraj2/Windows-basic-commands-batchscript/assets/153482637/eb1f92ea-4f6b-4957-9f04-5636932a15a0)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.

cd %userprofile%\Desktop\MyLab
![328464402-3fda6e27-edc8-4f39-a96c-5e49ee9103f5](https://github.com/yogaraj2/Windows-basic-commands-batchscript/assets/153482637/d8343d40-6ac1-4db0-8a20-7aa360e1091a)
![328464433-ee8aaf6a-bbaa-494f-b30c-1490967b620d](https://github.com/yogaraj2/Windows-basic-commands-batchscript/assets/153482637/89a87cbc-939d-49ef-850e-b2d8afdbea45)


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
dir %userprofile%\Desktop\MyLab

![328464543-de4c5ce3-8d4b-4b95-bef5-667a1dd3f35e](https://github.com/yogaraj2/Windows-basic-commands-batchscript/assets/153482637/b79aff82-0e3c-4439-b269-7e2dcb5adf03)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.

mkdir %userprofile%\Desktop\Backup copy MyFile.txt %userprofile%\Desktop\Backup

![328464612-4386bf12-e3e7-49f5-a345-0456eefe6d83](https://github.com/yogaraj2/Windows-basic-commands-batchscript/assets/153482637/edf5943b-b5a7-4c25-97c4-2e48e646a6ef)

## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents

![328464696-256237bb-c5f7-40ec-a572-34a301827cff](https://github.com/yogaraj2/Windows-basic-commands-batchscript/assets/153482637/04bf23bf-e600-4b55-b4db-160625aa5f41)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.


```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT

![328464870-6e279804-b748-4593-a7b7-a9fbe3b6f227](https://github.com/yogaraj2/Windows-basic-commands-batchscript/assets/153482637/7aa20be9-12d5-45a7-9716-5dded0ecefab)




# RESULT:
The commands/batch files are executed successfully.

