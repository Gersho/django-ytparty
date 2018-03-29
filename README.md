# django-ytparty
Karaoke manager over local network


##########
Installation
##########

You need the following environment variables:

Create a file named environment in this folder with the following


os.environ['YTPARTY_SECRET_KEY'] =
os.environ['YTPARTY_DEBUG'] =
os.environ['YTPARTY_API_KEY'] =

Either create a file named environment in this folder with the following information (it will be picked up by the installer script) or set them as you please


#####
To use display page you need an addon to ignore xframe cross domain block:

firefox 57+:
https://addons.mozilla.org/en-US/firefox/addon/ignore-x-frame-options-ff-57/


#####

At least one entry must be present in the song catalog to avoid issues

Duration format of the song is ISO 8601 duration used by Youtube.


#####

The database (db.sqlite3) should be in /ytparty (same folder as manage.py)
You need to create a superuser

##########
Usage
##########

The users on local network can visit the / page to choose their song

/manager allows handle Karaoke options (playlist, closing commands, delete songs,...)
Manager accounts must be added in /admin control panel
