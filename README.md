# Class7-week-1-2

This readme goes through what was done in week 1 to 2 

## Table of contents

- Creating a security group
- Creating an EC2
- Using the instance
- Using SSH
- Using a launch template

### Template used == https://github.com/jmmyles91-ux/BALERICACLASS7/blob/main/ec2scrpit

## Creating a security group

- a. search for EC2 (virtual servers in the cloud).
- b. At the left-hand corner where there are options, click on security groups.
- c. We NEVER use/touch the default security group.
- d.  add inbound rules.
- e. for the lesson, we will add http.
<img width="920" height="335" alt="image" src="https://github.com/user-attachments/assets/4c095765-7fdb-4bc5-8dc5-19105839fe56" />



- f. Do not change outbound rule!!
- g. tags can be added but not now. they are useful for organizational purposes as well as tracking resource usage across the organization. It is essential for the office.
- h. Save changes.


## Create the EC2

- a. Go to instances option, then click on launch instance
- b. Name the instance
- c. Ignore OS, instance type, Create new key pair.
- d.  Use the same name as the instance name for the key pair name
- e. Network settings - use the existing security group, Default
- f.  Leave storage alone
- g. Advanced details - ignore almost everything except at the very bottom where it says "User data - optional ". we are going to input the script into that blank field. This will allow the server/instance to run certain commands. We are essentially customizing the instance before it turns on.
- h. Check if you selected all the options correclty.

N.B - To ensure that you have are using the right security group, use the security group ID as reference.

## Using the instance

- a. When viewing the new instance, we will copy the public DNS, and make it a usable link.
- b. ensure that http:// is typed before entering the link.

Remember to delete your instance or else you will be billed!!!!!!!!



