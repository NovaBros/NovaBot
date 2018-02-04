# Installing discord.py
Since doing `pip install discord.py` in command line doesn't work, we're gonna try to install the package manually.  
It will require some kind of file unzipping tol, and a little use of command line.  
Firstly, download this .tar.gz file. Remember where it goes!  

[discord.py async version](https://github.com/Rapptz/discord.py/archive/async.zip)

- 
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
- Select that and click `Extract` at the top, and extra that to wherever, shouldn't matter.
- OR
- Simply drag that `dist` folder to somewhere else, Desktop or whatever, still shouldn't matter. Just pay attention to where you send it.
  
- Now that the `dist` folder is out on its own somewhere, do Windows key + R, `cmd` to open up the command prompt
- Right now it should say something like, you're in `> C:\Users\Owner` or something. This is called the working directory. It's the folder that the command prompt is currently looking in to execute any commands you give it.
- We want to change the working directory from `C:\Users\Owner` to the `dist` folder. We can do this with the `cd` command.
- In the command prompt, if you do `cd Desktop`, it will change the directory to `C:\Users\Owner\Desktop`.
- You could also give it the full path, rather than relative to the current directory path. For example, if you were in `C:\Users\Owner\Desktop`, and you wanted to get to `C:\Users\Owner\Downloads`, one possible way of doing that is to simply do `cd C:\Users\Owner\Downloads`.
- However you want to get to it, do what you have to do to change the current working directory to whever that `dist` folder is. If you plopped it onto your desktop, doing `cd C:\Users\Owner\Desktop\dist` should work.

- Your command line input line thinger should look like this now: `C:\Users\Owner\Desktop(if you put it here)\dist >` and it will be waiting for your next command.
- Do `python setup.py install`
- That should hopefully work maybe.
