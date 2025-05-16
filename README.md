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
```
mkdir %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-16 233635](https://github.com/user-attachments/assets/3db55ec7-3b8f-4757-918e-3ebb282a7a05)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-16 234102](https://github.com/user-attachments/assets/8cc2a958-1064-40f3-995c-07472e1d867b)
![Screenshot 2025-05-16 234111](https://github.com/user-attachments/assets/1e8d1cb1-8830-494b-b714-6f6a8d505346)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-16 234121](https://github.com/user-attachments/assets/0eebbcfd-041c-456e-8740-1ecf4ac69bb8)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup
mkdir %userprofile%\Desktop\Documents
```
![Screenshot 2025-05-16 234128](https://github.com/user-attachments/assets/f9064f28-7d35-4cbd-a3ab-1f0487ff7491)
![Screenshot 2025-05-16 234137](https://github.com/user-attachments/assets/b48dadd5-db9e-470e-b01a-064a891baad2)

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![Screenshot 2025-05-16 234146](https://github.com/user-attachments/assets/658ba9a1-8869-48a1-add6-7f3ac9159a9b)

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
  echo Backup and deletion completed successfully
```

## OUTPUT

![Screenshot 2025-05-16 234154](https://github.com/user-attachments/assets/09ce03ec-2ad2-49f6-a60e-65cf48387f3e)

![Screenshot 2025-05-16 234205](https://github.com/user-attachments/assets/cdb4dd35-f71e-42bd-82be-b250317dcdf0)




# RESULT:
The commands/batch files are executed successfully.

