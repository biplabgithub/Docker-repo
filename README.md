# Docker-repo
what is docker 

  Docker is an open‐source containerization platform that help us to packaging the application along with all its dependencies (libraries, configuration files, etc.) into a standardized, lightweight unit called a container.

why use the docker ? 
------------------------
   1.Consistency Across Environments:
    With Docker, you “containerize” your application so that it runs the same way on your development machine, in testing, and in production.

   2. Isolation and Resource Efficiency:
    Containers isolate your application from other software on the host system. Unlike traditional virtual machines, Docker containers share the host’s operating       system kernel, which means they use fewer resources and start up much faste.
Without docker what is the problem:
-------------------------------------------------------------------------
   3.Inconsistent Environments:
          Without Docker, you might run into issues where an application works on one machine but fails on another due to differences in installed software, 
          library        
    4. Complex Setup and Deployment:
        Installing all required dependencies manually on every machine or server is error-prone and time-consuming. Without containerization, ensuring that every 
        environment is set up identically becomes a major headache.
     5. Resource Overhead:
       Traditional virtual machines require running a full guest operating system on each instance, which consumes more resources and leads to longer startup times 
       compared to Docker’s lightweight containers.

 6. Difficulty in Scaling:
    Without a containerized approach, scaling an application—such as deploying additional instances to handle increased traffic—often involves manual setup and 
    configuration, making rapid scaling challenging and inefficient.

install Docker:
    install the docker in the ubuntu machine 
        open the terminal and run the command 
                   sudo apt update
                   sudo apt upgrade -y
