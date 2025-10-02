Who what when where and why

Creating an EC2

- Log into AWS Console
- Type EC2 in search bar or click ec2 in the top left if available. 
- Click security groups (The option will be on the left side of the screen under dashboard and then Network & Security). 
- Click create security group which should be in the top left of your screen. 
- Under basic details name the security group and give a description, possibly related to what ports you want to use to help you remember what the security group is for. 
	- Under inbound rules click add rule and click the dropdown tab and select http which should select and gray out TCP under protocol and 80 In Port Range. Click the source tab and select Anywhere IPv4 and give a description if you would like. 
	- Add a second inbound rule and this time select ssh with the type tab and select anywhere ipv4 with the source tab. 
	- DO NOT TOUCH OUTBOUND RULES!
	- You may create tags if you would like to assist with searching for the group. 
	- Click create security group. 
	- On the left dashboard click instances. 
	- Click launch instances which is at the top right of the screen. 
	- Scroll down to Key pair login and click create new key pair. 
	- Name the key pair what you would like then click create key pair. 
	- Scroll down to Network Settings and under Firewall click select existing security group and choose the one you created. 
	- Scroll down to Advanced details and click the dropdown. 
	- Scroll all the way down to the bottom to user data and then copy the script from the github repo and then paste it into the user data.
	- Click launch instance on the right. 
	- Click instances under EC2 and you should see your ec2 instance running. 
	- To make a template from your ec2 once you have clicked on your instance click actions then click image and templates and then click create template from instance.
	- Name your template and give a description
	- All other settings are changed as needed. Click create template.
	- To launch a template, click on the template you have created. Click actions then launch instance from template. 
	- On the new page it should have your instance selected under source template which is below choose a launch template. If it is not selected choose yours. 
	- Click launch template which is on the right of the screen. 
