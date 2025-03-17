# Docker-repo

what is docker 

 Docker is an open‐source containerization platform that help us to packaging the application along with all its dependencies (libraries, configuration files, etc.) into a standardized, lightweight unit called a container.

why use the docker ? 
-----------------------
1.Consistency Across Environments:
         
  With Docker, you “containerize” your application so that it runs the same way on your development machine, in testing, and in production.
  
2.Isolation and Resource Efficiency:
  
   Containers isolate your application from other software on the host system. Unlike traditional virtual machines, Docker containers share the host’s operating       system kernel, which means they use 
   fewer resources and start up much faste.
   
Without docker what is the problem:
-------------------------------------------------------------------------
1.Inconsistent Environments:
   
   Without Docker, you might run into issues where an application works on one machine but fails on another due to differences in installed software, 
   library
          
 2. Complex Setup and Deployment:
      
   Installing all required dependencies manually on every machine or server is error-prone and time-consuming. Without containerization, ensuring that every 
   environment is set up identically becomes a major headache.
      
 3. Resource Overhead:
      
   Traditional virtual machines require running a full guest operating system on each instance, which consumes more resources and leads to longer startup times 
    compared to Docker’s lightweight containers.

 4. Difficulty in Scaling:
      
   Without a containerized approach, scaling an application—such as deploying additional instances to handle increased traffic—often involves manual setup and 
   configuration, making rapid scaling challenging and inefficient.

install Docker:

  install the docker in the ubuntu machine 
  
  open the terminal and run the command 
  
         sudo apt update
                   
        sudo apt upgrade -y

   step 2: Add Docker’s GPG Key
   
    sudo install -m 0755 -d /etc/apt/keyrings
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo tee /etc/apt/keyrings/docker.asc > /dev/null
    sudo chmod a+r /etc/apt/keyrings/docker.asc
  step 3:Add the Docker Repository
  
    echo \
    "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
    $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
  step 4: Install the Docker
  
    sudo apt update
    sudo apt install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
  step 5: Verify Docker Installation
  
    docker --version
  step 6: Enable & Start Docker
  
    sudo systemctl enable docker
    sudo systemctl start docker
  then run the command 
  
    docker ps 
  it show the not permission to the  user / to permission the  user we can add the user in the docker group
  
    sudo usermod -aG docker $USER
    newgrp docker
    now your docker is running sucessfully 




  


