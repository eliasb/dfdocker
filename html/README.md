**HTML Folder**
===================
This folder was created to be a storage place for the website files in your **Docker Development Environment**

----------

Description
-------------
When your website is created and all the scripts executed, a copy of most of the files **"Drupal"** container will be synchronized with this folder by a **"cron"** job that will be running inside the container. This **"cron"** job will execute every minute. 

> **Note:**
> 
> If you have just made changes to your website, it would be advisable to wait for, at list, 2 minutes before stopping your container. This will give enough time for **"cron"** to synchronize your **"Drupal"** Docker Container HTML files with this backup folder.
