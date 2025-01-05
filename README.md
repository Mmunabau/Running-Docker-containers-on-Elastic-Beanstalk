<h1>Running Docker containers on Elastic Beanstalk</h1>

<h2>Description</h2>
  In this project i used Docker to create containers based on containers images  and set up my own container image.
 <b>Containers</b>
 are tools for packaging application in a way that's easy for developers to run. They are useful because it helps developers/engineers working in a team together to share their work in a more  efficient way.A container image is a template/blue print for creating containers.Containers spawned/created from the same container image behave in the same waywhich help developers in team have a unified experience.
 
<h1>How I used Docker & Elastic Beanstalk in this project</h1> 
 <b>Docker was used to package the application and its dependencies into a container, while Elastic Beanstalk handled the deployment and management of the application on AWS infrastructure.

<h2>Challenges Faced</h2>
<ul>
<li>Port Configuration: Ensured the exposed port in the container matched the port defined in Dockerrun.aws.json.</li>
<li>IAM Permissions: Configured proper IAM roles for Elastic Beanstalk to access the Docker repository.</li>
<li>Environment Variables: Managed sensitive data securely using Elastic Beanstalk environment variable settings.</li>
</ul>

 </b>

<h2>Languages and Utilities Used</h2>

- <b>AWS CONSOLE</b> 
- <b>DOCKER</b>
- <b>ELASTIC BEANSTALK </b>
- <b>command prompt</b>

<h2>Environments Used </h2>

- <b>Windows 11</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
DOWNLOAD DOCKER DESKTOP ON YOUR PC: <br/>
 <img src="images/qs1.png" height="80%" width="80%" alt="TF-IDF Steps"/>
<br />
 
<br />
Open command pompt on Mac or Windows then run "docker --version" to get the latest docker installed :  <br/>
<img src="images/qs3.png" height="80%" width="80%" alt="TF-IDF Steps"/>
<br />

<br />
On your command prompt run "-d -p 80:80 nginx to install nginx : The command I ran to start a new container was' 'docker run -d -p 80:80 nginx' which means we running the container in the background(-d) matching port 80 in our host computer to the container's port 80(-p 80:80) <br/>
<img src="images/qs4.png" height="80%" width="80%" alt="cont Steps"/>
<br />

<br />
 Nginx is a web server /a software that helps with serving web content.which means it helps with distributing traffic to your aplication across the instances running your application <br/>
<img src="images/qs6.png" height="80%" width="80%" alt="cont Steps"/>
<br />

<br />
Creat a custom image: There was an error when I ran my custom image because i tried to map the port 80 with the new container's port 80,but a running container was already
using port 80. I resolved this by'stopping the running container so that i can start a new one <br/>
<img src="images/qs7.png" height="80%" width="80%" alt="cont Steps"/>
<br />

<br />
Navigate to Elastic Beanstalk configure your Elastic Beanstalk environment upload and Deploy your Docker :  <br/>
<img src="images/qs8.png" height="80%" width="80%" alt="cont Steps"/>
<br />

<br />
Copy URL and paste your Elastic Beanstalk Application.  <br/>
<img src="images/qs9.png" height="80%" width="80%" alt="cont Steps"/>
<br />


<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
