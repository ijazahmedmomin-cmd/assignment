# assignment
cigna
1. big4health-admin
2. big4health-backend
   **Running in local :**
   1. Setup SSH keys to clone the repo
   2. Create a mongo DB cluster and generate the URL to be used by node.js app
   3. clone the repo in local
   4. npm install 
   5. create .env file ,add below variables and its values
      MONGO_CONNECTION_STRING=mongodb+srv://******:*******@****.*****.mongodb.net/?retryWrites=true&w=majority&appName=****
      PORT=3000
   6. npm start 
   7. launch http://http://localhost:3000/api-docs/ to verify the installation.
      <img width="1868" height="887" alt="image" src="https://github.com/user-attachments/assets/a5623369-b8e3-44f1-b2a7-73e682711373" />

  
     **Running in Docker: **
   1.	Create a dockerfile
   2.	Build the image locally – later this can be pushed to dockerhub 
      docker build -t big4health-backend:1.0.0 .
   3.	Run the container 
      docker run -d  -p 3000:3000 big4health-backend:1.0.0
   4.	Verify the container status and logs
      docker ps
      docker logs -f 43ffbdf3116b
   5.	Validate the swagger url 
        <img width="940" height="238" alt="image" src="https://github.com/user-attachments/assets/d1a06e34-2d41-4796-b97a-7bc347c0e4e4" />

     <img width="940" height="464" alt="image" src="https://github.com/user-attachments/assets/2771e288-d17a-4d6d-9cf2-6219f8e44c84" />


 
 



 
 


4. 

