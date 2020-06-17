This project is dealing with a system that has three parts...

<h2>Part-1</h2>
  <p>This part involves 2 docker containers launched...One for master and one for the Testing...</p>
  
  ![](images/master_docker.png)
  ![](images/branch_docker.png)
  
  <p> Now that container is created we need to setup jenkins with some jobs that will help us get the task done automated.</p>
  
  I am also setting up Webhook for the GitHub Repo so that when something is pushed the github triggers the jenkins job...
  
 <h2>Setting Up Github Webhook</h2>
 
You should have ngrok tool that converts private IP to Public IP...

![](images/ngrok1.png)
![](images/ngrok2.png)

Next we need to setup in GitHub Repository...

![](images/ngrok3.png)
![](images/ngrok4.png)
![](images/ngrok5.png)

<p><b>Now lets see the Jenkins configuration to be made...</b></p>

<h1>Jenkins Configurations</h1>

<p> There are three jobs made that will help us in achieveing a monitored automation system...</p>

![](images/j1.png)

<ol>
  
 <li>
  
  <h1>Production Job</h1>
 
 ![](images/p1.png)<hr/>
 
 <p>This part is done so that when Webhooks is triggered via master branch then this job runs...

 ![](images/p2.png)<hr/>
 
 <p>I actually did this configuration of merging so that when production part is going on then before start branch gets merged with the master</p>
 
 ![](images/p3.png)<hr/>
 
 ![](images/p4.png)<hr/>
 
 ![](images/p5.png)
 
    sudo cp -fvr * /root/task1
    
 Simply click on save and then apply and then this is done...
 
 </li>
 <li>
  <h1>Testing</h1>
  
  ![](images/p21.png)<hr/>
  
  ![](images/p22.png)
  
  <p>This job is triggered via webhook when something is pushed in the dev branch...</p>
  
  ![](images/p23.png)
  
    sudo cp -fvr * /root/task12
   </li>
   <li>
  <h2>QA trigger Job</h2>
  
  <p> Once the push is done in the dev branch then, the QA team will check the webpage and then run the job...</p>
  
  ![](images/p31.png)
  
  ![](images/p32.png)
  
  ![](images/p33.png)
  </li>
 </ol>
 
 <p><h2>And With all this you just have a semi-automation system ready<h2>
  Feel free to contact on WhatsApp 9338455463(No calls plzz) if you have any doubt or suggestions.</p>
