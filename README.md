# How to make a vm( virtual machine)
1.Go to
<br>
["https://aws.amazon.com/resources/create-account"] and follow the instructions.
<br>
<br>
# Starting an EC2 instance
1.On the AWS dashboard, search for EC2 and click EC2.
<BR>
2.Click Launch Instance
<br>
3.Type your server name and choose the OS you desire(we are choosing Ubuntu for this tutorial)
<br>
4.In the "Key Pair" section click on "Create new key pair"
<br>
5.Name your key pair and click on .ppk and then create new key (the key pair will get downloaded)
<br>
6.In the network section click on Allow HTTP traffic from the internet.
<br>
7.Finally click on Launch Instance.
<br>
<br>
# INSTALLING PUTTY
**STEP 1 DOWNLOAD PUTTY** 
<BR>
<BR>
1.Go to https://www.putty.org/
<br>
2.Click the download link"You can download PuTTY here"
<br>
3.In the package files group, click the link for the version that best suits your Windows System:
<br>
4.32-bit putty-0.70-installer.msi
<br>
5.64-bit putty-64bit-0.70-installer.msi
<br>
6.Save the file in your computer.
<br>
7.Run the file after finishing download.
<br>
8.Click Next
<BR>
<BR>
**STEP 2 SET THE INSTALLATION FOLDER**
<BR>
<br>
1.Accept or adjust the installation folder.
<br>
2.Click next
<br>
<br>
**STEP 3 INSTALL PUTTY** 
<BR>
<BR>
1.Click install to proceed.
<br>
<br>
**STEP 4 ACCEPT AUTHORIZATION TO MAKE CHANGES**
<BR>
<BR>
1.A warning message will ask for an authorization for the installation application tomake changes in your computer.
<br>
2.Click YES so the installation can proceed.
<br>
<br>
**STEP 5 INSTALLATION COMPLETED**
<BR>
<BR>
1.After finising installation PuTTY will show you the final screen.
<br>
2.Check the tick box if you want to view the README file...
<br>
3...or keep it unchecked if you don't need to view it.
<br>
4.Click finish to close the dialog window.
<br>
<br>
# Setting up PuTTY and the instance
1.Go to the Instance dashboard, you"ll notice that that the instance is running and below a public IP address is visible,copy it. If you open the IPaddress in your Browser you"ll notice nothing loads because no server is installed on your Instance as of yet.
<br><br>
2.Now Open PuTTY, you'll notice a space titled "Host Name", Paste the IP address you copied.
<br><br>
3.On the left column,click "SSH",then click "Auth",and click on "Credentials"
<br><br>
4.Click "Browse" and select the key pair you downloaded and click "Open"
<br><br>
5.Click accept and in the username type "ubuntu" and press ENTER.
<BR>
<BR>
# Using the command line interface
1.In the command line run the following linux commands in the following order

       sudo su

       apt update
 <br>
 It'll update the dependecies

2.We need to install apache2 HTTP server, for that run the following command

     apt install apache2
<br>
It'll starting install the apache2 server on your VM.
<br>
<br>
3.If you go into your browser and search the IP you got earlier now you'll see this
<br>
<br>
4.Now back on the PuTTY command line, run these commands

      /var/wwww/html/
       rm index.html
       vi index.html
<br><br>
5.Now you'll be in the edit window, Press I
<br><br>
6.Now you can edit the file, for this tutorial let us simply type "hi" using HTML format
<br><br>
7.Next to save the file, FIrst press Ctrl+C ( This will bring you out of the edit mode), then type :wq to exit the window
<br><br>
8. Now on the browser, the "hi" is displayed
<br>
Using this method you can connect it to your github too
# Closing the Running Instance
It is always recommended to close the running instance

1.On the Instances dashboard, right click on the running instance and click on "Terminate Running instance"



 
 
















,






















