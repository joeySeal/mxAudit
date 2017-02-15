# mxAudit
This tool retrieves all information from the mobotix camera info page and adds it to a csv file. Here is a screenshot of some sample output https://raw.githubusercontent.com/joeySeal/mxAudit/master/SampleOUTPUT.png

Prerequisites
Python 3.X (https://www.python.org/downloads/)

 

1. Create a csv file named in the same folder as main.py called input.csv with header rows for ip,login,password each row should contain the cameras ip or hostname followed by :portNumber, user name, and password. If public access is enabled than leave username and password blank. If public access is disabled any user account that can load http://000.000.000.000/control/camerainfo will work.

In this example the first camera has public access disabled and the second has it enabled

ip,login,password
000.000.000.001:80,admin,password
000.000.000.002:80,


2. Navigate to the location where main.py is stored and execute main.py if everything is correct the script will generate the file output.csv

