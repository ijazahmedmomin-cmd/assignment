# assignment
cigna
1. big4health-admin

   **Running in local:**
   1. Setup SSH keys to clone the repo
   2. verify node version and install ng
      node -v
      npm install -g @angular/cli
      ng --version
   3. Check for dependencies and update package.json respectively
   4. npm install
   5. ng serve
   6. launch localhost:4200 to access the GUI

   **Running in Docker:**
   1. create a Dockerfile
   2. build the Docker image and push to dockerhub for accessibility with portainer or k8s
      
        docker build -t big4health-admin:1.0.0 .
      
        docker tag <image id> username/ big4health-admin:1.0.0
      
        docker push username/ big4health-admin:1.0.0
      
        Running locally
      
        docker run -d -p 4200:4200 --network=host -e NODE_OPTIONS=--openssl-legacy-provider big4health-admin:1.0.0
      
   4. verify by running docker ps and docker logs command. 
   5. Access GUI by visiting localhost:4200
         <img width="1446" height="828" alt="image" src="https://github.com/user-attachments/assets/bd238f2d-6e5c-49dd-b5a6-9d572e1d4753" />


3. big4health-backend

   **Running in local :**
   1. Setup SSH keys to clone the repo
   2. Create a mongo DB cluster and generate the URL to be used by node.js app
   3. clone the repo in local
   4. npm install 
   5. create .env file ,add below variables and its values
      MONGO_CONNECTION_STRING=mongodb+srv://******:*******@****.*****.mongodb.net/?retryWrites=true&w=majority&appName=****
      
      PORT=3000
   7. npm start 
   8. launch http://http://localhost:3000/api-docs/ to verify the installation.
      <img width="1868" height="887" alt="image" src="https://github.com/user-attachments/assets/a5623369-b8e3-44f1-b2a7-73e682711373" />

  
     **Running in Docker: **
   1.	Create a dockerfile
   2.	Build the image locally – later this can be pushed to dockerhub
      
      docker build -t big4health-backend:1.0.0 .
   4.	Run the container
      
      docker run -d  -p 3000:3000 big4health-backend:1.0.0
   
   6.	Verify the container status and logs
      
      docker ps
     	
      docker logs -f 43ffbdf3116b
   
   8.	Validate the swagger url 
        <img width="940" height="238" alt="image" src="https://github.com/user-attachments/assets/d1a06e34-2d41-4796-b97a-7bc347c0e4e4" />

     <img width="940" height="464" alt="image" src="https://github.com/user-attachments/assets/2771e288-d17a-4d6d-9cf2-6219f8e44c84" />


 
 



 
 


5. 
