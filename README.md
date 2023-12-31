# osticket-prereqs

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enable IIS (Information Services )
- Web platform installer
- install MySQL
- Install C++ redistributable
- Config permissions and install OSTicket
<h2>Installation Steps</h2>

![rs group](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/03493dc8-1c2c-426d-8dd0-35d390e39365)

![Screenshot 2024-01-03 162227](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/51fa8f17-35f0-4a7a-93e6-aec302cf90c4)


The first thing we are going to do is go to Portal.Azure.com where we will be creating our resource group and eventually later on in this tutorial create our virtual machine and connect to it using Remote desktop or a Mac Equivalent but i am on pc so we will be using Remote desktop.
</p>
<br />

![Screenshot 2024-01-03 162446](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/69644701-9546-44fd-9634-d36d2e3d4a44)

Here we are creating our virtual machine. We will be placing this virtual machine inside of the resource group that we have created before ( mine is called osTicket but the name doesnt matter). I will be using the virtual pc specs of a 4 core processor and 16 gb of ram today for this tutortial and i will be naming our virtual machine VM-osticket . Then we will create a username and password ( i will be using lab user) but remember to know the information as we will be using it to connect to our Virtual machine using remote desktop.
</p>
<br />

![Screenshot 2024-01-08 142617](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/176a4c72-a973-4ae6-917a-550f19032bd8)
![Screenshot 2024-01-03 163216](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/f67910a4-fee1-410f-982e-6bba01ee422b)
![Screenshot 2024-01-08 141411](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/6e3983c5-b445-49d3-96aa-1fa460b33568)



Here we are copying the i.p address that is found in our virtual machines tab and if you click the name of your virtual machine you can easily copy your I.P address of your virtual machine and connect to your VM using Remote desktop and using the information 
created to sign in.
</p>
<br />

![Screenshot 2024-01-08 143751](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/93b20141-d32b-47da-a190-59412bfaea8d)
![Screenshot 2024-01-03 163959](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/f4e39652-e6ee-4494-83ad-9084ce4b1d35)
![Screenshot 2024-01-08 143828](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/d0643f87-79ac-4164-a04d-93b4e3d069d2)


we are going to install IIS ( internet information services). We will go to control panel go into programs. And then click turn windows features on and off. We will turn on Cgi which is under the " APPLICATION Development Features " and turn everything on under " Common HTTP Features". Then after you click OK it will install IIS.
To test it and make sure it works you will go to 127.0.0.1 and if it did not work just uncheck and recheck the items again until it works because you probably missed something


![Screenshot 2024-01-03 172206](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/70174258-1033-4074-961e-5476d5fe875f)

Then we will install PHP MANAGER for IIS.

![Screenshot 2024-01-03 172327](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/1dc64fe3-aa48-4fcc-9da2-ee90c89c9136)


Then we will install " IIS URL Rewrite MODULE 2 "

![Screenshot 2024-01-03 172504](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/588e64c6-8562-40a2-9b2d-ac2c6550321f)
![Screenshot 2024-01-03 172936](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/c34e9a08-d5a1-49c8-bb1a-ed9c9818886c)



Then we will create PHP folder on the windows C Drive. After that we will  Extract the PHP file into that PHP folder we created.

![Screenshot 2024-01-08 145350](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/e4392bd3-4a79-4026-b8dc-7b1d1da0dbd4)

![Screenshot 2024-01-03 173620](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/6d484968-700c-4901-975b-8f77d25795cc)


Then we will download the VC_redist.X86 as per required by php and  we will download MySQL Server ( which is installing a data base on the computer considering osTicket is an online Program)

![Screenshot 2024-01-08 145830](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/d5da12e6-9136-41a3-85d4-eb1fbeb51c32)
![Screenshot 2024-01-03 174149](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/61a1a2e5-cb91-4d11-98af-984d1e826c51)
![Screenshot 2024-01-05 130038](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/1e2f1643-5662-4fe2-9b17-3b7ddfc6899e)


Now we will run IIS as a ADMIN and install OsTICKET. But first after running iis we registered php. After that will upload the OSticket upload folder into ( windows C memory - under inetpub into the ROOTfolder)
and we will rename the upload ticket to osTicket.


![Screenshot 2024-01-05 130525](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/5add1766-dd50-468d-90e3-378c4dbef6bd)
![Screenshot 2024-01-05 131134](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/8b8c70c6-cee2-4f8a-9c53-a14eb00aa215)


Within the IIS we will go into the sites-Default web site- osticket and "BROWSE*80" ( on the right side of IIS)  to test if it works. Once tested We will Enable PHP Extensions so that the IIS can run more efficiently because it is recommended by osticket.
so in IIS - sites-default-osticket we will open php manager- click enable or disable an extension and enable php_imap Php_intil Php_opcache

![Screenshot 2024-01-05 131343](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/2951395a-52b9-452a-94b1-761ce9e9fec4)
![Screenshot 2024-01-08 151819](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/93e9bda6-c6c0-4c31-a14b-7b90c34a1caa)

Moving forward we will go back into wwwroot folder ( inside the windows c-inetpub folder) go to osticket-include and rename "ostsampleconfig.php" to "ost-config.php"
Then we will change the permissions on file "ost-config.php" we will right click it - go to properties- go to sercurity- advance - disable inheritance - then click add - select principle and add type everyone in the box- click check names - then give full control

![Screenshot 2024-01-05 132344](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/6545d7fb-88b1-40f0-a631-894cb02fa1df)
![Screenshot 2024-01-05 133020](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/1a344ddb-f1c6-4868-8ad9-7fad88fe0326)


Then we will continue to set up os ticket you can put what information you want just make sure to remember it. But before we are done we must download and install heidisql to connect to our sql server
within HeidiSql we will click new and sign in with the username and password you set up from my sqlserver and the connection is made. Finally we will go into heidisql and create our server and call it os ticket and then finish the install on osticket.

![Screenshot 2024-01-05 133330](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/974e029b-3813-476a-82cb-dc03a3f9641c)
![Screenshot 2024-01-08 152637](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/53704fef-733e-4295-a250-9b23cb16599e)


After the install we will go into the windowsc-inetpub-wwwroot-osticket and delete the set up folder. We will go back to (this pc > Windows c > inetpub > wwwroot > osTicket > include > ost-config.php file and change the security too read only.

![Screenshot 2024-01-08 152947](https://github.com/kevonrochester/osticket-prereqs/assets/155024615/59b6df74-3d57-406f-aaf3-c34fd586264a)

osticket is install but to check go to http://localhost/osTicket/scp/login.php and login with the username and password you set up.





