# nexus-raw-uploader

Overview
--------
Simple bash script to upload local files or folders to a Nexus RAW Repository:
   ```
   #################################
   # Nexus RAW Repository Uploader #
   #################################
   
   Usage:
     nexus-raw-uploader [Options] <Args>
   
   Required options:
     -u <username>     Username of the nexus repository manager server
     -l <local path>   The local path to upload (can be a file or folder, must start with '/')
     -r <repo name>    Name of the repository to upload the files
     -n <nexus url>    URL of the nexus repository manager server
   
   Not required options:
     -p <password>     Password of the nexus repository manager server (will be asked if not present)
     -t <target path>  The target path to upload to (default is empty, must start with '/')
     -h                Show this help text
   
   Examples:
     nexus-raw-uploader -u 'my-username' -l '/my/local/file/path' -r my-repo-name -n http://my-nexus-url
     nexus-raw-uploader -u 'my-username' -l '/my/local/file/path' -t '/my/target/folder/path' -r my-repo-name -n http://my-nexus-url
     nexus-raw-uploader -u 'my-username' -l '/my/local/folder/path' -r my-repo-name -n http://my-nexus-url
     nexus-raw-uploader -u 'my-username' -l '/my/local/folder/path' -t '/my/target/folder/path' -r my-repo-name -n http://my-nexus-url
   ```

Prerequisites
-------------
* [CURL](https://curl.haxx.se/) must be installed

Installation
------------
* Download nexus-raw-uploader script to `/usr/local/bin` folder:

   ```
   sudo wget https://raw.githubusercontent.com/chrisipa/nexus-raw-uploader/master/nexus-raw-uploader -O /usr/local/bin/nexus-raw-uploader
   ```
   
* Make nexus-raw-uploader script executable:   

   ```
   sudo chmod +x /usr/local/bin/nexus-raw-uploader
   ```
