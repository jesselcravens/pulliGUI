# pulliGUI

This is an application that I created to manage multiple linux servers at once with basic operations. This can push files, pull files, open a web browser to the server IP address, or 
even execute a BASH script file and save the stdout. 

## Build Instuctions

I like to make a sigle executable so that it can be used anywhere without an installer. I use Pyinstaller with a similar command:

```
pyinstaller --windowed  --add-data "pulley.ico;." --name PulliGUI --onefile app.py
```
