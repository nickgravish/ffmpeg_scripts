# FFMPEG scripts for easy use and batch converting

## Installation

Download the windows or mac specific binary from here, or check out www.ffmpeg.com for updates. Note these are the versions for 64 bit operating systems. 

### PC install

Download the zip file, unzip to it's own folder C:\ffmpeg\

The file path should then be 

```
C:\ffmpeg\
	|->bin
	|->doc
	|->licenses
	|->presets
	|->README.txt
	|->ff-prompt.bat
```

We need to now add ffmpeg to the system path. There are two paths. 

1 From the command line type 
```
setx path "%path%;C:\Program Files (x86)\Git\bin\"
```

2 Through the start menu, right click on my computer. Go to the advanced settings tab and click on environment variables button in bottom right hand cornere. There is a PATH variable in the top variable list. Click to edit, then add a semicolon spacer and the ffmpeg path. You can copy and past the following to the end of the path and then close the quotation mark at the end. 
```
;C:\ffmpeg\bin
```

Once ffmpeg is installed you can access it from the command line. Try typing ffmpeg at the command prompt. 

### Mac install

Download the mac binary and unzip to it's own folder in your user folder. 

```
~/ffmpeg/
	|->bin
	|->doc
	|->licenses
	|->presets
	|->README.txt
	|->ff-prompt.bat
```

Add to your path by opening your bash_profile in the mac terminal

```
pico ~/.bash_profile
```

and update the path variable by one of two ways, 1) adding the folder directly to the path, or 2) just add the following code to the end of the bash_profile 

```
export PATH="~/ffmpeg/bin/:~/ffmpeg/:$PATH"
```










