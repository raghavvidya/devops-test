
### Required tasks for the Solution

Your task is to create a CI build pipeline that deploys this web application to a load-balanced	
environment. You are free to complete the test in a local environment (using tools like Vagrant and	
Docker) or use any CI service, provisioning tool and cloud environment you feel comfortable with (we	
recommend creating a free tier account so you don't incur any costs).	

* Your CI job should:	
 * Run when a feature branch is pushed to Github (you should fork this repository to your Github account). If you are working locally feel free to use some other method for triggering your build.	
 * Deploy to a target environment when the job is successful.	
* The target environment should consist of:	
 * A load-balancer accessible via HTTP on port 80.	
 * Two application servers (this repository) accessible via HTTP on port 3000.	
* The load-balancer should use a round-robin strategy.	
* The application server should return the response "Hi there! I'm being served from {hostname}!".	

## Context	
We are testing your ability to implement modern automated infrastructure, as well as general knowledge of system administration. In your solution you should emphasize readability, maintainability and DevOps methodologies.	

## Submit your solution	
Create a public Github repository and push your solution in it. Commit often - we would rather see a history of trial and error than a single monolithic push. When you're finished, send us the URL to the repository.	

## Running this web application	
This is a NodeJS application:	This is a NodeJS application:

- `npm test` runs the application tests	- `npm test` runs the application tests
- `npm start` starts the http server


# Technical Test Solution
Load Balancing Node.js Application Servers with NGINX running on a simple docker containers.



## Prerequisites
* Docker >= 1.13
* Docker Compose >=1.2


### How to run

Login to the system

```   
   cd /root
   git clone https://github.com/raghavvidya/devops-test.git
   cd devops-test
   docker-compose up
```

### How to verify the Solution
Get the IP address of the system and try accessing `http://<systemip>`  

