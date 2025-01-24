# Deploy Application to EC2 
## Creat EC2 instances
**Step to launch instance**
1. Add Tags
2. Choose OS Image 
3. Choose Capacity
4. Network Configuration
5. Configure Security Group 
6. Add storage 
**Connect to instance**
1. Move .pem (key pair) to more secure location ~./ssh/
2. Change persion of .pem to make permission stricter with only me as a user can read that (chmod 400 instancefile)
3. Connect to instance : `ssh -i ~/.ssh/docker-server.pem ec2-user@Ipv4`
  - **-i**: This flag will take the pem file as a parameter
  - **ec2-user**: I need to ssh to instance as a ec2 user not as a root user

## Install Docker