# mxSurvey
This tool retrieves all information from the mobotix camera info page and adds it to a csv file 

Prerequisites
Python 3.X (can be downloaded here)

 

	1. Create a csv file named in the same folder as main.py called input.csv with header rows for url,login,password each row should contain the cameras ip or hostname folled by :portNumber, user name, and password. If public access is enabled than leave username and password blank. If public access is disabled any user account that can load http://000.000.000.000/control/camerainfo will work.

In this example the first camera has public access disabled and the second has it enabled

url,login,password
000.000.000.001:80,admin,password
000.000.000.002:80,


	2. Navigate to the location where mxSurvery.py is stored and execute mxSurvery.py if everything is correct the script will generate the file output.csv

