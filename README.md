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

mkdir %userprofile%\Desktop\MyLab

![325093274-30906be8-14a0-42df-be77-32fd1db31b60](https://github.com/user-attachments/assets/9a2cc7df-d480-435a-8f98-4feea6f2a0e9)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.



## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![325093472-219b74d7-05db-4607-ba11-27751dc8e214](https://github.com/user-attachments/assets/a8d269fb-9806-4780-9fc2-7ea10bac4326)

![325093753-231c6c4e-3340-415c-953c-3d929983c9ef](https://github.com/user-attachments/assets/15d92e5d-5935-4df3-b297-47a74d3afa13)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT

dir %userprofile%\Desktop\MyLab

![325094082-26b5dd3d-0930-4a7b-bbc1-b70d2eab433d](https://github.com/user-attachments/assets/291694b1-57a1-42b7-8925-ef6cecb12f48)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![325095313-4b522d08-477a-4ac2-bdf8-ce34b5377f8a](https://github.com/user-attachments/assets/cf8c1145-a98d-4290-996b-cb6f834dee13)
![325095614-2b3d2723-ef8d-47a6-a7a6-d230fc1e3937](https://github.com/user-attachments/assets/c189166f-5753-4ecd-ae03-77c2b1e71a9a)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![325095890-7a71bbce-a804-472a-96be-308a5862f6ba](https://github.com/user-attachments/assets/46718950-d9be-4ea8-b9e1-3c058c50ebc9)


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
![325099134-3d062ebb-7d20-4c09-95dc-b10861f34223](https://github.com/user-attachments/assets/06bc777d-4b47-461f-b392-a861609ffa7f)





# RESULT:
The commands/batch files are executed successfully.

