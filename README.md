<p align="center">
  <img src="https://github.com/user-attachments/assets/52fb680e-df8c-4430-a2b9-3dc6d43aa87f" width="250" /> <img src="https://upload.wikimedia.org/wikipedia/commons/2/2f/PowerShell_5.0_icon.png" alt="PowerShell Logo" width="150"/>
</p>

# Add and Remove Users with MicrosoftGraph PowerShell ISE

## Platform and Tools Used

- PowerShell ISE
- Microsoft Graph
- Microsoft Entra ID
- Web Browser

## Objective
In this project, I will demonstrate how to create and delete user accounts in Microsoft Entra ID using Microsoft Graph PowerShell. Specifically, I will:

- Create three new users: **Mitu, Mimi, and Eyoel**.

- Verify their successful creation.

- Delete the newly created users using Graph PowerShell commands.

This project showcases basic user lifecycle operations using Microsoft Graph PowerShell, useful for scripting and automating identity management tasks.

-------


### Add New Users

1. I first ran the `Connect-MgGraph` command to ensure that PowerShell ISE was connected to Microsoft Graph. Then, I used the `Get-MgUser` command to retrieve the list of existing users in Entra ID:

<img src="https://github.com/user-attachments/assets/157fe90e-cbc0-49dc-b8d7-a04739db003e" alt="Screenshot 2025-07-24 155933" width="800" />



2. I created a script pane in PowerShell ISE, added the commands along with the credentials for the three new users, and then ran the script:

<img src="https://github.com/user-attachments/assets/51e8c443-9102-4ff0-85ad-d4486692c537" alt="Screenshot 2025-07-24 192931" width="850" />


3. After running the script, PowerShell ISE returned confirmation that the new users were successfully added:

<img src="https://github.com/user-attachments/assets/2c2b4066-b6ce-44d8-bcf1-ab5b084eaac1" alt="Screenshot 2025-07-24 193019" width="850" />

4. To double check the new users were successfully added, I ran the `Get-MgUser` command in PowerShell and also checked my Microsoft Entra ID portal via the web interface. As it shows on the screenshots, they were successfully added:

<img src="https://github.com/user-attachments/assets/f35ce0e9-0813-403b-93c0-6685b1872f21" alt="Get-MgUser Result" width="850" />
<br>
<img src="https://github.com/user-attachments/assets/4868cf16-d8b5-42e5-af5c-6d4d81117de9" alt="Entra ID Confirmation" width="700" />

-----

### Remove Users

1. To remove the three users I previously created, I opened a new script pane in PowerShell ISE, added the necessary removal commands along with the user credentials, and then executed the script:

<img src="https://github.com/user-attachments/assets/693c7308-d1ab-4062-a7d1-9c13c8eb2a02" alt="User Deletion Script" width="600" />


2. I verified the successful removal of the users by running the `Get-MgUser` command and checking the Deleted Users section in my Microsoft Entra ID portalto ensure the accounts were no longer listed:
<img src="https://github.com/user-attachments/assets/cf98d194-91ca-4648-8019-8165ded1cb75" alt="Get-MgUser After Deletion" width="600" />
<br>
<img src="https://github.com/user-attachments/assets/e74b4cf4-09bd-4a9a-b6c8-8e7d3c83c629" alt="Deleted Users Section in Entra Portal" width="550" />

-----

## Conclusion

This project demonstrated the core user management capabilities of Microsoft Graph PowerShell within Microsoft Entra ID. By scripting the creation and deletion of user accounts in PowerShell ISE, I gained hands-on experience with identity lifecycle automation. Verifying actions through both PowerShell and the Entra portal ensured accuracy and reinforced how these tools work together for effective administration.




