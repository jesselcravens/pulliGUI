# pulliGUI

This is an application that I created to manage multiple linux servers at once with basic operations. This can push files, pull files, open a web browser to the server IP address, or 
even execute a BASH script file and save the stdout. 

#### Build Instructions

I like to make a sigle executable so that it can be used anywhere without an installer. I use Pyinstaller with a similar command:

```
pyinstaller --windowed  --add-data "pulley.ico;." --name PulliGUI --onefile app.py
```
#### How to Use the Program

1. Create a server_list.csv with up to 60 lines. Each line should be in the format of <server_name>,<ip_address>
2. Run the exe if precomplied


#### How to Pull files from Servers

1. Set a "Server Username" in the Server Username box 
2. Set a "Server Password" in the Server Password box. 
3. Select which servers to enable. 
3. Set a file name and its location in the "source location for filename to pull" box. 
4. Set a local location for the pulled file in the "Select local Backup Directory for pulled files"
5. Click the "Pull files from Servers" button. 


#### How to Push files to Servers

1. Set a "Server Username" in the Server Username box 
2. Set a "Server Password" in the Server Password box. 
3. Select which servers to enable.
3. Select a file to push using the "Select File to Push" button with a filedialog prompt.
4. Select a destination on the remote server(s) for the pushed file. 
5. Click the "Push files to Servers" button. 

#### How to Open webpages of Servers

1. Select which servers to enable.
2. Click the "Open Webpage to Servers" button. 

#### How to execute scripts at Servers

1. Push the script file to the servers using this program if needed. 
2. Set a "Server Username" in the Server Username box 
3. Set a "Server Password" in the Server Password box. 
4. Select which servers to enable.
5. Set the filename and its location in the "Remote Script Location to Execute" box.
6. Click the "Execute Script at Servers" button. 

