# backupService
Service for Windows 7-10, which backs up data from the specified directory.
For the service to work, 7-zip must be installed.

# Configurating
To set the service settings, a config.txt file was created that stores information in the following format:
- path to the directory from which the backup is performed;
- the path to the archive file storing the backup copy of the specified directory;
- masks / filenames to be saved in the archive.

# Example of config.txt
C:\Users\user1\dir\
C:\Users\user1\backup_storage\backup.zip
b?c*.txt
*.d???
doc*.exe

# Debug
Debug information is output using the addLogMessage () function to the log.txt file.
The paths to these files, as well as the path to the service and its name, are set explicitly in the program code.