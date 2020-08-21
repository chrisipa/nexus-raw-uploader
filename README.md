# nexus-repository-folder-uploader

Overview
--------
Simple bash script to recursively upload local folders to a Nexus Repository Manager server:
   ```
   ####################################
   # Nexus Repository Folder Uploader #
   ####################################

   Usage:
     nexus-repository-folder-uploader [Options] <Args>
   Required options:
     -u <username>         Username of the nexus repository manager server
     -p <password>         Password of the nexus repository manager server
     -f <folder path>      Path of the local folder to upload
     -n <nexus url>        URL of the nexus repository manager server
     -r <repo name>        Name of the repository to upload the files
     -h                    Show this help text
   Example:
     nexus-repository-folder-uploader -u my-username -p my-password -f /my/folder/path/to/upload -n http://my-nexus-url:8081 -r my-repo-name
   ```

Prerequisites
-------------
* [CURL](https://curl.haxx.se/) must be installed

Installation
------------
* Download nexus-repository-folder-uploader script to `/usr/local/bin` folder:

   ```
   sudo wget https://raw.githubusercontent.com/chrisipa/nexus-repository-folder-uploader/master/nexus-repository-folder-uploader -O /usr/local/bin/nexus-repository-folder-uploader
   ```
   
* Make nexus-repository-folder-uploader script executable:   

   ```
   sudo chmod +x /usr/local/bin/nexus-repository-folder-uploader
   ```
