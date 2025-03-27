# An-Introduction-to-DataGrip
**Important Tip:** Before opening any links (blue text), we highly recommend right-clicking on them and selecting **"Open link in new tab"** to ensure the guide remains open.

# DataGrip Installation Guide 🛢️
### What is PostgreSQL?
DataGrip is a powerful database IDE developed by JetBrains, designed for database developers and administrators. It supports multiple database management systems

## ✨ STEP 1 - Download 💾
- The first step is to go to the following link [JetBrains DataGrip](https://www.jetbrains.com/datagrip/) , which will redirect you to JetBrains' official website, where you can download DataGrip. Accept the cookies and proceed with the download
- Next, choose the appropriate download option based on your operating system (Windows, macOS, or Linux) and click "Download."
- ![image](https://github.com/user-attachments/assets/8ccdd232-e62e-48c6-ad6c-1291656ae0d2)

## ⚙️STEP 2 - Installation 🛠️ 
- After opening the downloaded file, the setup menu will appear. Click "Next", and when the Install Location screen appears, simply click "Next" again to proceed with the default folder.
- In the Installation Options screen, check the recommended options if preferred, although you can proceed without selecting any.
- ![image](https://github.com/user-attachments/assets/7d43d689-0acb-457b-89cf-a7afb8e0d1b1)
- In the Start Menu Folder screen, no changes are needed, so simply click "Install" to proceed.
- And that's it! 😊 Check the "Run DataGrip" option and click "Finish" to complete the installation.

## 🔐 STEP 3 - Activation 🛡️
- Once installed, a User Agreement window will appear. Simply click "Confirm and Continue" to proceed.
- Regarding Data Sharing, it is entirely up to you—it is not required.
- Now, the application will launch. Click on "Activate License", then go to the "Subscription" tab, where you will find the option to log in to JetBrains. Click on it to proceed.
- This will redirect you to Google or your default web browser. Important: Click on "Log in with Google" and use the account associated with your purchased license. Once logged in, you're all set! Just return to the app/IDE.
- Back in the app/IDE, click "Activate", and you're all set! Now, we can move on to the next part of the guide.

# PostgreSQL Installation Guide  🐘
### What is PostgreSQL?
PostgreSQL is a powerful, open-source relational database management system known for its reliability, extensibility, and compliance with SQL standards.

## STEP 1 - Download 💾
- The first step is to go to the following link [PostgreSQL](https://www.postgresql.org/download/). Once there, click on the option that matches your operating system.
-![image](https://github.com/user-attachments/assets/286141b0-d464-4708-bfd5-b5b38c896ab3)
- Next, click on "Download the installer." If you're unsure where it is, refer to the arrow in the following image.
- ![image](https://github.com/user-attachments/assets/46f27a71-c9c1-43b6-9e53-0d7b46fd264d)
- Then, click on the version 17.4 that matches your operating system, whether it's Windows or macOS.
- ![image](https://github.com/user-attachments/assets/86921748-0eb9-4b4e-aaa7-f7cb8ab60605)
- Next, the file will start downloading. Once it's finished, open it. Note: Registration on EDB is not required.

## ⚙️STEP 2 - Installation 🛠️ 
- Now, a setup window will appear. Click "Next." This setup process is a bit more complex than the previous one, so pay close attention.
- In the Installation Directory screen, simply click "Next."
- In the Select Components screen, only PostgreSQL Server and Command Line Tools are needed—select these and proceed.
- ![image](https://github.com/user-attachments/assets/85bf3d7b-af5e-4f57-bcb7-f1422ea555d6)
- In the Data Directory screen, click "Next."
- Now, in the Password section—this part is **very important**. Enter a password that **you will remember**, as we will need it frequently to access the database. If you're unsure, **write it down somewhere safe** or use another method to store it securely.
- In the Port section, leave it as 5432 and click "Next" to proceed.
- In the Advanced Options section, leave everything as it is and click "Next," just like in the Pre-Installation Summary screen.
- Once the installation is complete, click "Finish," and that's it! 😊

# DataGrip Custom 🎨 (OPTIONAL)
### Description
This is a small optional section of the guide that you can skip. It focuses on customization to make your experience with DataGrip more pleasant and user-friendly.

## Customize
- Theme: If you're like me and find bright screens a bit overwhelming, you can switch to Dark Mode, which is especially helpful for reducing eye strain at night.
- IDE Font: If you need larger text for better visibility when working with data or writing code, you can adjust the font size here.
- Region: You can set the region to Americas in the Region option, though this isn’t crucial. Keep in mind that changing this setting requires a restart.

## Plugins
To search for plugins, go to the search bar and type the names of the plugins you want to find.

- A must-have plugin is Atom Material Icons, which replaces file icons with their relevant logos, making navigation more intuitive.
- If you want more theme options, I highly recommend Material Theme UI, which offers a variety of stylish and customizable themes.

# First Steps in DataGrip 🎯
### Description
Now, we will proceed with setting up the databases on your computer, allowing you to visualize data, analyze it, and even generate charts. The chart generation part will be covered later in the guide.

## STEP 1 - Data BASE 🛢️
- We open DataGrip again and click on "Create New Project."
- We will name it "UNM - Database."
- Click on "Create Data Source", which is located on the left side.
- ![image](https://github.com/user-attachments/assets/8b41beec-b413-42dd-9745-9d2fa5d5aeb8)
- Then, select PostgreSQL, which is among the last options.
- A new window will open, and the first thing you need to do is click on "Download missing drivers", which is indicated at the bottom.
- Next, go to the User field and enter "postgres".
- In the Password field, enter the password you created earlier.
- And that's it! Now, click on "Test Connection" to verify that everything is working correctly. If you encounter an error, double-check the previous steps. If the issue persists, feel free to contact me for help. 😊
- ![image](https://github.com/user-attachments/assets/8d6468c3-924c-425f-8039-7062637d5190)
- Click "OK", and you're all set! 🎉

## STEP 2 - Tables 📊
- Now, double-click to open @localhost → postgres → public.
- Right-click on public, select New, and then click on Query Console.
- Now, we will create the IR Test table. We have separated it into two: R1 for Run 1 and R2 for Run 2.
- Now, copy and paste this code into the opened query console.
```sql
CREATE TABLE ir_test_r1 (
    ratio NUMERIC(20) ,
    funamental INTEGER,
    harmonic INTEGER,
    wave_leght VARCHAR NOT NULL,
    boxid VARCHAR NOT NULL,
    location VARCHAR NOT NULL,
    time_stamp VARCHAR NOT NULL,
    counter_id VARCHAR NOT NULL,
    es_ver VARCHAR NOT NULL,
    dp_ver VARCHAR NOT NULL,
    database_match VARCHAR NOT NULL,
    test_id INTEGER NOT NULL

);
```
- CONTINUE
