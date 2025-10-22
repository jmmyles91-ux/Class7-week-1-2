# Class7-week-1-2

This readme goes through what was done in weeks 1 to 2 

## Table of contents

- Creating a security group
- Creating an EC2
- Using the instance
- Using SSH
- Creating a launch template

### Template used for webserver https://github.com/jmmyles91-ux/BALERICACLASS7/blob/main/ec2scrpit

## Creating a security group

- a. search for EC2 (virtual servers in the cloud).
- b. In the left-hand corner, where there are options, click on security groups.
- c. We NEVER use/touch the default security group.
- d.  Add inbound rules.
- e. for the lesson, we will add http.
<img width="920" height="335" alt="image" src="https://github.com/user-attachments/assets/4c095765-7fdb-4bc5-8dc5-19105839fe56" />



- f. Do not change the outbound rule!!
- g. Tags can be added, but not now. they are useful for organizational purposes as well as tracking resource usage across the organization. It is essential for the office.
- h. Save changes.


## Create the EC2

- a. Go to the instances option, then click on launch instance
- b. Name the instance
- c. Ignore OS, instance type, create a new key pair.
- d.  Use the same name as the instance name for the key pair name
- e. Network settings - use the existing security group, Default
- f.  Leave storage alone
- g. Advanced details - ignore almost everything except at the very bottom, where it says "User data - optional ". we are going to input the script into that blank field. This will allow the server/instance to run certain commands. We are essentially customizing the instance before it turns on.
- h. Check if you selected all the options correctly.

N.B. - To ensure that you have are using the right security group, use the security group ID as a reference.

## Using the instance

- a. When viewing the new instance, we will copy the public DNS, and make it a usable link.
- b. ensure that http:// is typed before entering the link.

Remember to delete your instance or else you will be billed!!!!!!!!


## Using SSH

In this class, we created another EC2 instance.
- a. Use the steps from week 1 to create the security group and instance. 
- b. For this class, I used the same security group I created in week 1.
- c. In said security group, add SSH to the inbound rules.
  <img width="999" height="122" alt="image" src="https://github.com/user-attachments/assets/ff0b8174-1956-4b03-a1a9-8a46517e9a56" />
- d. Go back to the instance and click on connect
- e. When the server load ups, ping 8.8.8.8 (google dns).
- f. To stop the ping, press crtl+z
  
  *The SSH protocol will allow us to remote into the web server through the web browser. If this was not added, we would get an error. *


## Creating a launch template

- a. Before you can create a launch template, you need to ensure that you have EC2/instance available. 
- b. Go to the instances tab. Highlight the instance that you want to replicate and click on actions. Click on the image and templates.
- c. Click on Create template from instance.
- d. Name the template and add a description. All other options should already be preselected as they were already selected when you created the instance. 
- e. Double check everything and ensure it matches up to your preference. 
- f. Create template
- g. you can select the "launch instance from template" to do exactly what is says. you also have the option of creating more than one instance when on the template


