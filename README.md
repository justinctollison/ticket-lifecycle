<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1 align="center">osTicket - Ticket Lifecycle: Intake Through Resolution</h1>

This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)  
- Remote Desktop  
- Internet Information Services (IIS)


<h2>Operating Systems Used</h2>

- Windows 10 (21H2)


<h2>Ticket Lifecycle Stages</h2>

- Intake  
- Assignment and Communication  
- Working the Issue  
- Resolution


<h2>Lifecycle Stages</h2>

Let's log into our VM and get started. Navigate to the two web pages like before:  

- **Admin/Analyst Login Page:**  
  http://localhost/osTicket/scp/login.php  

- **End Users osTicket URL:**  
  http://localhost/osTicket  

Once you have those two up in your browser, we can get started. We'll be creating tickets as an end-user and then logging in as one of our previous agents to observe the ticket's properties.  

After everything is set up, navigate to the end-user page and open a new ticket. When you go to enter a new ticket, it's going to ask for your contact information. Let's fill in Karen's information from before and then choose one of the help topics.  

Users normally pick the wrong help topic, so we can simulate that. Let's go with **"Report a Problem"** and enter in some information such as:  

> "Entire mobile/online banking system is down."  

Then, write a quick description for it.  

<br>

<p align="center">
  <img width="847" height="958" src="https://github.com/user-attachments/assets/f625e374-9093-481d-b2f0-5c9a46fb7ca7" />
</p>

---

After creating the new ticket, move onto the **Admin/Analyst** login page and log in as **Jane**. Alternatively, we can also log in as **John**; however, sometimes tickets are automatically set to another department.  

In our case, the ticket gets automatically assigned to *Maintenance*. Since John is in another department, he cannot view it. This creates a great exercise: go into the **Admin Panel → Agents → Departments** and delete the *Maintenance* department.  

This will automatically assign the ticket's department to *Support*, where John can now view it.  

<br>

<p align="center">
  <img width="958" height="379" src="https://github.com/user-attachments/assets/019a1f08-61f1-48ce-ba3c-98caaa700414" />
</p>

---

Looking at the live ticket, John is able to do a variety of things with it. He can set the **SLA plan**, assign the ticket to himself, respond to the user, create a thread for the ticket, and even set the **priority** and **help topic**. This adds flexibility and depth to ticket handling.  

Since this is an entire business outage, we'll set the **SLA** to *Sev-A*, set the **Priority** to *Extreme*, assign ourselves the ticket, and then add a response at the bottom.  

It's important to maintain constant communication with the user to ensure that the issue is being handled.  

If you want to go further, navigate back to the **Admin Panel → Agents → Teams**, then go into **Online Banking**. Inside there, you can add Jane Doe as one of the members.  

Then, back in the ticket, instead of assigning it to one person such as John, you can assign it to the entire **Online Banking Team**, allowing Jane to see it. Inside Jane's account, you can set the **status** of the ticket to *Resolved* and then add a closing statement.  

<br>

<p align="center">
  <img width="1074" height="950" src="https://github.com/user-attachments/assets/91cce43f-4de9-4d23-bf8c-e201a62fdc23" />
  <br><br>
  <img width="951" height="416" src="https://github.com/user-attachments/assets/66dcf337-a8d0-4d60-bc69-71b0246c79c2" />
</p>

---

We can now simulate tickets as both an end-user and an agent working on the ticket. You can follow up and resolve tickets, then create new ones with more complexity.  

It's even a good idea to make up some scenarios in ChatGPT and input them to see how osTicket handles them. The system is very flexible and allows you to do a lot.  

**Happy ticketing!**

