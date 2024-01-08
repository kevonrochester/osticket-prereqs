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



Here we are copying the i.p address that is found in our virtual machines tab and if you click the name of your virtual machine you can easily copy your I.P address of your virtual machine and connect to your VM using Remote desktop and using the information created to sign in.
</p>
<br />
