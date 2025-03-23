<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
An easy-to-follow tutorial on the post-install configuration of the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Configuration Steps</h2>

We'll get started with configuring roles. First, get signed into OsTicket, click "agents", "rolls", then hit "add new role"
<p>
<p align="center"><strong><img src="https://i.imgur.com/Fe9kTqs.png" height="80%" width="80%" alt="Post Install Steps"/>
</p>
<p>
<p align="center"><strong>For the name, type in "Supreme Admin", then click "Permissions" above. Give the role every permission and hit "add role".
</p>
<br />

<p>
<p align="center"><strong><img src="https://i.imgur.com/vFh8vcG.png" height="80%" width="80%" alt="Post Install Steps"/>
<p align="center"><strong><img src="https://i.imgur.com/pjJGUGh.png" height="80%" width="80%" alt="Post Install Steps"/>
</p>
<p>
<p align="center"><strong>Next we'll configure departments. Click "Departments", then hit "Add new department". Set the parent to "top-level department", and type in "SysAdmin" for the name. Scroll down and click "Create dept".
<br />

<p>
<p align="center"><strong><img src="https://i.imgur.com/6jB5SXA.png" height="80%" width="80%" alt="Post Install Steps"/>
<p align="center"><strong><img src="https://i.imgur.com/3ieBfyg.png" height="80%" width="80%" alt="Post Install Steps"/>
</p>
<p>
<p align="center"><strong>Now we'll configure teams. hit "teams", then "create new team". Type in "Online Banking" for the name and click "Create Team".
<br />

<p>
<p align="center"><strong><img src="https://i.imgur.com/kJ8QJOt.png" height="80%" width="80%" alt="Post Install Steps"/>
<p align="center"><strong><img src="https://i.imgur.com/D3LMBS5.png" height="80%" width="80%" alt="Post Install Steps"/>
</p>
<p>
<p align="center"><strong>Click "Settings", then "Users" to make sure the "Registration Required" box is unchecked to allow users who aren't signed in to create help tickets.
</p>
<br />

<p>
<p align="center"><strong><img src="https://i.imgur.com/aufpcfG.png" height="80%" width="80%" alt="Post Install Steps"/>
</p>
<p>
<p align="center"><strong>Now we'll be adding 2 new agents. Click "agents" above, then click "add new agent".
<br />

<p>
<p align="center"><strong><img src="https://i.imgur.com/gYFuxyK.png" height="80%" width="80%" alt="Post Install Steps"/>
</p>
<p>
<p align="center"><strong>Create the credentials and write them down(you can use a fake email). Then click "access".
<br />

<p>
<p align="center"><strong><img src="https://i.imgur.com/wiJxgz3.png" height="80%" width="80%" alt="Post Install Steps"/>
</p>
<p>
<p align="center"><strong>Click the "select department" dropdown and choose "sysadmins", then on the "select role" dropdown choose "supreme admin". under "teams" select "online banking", and click "create".
</p>
<br />

<p>
<p align="center"><strong><img src="https://i.imgur.com/3SKFkEt.png" height="80%" width="80%" alt="Post Install Steps"/>
<p align="center"><strong><img src="https://i.imgur.com/DCmW1Wb.png" height="80%" width="80%" alt="Post Install Steps"/>
</p>
<p>
<p align="center"><strong> Create a second account. Under "Access" Click the "select department" dropdown and choose "support", then on the "select role" dropdown choose "view only" and click "create".
<br />

<p>
<p align="center"><strong><img src="https://i.imgur.com/M2im4ls.png" height="80%" width="80%" alt="Post Install Steps"/>
<p align="center"><strong><img src="https://i.imgur.com/JhSjwHM.png" height="80%" width="80%" alt="Post Install Steps"/>
</p>
<p>
<p align="center"><strong>Head back to the agents tab click one of the users you created, then click "Set password". Uncheck the 2 boxes and type in a password, be sure to write it down, then click update. Do the same for the other account you created as well.
<br />

<p>
<p align="center"><strong><img src="https://i.imgur.com/KUZMw13.png" height="80%" width="80%" alt="Post Install Steps"/>
</p>
<p>
<p align="center"><strong>Look to the top right and click "agent panel"
</p>
<br />

<p>
<p align="center"><strong><img src="https://i.imgur.com/ojKa8Qu.png" height="80%" width="80%" alt="Post Install Steps"/>
</p>
<p>
<p align="center"><strong>Click "users", then "add a user". Then create a user with a fake email, and click "add user".
<br />

<p>
<p align="center"><strong><img src="https://i.imgur.com/t2pTSdQ.png" height="80%" width="80%" alt="Post Install Steps"/>
<p align="center"><strong><img src="https://i.imgur.com/6QntZDN.png" height="80%" width="80%" alt="Post Install Steps"/>
</p>
<p>
<p align="center"><strong>Now head back to "the admin panel", click "manage", "SLA", and "add new SLA plan".
<br />

<p>
<p align="center"><strong><img src="https://i.imgur.com/HXbBskk.png" height="80%" width="80%" alt="Post Install Steps"/>
<p align="center"><strong><img src="https://i.imgur.com/aNYvTXa.png" height="80%" width="80%" alt="Post Install Steps"/>

</p>
<p>
<p align="center"><strong>We're going to create 3 different SLAs, one for each level of difficulty for any given ticket sent in by customers. For the name type "Sev-A, make "Grace period" an hour, and "Schedule" 24/7, then click "Add plan". For the other SLAs, set them up as shown in the examples below.
<br />

<p>
<p align="center"><strong><img src="https://i.imgur.com/QrKXIMB.png" height="80%" width="80%" alt="Post Install Steps"/>
<p align="center"><strong><img src="https://i.imgur.com/ycgZcnm.png" height="80%" width="80%" alt="Post Install Steps"/>
<p align="center"><strong><img src="https://i.imgur.com/07fc4yM.png" height="80%" width="80%" alt="Post Install Steps"/>
</p>
<p>
<p align="center"><strong>Now head to "Help Topics" under "Manage", then click "add new help topic" add the help topics as shown below, and change "parent topic" to "report a problem".
<br />

<p>
<p align="center"><strong><img src="https://i.imgur.com/dgEkBwF.png" height="80%" width="80%" alt="Post Install Steps"/>
<p align="center"><strong><img src="https://i.imgur.com/iISw0BH.png" height="80%" width="80%" alt="Post Install Steps"/>
<p align="center"><strong><img src="https://i.imgur.com/q41Uoxr.png" height="80%" width="80%" alt="Post Install Steps"/>
<p align="center"><strong><img src="https://i.imgur.com/EY4XDLN.png" height="80%" width="80%" alt="Post Install Steps"/>
<p align="center"><strong><img src="https://i.imgur.com/WBTiDxi.png" height="80%" width="80%" alt="Post Install Steps"/>
</p>
<p>
<p align="center"><strong>Congrats! You've set up OsTicket! This is valuable knowledge that can help you in IT, customer support, and beyond. Knowing how to configure and manage a ticketing system is a great skill that can set you apart in troubleshooting and workflow management.
</p>
<br />
