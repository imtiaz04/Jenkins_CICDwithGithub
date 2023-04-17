create 2 instances 1master, 1 agent will connect through ssh

in local in master go to .ssh/folder then ssh-key-gen--->this will generates key-gen which containes public& private keys

![image](https://user-images.githubusercontent.com/85178565/232555571-9996ffaa-8053-4dbc-8c5e-01be0e51bece.png)


take the public key & paste it in to the agnt .ssh folder inside authorize_keys paste it & then it will connect both instances

for checking you can ssh ubuntu@<public ip of the agent>
  
  
![image](https://user-images.githubusercontent.com/85178565/232556557-86f11a59-7ad4-4904-a05e-4cda583691d3.png)

  now will connect through jenkins
  
  add a agent --> give node name --> select permanent agent>create node> form will appear > fill it 
  
  
  ![image](https://user-images.githubusercontent.com/85178565/232557002-48630a43-aee2-4bf6-8b8d-8d3a7b281b39.png)

use ssh key for credencials add master private key add in jenkin credencials
  
  

  ![image](https://user-images.githubusercontent.com/85178565/232559577-1bf2b7f7-13d9-4c02-b9e6-a972f267ac96.png)

  
  
![image](https://user-images.githubusercontent.com/85178565/232559377-9b6fb26f-253b-4dab-bb65-229cf207ae62.png)

  ![image](https://user-images.githubusercontent.com/85178565/232579899-75461853-0619-4147-96f9-ad04f52eba5f.png)

  create web-hook in git hub for that for the project and create job on node with shell script
  
  ![image](https://user-images.githubusercontent.com/85178565/232590550-7d52a6fc-48db-4e83-b9fa-51457be2414c.png)
  
  ![image](https://user-images.githubusercontent.com/85178565/232590653-f2e550cb-93fb-4336-808d-baa45a3f589d.png)

install docker & give permissions
  
 ![image](https://user-images.githubusercontent.com/85178565/232598518-0fe3ed09-ac26-448d-af58-68f457cfd9a8.png)
 
 ![image](https://user-images.githubusercontent.com/85178565/232598723-5435b21b-2535-416a-a86a-b52753809059.png)
  
  ![image](https://user-images.githubusercontent.com/85178565/232598829-334c4dd9-2639-437e-9e3d-4c65757d7ed0.png)

 ![image](https://user-images.githubusercontent.com/85178565/232601170-81129712-ea49-4a1d-b90b-e5d4c421645a.png)
  
  

  ![image](https://user-images.githubusercontent.com/85178565/232601288-d00b0676-60bb-423e-b2f6-192b35b826ec.png)
  
  created pipeline with environment variables using dockerhub credentials;before that in manage jenkins tab added environment plugins and created environment variabes and then created pipeline
  
  ![image](https://user-images.githubusercontent.com/85178565/232613308-52b525f6-3e2b-4c6c-86f1-1b0ea6fc2270.png)
  
  


  
  
