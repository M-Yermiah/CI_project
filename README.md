# 3 Ec2 servers were created in AWS as Dev, QandA, and Prod.
Through git bash and ssh connected to ec2(Local Machine).
Java8, Git, Jenkins, and Maven were installed on DEV.
Tomcat8 was installed on QandA and Prod.
Connected to Jenkins, Created Development Job, Source Code was downloaded from(CI-CD Github).
Converted the java files into an artifact(.war file) using maven.
Deployed the war file into the QandA Server.
war/ear to a container was deployed. Credentials were configured in tomcat8 as users to access the application.
Configured Build other project and connected testing with development Job, The artifacts were archived in the development job.
A new job as Testing was created in Jenkins, Source Code was downloaded from(Test Github)
Archived artifacts were copied from the devolpment job to the testing job
war/ear to a container was deployed in the testing job, Credentials were configured in tomcat8(Prod) as users to access the application.
The application was successfully accessed using the configured dev publicip:8080/context path and prod privateip:8080/context path
all stages of Continous(Download, Build, Deployment, Testing, Delivery) were achieved.
tools-GIT, AWS, JAVA8, MAVEN, and JENKINS
