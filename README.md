
# Ex08-Windows-basic-commands-batchscript

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
mkdir %userprofile%\Desktop\MyLab  
![image](https://github.com/ANU23000217/Windows-basic-commands-batchscript/assets/139117108/c3084642-a4fd-4837-9f50-b10c80d70f39)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![image](https://github.com/ANU23000217/Windows-basic-commands-batchscript/assets/139117108/3740e6b0-4d44-43fa-b184-a08326467332)

![image](https://github.com/ANU23000217/Windows-basic-commands-batchscript/assets/139117108/78e0f30b-0991-488f-ba7e-60a77574fdcb)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/ANU23000217/Windows-basic-commands-batchscript/assets/139117108/e5ab08df-ece2-45d1-9296-29c75064c262)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup copy MyFile.txt %userprofile%\Desktop\Backup


![image](https://github.com/ANU23000217/Windows-basic-commands-batchscript/assets/139117108/242b52bb-d1d0-4471-8dfc-ccf90284e1ed)


![image](https://github.com/ANU23000217/Windows-basic-commands-batchscript/assets/139117108/3843b0eb-af53-4af0-b69b-14933778a6d7)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents


![image](https://github.com/ANU23000217/Windows-basic-commands-batchscript/assets/139117108/deb9338f-149d-4a97-8fbd-6ed445c223a5)



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




## OUTPUT:
  
![image](https://github.com/ANU23000217/Windows-basic-commands-batchscript/assets/139117108/4d3572d3-8438-46f6-92c6-112b284976de)



# RESULT:
The commands/batch files are executed successfully.

