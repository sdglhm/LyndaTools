# LyndaTools
Few bash scripts to help Lynda users to Download and Manage Lynda contents

-
# 1. Lynda downloader
## Lynda course downloader bash

Lynda course downloader is a bash script that I came up with to download lynda courses to my local computer so I could check them on the go. This uses Youtube-dl program which can be downloaded by running following command.

### To download Youtube-dl


To install it right away for all UNIX users (Linux, OS X, etc.), type:

    sudo curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
    sudo chmod a+rx /usr/local/bin/youtube-dl

If you do not have curl, you can alternatively use a recent wget:

    sudo wget https://yt-dl.org/downloads/latest/youtube-dl -O /usr/local/bin/youtube-dl
    sudo chmod a+rx /usr/local/bin/youtube-dl

Also you'd need to have lynx browser installed. 

    yum install lynx -y
    or
    apt-get install lynx
    or
    pacman -S lynx

### To download Lynda course downloader,

1. Download the LyndaDownload script  

	`wget -O lyndaDownload https://raw.githubusercontent.com/sdglhm/LyndaTools/master/LyndaTools-dl`
    
2. Give executing permission  

	`chmod +x lyndaDownload`

3. Run Lynda Dowload script  

	`./lyndaDownload `

---
You will be asked with your lynda password and username. Provide them to continue. Then Copy lynda course page URL and past when asked. It will fetch URL's and start the download automatically. Open your terminal window to finish the download.

### Enjoy !!!
-
# 2.Lynda File Rename

Usually, Lynda files are named with the format `lesson name -fileorder.mp4` but directory listing shows the files in alphabetical order which is kind of annoying. So I've written a small bash script which will rename files by prepending the file order number at the beginning of the file so I could easily click the file or my player can autoplay files at ease.

### How to use Lynda file Rename

1. Download the Lynda File Renamer  

	`wget -O "lyndaRename" https://raw.githubusercontent.com/sdglhm/LyndaTools/master/LyndaTools-Rename`
  
2. Give executing permission  

	`chmod +x lyndaRename`
        
3. Run Lynda Tool renamer with your folder path  

	`./lyndaRename "~/home/Lynda/Course"`
        
Enjoy !!!
