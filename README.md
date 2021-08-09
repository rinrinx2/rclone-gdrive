# Overview

Batch script to upload files/folders to Google Drive with logging and filtering enabled (both optional)

## Usage

If you want to use the default paths then create a folder called Scripts\Rclone on the OS root drive (C:) and extract the zip folder there (e.g C:\Scripts\Rclone). Otherwise you can extract it anywhere and change the variables inside the ***rclone-gdrive.bat*** file.

It's strongly recommended that you use your own client_id and client_secret to avoid potential issues with Google Drive. See the link below to learn more:

[Making your own client-id](https://rclone.org/drive/#making-your-own-client-id)

## Logging

Logging is enabled by default and everytime the script is run it'll create a .log file inside the ***logs*** folder with the date/time it was run. If you don't want this just comment out the ***RCLONE_LOG*** variable inside the ***rclone-gdrive.bat*** file

## Filtering

By default rclone will copy everything on the [source] folder, even hidden files. You can use filters to include (+) or exclude (-) files/folders, this is done on the filters.txt file. If you want to learn more about filtering and how to use then with advanced use cases, see the link below:

[Rclone filtering](https://rclone.org/filtering/)
