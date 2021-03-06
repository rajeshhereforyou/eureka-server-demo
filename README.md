# What is this?

This is a simple Eureka Server using Spring Boot 2. You can find the sample Eureka client code here

https://github.com/rajeshhereforyou/eureka-client-demo

## Pre-requisite

1. Before building and deploying this app, Please make sure that the port 8761 is available on your local machine because we are deploying our sample Eureka Server on the 8761 (default Eureka port). If you are using mac, you can check the port availability using below command

lsof -i :8761


## How to clone and run this app?

Step 1: Clone this repo at https://github.com/rajeshhereforyou/eureka-server-demo.git

Step 2: Once you cloned the repo,all the gradle dependencies should be resolved and available in your classpath to run the app as an Eureka Client

Step 3: Now, you can run the app using Spring boot 'bootRun' command

Step 4: Once you have the app up and running, you can the health of the app using 'http://localhost:8761/actuator/health'. This should return '{"status":"UP"}'

Step 5: That's it, it's so simple to build and deploy a sample Eureka Server.

### Now, if you have a question on where can i see my sample Eureka server status, hit the below URL

http://localhost:8761/eureka/status

As we have Eureka server up and running. Let's build and deploy a sample Eureka client by following instructions in 'README.md' of the below git repo

https://github.com/rajeshhereforyou/eureka-client-demo/

Step 7: Once the sample Eureka client is up and running, it should register itself as client with your sample Eureka Server.
 
### Now, if you have a question on where can i see all the registered clients (with your sample Eureka server), hit the below URL 

http://localhost:8761/eureka/apps

That's it. Now, you know the basic configuration of setting up a Eureka server, creating an Spring boot to as Eureka client and monitor it's status.

If you are interested to see the eureka server configuration, you can find the code at '/src/main/resources/application.yml' in this repo.













