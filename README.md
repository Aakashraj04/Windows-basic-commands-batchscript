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
![326793946-35388694-4606-485b-aca8-7849ef2b85fb](https://github.com/shalini170/Windows-basic-commands-batchscript/assets/151901983/0a4adfb3-2c0a-4f82-9298-df45661ea0ef)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![326794148-403ca7e2-1f8a-4e9f-90d8-49922a9dd02d](https://github.com/shalini170/Windows-basic-commands-batchscript/assets/151901983/e31f7c32-b0bb-41e5-8639-77202b56440d)
![326794263-177cd8b1-12e7-4da9-8b3e-a723da8b11e8](https://github.com/shalini170/Windows-basic-commands-batchscript/assets/151901983/d6b92099-208b-47bf-88e5-b15aa6d9a425)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![326794512-46827070-bb8e-4634-83cd-2df4302bc882](https://github.com/shalini170/Windows-basic-commands-batchscript/assets/151901983/5d127d37-e6ab-4561-b1cb-8f548605e629)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![326794716-4549db1f-7cdb-453f-9b48-49b51e781679](https://github.com/shalini170/Windows-basic-commands-batchscript/assets/151901983/e77a2f5d-6b65-492c-9858-b6bebc1da774)
![326794763-0e0a9956-d0c9-46ba-9fa7-ef43080a0697](https://github.com/shalini170/Windows-basic-commands-batchscript/assets/151901983/5e231514-722b-4c5a-b7bc-75f4be2b309c)


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![326794982-7419ffc4-3f49-4738-91b7-f32ecaa48433](https://github.com/shalini170/Windows-basic-commands-batchscript/assets/151901983/b14dedd2-a88c-4769-a233-ea575e2d52d0)

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
![326795147-983c3d33-e17d-413d-ae1e-57583aa33a2e](https://github.com/shalini170/Windows-basic-commands-batchscript/assets/151901983/da19c76e-6d4b-461b-828a-bebf54d1d14e)





# RESULT:
The commands/batch files are executed successfully.

