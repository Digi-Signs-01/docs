---
title: 'Using Ftp Clients'
slug: using-ftp-clients
publish: false
date: 2025-05-03
update: 2025-05-03
description: Using Ftp Clients
categories:
  - start
---

# Using FTP clients

FTP clients, softwares for file transfer, have several advantages such as continuing an upload from where it stopped when the internet connection was interrupted.

Most softwares in addition allow to queue items for uploading and to schedule transfers. In this tutorial you will learn how to use the FileZilla FTP client. Make sure you have [enabled FTP on your Digisigns account](02_enabling-ftp-service.md) beforehand.

1. Download and install [FileZilla](https://filezilla-project.org/download.php?type=client) and connect to the Digisigns server. If you are in doubt how to install FileZilla, refer to the [FileZilla installation guide](https://wiki.filezilla-project.org/Client_Installation).
2. When finished with the installation, open the program.
3. Copy your FTP credentials from Digisigns to FileZilla and then click on “Quickconnect”.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731581934561/using-ftp-clients_1.jpg)  
   All credentials you need are provided by the “FTP Info” on the expandable menu on the right on your Digisigns Content page.  
   ![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731581960160/using-ftp-clients_2.jpg)
4. Wait for the software to connect to the Digisigns server. You can check the status in the FileZilla window right under your credentials information.
5. When the process is completed, your Digisigns files will appear in the box on the right (see image below). Browse through your computer files in the box on the left. Upload files by dragging items from your computer to your Digisigns folders. You can also download items by dragging them from Digisigns to your computer.

The upload progress is displayed in the lower bar.

![](https://static.helpjuice.com/helpjuice_production/uploads/upload/image/23821/direct/1731581988921/using-ftp-clients_3.jpg)

Remember that **FileZilla won't prevent you from uploading unsupported file types to Digisigns account**. Although you won't be able to visualize incompatible files on your Digisigns Content tab on the browser, these files will occupy your cloud storage space. We reinforce you should always make sure to upload only supported files through the FTP client.
