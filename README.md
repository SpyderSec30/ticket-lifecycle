<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Life Cycle of a Ticket</h1>

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>
 
- Windows 10</b> (21H2)

<h2>Getting Started</h2>

First we will use the users we created in the post-install-config lab "Kathy Smith" and "Ben Smith" to create some tickets on the enduser's URL localhost/osTicket. Do this by selcting Open New Ticket and entering Ben or Kathy's email, no phone number is required.<br></br>

<img src="https://github.com/SpyderSec30/post-install-config/assets/174487140/5d38e204-b95e-4dc0-adeb-27e28fb03668"/><br></br>

Notice that the Help Topics are the same ones that we configured in the previous lab.
</br>

<img src="https://github.com/SpyderSec30/post-install-config/assets/174487140/6184e164-6d9d-4aeb-8872-5811b1f1494f"/><br></br>

Make a Ticket for each category we created. Doesnt have to be anything special, we just want to see them when we log back into the agent/admin panel.

- Business Critical
- Personal Computer Issues
- Equipment Request
- Password Reset

<h2>Jane.Doe</h2>
Now head back to the URL localhost/osTicket/scp and login using jane.doe's credentials. Jane Doe is an agent that we conifured in the post-install-config lab. But when I signed in as her, she cant see any of tickets we just created. We'll have to do some troubleshooting to find the issue. Was not expecting this, but it will be good practice to discover the reason behind it.
<br></br>

<img src="https://github.com/SpyderSec30/post-install-config/assets/174487140/985db357-a396-4630-bb12-ab92cbd9c568"/>
<br></br>

Lets start the investigation by logging back into our main Admin account.

<img src="https://github.com/SpyderSec30/post-install-config/assets/174487140/c28810b8-430f-4c22-bb74-71183c87455c"/><br></br>

I clicked on one of the tickets and noticed that it was being sent to the Support Department. Lets go to the Admin Panel to see if we need to put Jane Doe in the Support Department to view Tickets. Once in the Admin panel, select the Agents tab and click Jane Doe. This will open up a Manage Agent section and in here select the Access tab.<br></br>

<img src="https://github.com/SpyderSec30/post-install-config/assets/174487140/e79bcb5d-275e-4aee-bc43-263a290631d4"/><br></br>

Lets Extend her access by adding her to the Support Department and giving her Supreme Admin for this Lab

<img src="https://github.com/SpyderSec30/post-install-config/assets/174487140/fff43b9a-80b4-4b67-b53c-bfdfd4dbe098"/><br></br>

Log back into Jane Doe's account and you will see that I have successfully found a solution to my own Ticket. She can now see Tickets on her end.<br></br>

<img src="https://github.com/SpyderSec30/post-install-config/assets/174487140/8a7d777e-20b4-41dc-8ab2-969262f34f70"/><br></br>


<h2>Going Through a Ticket</h2>
 
Lets click on Mobile Banking not Working, so that we can work this Ticket.<br></br>

<img src="https://github.com/SpyderSec30/post-install-config/assets/174487140/18b35392-89d8-4d3a-9e0a-ef1c665f87e2"/><br></br>

This is a Business Critical event, so we need to update the Priority Level from normal to Emergency! Next we can assign it to the right person on the team who has the skills to handle this level of Ticket. We also need to set the SLA to match severity of the situation.<br></br>

<img src="https://github.com/SpyderSec30/post-install-config/assets/174487140/a2ce78e0-5f1f-4cca-883b-6df566d29c6b"/><br></br>

Pay Attention to the Ticket thread to see who has made changes to it during its life cycle.<br></br>

<img src="https://github.com/SpyderSec30/post-install-config/assets/174487140/fc70a486-6625-43a3-984e-c9d7dea0980a"/><br></br>

After working the Ticket, you'll notice that it has changed in the Ticket que. The Priority section is now highlighted in light red because of the Emergency Level we applied to it. Also in the Assigned to section you'll see Jane Doe instead of it just being blank.

<img src="https://github.com/SpyderSec30/post-install-config/assets/174487140/137926e3-c773-4c20-b8f4-161eb4701695"/><br></br>

Now click back into the ticket and scroll down and you will see the section where you can give updates on the status of the ticket. Your reponses will also be added to the ticket thread. You may also close the Ticket once the issue has been resolved in the Ticket Status drop box. <br></br>

<img src="https://github.com/SpyderSec30/post-install-config/assets/174487140/2f41d840-7f99-4483-af29-1e33b56cfac7"/>


<h2>Finished</h2>
In conclusion, the life cycle of a ticket in osTicket is a well-structured process that ensures efficient and effective resolution of issues within an IT environment. This Lab was to demonstrate my understanding of Ticketing systems in a real world environment.


