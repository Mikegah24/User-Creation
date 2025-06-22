# User-Creation

Now that our domain is running, we’ll create OUs to keep things organized — like separating users by department. Then we’ll add some user accounts to simulate real employees. This makes it easier to manage permissions, apply policies, and scale the domain in future labs.

## We will create OUs and users:

### Users:
- Alex Johnson (admin)
- Mia Torres (IT)
- Michael Jordan(HR)

### Departments/ OUs:
- ADMINS
- IT
- HR



To create an OU:
- Under Active Directory Users and Computers
- Left-click the domain, New, Organizational Unit
- Give it a name, we will create (example: _ADMINS), select `OK`

<img src="https://github.com/user-attachments/assets/efe6a79c-d55e-424c-8ec6-2e36468afa98" height="45%" width="45%" alt="Disk Sanitization Steps"/>
<img src="https://github.com/user-attachments/assets/cc44521e-1152-4783-ae5a-1fb009f9ed86" height="45%" width="45%" alt="Disk Sanitization Steps"/>


- Now add each user to their department
- Left-click in the department, New, User.
- Enter names of user, and user log on name, Pass
- Select password never expires for now (Note: in a real setting this is a security issue).
- Finish
- Do it for other users in their respective departments
<img src="https://github.com/user-attachments/assets/3af69808-3227-436c-ab3b-79b20a83d779" height="45%" width="45%" alt="Disk Sanitization Steps"/>
<img src="https://github.com/user-attachments/assets/18c60d23-0c34-4330-ad7f-1d0a8c3c2e0f" height="45%" width="45%" alt="Disk Sanitization Steps"/>

### Since User(Alex Johnson) is an Admin, he will need admin privileges:
- Double Click Alex Johnson.
- Select MemberOf.
- Add.
- type `Domain admins`, then Check_names on the right.
- Select OK
- Apply, then Ok again.

<img src="https://github.com/user-attachments/assets/4a53a0a2-97b8-4ce9-a020-9a3c5e2287eb" height="45%" width="45%" alt="Disk Sanitization Steps"/>

***NOW THAT WE HAVE SOME USERS, WE CAN LOGIN ON THE CLIENT AS ANY OF THE USERS.***


Remember, since you are part of the domain, login starts with ***domain\User***
In our case, tech.lab\anyUser (Alex, Mia, or Michael).

==========================================================
