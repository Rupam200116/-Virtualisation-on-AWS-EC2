# **Virtualisation-on-AWS-EC2**
DevOps Open-source 3 Tier Project Deployment | Virtualisation on AWS EC2

In this project, I've hosted a 3-tier application wanderlust which I have collected from github and hostted it on my local machin first then migreted in AWS by using virtualisation.


wanderlust is a three-tier web app which is having three parts: Frontend is made in ReactJS, Backend in NodeJS and a database in MongoDB.

First I've collected the code from github, then tested in my local machine. Then I've created a VM on AWS and hosted this web app on the virtual server.

**Steps for creationg a VM on AWS:**

1. Select your region and go to crate instance then name your VM.
![Screenshot 2024-04-07 184105](https://github.com/Rupam200116/-Virtualisation-on-AWS-EC2/assets/102980397/75ffb2d7-6eb3-42e0-9c37-aa66087782be)

2. Select an operating system.
![Screenshot 2024-04-07 183810](https://github.com/Rupam200116/-Virtualisation-on-AWS-EC2/assets/102980397/036cf599-4a3c-45e3-a175-03681a0e508c)

3. Select OS architecture and instance type:
![Screenshot 2024-04-07 183913](https://github.com/Rupam200116/-Virtualisation-on-AWS-EC2/assets/102980397/e1725bf5-cfd3-4d45-a1ca-1867b3904023)

4. Create and select your keypair and download your secret key:
![Screenshot 2024-04-07 184627](https://github.com/Rupam200116/-Virtualisation-on-AWS-EC2/assets/102980397/45ef7289-d0f3-4aa1-a2da-f5f8bf288c55)

5. Now select your network traffic and click launch instance.
![Screenshot 2024-04-07 184727](https://github.com/Rupam200116/-Virtualisation-on-AWS-EC2/assets/102980397/d177b761-29bd-470c-a8a4-a411c3296171)

After your instance is ready you can access it by ssh or your preferred method. Here I've connected through SSH and then selected keypair which was created in step 4.

Then I cloned the wanderlust web app to my VM and then installed nodejs, npm and after thet installed reactjs inside my VM. Then conncetd backend follewed by the steps from wanderlust.

Then I changed the local host IP under the env file and made it accessible from anywhere 0.0.0.0 under port 5000.

**Backend running view**
![Screenshot 2024-04-07 193220](https://github.com/Rupam200116/-Virtualisation-on-AWS-EC2/assets/102980397/8fd3911d-63d2-4abc-97cf-8c0119034fa0)

After that, I installed mongoDB and connected the database. 

Then I changed the local host IP under the env file and made it accessible from anywhere 0.0.0.0 under port 5173.

**Frontend running view**
![image](https://github.com/Rupam200116/-Virtualisation-on-AWS-EC2/assets/102980397/0afa400e-232f-40f1-a792-ec9deedd5c78)


**Live Project**
https://wanderlust-beta.vercel.app/




