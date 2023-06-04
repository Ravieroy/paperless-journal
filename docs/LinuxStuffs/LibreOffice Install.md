# LibreOffice Install

[Source](https://libre-software.net/how-to-install-libreoffice-on-ubuntu-linux-mint/#a_install_libreoffice)

First remove the older versions following the [[LibreOffice Remove]] steps 

# Install LibreOffice Manually 

## Step 1:  **Download compressed packages**
Download LibreOffice 7.x from the official [website](https://www.libreoffice.org/).

By default this should download in **Downloads** directory and this tutorial assumes that the downloaded file is in the **Downloads** directory.  

## Step 2: **Extract the .deb packages** 
Learn more about [[Extraction]] to understand the filetype.

The downloaded files are compressed and have a .tar.gz filename extension. To extract these archives, open the "Downloads" directory and look for file named:

>LibreOffice_7.x.x_Linux_x86_deb.tar.gz or
>LibreOffice_7.x.x_Linux_x86-64_deb.tar.gz

Right-click on the file name and select “extract here “. Repeat the extraction process for language packs (if you have downloaded them as well). The .tar.gz archive(s) can now be deleted.

## Step 3: **Install .deb packages**
Open [[Terminal]] and change the directory to the location of the .deb packages. 

For 64 bits version:
`cd ~/Downloads/LibreOffice_7.x.x_Linux_x86-64_deb/DEBS`

Install all the .deb packages:
`sudo dpkg -i *.deb`

In case you’re installing language packs, repeat the cd and dpkg steps for each language pack. 

**Done!** No need to restart, LibreOffice is ready to be used.

## Some Tips!
- If you have problems launching LibreOffice, try out the following command:
`libreoffice7.3`
or
``/opt/libreoffice7.3/program/soffice`

---




