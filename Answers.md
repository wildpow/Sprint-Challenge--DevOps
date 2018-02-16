### Your responses to the short answer questions should be laid out here using markdown.

For help with markdown syntax, [go here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)


1. Describe the differences between a Docker container and a virtual machine. What makes a container more aptly-suited for portability?

  VM's are complete virtual systems hosted by the guest OS. They are completely seperate which is a security benifit since they don't share the same kernal but, this adds overhead by running an operating system on top of another operating system. Containers on the other hand are closer to the metal so to speak. They run on the same kernal as the guest OS making them samller and some cases faster.

2. Using the command `docker run -p 49160:8080 -d <your_docker_username>/<your_docker_image_name>`, what does `49160:8080` specify?

  This command runs your docker container on your local machine. The numbers `49160:8080` is opening port 49160 on your local machine which is forwarded from the port 8080 in your docker instance.

3. What is the main purpose of using a "container orchestration platform" such as Kubernetes or Docker Swarm?

  Is a way to manage your docker container over many machines hince a pod or a swarm of machines in the cloud. These tools also give you access to load balancing of traffic and scaling to more machines quickly.

4. How do you change the number of replicas in a Kubernetes cluster?

  You can change the amount of replicas in your .yaml file at the root of your project.

5. What does it mean to scale a deployed application 'horizontally'? What does it mean to scale 'vertically'?

  Scaling horizontally essentially means to add more machines to your cluster/pod/swarm. Scaling vertically means to add more resourses to theose machines like processors, ram and disk space.

6. Heroku also utilizes software containers for deployment. What is the main difference between the 'free' tier of containers on Heroku vs. the paid tiers?

  In the free teir Heroku puts your container to sleep after 30 minutes of inactivity. So cold start times of your app are a lot slower. Also you only have access to one machine or dynos as they call it. The paid teirs never sleep and offer the ability to scale your app horizontally to more dynos

