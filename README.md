# Azuracast Website
A custom website for my azuracast web radio station.

For this website I used a python virtual enviornment on an ubuntu server. 

First navigate to your desired folder and use the following command:

python3 -m venv

Then once the folders and files from this repository are copied the your main website folder, run these commands:

source venv/bin/activate

gunicorn -w 4 -b 0.0.0.0:4592 app:app --daemon

Also be sure the add your mytuner link and  html widgets from your azuracast stream,history, and requests in the index.html file!
