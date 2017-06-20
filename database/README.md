**Database Folder**
===================
This folder was created to be a storage place for the database in your **Docker Development Environment**

----------

Description
-------------
When your website is created and all the scripts executed, the database in your **"MySQL"** container will be synchronized with this folder by a **"cron"** job that will be running inside the container. This **"cron"** job will execute every minute. 

> **Note:**
> 
> If you have just made changes to your database, it would be advisable to wait for, at list, a minute in order to allow **"cron"** to synchronize your **"MySQL"** Docker Container database with this backup folder.