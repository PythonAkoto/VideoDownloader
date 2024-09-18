# Video Downloader
This is a simple desktop app that allows you to download a YouTube video - so no more annoying adverts!

All you need to do is copy your link in the section provided on the **Download Video** page, then wait until it's downloaded! If it's a big file like an hour or so, then you may have to wait a couple minutes but most videos that are roughly 1 hour or so are downloaded within roughly 30 seconds.

Please be paitent with the downloads, and only press the download button **once**. However, as it will always try to download the highest resolution, if it's a very large video, it will cause the app to time out.

Once the video has been downloaded, you can watch it in the **View Video** page.
Your Videos are stored in the **downloads** directory found in `VideoDownloader/static/downloads` where the videos are played from.

As this is open source, feel free to add some contributions to make it better!


**When making any additional changes you want to add to the community make sure to remove the your perosnal video downloads when making a push request. GitHub will detect that there are large files in the repo and will not let the push request go through.**


## Instalation Guide
This is a Flask app, so I will be going through the step by step process to install and run the app on your desktop.
If you do not have python already installed on your machine you can download it from [here]("https://www.python.org/downloads/"). You can check if you have Python installed on your dektop/laptop by navigating to your command line and enter `python --vesion`, to find out the latest version you have. If it's not installed you will get an error message!


### Virtual Environment
First we need to create our  virtual environment for your laptop/desktop.

#### macOS, Linux, Windows
```
python -m venv venv
```

We now need to install the packages from the `requirements.txt` file, but before we do that we need to activate our virtual environment.

### macOS, Linux
```
source venv/bin/activate
```

### Windows
```
venv\Script\activate
```

### Installing the Libraries
We should have the libraries needed from the `requirements.txt` file, if for whatever reason you don't seem to have it, you can copy the libraries you need from below:
```
blinker==1.7.0
click==8.1.7
colorama==0.4.6
Flask==3.0.0
flaskwebgui==1.0.8
importlib-metadata==6.8.0
itsdangerous==2.1.2
Jinja2==3.1.2
MarkupSafe==2.1.3
psutil==5.9.6
pytube==15.0.0
Werkzeug==3.0.1
zipp==3.17.0
```
As this is an open source app, if you make any additioional changes, update the `requirements.txt` file and also here in the README!  The easiest way to update the `requirements.txt` file is to do the following in the terminal:
```
pip freeze > requirements.txt
``` 

Now we can install these packages by entering the following:
```
pip install -r requirements.txt
```

### Runnung The App
Now we haev what we need to run the app, all we need to do is run the following in the terminal:
```
python main.py
```