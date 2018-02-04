# Installing discord.py
Since doing `pip install discord.py` in command line doesn't work, we're gonna try to install the package manually.  
It will require some kind of file unzipping tol, and a little use of command line.  
Firstly, download this .tar.gz file. Remember where it goes!  

[discord.py async version](https://github.com/Rapptz/discord.py/archive/async.zip)

- If you don't have 7-zip installed, get that. It's pretty much the standard file compression tool. If you ever deal with .zip files ever, you're probably gonna want to use this.  
To get it, go to http://www.7-zip.org/  
- Near the top of that page will be two download links. Get the one that matches with the bit-version your operating system is using.  
- If you don't know what bit-version you've got, go to  
`Control Panel > System and Security > System`  
and in this screen you should find a number right about here, at the red arrow:  
![pictho](https://i.imgur.com/FgtnY8R.png)
- Install that version of 7zip

- K so 7zip is installed and you can properly open .zip files now.  
- So that file you downloaded a bit ago? the `discord.py-0.16.12.tar.gz` file? Go to wherever that is stored. Probably in `C:\Users\You\Downloads`
- Double-click that `discord.py-blahblahblah` file and open with 7zip, or right click and do `Open with` and choose 7zip.
- Looking at the inside of that .zip file you should see a folder called `dist`.
- Inside of `dist` there will be another thing called `discord.py-0.16.12.tar`. Go inside that with double click.
- Inside of that will finally be a folder simply called `discord.py-0.16.12`, with no file extension at the end of it.
  - Inside this folder you will find a bunch of different files and folders. It should look something like this:  
  ![picture](https://i.imgur.com/zXcMW6R.png)
- Now, looking at the folder for `discord.py-0.16.12`, either drag it somewhere easily accessible like Desktop, or click it and hit the Extract button up top, and put it somewhere easily accessible.  
![picture](https://i.imgur.com/934jP9f.png)
   
- Now that that `discord.py-0.16.12` folder is out on its own somewhere, do Windows key + R, `cmd` to open up the command prompt
- Right now it should say something like, you're in `> C:\Users\Owner` or something. This is called the working directory. It's the folder that the command prompt is currently looking in to execute any commands you give it.
- We want to change the working directory from `C:\Users\Owner` to the folder we should brought out of the zip file. We can do this with the `cd` command.
- In the command prompt, if you do `cd Desktop`, it will change the directory to `C:\Users\Owner\Desktop`.
- In the command prompt, if you want to change your working directory to one that's somewhere within your current working direcotry, you can do it in steps.
  - Say you're in `C:\Users\Owner` and you want to go to your desktop. `cd Desktop` would bring you there, if its a folder within `C:\Users\Owner`.
  - But that was a mistake, you actually want to go to `C:\Users\Owner\Downloads`. You don't want to shut down the command prompt and start from scratch, but you cant do `cd Downloads` because Downloads isn't a folder inside of Desktop.  
  You instead can do `cd ..` and it will bring you to the parent folder of the current directory, so `cd ..` in this case would get you back to `C:\Users\Owner`.
- You could also give it the full path, rather than relative to the current directory path. For example, if you were in `C:\Users\Owner\Desktop`, and you wanted to get to `C:\Users\Owner\Downloads`, one possible way of doing that is to simply do `cd C:\Users\Owner\Downloads`.
- However you want to get to it, do what you have to do to change the current working directory to wherever that new `discord.py-0.16.12` folder is. If you plopped it onto your desktop, doing `cd C:\Users\Owner\Desktop\discord.py-0.16.12` should work.
  
- Your command line input line thinger should look like this now: `C:\Users\Owner\Desktop(if you put it here)\discord.py-0.16.12 >` and it will be waiting for your next command.
- Do `python setup.py install`
- That should hopefully work maybe.
![picture](https://i.imgur.com/HRYBb3S.png)
